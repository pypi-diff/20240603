# Comparing `tmp/scalebar-0.3.1.tar.gz` & `tmp/scalebar-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalebar-0.3.1.tar", last modified: Wed Mar  6 14:27:25 2024, max compression
+gzip compressed data, was "scalebar-0.4.0.tar", last modified: Mon Jun  3 09:51:34 2024, max compression
```

## Comparing `scalebar-0.3.1.tar` & `scalebar-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-03-06 14:27:25.408903 scalebar-0.3.1/
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)    34523 2024-02-22 11:58:24.000000 scalebar-0.3.1/LICENSE
--rw-r--r--   0 dkorsch   (1001) dkorsch   (1001)      325 2024-03-06 14:27:25.408903 scalebar-0.3.1/PKG-INFO
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1781 2024-02-22 11:58:24.000000 scalebar-0.3.1/README.md
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       55 2024-02-22 11:58:24.000000 scalebar-0.3.1/requirements.txt
-drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-03-06 14:27:25.408903 scalebar-0.3.1/scalebar/
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)      139 2024-02-22 11:58:24.000000 scalebar-0.3.1/scalebar/__init__.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       22 2024-03-06 14:27:23.000000 scalebar-0.3.1/scalebar/_version.py
-drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-03-06 14:27:25.408903 scalebar-0.3.1/scalebar/core/
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        0 2024-02-22 11:58:24.000000 scalebar-0.3.1/scalebar/core/__init__.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     5312 2024-02-22 11:58:24.000000 scalebar-0.3.1/scalebar/core/estimation.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     2288 2024-03-06 14:12:07.000000 scalebar-0.3.1/scalebar/core/position.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1157 2024-02-22 11:58:24.000000 scalebar-0.3.1/scalebar/estimate.py
-drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-03-06 14:27:25.408903 scalebar-0.3.1/scalebar/utils/
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)      674 2024-03-06 13:19:19.000000 scalebar-0.3.1/scalebar/utils/__init__.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     2078 2024-02-22 11:58:24.000000 scalebar-0.3.1/scalebar/utils/corner_ops.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)      311 2024-02-22 11:58:24.000000 scalebar-0.3.1/scalebar/utils/image_ops.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1836 2024-03-06 14:13:45.000000 scalebar-0.3.1/scalebar/utils/pattern.py
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     2568 2024-02-26 12:51:06.000000 scalebar-0.3.1/scalebar/visualize.py
-drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-03-06 14:27:25.408903 scalebar-0.3.1/scalebar.egg-info/
--rw-r--r--   0 dkorsch   (1001) dkorsch   (1001)      325 2024-03-06 14:27:25.000000 scalebar-0.3.1/scalebar.egg-info/PKG-INFO
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)      508 2024-03-06 14:27:25.000000 scalebar-0.3.1/scalebar.egg-info/SOURCES.txt
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        1 2024-03-06 14:27:25.000000 scalebar-0.3.1/scalebar.egg-info/dependency_links.txt
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        1 2024-02-22 11:59:40.000000 scalebar-0.3.1/scalebar.egg-info/not-zip-safe
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       55 2024-03-06 14:27:25.000000 scalebar-0.3.1/scalebar.egg-info/requires.txt
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        9 2024-03-06 14:27:25.000000 scalebar-0.3.1/scalebar.egg-info/top_level.txt
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       38 2024-03-06 14:27:25.408903 scalebar-0.3.1/setup.cfg
--rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)      830 2024-02-22 11:58:24.000000 scalebar-0.3.1/setup.py
+drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-06-03 09:51:34.122048 scalebar-0.4.0/
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)    34523 2024-02-22 11:58:24.000000 scalebar-0.4.0/LICENSE
+-rw-r--r--   0 dkorsch   (1001) dkorsch   (1001)      325 2024-06-03 09:51:34.122048 scalebar-0.4.0/PKG-INFO
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1781 2024-02-22 11:58:24.000000 scalebar-0.4.0/README.md
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       55 2024-02-22 11:58:24.000000 scalebar-0.4.0/requirements.txt
+drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-06-03 09:51:34.122048 scalebar-0.4.0/scalebar/
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       91 2024-06-03 09:14:42.000000 scalebar-0.4.0/scalebar/__init__.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       22 2024-06-03 09:12:49.000000 scalebar-0.4.0/scalebar/_version.py
+drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-06-03 09:51:34.122048 scalebar-0.4.0/scalebar/core/
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        0 2024-02-22 11:58:24.000000 scalebar-0.4.0/scalebar/core/__init__.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1939 2024-06-03 08:21:28.000000 scalebar-0.4.0/scalebar/core/bounding_box.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     5267 2024-06-03 09:28:09.000000 scalebar-0.4.0/scalebar/core/estimation.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1882 2024-06-03 09:15:46.000000 scalebar-0.4.0/scalebar/core/image_wrapper.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     2288 2024-03-06 14:12:07.000000 scalebar-0.4.0/scalebar/core/position.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1092 2024-06-03 09:50:43.000000 scalebar-0.4.0/scalebar/estimate.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     4265 2024-05-31 13:00:37.000000 scalebar-0.4.0/scalebar/example.py
+drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-06-03 09:51:34.122048 scalebar-0.4.0/scalebar/utils/
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1020 2024-06-03 09:18:05.000000 scalebar-0.4.0/scalebar/utils/__init__.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     2078 2024-02-22 11:58:24.000000 scalebar-0.4.0/scalebar/utils/corner_ops.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     4303 2024-06-03 09:19:11.000000 scalebar-0.4.0/scalebar/utils/image_ops.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     1836 2024-03-06 14:13:45.000000 scalebar-0.4.0/scalebar/utils/pattern.py
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)     3271 2024-06-03 09:50:20.000000 scalebar-0.4.0/scalebar/visualize.py
+drwxrwxr-x   0 dkorsch   (1001) dkorsch   (1001)        0 2024-06-03 09:51:34.122048 scalebar-0.4.0/scalebar.egg-info/
+-rw-r--r--   0 dkorsch   (1001) dkorsch   (1001)      325 2024-06-03 09:51:34.000000 scalebar-0.4.0/scalebar.egg-info/PKG-INFO
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)      589 2024-06-03 09:51:34.000000 scalebar-0.4.0/scalebar.egg-info/SOURCES.txt
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        1 2024-06-03 09:51:34.000000 scalebar-0.4.0/scalebar.egg-info/dependency_links.txt
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        1 2024-02-22 11:59:40.000000 scalebar-0.4.0/scalebar.egg-info/not-zip-safe
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       55 2024-06-03 09:51:34.000000 scalebar-0.4.0/scalebar.egg-info/requires.txt
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)        9 2024-06-03 09:51:34.000000 scalebar-0.4.0/scalebar.egg-info/top_level.txt
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)       38 2024-06-03 09:51:34.122048 scalebar-0.4.0/setup.cfg
+-rw-rw-r--   0 dkorsch   (1001) dkorsch   (1001)      830 2024-02-22 11:58:24.000000 scalebar-0.4.0/setup.py
```

### Comparing `scalebar-0.3.1/LICENSE` & `scalebar-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scalebar-0.3.1/README.md` & `scalebar-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `scalebar-0.3.1/scalebar/core/estimation.py` & `scalebar-0.4.0/scalebar/core/estimation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,143 @@
 import cv2
 import numpy as np
 import typing as T
 
+from matplotlib import pyplot as plt
 from scipy.spatial.distance import pdist
-from skimage import feature
+from PIL import Image
+from dataclasses import dataclass
 
-from scalebar.core.position import Position
-from scalebar.utils import corner_ops
+from scalebar import utils
+from scalebar.core.bounding_box import BoundingBox
+from scalebar.core.image_wrapper import Images
+
+@dataclass
+class Result:
+    image_path: str
+    image_size: T.Tuple[int, int] = (0, 0)
+
+    images: T.Optional[Images] = None
+    position: T.Optional[BoundingBox] = None
+    scalebar: T.Optional[np.ndarray] = None
+    px_per_square: T.Optional[float] = None # [px/square]
+
+    roi_fraction: float = 0.2 # fraction of the image's border that will be used for the scale estimation
+    size_per_square: float = 1.0 # [mm/square] how many mm is a single square
+
+    def __post_init__(self):
+        with Image.open(self.image_path) as img:
+            self.image_size = img.size
+        im = utils.read_image(self.image_path)
+        self.images = Images(im, roi_fraction=self.roi_fraction)
+
+    @classmethod
+    def new(cls, file_name: str, *, max_corners: int = 50, **kwargs) -> 'Result':
+        res = cls(file_name, **kwargs)
+        res.locate()
+        res.estimate(max_corners=max_corners)
+        return res
+
+    def locate(self) -> BoundingBox:
+        """ this function will locate the scale bar in the image, store the bounding box, and finally return it """
+        temp_size = self.images.structure_sizes.template_size
+        self.match, self.template = utils.match_scalebar(self.images.masked, template_size=temp_size)
+        self.position = utils.detect_scalebar(self.match, enlarge=temp_size)
+        return self.position
+
+    def estimate(self, max_corners: int = 50) -> float:
+        """ this function will estimate the scale of the image and return it """
+        assert self.position is not None, "Position is required"
+        self.scalebar = self.position.crop(self.images.equalized)
+        mask = self.position.crop(self.match)
+        min_distance = self.images.structure_sizes.size
+
+        bin_crop = utils.threshold(self.scalebar, mode=cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+        corners = cv2.goodFeaturesToTrack(bin_crop,
+                                          maxCorners=0 if np.isinf(max_corners) else max_corners,
+                                          qualityLevel=0.1,
+                                          minDistance=min_distance,
+                                          mask=mask)
 
-
-def get_scale(img: np.ndarray,
-              pos: Position = Position.top_right,
-              crop_size: float = 0.2,
-              crop_square: bool = False,
-              square_unit: float = 1.0,
-              min_dist: int = 5,
-              max_corners: int = np.inf,
-              cv2_corners: bool = True,
-              filter_corners: bool = False,
-              rectify_corners: bool = False,
-              binarize: bool = False,
-              return_intermediate: bool = False) -> T.Optional[float]:
-    """
-        Estimates the scale from the image in pixel per mm
-
-        Arguments:
-            img: input image
-            pos: position of the scale bar in the image
-            square_unit: length of a single square in the scale bar in mm
-            min_dist: minimum distance in pixel between two corners
-            max_corners: maximum amount of corners that will be estimated
-            cv2_corners: flag to use the cv2 implementation (if True)
-                or the scikit-image implementation (if False, default)
-
-        Returns:
-            scale: scaling factor in pixel per mm
-            intermediate: (optional) returns intermediate estimations
-                as dictionary with following keys:
-                    * detected_corners
-                    * filter_mask
-                    * rectification_angle
-                    * final_corners
-    """
-    if isinstance(crop_size, float):
-        crop_x = crop_y = crop_size
-    elif isinstance(crop_size, (tuple, list)):
-        crop_x, crop_y = crop_size
-    else:
-        raise ValueError(f"Unsupported crop size type: {crop_size=} (of type {type(crop_size).__name__})!")
-    crop = pos.crop(img, x=crop_x, y=crop_y, square=crop_square)
-
-    intermediate = dict(
-        init_crop=crop,
-        detected_corners=None,
-        filter_mask=None,
-        rectification_angle=None,
-        final_corners=None,
-    )
-
-    crop = cv2.cvtColor(crop, cv2.COLOR_RGB2GRAY)
-
-    if binarize:
-        blur = cv2.GaussianBlur(crop, (5,5),0)
-        thresh, crop = cv2.threshold(blur,0,255,cv2.THRESH_BINARY+cv2.THRESH_OTSU)
-
-    intermediate["crop"] = crop
-
-    if cv2_corners:
-        # OpenCV's corner/feature detector
-        corners = cv2.goodFeaturesToTrack(crop, 0 if np.isinf(max_corners) else max_corners, 0.5, min_dist)
-        # termination criteria
         criteria = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 30, 0.001)
-        corners = cv2.cornerSubPix(crop, corners, (11,11), (-1,-1), criteria)
+        shape = (2*min_distance+1, 2*min_distance+1)
+        corners = cv2.cornerSubPix(self.scalebar, corners, shape, (-1,-1), criteria)
         # switch x and y coordinates for convenience (needed only for OpenCV)
         corners = corners[:, 0, ::-1].astype(int)
-    else:
-        # This is from Erik's code
-        resp = feature.corner_shi_tomasi(crop)
-        corners = feature.corner_peaks(resp,
-                                       min_distance=min_dist,
-                                       num_peaks=max_corners)
-    if len(corners) == 0:
-        if return_intermediate:
-            return None, intermediate
-        else:
-            return None
-
-    intermediate["detected_corners"] = corners
-
-    if filter_corners:
-        mask = corner_ops.filter(corners, crop)
-    else:
-        mask = np.ones(len(corners), dtype=bool)    
-
-    intermediate["filter_mask"] = mask
-    corners = corners[mask]
-
-    if rectify_corners:
-        corners, angle = corner_ops.rectify(corners)
-    else:
-        angle = 0.0
-
-    intermediate["rectification_angle"] = angle
-    intermediate["final_corners"] = corners
-
-    distances = pdist(corners, metric="cityblock")
-    if len(distances) != 0:
-        # unit_distance is in "pixel per square-block"
-        unit_distance = optimal_distance(distances)
-
-        scale = unit_distance / square_unit
-    
-    else:
-        scale = None
-
-    if return_intermediate:
-        return scale, intermediate
-    else:
-        return scale
-
-
-def optimal_distance(distances: np.ndarray, step: float = 0.25) -> float:
-    """
-        Estimates the best distance by solving an
-        optimization problem
-    """
-
-    smallest_err = np.inf
-    best_distance = None
-    max_d = np.percentile(distances, 20)
-    min_d = max(1.0, np.percentile(distances, 1))
-
-    for d in np.arange(min_d, max_d):
-        grid = np.arange(0, np.max(distances) + d, d)
-        if len(grid) <= 2:
-            continue
-
-        # compute quantization error
-        bins = (grid[:-1] + grid[1:]) / 2.0
-        prototypes = grid[1:-1]
-        bin_idxs = np.digitize(distances, bins)
-        bin_idxs -= 1
-        bin_idxs[bin_idxs == -1] = 0
-        bin_idxs[bin_idxs == len(prototypes)] = len(prototypes) - 1
-
-        # quantization error with BIC model selection
-        # adhoc version
-        n = len(distances)
-        err = np.linalg.norm(distances - prototypes[bin_idxs]) + \
-            len(prototypes) * np.log(n)
-        # theoretically derived criterion
-        # err = n * np.log(2 * np.pi) + \
-        #     np.linalg.norm(distances - prototypes[bin_idxs])**2 + \
-        #     len(prototypes) * np.log(n)
-
-        if err < smallest_err:
-            smallest_err = err
-            best_distance = d
 
-    return best_distance
+        self.distances = Distances(corners)
+        self.px_per_square = self.distances.optimal_distance()
+
+        return self.scale
+
+    @property
+    def scale(self) -> float:
+        return self.px_per_square / self.size_per_square
+
+
+class Distances:
+    def __init__(self, corners: np.ndarray, metric: str = "cityblock"):
+        self.corners = corners
+        self.distances = pdist(corners, metric=metric)
+
+    def reset(self):
+
+        self.errors = [[], []]
+        self.n_bins = []
+
+        self.unique_dists = sorted(np.unique(np.maximum(self.distances, 10)))
+        self.unique_dists = self.unique_dists[:len(self.unique_dists)//5]
+
+    def optimal_distance(self, use_bic: bool = False) -> float:
+        self.reset()
+        smallest_err = np.inf
+        best_distance = None
+
+        for d in self.unique_dists:
+            norm_dist = self.distances / d
+            grid = np.arange(0, np.max(self.distances) + d, d) / d
+
+            if len(grid) <= 2:
+                print(f"FOO: {d}")
+                continue
+
+            # compute quantization error
+            bins = (grid[:-1] + grid[1:]) / 2.0
+
+            prototypes = grid[1:-1]
+            self.n_bins.append(len(prototypes))
+            bin_idxs = np.digitize(norm_dist, bins)
+
+            bin_idxs -= 1
+            bin_idxs[bin_idxs == -1] = 0
+            bin_idxs[bin_idxs == len(prototypes)] = len(prototypes) - 1
+
+            # theoretically derived criterion
+            # err = n * np.log(2 * np.pi) + \
+            #     np.linalg.norm(distances - prototypes[bin_idxs])**2 + \
+            #     len(prototypes) * np.log(n)
+            # quantization error with BIC model selection
+            # adhoc version
+            n = len(norm_dist)
+            err = np.linalg.norm((norm_dist - prototypes[bin_idxs]))
+            self.errors[0].append(err)
+
+            if use_bic:
+                err = err + len(prototypes) * np.log(n)
+            self.errors[1].append(err)
+
+
+            if err < smallest_err:
+                smallest_err, best_distance = err, d
+
+        return best_distance
+
+    def plot_errors(self, **kwargs)-> T.Tuple[plt.Figure, plt.Axes]:
+        fig, ax = plt.subplots(**kwargs)
+
+        ax.plot(self.unique_dists, self.errors[0], label="err0")
+        ax.plot(self.unique_dists, self.errors[1], label="err1")
+        ax = ax.twinx()
+        ax.plot(self.unique_dists, np.log(self.n_bins), linestyle="dashed",
+                label="# bins")
+
+        return fig, ax
```

