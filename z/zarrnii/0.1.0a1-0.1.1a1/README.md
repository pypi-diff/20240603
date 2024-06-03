# Comparing `tmp/zarrnii-0.1.0a1.tar.gz` & `tmp/zarrnii-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrnii-0.1.0a1.tar", max compression
+gzip compressed data, was "zarrnii-0.1.1a1.tar", max compression
```

## Comparing `zarrnii-0.1.0a1.tar` & `zarrnii-0.1.1a1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      123 2024-05-24 15:08:33.511993 zarrnii-0.1.0a1/README.md
--rw-r--r--   0        0        0     1069 2024-05-24 16:23:20.951270 zarrnii-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0       95 2024-05-24 15:08:33.515993 zarrnii-0.1.0a1/zarrnii/__init__.py
--rw-r--r--   0        0        0    13296 2024-05-24 15:08:33.515993 zarrnii-0.1.0a1/zarrnii/core.py
--rw-r--r--   0        0        0      216 2024-05-24 15:08:33.515993 zarrnii-0.1.0a1/zarrnii/enums.py
--rw-r--r--   0        0        0    25787 2024-05-24 15:08:33.515993 zarrnii-0.1.0a1/zarrnii/scratch_extractsubvol.ipynb
--rw-r--r--   0        0        0     7348 2024-05-24 15:08:33.515993 zarrnii-0.1.0a1/zarrnii/transform.py
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 zarrnii-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-06-03 13:35:45.004651 zarrnii-0.1.1a1/README.md
+-rw-r--r--   0        0        0     1108 2024-06-03 14:25:59.551383 zarrnii-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-06-03 13:35:45.008652 zarrnii-0.1.1a1/zarrnii/__init__.py
+-rw-r--r--   0        0        0    16523 2024-06-03 14:25:59.551383 zarrnii-0.1.1a1/zarrnii/core.py
+-rw-r--r--   0        0        0      216 2024-06-03 13:35:45.008652 zarrnii-0.1.1a1/zarrnii/enums.py
+-rw-r--r--   0        0        0     8933 2024-06-03 14:25:59.555383 zarrnii-0.1.1a1/zarrnii/transform.py
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 zarrnii-0.1.1a1/PKG-INFO
```

### Comparing `zarrnii-0.1.0a1/pyproject.toml` & `zarrnii-0.1.1a1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zarrnii"
-version = "0.1.0-alpha.1"
+version = "0.1.1-alpha.1"
 description = "Package for working with OME-Zarr and NIFTI images in a unified manner, with a focus on spatial transformations"
 authors = ["Ali Khan <alik@robarts.ca>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "zarrnii"}]
 
 
@@ -22,14 +22,16 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 poethepoet = "^0.13.1"
 pre-commit = "^2.17.0"
 ruff = "^0.1.14"
 jupyterlab = "^4.2.1"
+matplotlib = "^3.9.0"
+bokeh = "^3.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poe.tasks]
```

### Comparing `zarrnii-0.1.0a1/zarrnii/core.py` & `zarrnii-0.1.1a1/zarrnii/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     axes_nifti: bool = (
         False  # set to true if the axes are ordered for NIFTI (X,Y,Z,C,T)
     )
     
 
     @classmethod
     def from_path_as_ref(
-        cls, path, level=0, channels=[0], chunks=(50, 50, 50), zooms=None
+        cls, path, level=0, channels=[0], chunks='auto', zooms=None
     ):
         """ref image dont need data,  just the shape and affine"""
 
         from .transform import Transform
 
         img_type = cls.check_img_type(path)
         if img_type is ImageType.OME_ZARR:
@@ -44,16 +44,15 @@
                 channels, :, :, :
             ]
             axes_nifti = False
         elif img_type is ImageType.NIFTI:
             darr_base = da.from_array(nib.load(path).get_fdata())
             axes_nifti = True
         else:
