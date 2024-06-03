# Comparing `tmp/MedicalImageConverter-1.4.tar.gz` & `tmp/medicalimageconverter-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedicalImageConverter-1.4.tar", last modified: Wed Apr 10 23:46:05 2024, max compression
+gzip compressed data, was "medicalimageconverter-1.5.tar", last modified: Mon Jun  3 00:42:03 2024, max compression
```

## Comparing `MedicalImageConverter-1.4.tar` & `medicalimageconverter-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 23:46:05.415540 MedicalImageConverter-1.4/
--rw-rw-rw-   0        0        0    35821 2023-07-22 22:51:40.000000 MedicalImageConverter-1.4/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 23:46:05.332920 MedicalImageConverter-1.4/MedicalImageConverter/
--rw-rw-rw-   0        0        0      102 2023-07-23 20:35:17.000000 MedicalImageConverter-1.4/MedicalImageConverter/__init__.py
--rw-rw-rw-   0        0        0      690 2023-07-26 23:11:11.000000 MedicalImageConverter-1.4/MedicalImageConverter/memory.py
--rw-rw-rw-   0        0        0     1343 2024-02-23 14:56:25.000000 MedicalImageConverter-1.4/MedicalImageConverter/parsar.py
--rw-rw-rw-   0        0        0    24481 2024-04-10 23:39:01.000000 MedicalImageConverter-1.4/MedicalImageConverter/reader.py
-drwxrwxrwx   0        0        0        0 2024-04-10 23:46:05.392641 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/
--rw-rw-rw-   0        0        0     4327 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4327 2024-04-10 23:46:05.403593 MedicalImageConverter-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3840 2023-09-03 04:16:10.000000 MedicalImageConverter-1.4/README.md
--rw-rw-rw-   0        0        0       97 2023-07-23 20:12:24.000000 MedicalImageConverter-1.4/pyproject.toml
--rw-rw-rw-   0        0        0      592 2024-04-10 23:46:05.419522 MedicalImageConverter-1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 00:42:03.876525 medicalimageconverter-1.5/
+-rw-rw-rw-   0        0        0    35821 2023-07-22 22:51:40.000000 medicalimageconverter-1.5/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 00:42:03.771986 medicalimageconverter-1.5/MedicalImageConverter/
+-rw-rw-rw-   0        0        0      102 2023-07-23 20:35:17.000000 medicalimageconverter-1.5/MedicalImageConverter/__init__.py
+-rw-rw-rw-   0        0        0      690 2023-07-26 23:11:11.000000 medicalimageconverter-1.5/MedicalImageConverter/memory.py
+-rw-rw-rw-   0        0        0     1343 2024-02-23 14:56:25.000000 medicalimageconverter-1.5/MedicalImageConverter/parsar.py
+-rw-rw-rw-   0        0        0    23145 2024-06-03 00:39:20.000000 medicalimageconverter-1.5/MedicalImageConverter/reader.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:42:03.849643 medicalimageconverter-1.5/MedicalImageConverter.egg-info/
+-rw-rw-rw-   0        0        0     4327 2024-06-03 00:42:03.000000 medicalimageconverter-1.5/MedicalImageConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2024-06-03 00:42:03.000000 medicalimageconverter-1.5/MedicalImageConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 00:42:03.000000 medicalimageconverter-1.5/MedicalImageConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-06-03 00:42:03.000000 medicalimageconverter-1.5/MedicalImageConverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4327 2024-06-03 00:42:03.862586 medicalimageconverter-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3840 2023-09-03 04:16:10.000000 medicalimageconverter-1.5/README.md
+-rw-rw-rw-   0        0        0       97 2023-07-23 20:12:24.000000 medicalimageconverter-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      592 2024-06-03 00:42:03.880507 medicalimageconverter-1.5/setup.cfg
```

### Comparing `MedicalImageConverter-1.4/LICENSE.txt` & `medicalimageconverter-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.4/MedicalImageConverter/memory.py` & `medicalimageconverter-1.5/MedicalImageConverter/memory.py`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.4/MedicalImageConverter/parsar.py` & `medicalimageconverter-1.5/MedicalImageConverter/parsar.py`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.4/MedicalImageConverter/reader.py` & `medicalimageconverter-1.5/MedicalImageConverter/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     The CT and MR modalities have been tested extensively, along with their respective ROIs. The other 7 modalities
     have been tested but only on a few datasets a piece. For RTSTRUCTS, only those referencing CT and MR have been
     tested.
 """
 
 import os
 import time
+import gdcm
 import threading
 
 import numpy as np
 import pandas as pd
 import pydicom as dicom
 
 
@@ -90,20 +91,22 @@
         self.ds_images = []
         self.ds_dictionary = dict.fromkeys(['CT', 'MR', 'PT', 'US', 'DX', 'MG', 'NM', 'XA', 'CR', 'RTSTRUCT'])
         self.rt_df = pd.DataFrame(columns=['FilePath', 'SeriesInstanceUID', 'RoiSOP', 'RoiNames'])
 
         keep_tags = ['FilePath', 'SOPInstanceUID', 'PatientID', 'PatientName', 'Modality',
                      'SeriesDescription', 'SeriesDate', 'SeriesTime', 'SeriesInstanceUID', 'SeriesNumber',
                      'AcquisitionNumber', 'SliceThickness', 'PixelSpacing', 'Rows', 'Columns', 'PatientPosition',
-                     'ImagePositionPatient', 'ImageOrientationPatient', 'Slices', 'DefaultWindow', 'FullWindow']
+                     'ImagePositionPatient', 'ImageOrientationPatient', 'ImageMatrix', 'Slices', 'DefaultWindow',
+                     'FullWindow']
         self.image_info = pd.DataFrame(columns=keep_tags)
         self.image_data = []
 
         self.roi_info = pd.DataFrame(columns=['FilePath', 'RoiNames'])
         self.roi_contour = []
+        self.roi_pixel_position = []
 
         self.contours = []
 
     def add_dicom_extension(self):
         """
         Will add .dcm extension to any file inside self.dicom_files that doesn't have an extension
         Returns