### Comparing `scalebar-0.3.1/scalebar/core/position.py` & `scalebar-0.4.0/scalebar/core/position.py`

 * *Files identical despite different names*

### Comparing `scalebar-0.3.1/scalebar/estimate.py` & `scalebar-0.4.0/scalebar/estimate.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,37 +10,35 @@
 with utils.try_import("cvargparse"):
     from cvargparse import Arg
     from cvargparse import BaseParser
 
 
 def main(args):
 
-    im = utils.read_image(args.image_path)
+    res = scalebar.Result.new(args.image_path,
+                              roi_fraction=args.fraction,
+                              size_per_square=args.unit)
 
-    positions = {pos.name.lower(): pos for pos in scalebar.Position}
-    pos = positions[args.position]
-    px_per_mm = scalebar.get_scale(im,
-                                   pos=pos,
-                                   square_unit=args.unit)
+    px_per_mm = res.scale
 
     if args.output:
         assert not os.path.exists(args.output), \
             f"Output file ({args.output}) already exists!"
         with open(args.output, "w") as f:
             f.write(f"{px_per_mm:f}\n")
     else:
         print(px_per_mm)
 
 
 parser = BaseParser([
     Arg("image_path"),
 
-    Arg("--position", "-pos", default="top_right",
-        choices=[pos.name.lower() for pos in scalebar.Position]),
+    Arg.float("--unit", "-u", default=1.0,
+              help="Size of a single square in the scale bar (in mm). Default: 1"),
 
-    Arg("--unit", "-u", type=float, default=1.0,
-        help="Size of a single square in the scale bar (in mm). Default: 1"),
+    Arg.float("--fraction", default=0.1,
+              help="Fraction of the image's border that will be used for the scale estimation. Default: 0.1"),
 
     Arg("--output", "-o")
 ])
 
 main(parser.parse_args())