-            print("unknown image type")
-            return None
+            raise TypeError("Unsupported image type for ZarrNii")
 
         vox2ras = Transform.vox2ras_from_image(path)
         ras2vox = Transform.ras2vox_from_image(path)
 
         out_shape = [
             len(channels),
             darr_base.shape[-3],
@@ -72,45 +71,46 @@
             np.fill_diagonal(vox2ras.affine[:3, :3], zooms)
 
         ras2vox.affine = np.linalg.inv(vox2ras.affine)
 
         darr_empty = da.empty(
             darr_base,
             shape=out_shape,
-            chunks=(len(channels), chunks[0], chunks[1], chunks[2]),
+            chunks=chunks,
         )
 
         return cls(
             darr_empty, ras2vox=ras2vox, vox2ras=vox2ras, axes_nifti=axes_nifti
         )
 
     @classmethod
-    def from_path(cls, path, level=0, channels=[0], chunks="auto"):
+    def from_path(cls, path, level=0, channels=[0], chunks="auto", rechunk=False):
         """returns a dask array whether a nifti or ome_zarr is provided"""
         from .transform import Transform
 
         img_type = cls.check_img_type(path)
         if img_type is ImageType.OME_ZARR:
             darr = da.from_zarr(path, component=f"/{level}")[channels, :, :, :]
+            if rechunk:
+                darr = darr.rechunk(chunks)
             zi = zarr
             axes_nifti = False
         elif img_type is ImageType.NIFTI:
             darr = da.from_array(
                 np.expand_dims(nib.load(path).get_fdata(), axis=0),
                 chunks=chunks,
             )
             axes_nifti = True
         else:
-            print("unknown image type")
-            return None
+            raise TypeError("Unsupported image type for ZarrNii")
 
         return cls(
             darr,
-            ras2vox=Transform.ras2vox_from_image(path),
-            vox2ras=Transform.vox2ras_from_image(path),
+            ras2vox=Transform.ras2vox_from_image(path,level=level),
+            vox2ras=Transform.vox2ras_from_image(path,level=level),
             axes_nifti=axes_nifti,
         )
 
     @classmethod
     def from_darr(cls, darr, vox2ras=np.eye(4), axes_nifti=False):
         from .transform import Transform
         
@@ -135,52 +135,52 @@
         if suffixes[-1] == ".zarr":
             return ImageType.ZARR
         elif suffixes[-1] == ".nii":
             return ImageType.NIFTI
         else:
             return ImageType.UNKNOWN
 
-    def apply_transform(self, *tfms, ref_dimg):
+    def apply_transform(self, *tfms, ref_znimg):
         """return ZarrNii applying transform to floating image.
         this is a lazy function, doesn't do any work until you compute()
         on the returned dask array.
         """
 
         # tfms already has the transformations to apply,
         # just need the conversion to/from vox/ras at start and end
         tfms_to_apply = []
-        tfms_to_apply.append(ref_dimg.vox2ras)
+        tfms_to_apply.append(ref_znimg.vox2ras)
         for tfm in tfms:
             tfms_to_apply.append(tfm)
         tfms_to_apply.append(self.ras2vox)
 
         # out image in space of ref
-        interp_dimg = ref_dimg
+        interp_znimg = ref_znimg
 
         # perform interpolation on each block in parallel
-        interp_dimg.darr = da.map_blocks(
+        interp_znimg.darr = da.map_blocks(
             interp_by_block,
-            ref_dimg.darr,
+            ref_znimg.darr,
             dtype=np.float32,
             transforms=tfms_to_apply,
-            flo_dimg=self,
+            flo_znimg=self,
         )
 
-        return interp_dimg
+        return interp_znimg
 
     def apply_transform_ref_to_flo_indices(
-        self, *tfms, ref_dimg, indices
+        self, *tfms, ref_znimg, indices
     ):
         """takes indices in ref space, transforms, and provides
         indices in the flo space."""
 
         # tfms already has the transformations to apply, just
         # need the conversion to/from vox/ras at start and end
         tfms_to_apply = []
-        tfms_to_apply.append(ref_dimg.vox2ras)
+        tfms_to_apply.append(ref_znimg.vox2ras)
         for tfm in tfms:
             tfms_to_apply.append(tfm)
         tfms_to_apply.append(self.ras2vox)
 
         # here we use indices as vectors (indices should be 3xN array),
         # we add ones to make 4xN so we can matrix multiply
 
@@ -191,26 +191,26 @@
         for tfm in tfms_to_apply:
             xfm_vecs = tfm.apply_transform(xfm_vecs)
 
         # now we should have vecs in space of ref
         return xfm_vecs[:3, :]
 
     def apply_transform_flo_to_ref_indices(
-        self, *tfms, ref_dimg, indices
+        self, *tfms, ref_znimg, indices
     ):
         """takes indices in flo space, transforms, and
         provides indices in the ref space."""
 
         # tfms already has the transformations to apply,
         # just need the conversion to/from vox/ras at start and end
         tfms_to_apply = []
         tfms_to_apply.append(self.vox2ras)
         for tfm in tfms:
             tfms_to_apply.append(tfm)
-        tfms_to_apply.append(ref_dimg.ras2vox)
+        tfms_to_apply.append(ref_znimg.ras2vox)
 
         homog = np.ones((1, indices.shape[1]))
         xfm_vecs = np.vstack((indices, homog))
 
         # apply tfms_to_apply one at a time
         for tfm in tfms_to_apply:
             xfm_vecs = tfm.apply_transform(xfm_vecs)
@@ -266,71 +266,92 @@
             np.arange(min_extent[0], max_extent[0]),
             np.arange(min_extent[1], max_extent[1]),
             np.arange(min_extent[2], max_extent[2]),
         )
 
         return (grid_points, subvol)
 
+    def as_Nifti1Image(self, filename, **kwargs):
+        
+        return nib.Nifti1Image(self.darr.squeeze(), affine=self.vox2ras.affine)
+    
+        
     def to_nifti(self, filename, **kwargs):
-        if self.axes_nifti:
-            out_darr = self.darr.squeeze().compute(**kwargs)
-            out_affine = self.vox2ras.affine
 
-        else:
-            # we need to convert to nifti convention
-            # (XYZ by reordering and negating)
-            out_darr = (
-                da.flip(da.moveaxis(self.darr, (0, 1, 2, 3), (0, 3, 2, 1)))
-                .squeeze()
-                .compute(**kwargs)
-            )
-            voxdim = np.diag(np.flip(self.vox2ras.affine[:3, :3], axis=0))
+        if self.axes_nifti: #this means it was read-in as a NIFTI, so we write out as normal
+            out_darr = self.darr.squeeze()
+            affine = self.vox2ras.affine
 
-            voxdim = -voxdim[::-1]
-            out_affine = np.diag(np.hstack((voxdim, 1)))
-            #add back the offset offset 
-            out_affine[:3,3] = -self.vox2ras.affine[:3,3]
-
-        out_nib = nib.Nifti1Image(out_darr, affine=out_affine)
+        else: #was read-in as a Zarr, so we reorder/flip data, and adjust affine accordingly
+    
+            out_darr = da.flip(
+                    da.moveaxis(self.darr, (0, 1, 2, 3), (0, 3, 2, 1))
+            ).squeeze()
+            #adjust affine accordingly
+    
+            # reorder_xfm -- changes from z,y,x to x,y,z ordering
+            reorder_xfm = np.eye(4)
+            reorder_xfm[:3, :3] = np.flip(
+                reorder_xfm[:3, :3], axis=0
+            )  # reorders z-y-x to x-y-z and vice versa
+            
+            flip_xfm = np.diag((-1,-1,-1,1))
+    
+            affine = reorder_xfm @ flip_xfm @ self.vox2ras.affine
+            
+        
+        out_nib = nib.Nifti1Image(out_darr, affine=affine)
         out_nib.to_filename(filename)
 
     def to_ome_zarr(
         self, filename, max_layer=4, scaling_method="local_mean", **kwargs
     ):
-        offset=self.vox2ras.affine[:3,3]
+        #the affine specifies how to go from the darr to nifti RAS space
 
-        if (
-            self.axes_nifti
-        ):  # double check to see if this is needed, add a test too..
-            voxdim = np.diag(self.vox2ras.affine)[:3]
+        #in creating affine for zarr, we had to apply scale, translation
+        # then reorder, flip
 
-            # if the reference image came from nifti space, we need to
-            # swap axes ordering and flip
-            if voxdim[0] < 0:
-                out_darr = da.moveaxis(self.darr, (0, 1, 2, 3), (0, 3, 2, 1))
-                voxdim = -voxdim[::-1]
-                offset=offset[::-1]
+        # we can apply steps 
 
-            else:
-                out_darr = da.flip(
+        
+        offset=self.vox2ras.affine[:3,3]
+
+        if self.axes_nifti:
+            #we have a nifti image -- need to apply the transformations (reorder, flip) to the 
+            # data in the OME_Zarr, so it is consistent.
+            out_darr = da.flip(
                     da.moveaxis(self.darr, (0, 1, 2, 3), (0, 3, 2, 1))
-                )
-                voxdim = voxdim[::-1]
-                offset=offset[::-1]
+            )
         else:
-            voxdim = np.diag(np.flip(self.vox2ras.affine[:3, :3], axis=0))
             out_darr = self.darr
-            offset=offset[::-1]
-            voxdim = -voxdim
+
+        
+        if self.vox2ras.affine[1,1]>0:
+            #we have voxdims on the diagonal
+            voxdim = np.diag(self.vox2ras.affine)[:3]
+        else:
+            
+            # reorder_xfm -- changes from z,y,x to x,y,z ordering
+            reorder_xfm = np.eye(4)
+            reorder_xfm[:3, :3] = np.flip(
+                reorder_xfm[:3, :3], axis=0
+            )  # reorders z-y-x to x-y-z and vice versa
+            
+            flip_xfm = np.diag((-1,-1,-1,1))
+    
+            affine_zarr = reorder_xfm @ flip_xfm @ self.vox2ras.affine
+
+            voxdim = np.diag(affine_zarr)[:3]
+
 
         coordinate_transformations = []
         # for each resolution (dataset), we have a list of dicts,
         # transformations to apply..
         # in this case just a single one (scaling by voxel size)
-
+        
         for layer in range(max_layer + 1):
             coord_transform_layer=[]
             #add scale
             coord_transform_layer.append(
                     {
                         "scale": [
                             1,
@@ -372,28 +393,96 @@
                 image=out_darr.rechunk(),
                 group=group,
                 scaler=scaler,
                 coordinate_transformations=coordinate_transformations,
                 axes=axes,
             )
 
-    def crop_with_bounding_box(self, bbox_min, bbox_max):
+    def crop_with_bounding_box(self, bbox_min, bbox_max, ras_coords=False):
         # adjust darr using slicing with bbox indices
         # bbox_min and bbox_max are tuples 
+
+        if ras_coords:
+            #get vox coords by using ras2vox
+            bbox_min = np.round(self.ras2vox @ np.array(bbox_min))
+            bbox_max = np.round(self.ras2vox @ np.array(bbox_max))
+            bbox_min = tuple(bbox_min[:3].flatten())
+            bbox_max = tuple(bbox_max[:3].flatten())        
+
         darr_cropped = self.darr[:,
                 bbox_min[0]:bbox_max[0],
                 bbox_min[1]:bbox_max[1],
                 bbox_min[2]:bbox_max[2]]
 
-        # bbox is indices (ie voxels), so need to convert to ras
+        trans_vox = np.eye(4,4)
+        trans_vox[:3,3] = bbox_min
+        
+        new_vox2ras = self.vox2ras.affine @ trans_vox
+        
+        return ZarrNii.from_darr(darr_cropped,vox2ras=new_vox2ras,axes_nifti=self.axes_nifti)
+
+        
+    def get_bounding_box_around_label(self,label_number, padding=0, ras_coords=False):
+        
+        indices = da.argwhere(self.darr==label_number).compute()
+
+        # Compute the minimum and maximum extents in each dimension
+        bbox_min = indices.min(axis=0).reshape((4,1))[1:] - padding
+        bbox_max = indices.max(axis=0).reshape((4,1))[1:] + 1 + padding
+
+        #clip the data in case padding puts it out of bounds
+        bbox_min = np.clip(bbox_min,np.zeros((3,1)),np.array(self.darr.shape[1:]).reshape(3,1))
+        bbox_max = np.clip(bbox_max,np.zeros((3,1)),np.array(self.darr.shape[1:]).reshape(3,1))
+        
+        if ras_coords:
+            bbox_min = self.vox2ras @ np.array(bbox_min)
+            bbox_max = self.vox2ras @ np.array(bbox_max)
+            
+        return (bbox_min,bbox_max)
+
+        
+
+
+    def downsample(self,along_x=1,along_y=1,along_z=1):
+        """ downsamples by local mean"""
 
+        if self.axes_nifti:
+            axes ={0:1, 
+                                                        1: along_x,
+                                                        2: along_y,
+                                                        3: along_z}
+        else:
+            axes ={0:1, 
+                                                        1: along_z,
+                                                        2: along_y,
+                                                        3: along_x}
+
+        #coarsen performs a reduction in a local neighbourhood, defined by axes
+        darr_scaled = da.coarsen(np.mean,x=self.darr,axes=axes, trim_excess=True)
+        
+        
+        #we need to also update the affine, scaling by the ds_factor
+        scaling_matrix = np.diag((along_x,along_y,along_z,1))
+        new_vox2ras = scaling_matrix @ self.vox2ras.affine
 
-        offset_indices = np.array(bbox_min).reshape(3,1)        
-        homog = np.ones((1, offset_indices.shape[1]))
-        vecs = np.vstack((offset_indices, homog))
+        return ZarrNii.from_darr(darr_scaled,vox2ras=new_vox2ras,axes_nifti=self.axes_nifti)
 
-        xfm_vecs = self.vox2ras.apply_transform(vecs)
 
-        offset_vox2ras = self.vox2ras.affine
-        offset_vox2ras[:3,3]=-xfm_vecs[:3,0]
+    """ WIP 
+    def set_zooms(self,along_x=1,along_y=1,along_z=1):
+        
+        if self.axes_nifti:
+            new_shape = [self.darr.shape[1]
+        
+    new_shape = tuple(int(dim * zoom) for dim, zoom in zip(dask_array.shape, zoom_factors))
 
-        return ZarrNii.from_darr(darr_cropped,vox2ras=offset_vox2ras,axes_nifti=self.axes_nifti)
+        
+        #we need to also update the affine, scaling by the ds_factor
+        scaling_matrix = np.diag((],1))
+        new_vox2ras = scaling_matrix @ self.vox2ras.affine
+        
+
+        return ZarrNii.from_darr(darr_scaled,vox2ras=new_vox2ras,axes_nifti=self.axes_nifti)
+        """
+
+
+
```

### Comparing `zarrnii-0.1.0a1/zarrnii/transform.py` & `zarrnii-0.1.1a1/zarrnii/transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,21 +27,26 @@
     def affine_ras_from_txt(cls, path, invert=False):
         affine = np.loadtxt(path)
         if invert:
             affine = np.linalg.inv(self.affine)
 
         return cls(TransformType.AFFINE_RAS, affine=affine)
 
+
+    
     @classmethod
     def affine_ras_from_array(cls, affine, invert=False):
         if invert:
             affine = np.linalg.inv(affine)
 
         return cls(TransformType.AFFINE_RAS, affine=affine)
 
+    
+
+    
     @classmethod
     def displacement_from_nifti(cls, path):
         disp_nib = nib.load(path)
         disp_xyz = disp_nib.get_fdata().squeeze()
         disp_ras2vox = np.linalg.inv(disp_nib.affine)
 
         # convert from itk transform
@@ -73,16 +78,15 @@
                 affine=cls.get_vox2ras_zarr(path, level),
             )
         elif img_type is ImageType.NIFTI:
             return cls(
                 TransformType.AFFINE_RAS, affine=cls.get_vox2ras_nii(path)
             )
         else:
-            print("unknown image type for vox2ras")
-            return None
+            raise TypeError("Unsupported image type for vox2ras_from_image()")
 
     @classmethod
     def ras2vox_from_image(cls, path: str, level=0):
         from .core import ZarrNii
 
         img_type = ZarrNii.check_img_type(path)
         if img_type is ImageType.OME_ZARR:
@@ -91,17 +95,39 @@
                 affine=cls.get_ras2vox_zarr(path, level),
             )
         elif img_type is ImageType.NIFTI:
             return cls(
                 TransformType.AFFINE_RAS, affine=cls.get_ras2vox_nii(path)
             )
         else:
-            print("unknown image type for ras2vox")
-            return None
+            raise TypeError("Unsupported image type for ras2vox_from_image()")
 
+    def __matmul__(self, other):
+
+        if self.tfm_type == TransformType.AFFINE_RAS and isinstance(other, np.ndarray):
+            if other.shape == (3,) or other.shape == (3, 1):
+                # Convert 3D point/vector to homogeneous coordinates
+                homog_point = np.append(other, 1)
+                result = self.affine @ homog_point
+                # Convert back from homogeneous coordinates to 3D
+                return result[:3] / result[3]
+            elif other.shape == (4,) or other.shape == (4, 1):
+                # Directly use 4D point/vector
+                result = self.affine @ other
+                # Convert back from homogeneous coordinates to 3D
+                return result[:3] / result[3]
+            elif other.shape == (4,4):
+                #perform matrix multiplication, and return a Transform object
+                return Transform.affine_ras_from_array(self.affine @ other)
+            else:
+                raise ValueError("Unsupported shape for multiplication.")
+        else:
+            raise TypeError("Unsupported type for multiplication.")
+    
+    
     @staticmethod
     def get_vox2ras_nii(in_nii_path: str) -> np.array:
         return nib.load(in_nii_path).affine
 
     @staticmethod
     def get_ras2vox_nii(in_nii_path: str) -> np.array:
         return np.linalg.inv(Transform.get_vox2ras_nii(in_nii_path))
@@ -112,30 +138,41 @@
         zi = zarr.open(in_zarr_path)
         attrs = zi["/"].attrs.asdict()
         multiscale = 0  # first multiscale image
         transforms = attrs["multiscales"][multiscale]["datasets"][level][
             "coordinateTransformations"
         ]
 
+        affine = np.eye(4)
+
+        #apply each ome zarr transform sequentially
+        for transform in transforms:
+        # (for now, we just assume the transformations will be called scale and translation)
+            if transform['type'] == "scale":
+                scaling_zyx = transform["scale"][1:]
+                scaling_xfm = np.diag(np.hstack((scaling_zyx,1)))
+                affine = scaling_xfm @ affine
+            elif transform['type'] == "translation":
+                translation_xfm = np.eye(4)
+                translation_xfm[:3,3] = transform["translation"][1:]
+                affine = translation_xfm @ affine
+            
         # reorder_xfm -- changes from z,y,x to x,y,z ordering
         reorder_xfm = np.eye(4)
         reorder_xfm[:3, :3] = np.flip(
             reorder_xfm[:3, :3], axis=0
         )  # reorders z-y-x to x-y-z and vice versa
 
-        # scaling xfm
-        scaling_xfm = np.eye(4)
-        scaling_xfm[0, 0] = -transforms[0]["scale"][
-            -1
-        ]  # x  # 0-index in transforms is the first (and only) transform
-        scaling_xfm[1, 1] = -transforms[0]["scale"][-2]  # y
-        scaling_xfm[2, 2] = -transforms[0]["scale"][-3]  # z
-
-        return scaling_xfm @ reorder_xfm
-
+        affine = reorder_xfm @ affine
+        
+        flip_xfm = np.diag((-1,-1,-1,1))
+        affine = flip_xfm @ affine
+        
+        return affine
+        
     @staticmethod
     def get_ras2vox_zarr(in_zarr_path: str, level=0) -> np.array:
         return np.linalg.inv(
             Transform.get_vox2ras_zarr(in_zarr_path, level=level)
         )
 
     def apply_transform(self, vecs: np.array) -> np.array:
@@ -163,15 +200,15 @@
 
             return vecs + disp_vecs
 
 
 def interp_by_block(
     x,
     transforms: list[Transform],
-    flo_dimg: ZarrNii,
+    flo_znimg: ZarrNii,
     block_info=None,
     interp_method="linear",
 ):
     """
     main idea here is we take coordinates from the current block (ref image)
     transform them, then in that transformed space, then interpolate the
     floating image intensities
@@ -203,15 +240,15 @@
 
     # then finally interpolate those points on the template dseg volume
     # need to interpolate for each channel
 
     interpolated = np.zeros(x.shape)
 
     # find bounding box required for flo vol
-    (grid_points, flo_vol) = flo_dimg.get_bounded_subregion(xfm_vecs)
+    (grid_points, flo_vol) = flo_znimg.get_bounded_subregion(xfm_vecs)
     if grid_points is None and flo_vol is None:
         # points were fully outside the floating image, so just return zeros
         return interpolated
     else:
         for c in range(flo_vol.shape[0]):
             interpolated[c, :, :, :] = (
                 interpn(
```

### Comparing `zarrnii-0.1.0a1/PKG-INFO` & `zarrnii-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarrnii
-Version: 0.1.0a1
+Version: 0.1.1a1
 Summary: Package for working with OME-Zarr and NIFTI images in a unified manner, with a focus on spatial transformations
 License: MIT
 Author: Ali Khan
 Author-email: alik@robarts.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