@@ -160,124 +163,54 @@
             threads.append(thread)
             thread.start()
 
         for thread in threads:
             thread.join()
 
     def separate_modalities(self):
-        """
-        Currently, separates the files into 10 different modalities. Files with a different modality are not kept.
-        Certain tags are required depending on the modality, if those tags don't exist for its respective modality
-        then it is not kept.
-
-        Returns
-        -------
-
-        """
-        req = {'CT': ['SeriesInstanceUID', 'AcquisitionNumber', 'ImagePositionPatient', 'SliceThickness', 'PixelData',
-                      'FrameOfReferenceUID'],
-               'MR': ['SeriesInstanceUID', 'AcquisitionNumber', 'ImagePositionPatient', 'SliceThickness', 'PixelData',
-                      'FrameOfReferenceUID'],
-               'PT': ['SeriesInstanceUID', 'ImagePositionPatient', 'SliceThickness', 'PixelData',
-                      'FrameOfReferenceUID'],
-               'US': ['SeriesInstanceUID', 'PixelData'],
-               'DX': ['SeriesInstanceUID', 'PixelData'],
-               'MG': ['SeriesInstanceUID', 'PixelData'],
-               'NM': ['SeriesInstanceUID', 'PixelData'],
-               'XA': ['SeriesInstanceUID', 'NumberOfFrames', 'PixelData'],
-               'CR': ['SeriesInstanceUID', 'PixelData'],
-               'RTSTRUCT': ['SeriesInstanceUID']}
-
         for modality in list(self.ds_dictionary.keys()):
             ds_modality = [d for d in self.ds if d['Modality'].value == modality]