```

### Comparing `scalebar-0.3.1/scalebar/utils/__init__.py` & `scalebar-0.4.0/scalebar/utils/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import contextlib
 
 from scalebar.utils.image_ops import read_image
+from scalebar.utils.image_ops import equalize
+from scalebar.utils.image_ops import threshold
+from scalebar.utils.image_ops import hide_non_roi
+from scalebar.utils.image_ops import match_scalebar
+from scalebar.utils.image_ops import detect_scalebar
 from scalebar.utils.pattern import create as create_pattern
 from scalebar.utils.pattern import match as match_pattern
 from scalebar.utils.corner_ops import rectify
 from scalebar.utils.corner_ops import filter as filter_corners
 
 
 @contextlib.contextmanager
@@ -18,11 +23,16 @@
         raise
 
 
 __all__ = [
     "try_import",
     "read_image",
     "rectify",
+    "equalize",
+    "threshold",
+    "hide_non_roi",
+    "match_scalebar",
+    "detect_scalebar",
     "create_pattern",
     "match_pattern",
     "filter_corners",
 ]
```

### Comparing `scalebar-0.3.1/scalebar/utils/corner_ops.py` & `scalebar-0.4.0/scalebar/utils/corner_ops.py`

 * *Files identical despite different names*

### Comparing `scalebar-0.3.1/scalebar/utils/pattern.py` & `scalebar-0.4.0/scalebar/utils/pattern.py`

 * *Files identical despite different names*

### Comparing `scalebar-0.3.1/scalebar/visualize.py` & `scalebar-0.4.0/scalebar/visualize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,108 @@
 #!/usr/bin/env python
 if __name__ != '__main__':
     raise Exception("Do not import me!")
 
 import cv2
