# Comparing `tmp/image_functions-0.1.2.tar.gz` & `tmp/image_functions-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_functions-0.1.2.tar", last modified: Wed May 29 04:04:05 2024, max compression
+gzip compressed data, was "image_functions-0.1.3.tar", last modified: Mon Jun  3 13:41:59 2024, max compression
```

## Comparing `image_functions-0.1.2.tar` & `image_functions-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 04:04:05.900847 image_functions-0.1.2/
--rw-rw-rw-   0        0        0     1101 2023-05-09 16:58:11.000000 image_functions-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1101 2023-05-12 12:23:49.000000 image_functions-0.1.2/LICENSE.rst
--rw-rw-rw-   0        0        0     6062 2024-05-29 04:04:05.899847 image_functions-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4080 2024-05-29 04:02:05.000000 image_functions-0.1.2/README.md
--rw-rw-rw-   0        0        0      867 2024-05-29 04:02:33.000000 image_functions-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 04:04:05.900847 image_functions-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 04:04:05.881001 image_functions-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 04:04:05.897847 image_functions-0.1.2/src/image_functions.egg-info/
--rw-rw-rw-   0        0        0     6062 2024-05-29 04:04:05.000000 image_functions-0.1.2/src/image_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-05-29 04:04:05.000000 image_functions-0.1.2/src/image_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 04:04:05.000000 image_functions-0.1.2/src/image_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-29 04:04:05.000000 image_functions-0.1.2/src/image_functions.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       59 2024-05-29 04:04:05.000000 image_functions-0.1.2/src/image_functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-29 04:04:05.000000 image_functions-0.1.2/src/image_functions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 04:04:05.895851 image_functions-0.1.2/src/imfun/
--rw-rw-rw-   0        0        0      113 2024-05-29 04:02:57.000000 image_functions-0.1.2/src/imfun/__init__.py
--rw-rw-rw-   0        0        0   127519 2024-05-29 03:28:44.000000 image_functions-0.1.2/src/imfun/__main__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:41:59.075409 image_functions-0.1.3/
+-rw-rw-rw-   0        0        0     1101 2023-05-09 16:58:11.000000 image_functions-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1101 2023-05-12 12:23:49.000000 image_functions-0.1.3/LICENSE.rst
+-rw-rw-rw-   0        0        0     6278 2024-06-03 13:41:59.075409 image_functions-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4271 2024-06-03 13:41:11.000000 image_functions-0.1.3/README.md
+-rw-rw-rw-   0        0        0      884 2024-06-03 13:34:52.000000 image_functions-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:41:59.075409 image_functions-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 13:41:59.054279 image_functions-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:41:59.075409 image_functions-0.1.3/src/image_functions.egg-info/
+-rw-rw-rw-   0        0        0     6278 2024-06-03 13:41:59.000000 image_functions-0.1.3/src/image_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-06-03 13:41:59.000000 image_functions-0.1.3/src/image_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:41:59.000000 image_functions-0.1.3/src/image_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-06-03 13:41:59.000000 image_functions-0.1.3/src/image_functions.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2024-06-03 13:41:59.000000 image_functions-0.1.3/src/image_functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 13:41:59.000000 image_functions-0.1.3/src/image_functions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 13:41:59.075409 image_functions-0.1.3/src/imfun/
+-rw-rw-rw-   0        0        0      113 2024-06-03 13:35:09.000000 image_functions-0.1.3/src/imfun/__init__.py
+-rw-rw-rw-   0        0        0   130242 2024-06-03 13:39:52.000000 image_functions-0.1.3/src/imfun/__main__.py
```

### Comparing `image_functions-0.1.2/LICENSE` & `image_functions-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `image_functions-0.1.2/LICENSE.rst` & `image_functions-0.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `image_functions-0.1.2/PKG-INFO` & `image_functions-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-functions
-Version: 0.1.2
+Version: 0.1.3
 Summary: Image Processing Functions
 Author-email: Marlon Rodrigues Garcia <marlon.garcia@unesp.br>
 License: MIT License
         
         Copyright (c) 2023 Marlon Rodrigues Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,28 +36,32 @@
 License-File: LICENSE.rst
 Requires-Dist: numpy
 Requires-Dist: opencv-contrib-python
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: pynput
 Requires-Dist: pandas