-            if modality == 'CT' or modality == 'MR' or modality == 'PT':
-                self.ds_dictionary[modality] = [ds_mod for ds_mod in ds_modality if
-                                                len([r for r in req[modality] if r in ds_mod]) == len(req[modality]) and
-                                                ds_mod['SliceThickness'].value]
-            else:
-                self.ds_dictionary[modality] = [ds_mod for ds_mod in ds_modality if
-                                                len([r for r in req[modality] if r in ds_mod]) == len(req[modality])]
+            self.ds_dictionary[modality] = [ds_mod for ds_mod in ds_modality]
 
     def separate_images(self):
-        """
-        This is used to separate the different modalities into images. Each modality has specific requirements to exist
-        in the tags:
-            CT/MR = SeriesInstanceUID, SliceThickness, AcquisitionNumber, ImagePositionPatient
-            US = SeriesInstanceUID
-
-        CT - the 4 main tags are pulled into a numpy array. There is a quick fix because sometimes AcquisitionNumber is
-             empty, if so then '1001' is inserted in its place. All the unique combinations are found using series
-             instance uid, slice thickness, acquisition number. The unique combinations are used in a for loop and
-             all slices that match that criteria are selected. Those slices are then sorted by image position patient.
-        MR/PT - same as CT
-        US/DX/MG/NM/XA/CR - The images are just sorted using series instance uid.
-
-
-        Note: slices thickness is needed because some scans are saved with the first slice being a single slice of
-              coronal plane, then the rest of the slices are in the axial plane. I think it is called a scout scan,
-              basically they have a single coronal slice to show the area that will be covered, then it is followed
-              by your standard axial plane view. Anyway, I separate out that slice using the slice thickness because
-              it will be different from the axial.
+        for modality in list(self.ds_dictionary.keys()):
+            if len(self.ds_dictionary[modality]) > 0 and modality not in ['RTSTRUCT', 'US', 'DX']:
+                sorting_tags = np.asarray([[img['SeriesInstanceUID'].value, img['AcquisitionNumber'].value]
+                                           if 'AcquisitionNumber' in img and img['AcquisitionNumber'].value is not None
+                                           else [img['SeriesInstanceUID'].value, 1]
+                                           for img in self.ds_dictionary[modality]])
+
+                unique_tags = np.unique(sorting_tags, axis=0)
+                for tag in unique_tags:
+                    sorted_idx = np.where((sorting_tags[:, 0] == tag[0]) & (sorting_tags[:, 1] == tag[1]))
+                    image_tags = [self.ds_dictionary[modality][idx] for idx in sorted_idx[0]]
+
+                    if 'ImageOrientationPatient' in image_tags[0] and 'ImagePositionPatient' in image_tags[0]:
+                        orientation = image_tags[0]['ImageOrientationPatient'].value
+                        position_tags = np.asarray([t['ImagePositionPatient'].value for t in image_tags])
+
+                        x = np.abs(orientation[0]) + np.abs(orientation[3])
+                        y = np.abs(orientation[1]) + np.abs(orientation[4])
+                        z = np.abs(orientation[2]) + np.abs(orientation[5])
+
+                        if x < y and x < z:
+                            slice_idx = np.argsort(position_tags[:, 0])
+                        elif y < x and y < z:
+                            slice_idx = np.argsort(position_tags[:, 1])
+                        else:
+                            slice_idx = np.argsort(position_tags[:, 2])
 
-        Returns
-        -------
+                        self.ds_images.append([image_tags[idx] for idx in slice_idx])
 
-        """
-        standard_modalities = ['CT', 'MR', 'PT']
-        for mod in standard_modalities:
-            if len(self.ds_dictionary[mod]) > 0:
-                if mod in ['CT', 'MR']:
-                    sorting_tags = np.asarray([[img['SeriesInstanceUID'].value, img['SliceThickness'].value,
-                                                img['AcquisitionNumber'].value, img['ImagePositionPatient'].value[0],
-                                                img['ImagePositionPatient'].value[1],
-                                                img['ImagePositionPatient'].value[2], ii]
-                                               for ii, img in enumerate(self.ds_dictionary[mod])])
-                else:
-                    sorting_tags = np.asarray([[img['SeriesInstanceUID'].value, img['SliceThickness'].value,
-                                                None, img['ImagePositionPatient'].value[0],
-                                                img['ImagePositionPatient'].value[1],
-                                                img['ImagePositionPatient'].value[2], ii]
-                                               for ii, img in enumerate(self.ds_dictionary[mod])])
-
-                sorting_tags_fix = np.asarray([[s[0], s[1], '1001', s[3], s[4], s[5], s[6]] if s[2] is None else s
-                                               for s in sorting_tags])
-                unique_tags = np.unique(sorting_tags_fix[:, 0:3].astype(str), axis=0)
-
-                for tags in unique_tags:
-                    unsorted_values = sorting_tags_fix[np.where((sorting_tags_fix[:, 0] == tags[0]) &
-                                                                (sorting_tags_fix[:, 1] == tags[1]) &
-                                                                (sorting_tags_fix[:, 2] == tags[2]))]
-
-                    # noinspection PyBroadException
-                    try:
-                        orientation = np.round(self.ds_dictionary[mod][0].ImageOrientationPatient)
-                        if orientation[0] == 1 and orientation[4] == 1:
-                            orient_idx = 5
-                        elif orientation[0] == 0 and orientation[3] == 0:
-                            orient_idx = 3
-                        elif orientation[1] == 0 and orientation[4] == 0:
-                            orient_idx = 4
-                        else:
-                            orient_idx = 5
-                    except:
-                        orient_idx = 5
-
-                    sorted_values = unsorted_values[np.argsort(unsorted_values[:, orient_idx].astype('float'))[::-1]]
-                    self.ds_images.append([self.ds_dictionary[mod][int(idx[6])] for idx in sorted_values])
-
-        nonstandard_modalities = ['US', 'DX', 'MG', 'NM', 'XA', 'CR']
-        for mod in nonstandard_modalities:
-            if len(self.ds_dictionary[mod]) > 0:
-                sorting_tags = np.asarray([[img['SeriesInstanceUID'].value, ii]
-                                           for ii, img in enumerate(self.ds_dictionary[mod])])
-                unique_tags = np.unique(sorting_tags[:, 0], axis=0)
-                for tags in unique_tags:
-                    unsorted_values = sorting_tags[np.where(sorting_tags[:, 0] == tags)]
-                    sorted_values = unsorted_values[np.argsort(unsorted_values[:, 0])]
-                    self.ds_images.append([self.ds_dictionary[mod][int(idx[1])] for idx in sorted_values])
+                    else:
+                        self.ds_images.append(image_tags)
+
+            elif len(self.ds_dictionary[modality]) > 0 and modality in ['US', 'DX']:
+                for image in self.ds_dictionary[modality]:
+                    self.ds_images.append([image])
 
     def separate_rt_images(self):
         """
         Loops through all RTSTRUCT files found. Some required information that will be used later in making the contours
         is pulled:
             SeriesInstanceUID
             RoiNames
@@ -321,59 +254,74 @@
                     self.image_info.at[ii, t] = [img.filename for img in image]
 
                 elif t == 'SOPInstanceUID':
                     self.image_info.at[ii, t] = [img.SOPInstanceUID for img in image]
 
                 elif t == 'PixelSpacing':
                     if image[0].Modality == 'US':
-                        self.image_info.at[ii, t] = [
-                            np.round(image[0].SequenceOfUltrasoundRegions[0].PhysicalDeltaX, 4),
-                            np.round(image[0].SequenceOfUltrasoundRegions[0].PhysicalDeltaY, 4)]
+                        if 'PhysicalDeltaX' in image[0]:
+                            self.image_info.at[ii, t] = [
+                                10 * np.round(image[0].SequenceOfUltrasoundRegions[0].PhysicalDeltaX, 4),
+                                10 * np.round(image[0].SequenceOfUltrasoundRegions[0].PhysicalDeltaY, 4)]
+                        else:
+                            self.image_info.at[ii, t] = [1, 1]
+
                     elif image[0].Modality in ['DX', 'XA']:
                         self.image_info.at[ii, t] = image[0].ImagerPixelSpacing
-                    else:
+
+                    elif 'PixelSpacing' in image[0]:
                         self.image_info.at[ii, t] = image[0].PixelSpacing
 
+                    elif 'ContributingSourcesSequence' in image[0]:
+                        sequence = 'ContributingSourcesSequence'
+                        if 'DetectorElementSpacing' in image[0][sequence][0]:
+                            self.image_info.at[ii, t] = image[0][sequence][0]['DetectorElementSpacing'].value
+
                 elif t == 'ImagePositionPatient':
                     if image[0].Modality in ['US', 'CR', 'DX', 'MG', 'NM', 'XA']:
                         self.image_info.at[ii, t] = [0, 0, 0]
                     else:
-                        self.image_info.at[ii, t] = image[-1].ImagePositionPatient
+                        self.image_info.at[ii, t] = image[0].ImagePositionPatient
 
                 elif t == 'SliceThickness':
                     if len(image) > 1:
-                        thickness = (np.asarray(image[0]['ImagePositionPatient'].value[2]).astype(float) -
-                                     np.asarray(image[1]['ImagePositionPatient'].value[2]).astype(float))
+                        thickness = (np.asarray(image[1]['ImagePositionPatient'].value[2]).astype(float) -
+                                     np.asarray(image[0]['ImagePositionPatient'].value[2]).astype(float))
                     else:
-                        thickness = np.asarray(image[0]['SliceThickness']).astype(float)
+                        thickness = 1
 
                     self.image_info.at[ii, t] = thickness
 
                 elif t == 'Slices':
                     self.image_info.at[ii, t] = len(image)
 
                 elif t == 'DefaultWindow':
                     if (0x0028, 0x1050) in image[0] and (0x0028, 0x1051) in image[0]:
-                        if image[0].Modality == 'DX':
-                            self.image_info.at[ii, t] = [int(image[0].WindowCenter[0]),
-                                                         int(np.round(image[0].WindowWidth[0]/2))]
-                        else:
-                            center = image[0].WindowCenter
-                            width = image[0].WindowWidth
-                            if not isinstance(center, float):
-                                center = center[0]
-                            if not isinstance(width, float):
-                                width = width[0]
-                            self.image_info.at[ii, t] = [int(center), int(np.round(width/2))]
+                        center = image[0].WindowCenter
+                        width = image[0].WindowWidth
+                        if not isinstance(center, float):
+                            center = center[0]
+
+                        if not isinstance(width, float):
+                            width = width[0]
+
+                        self.image_info.at[ii, t] = [int(center), int(np.round(width/2))]
+
                     elif image[0].Modality == 'US':
                         self.image_info.at[ii, t] = [128, 128]
+
                     else:
                         self.image_info.at[ii, t] = None
+
                 elif t == 'FullWindow':
                     self.image_info.at[ii, t] = None
+
+                elif t == 'ImageMatrix':
+                    pass
+
                 else:
                     if t in image[0]:
                         self.image_info.at[ii, t] = image[0][t].value
                     else:
                         self.image_info.at[ii, t] = None
 
     def convert_images(self):
@@ -391,35 +339,52 @@
         is there, so it checks if the shape is 4 and if so it only saves the image as a [10, 512, 512]
         Returns
         -------
 
         """
         for ii, image in enumerate(self.ds_images):
             image_slices = []