+import numpy as np
 import logging
 import scalebar
 
 from scalebar import utils
 
 with utils.try_import("cvargparse"):
     from cvargparse import Arg
     from cvargparse import BaseParser
 
 with utils.try_import("matplotlib, pyqt5"):
     from matplotlib import pyplot as plt
 
+def imshow(ims):
 
-def main(args) -> None:
-    fig = plt.figure()
+    if len(ims) <= 3:
+        nrows, ncols = 1, len(ims)
+    else:
+        nrows = int(np.ceil(np.sqrt(len(ims))))
+        ncols = int(np.ceil( len(ims) / nrows))
 
-    im = utils.read_image(args.image_path)
-    H, W, *C = im.shape
+    fig, axs = plt.subplots(ncols=ncols, nrows=nrows,
+                            figsize=(16,9), squeeze=False)
+    for i, (title, im, cmap) in enumerate(ims):
+        ax = axs[np.unravel_index(i, axs.shape)]
+
+        if isinstance(im, (list, tuple)):
+            alpha = 1 / len(im)
+            for _im, _cm in zip(im, cmap):
+                ax.imshow(_im, cmap=_cm, alpha=alpha)
+        else:
+            ax.imshow(im, cmap=cmap)
+        ax.set_title(title)
+
+    for _ in range(i+1, nrows*ncols):
+        ax = axs[np.unravel_index(_, axs.shape)]
+        ax.axis("off")
 