+Requires-Dist: tifffile
 
 # Image Functions Library
 
 Library for image pre-processing, with functions to handle and prepare images for machine learning and image processing. This library accounts for functions to load and plot a group of images, pre-processing, choose ROI regions (even polygonal), choose points, get image properties, align and transform images (including rotate, scale, etc.), filter signals and images (2D data), among others. All the functions with GUI (stands for graphical user interface) have an interface to interact with the user.
 
 
 ### 1. Functions to Load and Plot
 
 - `load_gray_images`: loads all images from a folder, in grayscale
 - `load_color_images`: loads all color images from a folder
 - `plot_gray_images`: prints all grayscale images from a variable 'I'
 - `plot_color_images`: prints all color images from a variable 'I'
 - `plot_gray`: prints a grayscale image
 - `plot_bgr`: prints a color image in BGR format
+- `list_folders`: list all folders inside a directory
+- `list_images`: list all images inside a folder
+- `read_lsm`: reading and mounting images of '.lsm' extension from Zeiss microscope 
 
 
 ### 2. Pre-Processing for Machine Learning and Computer Vision
 
 #### 2.1. ROI and Handling (*Most Important Ones*)
 
 - `polyroi`: GUI to create a polygonal region of interest (ROI)
@@ -100,15 +104,15 @@
     
 
 ## How to Install
 
 You can install using `pip`:
 
 ```
-pip install image-functions==0.1.2
+pip install image-functions==0.1.3
 ```
 
 *OBS*: some functions use the 'pynput' and 'windsound' libraries, which may be difficult to install and do not works on non-windows platforms. Comment on these library imports if there are problems during installation or loading.
 
 - author: Marlon Rodrigues Garcia
 - contact: marlon.garcia@unesp.br
 - institution: Sao Paulo State University (Unesp)
```

### Comparing `image_functions-0.1.2/README.md` & `image_functions-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 - `load_gray_images`: loads all images from a folder, in grayscale
 - `load_color_images`: loads all color images from a folder
 - `plot_gray_images`: prints all grayscale images from a variable 'I'
 - `plot_color_images`: prints all color images from a variable 'I'
 - `plot_gray`: prints a grayscale image
 - `plot_bgr`: prints a color image in BGR format
+- `list_folders`: list all folders inside a directory
+- `list_images`: list all images inside a folder
+- `read_lsm`: reading and mounting images of '.lsm' extension from Zeiss microscope 
 
 
 ### 2. Pre-Processing for Machine Learning and Computer Vision
 
 #### 2.1. ROI and Handling (*Most Important Ones*)
 
 - `polyroi`: GUI to create a polygonal region of interest (ROI)
@@ -57,15 +60,15 @@
     
 
 ## How to Install
 
 You can install using `pip`:
 
 ```
-pip install image-functions==0.1.2
+pip install image-functions==0.1.3
 ```
 
 *OBS*: some functions use the 'pynput' and 'windsound' libraries, which may be difficult to install and do not works on non-windows platforms. Comment on these library imports if there are problems during installation or loading.
 
 - author: Marlon Rodrigues Garcia
 - contact: marlon.garcia@unesp.br
 - institution: Sao Paulo State University (Unesp)