-            if self.image_info.at[ii, 'Modality'] in ['CT', 'MR', 'PT', 'DX', 'MG', 'NM', 'XA', 'CR']:
+            if self.image_info.at[ii, 'Modality'] in ['CT', 'MR', 'PT', 'MG', 'NM', 'XA', 'CR']:
                 for slice_ in reversed(image):
                     if (0x0028, 0x1052) in slice_:
                         intercept = slice_.RescaleIntercept
                     else:
                         intercept = 0
 
                     if (0x0028, 0x1053) in slice_:
                         slope = slice_.RescaleSlope
                     else:
                         slope = 1
 
                     image_slices.append(((slice_.pixel_array*slope)+intercept).astype('int16'))
 
+            elif self.image_info.at[ii, 'Modality'] == 'DX':
+                if (0x2050, 0x0020) in image[0]:
+                    if image[0].PresentationLUTShape == 'INVERSE':
+                        hold_array = image[0].pixel_array.astype('int16')
+                        image_slices.append(16383 - hold_array)
+                        self.image_info.at[ii, 'DefaultWindow'][0] = 16383 - self.image_info.at[ii, 'DefaultWindow'][0]
+                    else:
+                        image_slices.append(image[0].pixel_array.astype('int16'))
+                else:
+                    image_slices.append(image[0].pixel_array.astype('int16'))
+
             elif self.image_info.at[ii, 'Modality'] == 'US':
                 if len(image) == 1:
                     us_data = image[0].pixel_array