-    grid = plt.GridSpec(3, 2)
+    return fig, axs
+
+def main(args) -> None:
+    logging.info(f"Processing {args.image_path}")
+    res = scalebar.Result.new(args.image_path,
+                              roi_fraction=args.fraction,
+                              size_per_square=args.unit)
+
+    images = res.images
+    ROI = utils.hide_non_roi(images.binary, res.roi_fraction, 127)
+    scalebar_crop = res.position.crop(images.equalized)
+    px_per_mm = res.scale
+
+    logging.info(f"Estimated Pixel per square: {res.px_per_square:.2f}")
+    logging.info(f"Used size per square: {res.size_per_square:.2f}")
+    logging.info(f"Result: {px_per_mm:.2f} px/mm | Image size: {res.image_size} | ")
+
+    logging.info("Plotting results")
+    fig, axs = imshow([
+        ("Original", images.original, None),
+        ("B/W image", images.gray, plt.cm.gray),
+        ("B/W image equalized", images.equalized, plt.cm.gray),
+
+        ("Binarized", images.binary, plt.cm.gray),
+        ("ROI to be masked", ROI, plt.cm.gray),
+        ("Masked", images.masked, plt.cm.gray),
+
+        ("Template Matches", (
+            images.binary,
+            res.match), (plt.cm.gray, plt.cm.viridis)),
+        (f"Scalebar | {res.scale} px/mm", scalebar_crop, plt.cm.gray),
+    ])
 