```

### Comparing `image_functions-0.1.2/pyproject.toml` & `image_functions-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "image-functions"
-version = "0.1.2"
+version = "0.1.3"
 description = "Image Processing Functions"
 readme = "README.md"
 authors = [{ name = "Marlon Rodrigues Garcia", email = "marlon.garcia@unesp.br" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,14 +20,15 @@
 dependencies = [
     "numpy",
     "opencv-contrib-python",
     "matplotlib",
     "scipy",
     "pynput",
     "pandas",
+    "tifffile",
 ]
 
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/MarlonGarcia/imfun"
```

### Comparing `image_functions-0.1.2/src/image_functions.egg-info/PKG-INFO` & `image_functions-0.1.3/src/image_functions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-functions
-Version: 0.1.2
+Version: 0.1.3
 Summary: Image Processing Functions
 Author-email: Marlon Rodrigues Garcia <marlon.garcia@unesp.br>
 License: MIT License
         
         Copyright (c) 2023 Marlon Rodrigues Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,28 +36,32 @@
 License-File: LICENSE.rst
 Requires-Dist: numpy
 Requires-Dist: opencv-contrib-python
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: pynput
 Requires-Dist: pandas
+Requires-Dist: tifffile
 
 # Image Functions Library
 
 Library for image pre-processing, with functions to handle and prepare images for machine learning and image processing. This library accounts for functions to load and plot a group of images, pre-processing, choose ROI regions (even polygonal), choose points, get image properties, align and transform images (including rotate, scale, etc.), filter signals and images (2D data), among others. All the functions with GUI (stands for graphical user interface) have an interface to interact with the user.
 
 
 ### 1. Functions to Load and Plot
 
 - `load_gray_images`: loads all images from a folder, in grayscale
 - `load_color_images`: loads all color images from a folder
 - `plot_gray_images`: prints all grayscale images from a variable 'I'
 - `plot_color_images`: prints all color images from a variable 'I'
 - `plot_gray`: prints a grayscale image
 - `plot_bgr`: prints a color image in BGR format
+- `list_folders`: list all folders inside a directory
+- `list_images`: list all images inside a folder
+- `read_lsm`: reading and mounting images of '.lsm' extension from Zeiss microscope 
 
 
 ### 2. Pre-Processing for Machine Learning and Computer Vision
 
 #### 2.1. ROI and Handling (*Most Important Ones*)
 
 - `polyroi`: GUI to create a polygonal region of interest (ROI)
@@ -100,15 +104,15 @@
     
 
 ## How to Install
 
 You can install using `pip`:
 
 ```
-pip install image-functions==0.1.2
+pip install image-functions==0.1.3
 ```
 
 *OBS*: some functions use the 'pynput' and 'windsound' libraries, which may be difficult to install and do not works on non-windows platforms. Comment on these library imports if there are problems during installation or loading.
 
 - author: Marlon Rodrigues Garcia
 - contact: marlon.garcia@unesp.br
 - institution: Sao Paulo State University (Unesp)
```

### Comparing `image_functions-0.1.2/src/imfun/__main__.py` & `image_functions-0.1.3/src/imfun/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 import ctypes
 from random import shuffle
 from scipy import fftpack     # to apply FFT and iFFT
 from scipy import signal
 from scipy.fft import fft, fftfreq
 from scipy.interpolate import interp1d
 import pandas as pd
+import tkinter as tk
+from tkinter import filedialog, messagebox
+import tifffile as tiff       # To import ".lsm" images
 from pynput import keyboard   # It does not worked on Google Colab
 # To use a 'beep' sound, uncomment: winsound, time.
 import winsound               # it only works on Windows
 
 
 
 def list_folders(directory):
@@ -242,14 +245,64 @@
     numb = 5 # number of beeps
     for n in range(0, numb):
         time.sleep(0.0005)
         winsound.Beep(freq, duration)
 
 
 
+def read_lsm(file_path):
+    '''Reading and mounting images of '.lsm' extension from Zeiss microscope 
+
+    Parameters
+    ----------
+    file_path : string
+        Path/Directory to the '.lsm' file.
+
+    Returns
+    -------
+    full_image : numpy.ndarray
+        Full assembled image.
+    '''
+    # Reading image and its metadata
+    with tiff.TiffFile(file_path) as tif:
+        images = tif.asarray()
+        metadata = tif.lsm_metadata
+    
+    # Transforming shape (Tiles, Channels, Width, Height) in (Tiles, Chan., W, H)
+    images = np.transpose(images, (0, 2, 3, 1))
+    
+    # Extracting the tile positions
+    tile_positions = metadata['TilePositions']
+    
+    # Discovering how many tiles we have on the horizontal axis (x axis)
+    tile_x = 1
+    for n in range(1, len(tile_positions)):
+        if tile_positions[n, 0] == tile_positions[0, 0]:
+            tile_x = n
+            break
+    
+    # Discovering how many tiles we have on the vertical axis (y axis)
+    tile_y = 1
+    value = tile_positions[0, 1]
+    for n in range(1, len(tile_positions)):
+        if tile_positions[n, 1] != value:
+            tile_y += 1
+            value = tile_positions[n, 1]
+    
+    # Mounting the full image
+    shape = np.shape(images)
+    full_image = np.zeros([shape[2]*tile_y, shape[1]*tile_x, 3], dtype='uint8')
+    for x in range(tile_x):
+        for y in range(tile_y):
+            full_image[y*shape[2]:(y+1)*shape[2], shape[1]*x:shape[1]*(x+1), :] = images[x + tile_x*y, :, :, :]
+    
+    return full_image
+
+
+
 def rotate2D(pts, cnt, ang):
     '''Rotating the points about a center 'cnt' by an ang 'ang' in radians.
     
     [pts_r] = rotate2D(pts, cnt, ang)
     
     '''
     return np.dot(pts-cnt,np.array([[ np.cos(ang),np.sin(ang)],
@@ -2041,15 +2094,15 @@
     # Standar deviation from pixels in ROI:
     props[2] = Itemp[Itemp!=0].std()
     
     return props, Imask
 
 
 
-def roi_stats(images_dir, save_dir, experiments, colors, **kwargs):
+def roi_stats(experiments, colors, **kwargs):
     ''' Easely calculate statistics of images in a given region of the images
     
     This function uses a interactive graphical user interface (GUI) to calcula-
     te the statistics of multiple images, in a given region of interest (ROI)
     inside the image. To use this function, your images have to be in a folder
     tree like bellow. The outer folder will be 'Images Folder', that has to be
     passed to this function in the 'images_dir' variable. Inside this folder
@@ -2065,51 +2118,74 @@
         |
         |--- Animal 1
         |       |
         |       |--- Experiment 1
         |       |
         |       |--- Experiment 2
         |       |
-        |       |--- Experiment 3
+        |       '--- Experiment 3
         |
         |
-        |--- Animal 2
+        '--- Animal 2
                 |
                 |--- Experiment 1
                 |
                 |--- Experiment 2
                 |
-                |--- Experiment 3
+                '--- Experiment 3
     
     Parameters
     ----------
-    images_dir : string
-        Root directory (outer folder) of your images. E.g. 'C:/Users/User/data'
-    save_dir : string
-        Directory to save the images.
     experiments : list
         Names of the experiments. Note that it has to mach the experiment names
         e.g. ['Experiment 1', 'Experiment 2', 'Experiment 3'] in the example.
     colors : list
         Name of the colors (or channels) to be analized in the image, or a list
         with the string 'gray' for grayscale images. E.g.: ['gray'] or ['red'],
         or even all the colors ['red', 'green', 'blue']
     
     **kwargs (arguments that may or may not be passed to the function)
     ----------
-        stats : list
-            A list with the statistics to be calculated. Only mean and standard
-            deviation are suported until now. E.g. ['mean'] or ['mean', 'std']
-        colormap : int
-            The colormap to use while choosing the region of interest
-            examples: cv2.COLORMAP_PINK, cv2.COLORMAP_HSV, cv2.COLORMAP_PARULA.
+    images_dir : string
+        Root directory (outer folder) of your images. E.g. 'C:/Users/User/data'
+    save_dir : string
+        Directory to save the images.
+    stats : list
+        A list with the statistics to be calculated. Only mean and standard
+        deviation are suported until now. E.g. ['mean'] or ['mean', 'std']
+    colormap : int
+        The colormap to use while choosing the region of interest
+        examples: cv2.COLORMAP_PINK, cv2.COLORMAP_HSV, cv2.COLORMAP_PARULA.
     '''
     colormap = kwargs.get('colormap', cv2.COLORMAP_PINK)
     stats = kwargs.get('stats', ['mean', 'std'])
+    images_dir = kwargs.get('images_dir', None)
+    save_dir = kwargs.get('save_dir', None)
+    
+    ## Display a message to choose the folder the folders
+    # Create the root window and hide it
+    root = tk.Tk()
+    root.withdraw()
+    
+    ## Prompt a dialog to user to select the folder 'images_dir' and 'save_dir'
+    if not images_dir:
+        images_dir = filedialog.askdirectory(title='Please select the folder where the images are')
+        if not images_dir:
+            messagebox.showinfo('Selection Cancelled', 'No folder selected for images.')
+    
+    # Prompt the user to select the second folder
+    if not save_dir:
+        save_dir = filedialog.askdirectory(title='Please select the folder to save files')
+        if not save_dir:
+            messagebox.showinfo('Selection Cancelled', 'No folder selected to save the data.')
+    
+    # Show a message confirming the selections
+    messagebox.showinfo('Folders Selected', f'Images folder: {images_dir}\nSave folder: {save_dir}')
     
+    # Verify if user choose the colors to be processed
     if not colors or not experiments:
         raise ValueError('\n\n- You did not choose the colors or the experiments correctly')
 
     # Entering into the folder of images
     folders = list_folders(images_dir)
     
     # Initiating the variable with the data to be saved
```