-                    us_binary = (1 * (np.std(us_data, axis=3) == 0) == 1)
-                    image_slices = (us_binary * us_data[:, :, :, 0]).astype('uint8')
+                    if len(us_data.shape) == 3:
+                        us_binary = (1 * (np.std(us_data, axis=2) == 0) == 1)
+                        image_slices = (us_binary * us_data[:, :, 0]).astype('uint8')
+
+                    else:
+                        us_binary = (1 * (np.std(us_data, axis=3) == 0) == 1)
+                        image_slices = (us_binary * us_data[:, :, :, 0]).astype('uint8')
                 else:
                     print('Need to finish')
+                self.image_info.at[ii, 'Slices'] = len(image_slices)
 
             image_hold = np.asarray(image_slices)
             if len(image_hold.shape) > 3:
                 self.image_data.append(image_hold[0])
             else:
                 self.image_data.append(image_hold)
 
@@ -437,35 +402,64 @@
                 coordinates = self.image_info.at[ii, 'ImagePositionPatient']
 
                 if position in ['HFDR', 'FFDR']:
                     self.image_data[ii] = np.rot90(image, 3, (1, 2))
 
                     new_coordinates = np.double(coordinates[0]) - spacing[0] * (columns - 1)
                     self.image_info.at[ii, 'ImagePositionPatient'][0] = new_coordinates