-    ax = plt.subplot(grid[:1, :])
-    ax.axis("off")
-    ax.imshow(im)
-    ax.set_title("Input image")
-
-    positions = {pos.name.lower(): pos for pos in scalebar.Position}
-    pos = positions[args.position]
-    crop = pos.crop(im)
-    result = scalebar.get_scale(im,
-                                pos=pos,
-                                square_unit=args.unit,
-                                return_intermediate=True)
-
-    if result is None:
-        logging.info("Cannot estimate the scale in the given image!")
-
-    px_per_mm, interm = result
-
-    init_corners = interm["detected_corners"]
-    mask = interm["filter_mask"]
-    angle = interm["rectification_angle"]
-    corners = interm["final_corners"]
-
-    ax = plt.subplot(grid[-2:, 0])
-    ax.axis("off")
-    ax.imshow(crop)
-    ax.set_title("Original crop")
-
-    ys, xs = init_corners[mask].transpose(1, 0)
-    ax.scatter(xs, ys, marker=".", c="red", label="used")
-    ys, xs = init_corners[~mask].transpose(1, 0)
-    ax.scatter(xs, ys, marker=".", c="blue", alpha=0.7, label="rejected")
-    ax.legend(loc="upper right")
-
-    ax = plt.subplot(grid[-2:, 1])
-
-    rot_mat = cv2.getRotationMatrix2D([0, 0], angle, 1.0)
-    new_crop = cv2.warpAffine(crop, rot_mat, crop.shape[:2])
-
-    ax.imshow(new_crop)
-    ax.axis("off")
-    ax.set_title("Rectified crop")
-    ys, xs = corners.transpose(1, 0)
+    ax = axs[np.unravel_index(7, axs.shape)]
+    ys, xs = res.distances.corners.transpose(1, 0)
     ax.scatter(xs, ys, marker=".", c="red")
 
+    W, H = res.image_size
     if px_per_mm is None:
         fig.suptitle("Estimation Failed!")
     else:
         size = W / px_per_mm, H / px_per_mm
         fig.suptitle(" | ".join(
             [
                 f"{px_per_mm:.2f} px/mm",
                 f"Image size: {size[0]:.2f} x {size[1]:.2f}mm"
             ]))
 
     plt.tight_layout()
-    plt.show()
+    if args.output is not None:
+        logging.info(f"Saving results to {args.output}")
+        plt.savefig(args.output)
+    else:
+        plt.show()
     plt.close()
 
 
 parser = BaseParser([
     Arg("image_path"),
-
-    Arg("--position", "-pos", default="top_right",
-        choices=[pos.name.lower() for pos in scalebar.Position]),
-
     Arg("--unit", "-u", type=float, default=1.0,
         help="Size of a single square in the scale bar (in mm). Default: 1"),
+    Arg.float("--fraction", default=0.1),
+    Arg("--output", "-o"),
 ])
 main(parser.parse_args())
```

### Comparing `scalebar-0.3.1/setup.py` & `scalebar-0.4.0/setup.py`

 * *Files identical despite different names*