+
                 elif position in ['HFP', 'FFP']:
                     self.image_data[ii] = np.rot90(image, 2, (1, 2))
 
                     new_coordinates = np.double(coordinates[0]) - spacing[0] * (columns - 1)
                     self.image_info.at[ii, 'ImagePositionPatient'][0] = new_coordinates
 
                     new_coordinates = np.double(coordinates[1]) - spacing[1] * (rows - 1)
                     self.image_info.at[ii, 'ImagePositionPatient'][1] = new_coordinates
                 elif position in ['HFDL', 'FFDL']:
                     self.image_data[ii] = np.rot90(image, 1, (1, 2))
 
                     new_coordinates = np.double(coordinates[1]) - spacing[1] * (rows - 1)
                     self.image_info.at[ii, 'ImagePositionPatient'][1] = new_coordinates
 
+                self.compute_image_matrix(ii)
+
+    def compute_image_matrix(self, ii):
+        row_direction = np.array(self.image_info.at[ii, 'ImageOrientationPatient'][:3])
+        column_direction = np.array(self.image_info.at[ii, 'ImageOrientationPatient'][3:])
+        # noinspection PyUnreachableCode
+        slice_direction = np.cross(row_direction, column_direction)
+        offset = np.asarray(self.image_info.at[ii, 'ImagePositionPatient'])
+
+        row_spacing = self.image_info.at[ii, 'PixelSpacing'][0]
+        column_spacing = self.image_info.at[ii, 'PixelSpacing'][1]
+
+        first = np.dot(slice_direction, self.ds_images[ii][0].ImagePositionPatient)
+        last = np.dot(slice_direction, self.ds_images[ii][-1].ImagePositionPatient)
+
+        self.image_info.at[ii, 'SliceThickness'] = (last - first) / (self.image_info.at[ii, 'Slices'] - 1)
+        slice_spacing = self.image_info.at[ii, 'SliceThickness']
+
+        linear = np.identity(3, dtype=np.float32)
+        linear[0, :3] = row_direction / row_spacing
+        linear[1, :3] = column_direction / column_spacing
+        linear[2, :3] = slice_direction / slice_spacing
+
+        mat = np.identity(4, dtype=np.float32)
+        mat[:3, :3] = linear
+        mat[:3, 3] = offset.dot(-linear.T)
+        self.image_info.at[ii, 'ImageMatrix'] = mat
+
     def separate_contours(self):
         """
         existing_image_info is required if the users only loads a RTSTRUCT file, this is needed to match contours with
         the image they correspond to.
 
         It is pretty gross after that. For a given ROI each contour is read-in, matched with their image, then combined
-        all the slices of each contour into there own numpy array.
+        all the slices of each contour into their own numpy array.
 
         Returns
         -------
 
         """
         info = self.image_info
         if self.existing_image_info is not None:
@@ -504,14 +498,29 @@
                 self.roi_info.at[ii, 'FilePath'] = roi_filepaths
                 self.roi_info.at[ii, 'RoiNames'] = roi_names
             else:
                 self.roi_contour.append([])
                 self.roi_info.at[ii, 'FilePath'] = None
                 self.roi_info.at[ii, 'RoiNames'] = None
 
+    def contour_pixel_location(self):
+        for ii, roi in enumerate(self.roi_contour):
+            matrix = self.image_info.at[ii, 'ImageMatrix']
+
+            roi_hold = []
+            for r in roi:
+                r_hold = []
+                for contours in r:
+                    c = np.concatenate((contours, np.ones((contours.shape[0], 1))), axis=1)
+                    r_hold.append(c.dot(matrix.T)[:, :3])
+
+                roi_hold.append(r_hold)
+
+            self.roi_pixel_position.append(roi_hold)
+
     def get_image_info(self):
         return self.image_info
 
     def get_image_data(self):
         return self.image_data
 
     def get_roi_contour(self):
@@ -522,8 +531,7 @@
 
     def get_ds_images(self):
         return self.ds_images
 
 
 if __name__ == '__main__':
     pass
-
```

### Comparing `MedicalImageConverter-1.4/MedicalImageConverter.egg-info/PKG-INFO` & `medicalimageconverter-1.5/MedicalImageConverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedicalImageConverter
-Version: 1.4
+Version: 1.5
 Summary: Reads in medical images and converts them into numpy arrays.
 Home-page: https://github.com/caleb-oconnor/MedicalImageConverter
 Author: Caleb OConnor
 Author-email: csoconnor@mdanderson.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `MedicalImageConverter-1.4/PKG-INFO` & `medicalimageconverter-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedicalImageConverter
-Version: 1.4
+Version: 1.5
 Summary: Reads in medical images and converts them into numpy arrays.
 Home-page: https://github.com/caleb-oconnor/MedicalImageConverter
 Author: Caleb OConnor
 Author-email: csoconnor@mdanderson.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `MedicalImageConverter-1.4/README.md` & `medicalimageconverter-1.5/README.md`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.4/setup.cfg` & `medicalimageconverter-1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6564 6963 616c 496d 6167 6543   = MedicalImageC
 00000020: 6f6e 7665 7274 6572 0d0a 7665 7273 696f  onverter..versio
-00000030: 6e20 3d20 312e 340d 0a61 7574 686f 7220  n = 1.4..author 
+00000030: 6e20 3d20 312e 350d 0a61 7574 686f 7220  n = 1.5..author 
 00000040: 3d20 4361 6c65 6220 4f43 6f6e 6e6f 720d  = Caleb OConnor.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6373 6f63 6f6e 6e6f 7240 6d64 616e 6465  csoconnor@mdande
 00000070: 7273 6f6e 2e6f 7267 0d0a 6465 7363 7269  rson.org..descri
 00000080: 7074 696f 6e20 3d20 5265 6164 7320 696e  ption = Reads in
 00000090: 206d 6564 6963 616c 2069 6d61 6765 7320   medical images 
 000000a0: 616e 6420 636f 6e76 6572 7473 2074 6865  and converts the
```

