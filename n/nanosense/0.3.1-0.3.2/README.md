# Comparing `tmp/nanosense-0.3.1.tar.gz` & `tmp/nanosense-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanosense-0.3.1.tar", last modified: Tue May 28 05:14:55 2024, max compression
+gzip compressed data, was "nanosense-0.3.2.tar", last modified: Mon Jun  3 02:58:35 2024, max compression
```

## Comparing `nanosense-0.3.1.tar` & `nanosense-0.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.384300 nanosense-0.3.1/
--rw-r--r--   0 shankardutt   (501) staff       (20)       98 2024-05-27 06:08:37.000000 nanosense-0.3.1/MANIFEST.in
--rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-28 05:14:55.384058 nanosense-0.3.1/PKG-INFO
--rw-r--r--   0 shankardutt   (501) staff       (20)       11 2024-04-05 23:59:28.000000 nanosense-0.3.1/README.md
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.374658 nanosense-0.3.1/nanosense/
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.375761 nanosense-0.3.1/nanosense/Clustering and Data Reduction/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Clustering and Data Reduction/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)   107280 2024-05-20 03:54:27.000000 nanosense-0.3.1/nanosense/Clustering and Data Reduction/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.376639 nanosense-0.3.1/nanosense/Combine Datasets/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Combine Datasets/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)     5973 2024-05-08 03:18:56.000000 nanosense-0.3.1/nanosense/Combine Datasets/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.377333 nanosense-0.3.1/nanosense/Data Reduction/
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.378065 nanosense-0.3.1/nanosense/Data Reduction/Docs/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Data Reduction/Docs/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Data Reduction/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)   228038 2024-05-20 04:16:55.000000 nanosense-0.3.1/nanosense/Data Reduction/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.378284 nanosense-0.3.1/nanosense/Data Visualisation/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Data Visualisation/__init__.py
--rwx------   0 shankardutt   (501) staff       (20)   101413 2024-05-19 00:30:33.000000 nanosense-0.3.1/nanosense/Data Visualisation/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.378950 nanosense-0.3.1/nanosense/Event Analysis/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Event Analysis/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    32048 2024-05-19 00:26:20.000000 nanosense-0.3.1/nanosense/Event Analysis/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.379392 nanosense-0.3.1/nanosense/Frequency and multi-plots/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Frequency and multi-plots/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    39035 2024-05-19 00:31:20.000000 nanosense-0.3.1/nanosense/Frequency and multi-plots/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.380064 nanosense-0.3.1/nanosense/ML Analysis/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/ML Analysis/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    60685 2024-05-07 07:33:17.000000 nanosense-0.3.1/nanosense/ML Analysis/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.380827 nanosense-0.3.1/nanosense/Nanopore Size Calc/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Nanopore Size Calc/__init__.py
--rwx------   0 shankardutt   (501) staff       (20)     5069 2024-05-08 03:29:30.000000 nanosense-0.3.1/nanosense/Nanopore Size Calc/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.381548 nanosense-0.3.1/nanosense/Plotting and selecting/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Plotting and selecting/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    28580 2024-05-07 07:27:05.000000 nanosense-0.3.1/nanosense/Plotting and selecting/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.382155 nanosense-0.3.1/nanosense/Resource Monitor/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Resource Monitor/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    11105 2024-05-11 05:45:18.000000 nanosense-0.3.1/nanosense/Resource Monitor/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.382865 nanosense-0.3.1/nanosense/Spectrogram and PSD/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/Spectrogram and PSD/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    28223 2024-05-10 06:05:42.000000 nanosense-0.3.1/nanosense/Spectrogram and PSD/main.py
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.3.1/nanosense/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)      504 2024-04-26 09:46:44.000000 nanosense-0.3.1/nanosense/activation_codes.enc
--rw-r--r--   0 shankardutt   (501) staff       (20)   989781 2024-03-21 23:51:54.000000 nanosense-0.3.1/nanosense/icons.icns
--rw-r--r--   0 shankardutt   (501) staff       (20)   256727 2024-03-21 23:31:47.000000 nanosense-0.3.1/nanosense/image_1.jpg
--rw-r--r--   0 shankardutt   (501) staff       (20)    16033 2024-05-28 05:10:15.000000 nanosense-0.3.1/nanosense/nanosense.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-28 05:14:55.383762 nanosense-0.3.1/nanosense.egg-info/
--rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-28 05:14:55.000000 nanosense-0.3.1/nanosense.egg-info/PKG-INFO
--rw-r--r--   0 shankardutt   (501) staff       (20)     1257 2024-05-28 05:14:55.000000 nanosense-0.3.1/nanosense.egg-info/SOURCES.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)        1 2024-05-28 05:14:55.000000 nanosense-0.3.1/nanosense.egg-info/dependency_links.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       55 2024-05-28 05:14:55.000000 nanosense-0.3.1/nanosense.egg-info/entry_points.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)      235 2024-05-28 05:14:55.000000 nanosense-0.3.1/nanosense.egg-info/requires.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       10 2024-05-28 05:14:55.000000 nanosense-0.3.1/nanosense.egg-info/top_level.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       38 2024-05-28 05:14:55.384343 nanosense-0.3.1/setup.cfg
--rw-r--r--   0 shankardutt   (501) staff       (20)     1361 2024-05-28 05:14:49.000000 nanosense-0.3.1/setup.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.535294 nanosense-0.3.2/
+-rw-r--r--   0 shankardutt   (501) staff       (20)       98 2024-05-27 06:08:37.000000 nanosense-0.3.2/MANIFEST.in
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-06-03 02:58:35.535031 nanosense-0.3.2/PKG-INFO
+-rw-r--r--   0 shankardutt   (501) staff       (20)       11 2024-04-05 23:59:28.000000 nanosense-0.3.2/README.md
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.530394 nanosense-0.3.2/nanosense/
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.531396 nanosense-0.3.2/nanosense/Clustering and Data Reduction/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Clustering and Data Reduction/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    79684 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Clustering and Data Reduction/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.531684 nanosense-0.3.2/nanosense/Combine Datasets/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Combine Datasets/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)     6102 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Combine Datasets/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.531966 nanosense-0.3.2/nanosense/Data Reduction/
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.532210 nanosense-0.3.2/nanosense/Data Reduction/Docs/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/Data Reduction/Docs/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/Data Reduction/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)   193713 2024-06-03 02:58:24.000000 nanosense-0.3.2/nanosense/Data Reduction/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.532416 nanosense-0.3.2/nanosense/Data Visualisation/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Data Visualisation/__init__.py
+-rwx------   0 shankardutt   (501) staff       (20)    80089 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Data Visualisation/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.532693 nanosense-0.3.2/nanosense/Event Analysis/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Event Analysis/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    26190 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Event Analysis/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.532935 nanosense-0.3.2/nanosense/Frequency and multi-plots/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/Frequency and multi-plots/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    35845 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/Frequency and multi-plots/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.533206 nanosense-0.3.2/nanosense/ML Analysis/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/ML Analysis/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    55570 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/ML Analysis/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.533524 nanosense-0.3.2/nanosense/Nanopore Size Calc/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Nanopore Size Calc/__init__.py
+-rwx------   0 shankardutt   (501) staff       (20)     4605 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Nanopore Size Calc/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.533827 nanosense-0.3.2/nanosense/Plotting and selecting/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Plotting and selecting/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    28365 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Plotting and selecting/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.534133 nanosense-0.3.2/nanosense/Resource Monitor/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/Resource Monitor/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    11411 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/Resource Monitor/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.534510 nanosense-0.3.2/nanosense/Spectrogram and PSD/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Spectrogram and PSD/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    27746 2024-06-03 02:57:11.000000 nanosense-0.3.2/nanosense/Spectrogram and PSD/main.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)      504 2024-04-26 09:46:44.000000 nanosense-0.3.2/nanosense/activation_codes.enc
+-rw-r--r--   0 shankardutt   (501) staff       (20)   989781 2024-03-21 23:51:54.000000 nanosense-0.3.2/nanosense/icons.icns
+-rw-r--r--   0 shankardutt   (501) staff       (20)   256727 2024-03-21 23:31:47.000000 nanosense-0.3.2/nanosense/image_1.jpg
+-rw-r--r--   0 shankardutt   (501) staff       (20)    14271 2024-06-03 02:57:10.000000 nanosense-0.3.2/nanosense/nanosense.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-06-03 02:58:35.534741 nanosense-0.3.2/nanosense.egg-info/
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-06-03 02:58:35.000000 nanosense-0.3.2/nanosense.egg-info/PKG-INFO
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1257 2024-06-03 02:58:35.000000 nanosense-0.3.2/nanosense.egg-info/SOURCES.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)        1 2024-06-03 02:58:35.000000 nanosense-0.3.2/nanosense.egg-info/dependency_links.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       55 2024-06-03 02:58:35.000000 nanosense-0.3.2/nanosense.egg-info/entry_points.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)      235 2024-06-03 02:58:35.000000 nanosense-0.3.2/nanosense.egg-info/requires.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       10 2024-06-03 02:58:35.000000 nanosense-0.3.2/nanosense.egg-info/top_level.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       38 2024-06-03 02:58:35.535339 nanosense-0.3.2/setup.cfg
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1361 2024-06-03 02:57:55.000000 nanosense-0.3.2/setup.py
```

### Comparing `nanosense-0.3.1/PKG-INFO` & `nanosense-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosense
-Version: 0.3.1
+Version: 0.3.2
 Summary: A comprehensive package for nanosense data analysis and visualization.
 Home-page: https://github.com/shankardutt/nanosense
 Author: Shankar Dutt
 Author-email: shankar.dutt@anu.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanosense-0.3.1/nanosense/Combine Datasets/main.py` & `nanosense-0.3.2/nanosense/Combine Datasets/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import sys
-import os
-from PySide6.QtWidgets import QApplication, QWidget, QLabel, QPushButton, QCheckBox, QComboBox, QListWidget, QVBoxLayout, QHBoxLayout, QFileDialog, QMessageBox, QStyleFactory
-from PySide6.QtCore import Qt
-from PySide6.QtGui import QPalette, QColor, QFont
-import numpy as np
-
-class SDCombineDatasets(QWidget):
-    def __init__(self):
-        super().__init__()
-        self.setWindowTitle("SD Combine Datasets")
-        self.resize(500, 700)
-
-        # Create widgets
-        self.app_name_label = QLabel("SD Combine Datasets")
-        self.app_name_label.setAlignment(Qt.AlignCenter)
-        self.app_name_label.setFont(QFont("Arial", 16, QFont.Bold))
-        self.email_label = QLabel("shankar.dutt@anu.edu.au")
-        self.email_label.setAlignment(Qt.AlignCenter)
-        self.select_folder_button = QPushButton("Select Folder")
-        self.include_subfolders_checkbox = QCheckBox("Include Subfolders")
-        self.extension_dropdown = QComboBox()
-        self.extension_dropdown.addItems([".dataset.npz", ".MLdataset.npz"])
-        self.file_list = QListWidget()
-        self.file_list.setSelectionMode(QListWidget.SelectionMode.MultiSelection)
-        self.select_all_checkbox = QCheckBox("Select All")
-        self.folder_path_label = QLabel()
-        self.folder_path_label.setWordWrap(True)
-        self.combine_datasets_button = QPushButton("Combine Datasets")
-
-        # Create layouts
-        main_layout = QVBoxLayout()
-        main_layout.addWidget(self.app_name_label)
-        main_layout.addWidget(self.email_label)
-        main_layout.addWidget(self.select_folder_button)
-        main_layout.addWidget(self.include_subfolders_checkbox)
-        main_layout.addWidget(self.extension_dropdown)
-        main_layout.addWidget(self.file_list)
-        main_layout.addWidget(self.select_all_checkbox)
-        main_layout.addWidget(self.folder_path_label)
-        main_layout.addWidget(self.combine_datasets_button)
-
-        self.setLayout(main_layout)
-
-        # Connect signals and slots
-        self.select_folder_button.clicked.connect(self.select_folder)
-        self.select_all_checkbox.stateChanged.connect(self.select_all)
-        self.combine_datasets_button.clicked.connect(self.combine_datasets)
-
-    def select_folder(self):
-        folder_path = QFileDialog.getExistingDirectory(self, "Select Folder")
-        if folder_path:
-            self.file_list.clear()
-            self.folder_path_label.setText(f"Selected Folder: {folder_path}")
-            extension = self.extension_dropdown.currentText()
-            if self.include_subfolders_checkbox.isChecked():
-                for root, dirs, files in os.walk(folder_path):
-                    for file in files:
-                        if file.endswith(extension):
-                            file_path = os.path.relpath(os.path.join(root, file), folder_path)
-                            self.file_list.addItem(file_path)
-            else:
-                for file in os.listdir(folder_path):
-                    if file.endswith(extension):
-                        self.file_list.addItem(file)
-
-    def select_all(self, state):
-        is_checked = self.select_all_checkbox.isChecked()
-        for index in range(self.file_list.count()):
-            item = self.file_list.item(index)
-            item.setSelected(is_checked)
-
-    def combine_datasets(self):
-        selected_files = [self.file_list.item(i).text() for i in range(self.file_list.count()) if self.file_list.item(i).isSelected()]
-        if selected_files:
-            combined_data = None
-            settings_file = None
-            folder_path = self.folder_path_label.text().replace("Selected Folder: ", "")
-            for file_path in selected_files:
-                full_path = os.path.join(folder_path, file_path)
-                with np.load(full_path) as data:
-                    if combined_data is None:
-                        combined_data = data['X']
-                    else:
-                        combined_data = np.concatenate((combined_data, data['X']))
-                    if settings_file is None:
-                        settings_file = data['settings']
-
-            extension = self.extension_dropdown.currentText()
-            save_path, _ = QFileDialog.getSaveFileName(self, "Save Combined Dataset", "", f"NumPy Files (*{extension})")
-            if save_path:
-                if not save_path.endswith(extension):
-                    save_path += extension
-                np.savez(save_path, X=combined_data, settings=settings_file)
-                QMessageBox.information(self, "Success", "Datasets combined successfully.")
-        else:
-            QMessageBox.warning(self, "Warning", "No files selected.")
-
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
-    app.setStyle(QStyleFactory.create('Fusion'))  # Use Fusion or other available styles
-
-    # Customize the palette for a darker, more modern look
-    palette = QPalette()
-    palette.setColor(QPalette.ColorRole.Window, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.WindowText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Base, QColor(25, 25, 25))
-    palette.setColor(QPalette.ColorRole.AlternateBase, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.ToolTipBase, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.ToolTipText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Text, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Button, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.ButtonText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.BrightText, Qt.GlobalColor.red)
-    palette.setColor(QPalette.ColorRole.Link, QColor(42, 130, 218))
-    palette.setColor(QPalette.ColorRole.Highlight, QColor(42, 130, 218))
-    palette.setColor(QPalette.ColorRole.HighlightedText, Qt.GlobalColor.black)
-    app.setPalette(palette)
-
-    window = SDCombineDatasets()
-    window.show()
-    sys.exit(app.exec())
+import sys 
+import os 
+from PySide6 .QtWidgets import QApplication ,QWidget ,QLabel ,QPushButton ,QCheckBox ,QComboBox ,QListWidget ,QVBoxLayout ,QHBoxLayout ,QFileDialog ,QMessageBox ,QStyleFactory 
+from PySide6 .QtCore import Qt 
+from PySide6 .QtGui import QPalette ,QColor ,QFont 
+import numpy as np 
+
+class SDCombineDatasets (QWidget ):
+    def __init__ (self ):
+        super ().__init__ ()
+        self .setWindowTitle ("SD Combine Datasets")
+        self .resize (500 ,700 )
+
+
+        self .app_name_label =QLabel ("SD Combine Datasets")
+        self .app_name_label .setAlignment (Qt .AlignCenter )
+        self .app_name_label .setFont (QFont ("Arial",16 ,QFont .Bold ))
+        self .email_label =QLabel ("shankar.dutt@anu.edu.au")
+        self .email_label .setAlignment (Qt .AlignCenter )
+        self .select_folder_button =QPushButton ("Select Folder")
+        self .include_subfolders_checkbox =QCheckBox ("Include Subfolders")
+        self .extension_dropdown =QComboBox ()
+        self .extension_dropdown .addItems ([".dataset.npz",".MLdataset.npz"])
+        self .file_list =QListWidget ()
+        self .file_list .setSelectionMode (QListWidget .SelectionMode .MultiSelection )
+        self .select_all_checkbox =QCheckBox ("Select All")
+        self .folder_path_label =QLabel ()
+        self .folder_path_label .setWordWrap (True )
+        self .combine_datasets_button =QPushButton ("Combine Datasets")
+
+
+        main_layout =QVBoxLayout ()
+        main_layout .addWidget (self .app_name_label )
+        main_layout .addWidget (self .email_label )
+        main_layout .addWidget (self .select_folder_button )
+        main_layout .addWidget (self .include_subfolders_checkbox )
+        main_layout .addWidget (self .extension_dropdown )
+        main_layout .addWidget (self .file_list )
+        main_layout .addWidget (self .select_all_checkbox )
+        main_layout .addWidget (self .folder_path_label )
+        main_layout .addWidget (self .combine_datasets_button )
+
+        self .setLayout (main_layout )
+
+
+        self .select_folder_button .clicked .connect (self .select_folder )
+        self .select_all_checkbox .stateChanged .connect (self .select_all )
+        self .combine_datasets_button .clicked .connect (self .combine_datasets )
+
+    def select_folder (self ):
+        folder_path =QFileDialog .getExistingDirectory (self ,"Select Folder")
+        if folder_path :
+            self .file_list .clear ()
+            self .folder_path_label .setText (f"Selected Folder: {folder_path}")
+            extension =self .extension_dropdown .currentText ()
+            if self .include_subfolders_checkbox .isChecked ():
+                for root ,dirs ,files in os .walk (folder_path ):
+                    for file in files :
+                        if file .endswith (extension ):
+                            file_path =os .path .relpath (os .path .join (root ,file ),folder_path )
+                            self .file_list .addItem (file_path )
+            else :
+                for file in os .listdir (folder_path ):
+                    if file .endswith (extension ):
+                        self .file_list .addItem (file )
+
+    def select_all (self ,state ):
+        is_checked =self .select_all_checkbox .isChecked ()
+        for index in range (self .file_list .count ()):
+            item =self .file_list .item (index )
+            item .setSelected (is_checked )
+
+    def combine_datasets (self ):
+        selected_files =[self .file_list .item (i ).text ()for i in range (self .file_list .count ())if self .file_list .item (i ).isSelected ()]
+        if selected_files :
+            combined_data =None 
+            settings_file =None 
+            folder_path =self .folder_path_label .text ().replace ("Selected Folder: ","")
+            for file_path in selected_files :
+                full_path =os .path .join (folder_path ,file_path )
+                with np .load (full_path )as data :
+                    if combined_data is None :
+                        combined_data =data ['X']
+                    else :
+                        combined_data =np .concatenate ((combined_data ,data ['X']))
+                    if settings_file is None :
+                        settings_file =data ['settings']
+
+            extension =self .extension_dropdown .currentText ()
+            save_path ,_ =QFileDialog .getSaveFileName (self ,"Save Combined Dataset","",f"NumPy Files (*{extension})")
+            if save_path :
+                if not save_path .endswith (extension ):
+                    save_path +=extension 
+                np .savez (save_path ,X =combined_data ,settings =settings_file )
+                QMessageBox .information (self ,"Success","Datasets combined successfully.")
+        else :
+            QMessageBox .warning (self ,"Warning","No files selected.")
+
+if __name__ =='__main__':
+    app =QApplication (sys .argv )
+    app .setStyle (QStyleFactory .create ('Fusion'))
+
+
+    palette =QPalette ()
+    palette .setColor (QPalette .ColorRole .Window ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .WindowText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Base ,QColor (25 ,25 ,25 ))
+    palette .setColor (QPalette .ColorRole .AlternateBase ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .ToolTipBase ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .ToolTipText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Text ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Button ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .ButtonText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .BrightText ,Qt .GlobalColor .red )
+    palette .setColor (QPalette .ColorRole .Link ,QColor (42 ,130 ,218 ))
+    palette .setColor (QPalette .ColorRole .Highlight ,QColor (42 ,130 ,218 ))
+    palette .setColor (QPalette .ColorRole .HighlightedText ,Qt .GlobalColor .black )
+    app .setPalette (palette )
+
+    window =SDCombineDatasets ()
+    window .show ()
+    sys .exit (app .exec ())
```

### Comparing `nanosense-0.3.1/nanosense/Data Reduction/main.py` & `nanosense-0.3.2/nanosense/Data Reduction/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,547 +1,547 @@
-from PySide6.QtWidgets import (QApplication, QMainWindow, QWidget, QVBoxLayout, QHBoxLayout, QDialog,
-                             QTabWidget, QPushButton, QLabel, QLineEdit, QCheckBox, QComboBox,
-                             QProgressBar, QFileDialog, QListWidget, QGroupBox, QFormLayout,
-                             QSpinBox, QDoubleSpinBox, QScrollArea, QSplitter, QTableWidget, 
-                             QTextEdit, QTableWidgetItem, QToolBar,QListWidgetItem, QSizePolicy,QMessageBox, QInputDialog, QStyleFactory)
-from PySide6.QtCore import Qt, QSize, QTimer
-from PySide6.QtGui import QIcon, QValidator, QTextCursor,QPalette, QColor
-import sys, os
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-from matplotlib.figure import Figure
-import matplotlib.pyplot as plt
-import matplotlib.patches as patches
-from matplotlib.patches import Rectangle
-import neo
-from neo.rawio.axonrawio import AxonRawIO
-from neo.rawio import AxonRawIO
-from neo.core import AnalogSignal
-import numpy as np
-import pyabf
-from scipy.signal import butter, sosfilt, sosfilt_zi, bessel, cheby1, cheby2, ellip, lfilter, firwin
-from scipy.ndimage import uniform_filter1d
-from joblib import Parallel, delayed
-import ruptures as rpt
-import scipy.signal as sig
-import scipy.stats as stats
-import pywt
-import logging
-from datetime import datetime
-import time
-import gc
-import multiprocessing as mp
-from joblib import parallel_backend
-parallel_backend("loky")
-from detecta import detect_cusum
-from hmmlearn import hmm
-from sklearn.mixture import GaussianMixture
-import h5py
-import json
-import math
-import numexpr as ne
-import logging
-
-logging.getLogger("qt").setLevel(logging.WARNING)
-
-def get_hdf5_file_info_window(file_path):
-    with h5py.File(file_path, 'r') as f:
-        sampling_rate = f.attrs['sampling_rate']
-    return sampling_rate
-
-def load_hdf5_file(file_path):
-    global sampling_rate
-    with h5py.File(file_path, 'r') as f:
-        selected_data = f['selected_data'][()]
-        sampling_rate = f.attrs['sampling_rate']
-    return selected_data, sampling_rate
+from PySide6 .QtWidgets import (QApplication ,QMainWindow ,QWidget ,QVBoxLayout ,QHBoxLayout ,QDialog ,
+QTabWidget ,QPushButton ,QLabel ,QLineEdit ,QCheckBox ,QComboBox ,
+QProgressBar ,QFileDialog ,QListWidget ,QGroupBox ,QFormLayout ,
+QSpinBox ,QDoubleSpinBox ,QScrollArea ,QSplitter ,QTableWidget ,
+QTextEdit ,QTableWidgetItem ,QToolBar ,QListWidgetItem ,QSizePolicy ,QMessageBox ,QInputDialog ,QStyleFactory )
+from PySide6 .QtCore import Qt ,QSize ,QTimer 
+from PySide6 .QtGui import QIcon ,QValidator ,QTextCursor ,QPalette ,QColor 
+import sys ,os 
+from matplotlib .backends .backend_qt5agg import FigureCanvasQTAgg as FigureCanvas 
+from matplotlib .backends .backend_qt5agg import NavigationToolbar2QT as NavigationToolbar 
+from matplotlib .figure import Figure 
+import matplotlib .pyplot as plt 
+import matplotlib .patches as patches 
+from matplotlib .patches import Rectangle 
+import neo 
+from neo .rawio .axonrawio import AxonRawIO 
+from neo .rawio import AxonRawIO 
+from neo .core import AnalogSignal 
+import numpy as np 
+import pyabf 
+from scipy .signal import butter ,sosfilt ,sosfilt_zi ,bessel ,cheby1 ,cheby2 ,ellip ,lfilter ,firwin 
+from scipy .ndimage import uniform_filter1d 
+from joblib import Parallel ,delayed 
+import ruptures as rpt 
+import scipy .signal as sig 
+import scipy .stats as stats 
+import pywt 
+import logging 
+from datetime import datetime 
+import time 
+import gc 
+import multiprocessing as mp 
+from joblib import parallel_backend 
+parallel_backend ("loky")
+from detecta import detect_cusum 
+from hmmlearn import hmm 
+from sklearn .mixture import GaussianMixture 
+import h5py 
+import json 
+import math 
+import numexpr as ne 
+import logging 
+
+logging .getLogger ("qt").setLevel (logging .WARNING )
+
+def get_hdf5_file_info_window (file_path ):
+    with h5py .File (file_path ,'r')as f :
+        sampling_rate =f .attrs ['sampling_rate']
+    return sampling_rate 
+
+def load_hdf5_file (file_path ):
+    global sampling_rate 
+    with h5py .File (file_path ,'r')as f :
+        selected_data =f ['selected_data'][()]
+        sampling_rate =f .attrs ['sampling_rate']
+    return selected_data ,sampling_rate 
 
-def get_abf_file_info(file_path):
+def get_abf_file_info (file_path ):
     """
     Returns the total number of data points, length in time, and sampling rate of an .abf file without fully loading it.
     
     Args:
         - file_path (str): Path to the .abf file.
     
     Returns:
         - tuple: A tuple containing the following elements:
             - float: Length of the file in seconds.
             - float: Sampling rate in Hz.
     """
-    # Initialize AxonRawIO with the path to the .abf file
-    raw_io = AxonRawIO(filename=file_path)
-    
-    # Parse the file header to access metadata
-    raw_io.parse_header()
-    
-    # Get the total number of samples for the first block and segment
-    # Note: This example assumes a single block and segment.
-    # Adjust as necessary for files with multiple blocks or segments.
-    signal_size = raw_io.get_signal_size(block_index=0, seg_index=0)
-    
-    # Get the sampling rate
-    sampling_rate = raw_io.get_signal_sampling_rate()
-    
-    # Calculate the length of the file in seconds
-    length_in_seconds = signal_size / sampling_rate
-    return length_in_seconds, sampling_rate
-
-
-def load_abf_file_nth(file_path, nth_point):
-    try:
-        # Create an instance of AxonRawIO
-        raw_io = AxonRawIO(filename=file_path)
-        # Parse the header information
-        raw_io.parse_header()
-        # Define the channel index you're interested in
-        channel_index = 0
-        # Read the signal size for the given block and segment
-        signal_size = raw_io.get_signal_size(block_index=0, seg_index=0)
-        # Calculate the new signal size based on the nth_point
-        new_signal_size = (signal_size + nth_point - 1) // nth_point
-        # Get the byte offset and data type of the signal data
-        sig_dtype = raw_io._raw_data.dtype
-        sig_offset = raw_io._raw_data.offset
-        # Create a memory-mapped array of the signal data
-        signal_data = np.memmap(file_path, dtype=sig_dtype, mode='r', offset=sig_offset, shape=(signal_size,))
-        # Select every nth data point using slicing
-        data = signal_data[::int(nth_point)]
-        # Convert the data to a physical quantity
-        data = raw_io.rescale_signal_raw_to_float(data[:, np.newaxis], dtype='float64', channel_indexes=[channel_index]).flatten()
-        # Get the original sampling rate
-        original_sampling_rate = raw_io.get_signal_sampling_rate()
-        # Calculate the new sampling rate based on the nth_point
-        sampling_rate = original_sampling_rate / nth_point
-        return data, sampling_rate
-    except:
-        try:
-            reader = neo.io.AxonIO(filename=file_path)
-            block = reader.read_block(signal_group_mode='split-all')
-            seg = block.segments[0]
-            analogsignal = seg.analogsignals[0]
-            data = analogsignal.magnitude.flatten()
-            sampling_rate = analogsignal.sampling_rate.magnitude
-            return data, sampling_rate
-        except:
-            try:
-                abf = pyabf.ABF(file_path)
-                data = abf.sweepY
-                sampling_rate = abf.dataRate
-                return data, sampling_rate
-            except:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Icon.Critical)
-                msg.setWindowTitle("Error")
-                msg.setText("An error has occurred.")
-                msg.setInformativeText(f"The selected file ({file_path}) cannot be loaded. \nContact shankar.dutt@anu.edu.au")
-                msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-                msg.exec()
-                return None, None
-
-
-def load_abf_file(file_path):
-    try:
-        # Create an instance of AxonRawIO
-        raw_io = AxonRawIO(filename=file_path)
-
-        # Parse the header information
-        raw_io.parse_header()
-
-        # Define the channel index you're interested in
-        channel_index = 0
-
-        # Read the signal size for the given block and segment without specifying channel_indexes
-        signal_size = raw_io.get_signal_size(block_index=0, seg_index=0)
-
-        # Now, read the analog signal data
-        # Here, we specify channel_indexes when reading the chunk to ensure we only get data for the desired channel
-        data = raw_io.get_analogsignal_chunk(block_index=0, seg_index=0, i_start=0, i_stop=signal_size, channel_indexes=[channel_index])
-
-        # Convert the chunk to a physical quantity
-        data = raw_io.rescale_signal_raw_to_float(data, dtype='float64', channel_indexes=[channel_index]).flatten()
-
-        # Get the sampling rate for the specified channel
-        sampling_rate = raw_io.get_signal_sampling_rate()
-        return data, sampling_rate
-    
-    except:
-        try:
-            reader = neo.io.AxonIO(filename=file_path)
-            block = reader.read_block(signal_group_mode='split-all')
-            seg = block.segments[0]
-            analogsignal = seg.analogsignals[0]
-            data = analogsignal.magnitude.flatten()
-            sampling_rate = analogsignal.sampling_rate.magnitude
-            return data, sampling_rate
-        except:
-            try:
-                abf = pyabf.ABF(file_path)
-                data = abf.sweepY
-                sampling_rate = abf.dataRate
-                return data, sampling_rate
-            except:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Icon.Critical)
-                msg.setWindowTitle("Error")
-                msg.setText("An error has occurred.")
-                msg.setInformativeText(f"The selected file ({file_path}) cannot be loaded. \nContact shankar.dutt@anu.edu.au")
-                msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-                msg.exec()
-                return None, None
-
-def _thselect(data, th_type):
-    def _sqtwolog(x, n):
-        return np.sqrt(2 * np.log(n))
-    
-    def _minimaxi(x, n):
-        if n <= 32:
-            return 0
-        else:
-            return 0.3936 + 0.1829 * (np.log(n) / np.log(2))
-    
-    try:
-        th_algo = {
-            'sqtwolog': _sqtwolog,
-            'minimaxi': _minimaxi,
-        }[th_type]
-        
-        # Apply to flattened data to handle multi-level coefficients
-        flat_data = np.concatenate([np.ravel(d) for d in data[1:]])
-        return th_algo(flat_data, len(flat_data))
-    except KeyError:
-        # Fallback to sqtwolog if th_type is not recognized
-        flat_data = np.concatenate([np.ravel(d) for d in data[1:]])
-        return _sqtwolog(flat_data, len(flat_data))
-    
 
-def apply_low_pass_filter_window(data, cutoff_frequency,type, sampling_rate_window):
-    if cutoff_frequency<sampling_rate_window/2:    
-        if type == 'Butterworth':
-            nyquist_rate = sampling_rate_window / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            sos = butter(N=8, Wn=cutoff, btype='low', analog=False, output='sos')
-            
-            # Compute initial conditions for the filter
-            zi = sosfilt_zi(sos) * data[0]
-            
-            # Apply the filter with the initial conditions
-            filtered_data, _ = sosfilt(sos, data, zi=zi)
-            
-            return filtered_data
-        elif type == 'Bessel':
-            nyquist_rate = sampling_rate_window / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            sos = bessel(N=8, Wn=cutoff, btype='low', analog=False, output='sos')
-            
-            # Compute initial conditions for the filter
-            zi = sosfilt_zi(sos) * data[0]
-            
-            # Apply the filter with the initial conditions
-            filtered_data, _ = sosfilt(sos, data, zi=zi)
-            
-            return filtered_data
-        
-        elif type == 'Wavelet':
-            wavelet_type='db4'
-            wavelet_level=None
-            wavelet_threshold_sub_type='sqtwolog'
-            wavelet_threshold_type='soft'
-            w = pywt.Wavelet(wavelet_type)
-            max_level = pywt.dwt_max_level(len(data), filter_len=w.dec_len)
-            if wavelet_level is None:
-                wavelet_level = max_level
-            wcoeff = pywt.wavedec(data, w, mode='sym', level=wavelet_level)
-            
-            thresh = np.std(wcoeff[-1]) * _thselect(wcoeff, wavelet_threshold_sub_type)
-            wcoeff[1:] = [pywt.threshold(wc, thresh, wavelet_threshold_type) for wc in wcoeff[1:]]
-            
-            filtered_data = pywt.waverec(wcoeff, wavelet_type, mode='sym')
-            return filtered_data
-    else:
-        msg = QMessageBox()
-        msg.setIcon(QMessageBox.Icon.Critical)
-        msg.setWindowTitle("Error")
-        msg.setText("An error has occurred.")
-        msg.setInformativeText(f"The selected cutoff frequency is more than sampling rate/2.")
-        msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-        msg.exec()
-        return data
-    
-def exponential_weights(window_size):
-    alpha = 2 / (window_size + 1)
-    weights = np.exp(-alpha * np.arange(window_size))
-    return weights / weights.sum()
-
-def smooth_threshold(threshold, window_size, smoothing_index, exp_weights=None):
-    window_size = 10*window_size
-    if smoothing_index == 0:
-        smoothed_threshold = sig.fftconvolve(threshold, np.ones(window_size) / window_size, mode='same')
-    elif smoothing_index == 1:
-        if exp_weights is None:
-            exp_weights = exponential_weights(window_size)
-        smoothed_threshold = sig.fftconvolve(threshold, exp_weights, mode='same')
-    else:
-        raise ValueError("Invalid smoothing method. Choose 'moving_average' or 'exponential'.")
-    return smoothed_threshold
-    
-def calculate_rolling_stats_window(data, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate_window):
-    avg_window_size_samples = int((avg_window_size_in_ms / 1000) * sampling_rate_window)
-    std_window_size_samples = int((std_window_size_in_ms / 1000) * sampling_rate_window)
-    
-    rolling_avg = uniform_filter1d(data, size=avg_window_size_samples)
-    rolling_std = np.sqrt(uniform_filter1d(data**2, size=std_window_size_samples) - uniform_filter1d(data, size=std_window_size_samples)**2)
-    
-    return rolling_avg, rolling_std
+    raw_io =AxonRawIO (filename =file_path )
 
 
-def find_preliminary_events_window(data, threshold_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, dips, sampling_rate_window):
-    rolling_avg, rolling_std = calculate_rolling_stats_window(data, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate_window)
-    
-    if threshold_method == "multiplier":
-        if dips == "Yes":
-            threshold = rolling_avg - (threshold_multiplier * rolling_std)
-        else:
-            threshold = rolling_avg + (threshold_multiplier * rolling_std)
-    elif threshold_method == "difference":
-        if dips == "Yes":
-            threshold = rolling_avg - (threshold_difference / 1000)
-        else:
-            threshold = rolling_avg + (threshold_difference / 1000)
-    else:
-        raise ValueError("Unsupported threshold_method. Use 'multiplier' or 'difference'.")
-    
-    
-    events = []
-    in_event = False
-    for i in range(1, len(data)):
-        if not in_event and data[i] < threshold[i] and data[i-1] >= threshold[i-1]:
-            in_event = True
-            event_start = i
-        elif in_event and data[i] >= threshold[i] and data[i-1] < threshold[i-1]:
-            event_end = i  # Mark the event end at the first crossing
-            events.append((event_start, event_end))
-            in_event = False
-    return events
-
-
-def exclude_events_and_recalculate_stats_window(data, events, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate_window):
-    data_without_events = np.copy(data)
-    for start, end in events:
-        data_without_events[start:end] = np.nan  # Exclude event data by setting it to NaN
-
-    # Replace NaNs with the mean of their neighboring values for a smooth transition
-    nan_indices = np.where(np.isnan(data_without_events))[0]
-    for idx in nan_indices:
-        if idx > 0 and idx < len(data_without_events) - 1:
-            data_without_events[idx] = np.nanmean(data_without_events[idx - 1:idx + 2])
-
-    rolling_avg, rolling_std = calculate_rolling_stats_window(data, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate_window)
-    return rolling_avg, rolling_std
-
-
-def find_events_refined_window(data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, dips, sampling_rate_window):
-    # Step 1: Find preliminary events
-    preliminary_events = find_preliminary_events_window(data, threshold_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, dips, sampling_rate_window)
-
-    # Step 2: Recalculate statistics excluding preliminary events
-    rolling_avg_refined, rolling_std_refined = exclude_events_and_recalculate_stats_window(data, preliminary_events, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate_window)
-
-    # Step 3: Use the refined statistics to find events again
-    adjusted_baseline_start = rolling_avg_refined - start_multiplier * rolling_std_refined
-    adjusted_baseline_end = rolling_avg_refined - end_multiplier * rolling_std_refined
-
-    if threshold_method == "multiplier":
-        if dips == "Yes":
-            threshold_refined = rolling_avg_refined - (threshold_multiplier * rolling_std_refined)
-        else:
-            threshold_refined = rolling_avg_refined + (threshold_multiplier * rolling_std_refined)
-    elif threshold_method == "difference":
-        if dips == "Yes":
-            threshold_refined = rolling_avg_refined - (threshold_difference / 1000)   
-        else:
-            threshold_refined = rolling_avg_refined + (threshold_difference / 1000)   
-
-    all_refined_events = []
-    in_event = False
-    for i in range(1, len(data)):
-        if not in_event and data[i] < threshold_refined[i] and data[i-1] >= threshold_refined[i-1]:
-            in_event = True
-            event_start = i
-            # Backtrack to refine event start
-            while event_start > 0 and not (data[event_start] < adjusted_baseline_start[event_start] and data[event_start-1] >= adjusted_baseline_start[event_start-1]):
-                event_start -= 1
-        elif in_event and data[i] >= adjusted_baseline_end[i] and data[i-1] < adjusted_baseline_end[i-1]:
-            event_end = i  # Mark the event end at the first crossing
-            all_refined_events.append((event_start, event_end))
-            in_event = False
-
-    # Step 4: Filter events based on their width (duration)
-    filtered_events = []
-    for start, end in all_refined_events:
-        event_width_in_seconds = (end - start) / sampling_rate_window
-        if min_event_width <= event_width_in_seconds <= max_event_width:
-            filtered_events.append((start, end))
-    
-    return filtered_events
+    raw_io .parse_header ()
+
+
+
+
+    signal_size =raw_io .get_signal_size (block_index =0 ,seg_index =0 )
+
+
+    sampling_rate =raw_io .get_signal_sampling_rate ()
+
+
+    length_in_seconds =signal_size /sampling_rate 
+    return length_in_seconds ,sampling_rate 
+
+
+def load_abf_file_nth (file_path ,nth_point ):
+    try :
+
+        raw_io =AxonRawIO (filename =file_path )
+
+        raw_io .parse_header ()
+
+        channel_index =0 
+
+        signal_size =raw_io .get_signal_size (block_index =0 ,seg_index =0 )
+
+        new_signal_size =(signal_size +nth_point -1 )//nth_point 
+
+        sig_dtype =raw_io ._raw_data .dtype 
+        sig_offset =raw_io ._raw_data .offset 
+
+        signal_data =np .memmap (file_path ,dtype =sig_dtype ,mode ='r',offset =sig_offset ,shape =(signal_size ,))
+
+        data =signal_data [::int (nth_point )]
+
+        data =raw_io .rescale_signal_raw_to_float (data [:,np .newaxis ],dtype ='float64',channel_indexes =[channel_index ]).flatten ()
+
+        original_sampling_rate =raw_io .get_signal_sampling_rate ()
+
+        sampling_rate =original_sampling_rate /nth_point 
+        return data ,sampling_rate 
+    except :
+        try :
+            reader =neo .io .AxonIO (filename =file_path )
+            block =reader .read_block (signal_group_mode ='split-all')
+            seg =block .segments [0 ]
+            analogsignal =seg .analogsignals [0 ]
+            data =analogsignal .magnitude .flatten ()
+            sampling_rate =analogsignal .sampling_rate .magnitude 
+            return data ,sampling_rate 
+        except :
+            try :
+                abf =pyabf .ABF (file_path )
+                data =abf .sweepY 
+                sampling_rate =abf .dataRate 
+                return data ,sampling_rate 
+            except :
+                msg =QMessageBox ()
+                msg .setIcon (QMessageBox .Icon .Critical )
+                msg .setWindowTitle ("Error")
+                msg .setText ("An error has occurred.")
+                msg .setInformativeText (f"The selected file ({file_path}) cannot be loaded. \nContact shankar.dutt@anu.edu.au")
+                msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+                msg .exec ()
+                return None ,None 
+
+
+def load_abf_file (file_path ):
+    try :
+
+        raw_io =AxonRawIO (filename =file_path )
+
+
+        raw_io .parse_header ()
+
+
+        channel_index =0 
+
+
+        signal_size =raw_io .get_signal_size (block_index =0 ,seg_index =0 )
+
+
+
+        data =raw_io .get_analogsignal_chunk (block_index =0 ,seg_index =0 ,i_start =0 ,i_stop =signal_size ,channel_indexes =[channel_index ])
+
+
+        data =raw_io .rescale_signal_raw_to_float (data ,dtype ='float64',channel_indexes =[channel_index ]).flatten ()
 
-def process_chunk_window_abf(file_path, desired_duration, chunk_index, chunk_size, step, channel_index, signal_size, sampling_rate, filter_type, cutoff_freq, threshold_method, dips, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference,avg_window_size_in_ms, std_window_size_in_ms, min_event_width, max_event_width, start_index):
+
+        sampling_rate =raw_io .get_signal_sampling_rate ()
+        return data ,sampling_rate 
+
+    except :
+        try :
+            reader =neo .io .AxonIO (filename =file_path )
+            block =reader .read_block (signal_group_mode ='split-all')
+            seg =block .segments [0 ]
+            analogsignal =seg .analogsignals [0 ]
+            data =analogsignal .magnitude .flatten ()
+            sampling_rate =analogsignal .sampling_rate .magnitude 
+            return data ,sampling_rate 
+        except :
+            try :
+                abf =pyabf .ABF (file_path )
+                data =abf .sweepY 
+                sampling_rate =abf .dataRate 
+                return data ,sampling_rate 
+            except :
+                msg =QMessageBox ()
+                msg .setIcon (QMessageBox .Icon .Critical )
+                msg .setWindowTitle ("Error")
+                msg .setText ("An error has occurred.")
+                msg .setInformativeText (f"The selected file ({file_path}) cannot be loaded. \nContact shankar.dutt@anu.edu.au")
+                msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+                msg .exec ()
+                return None ,None 
+
+def _thselect (data ,th_type ):
+    def _sqtwolog (x ,n ):
+        return np .sqrt (2 *np .log (n ))
+
+    def _minimaxi (x ,n ):
+        if n <=32 :
+            return 0 
+        else :
+            return 0.3936 +0.1829 *(np .log (n )/np .log (2 ))
+
+    try :
+        th_algo ={
+        'sqtwolog':_sqtwolog ,
+        'minimaxi':_minimaxi ,
+        }[th_type ]
+
+
+        flat_data =np .concatenate ([np .ravel (d )for d in data [1 :]])
+        return th_algo (flat_data ,len (flat_data ))
+    except KeyError :
+
+        flat_data =np .concatenate ([np .ravel (d )for d in data [1 :]])
+        return _sqtwolog (flat_data ,len (flat_data ))
+
+
+def apply_low_pass_filter_window (data ,cutoff_frequency ,type ,sampling_rate_window ):
+    if cutoff_frequency <sampling_rate_window /2 :
+        if type =='Butterworth':
+            nyquist_rate =sampling_rate_window /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            sos =butter (N =8 ,Wn =cutoff ,btype ='low',analog =False ,output ='sos')
+
+
+            zi =sosfilt_zi (sos )*data [0 ]
+
+
+            filtered_data ,_ =sosfilt (sos ,data ,zi =zi )
+
+            return filtered_data 
+        elif type =='Bessel':
+            nyquist_rate =sampling_rate_window /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            sos =bessel (N =8 ,Wn =cutoff ,btype ='low',analog =False ,output ='sos')
+
+
+            zi =sosfilt_zi (sos )*data [0 ]
+
+
+            filtered_data ,_ =sosfilt (sos ,data ,zi =zi )
+
+            return filtered_data 
+
+        elif type =='Wavelet':
+            wavelet_type ='db4'
+            wavelet_level =None 
+            wavelet_threshold_sub_type ='sqtwolog'
+            wavelet_threshold_type ='soft'
+            w =pywt .Wavelet (wavelet_type )
+            max_level =pywt .dwt_max_level (len (data ),filter_len =w .dec_len )
+            if wavelet_level is None :
+                wavelet_level =max_level 
+            wcoeff =pywt .wavedec (data ,w ,mode ='sym',level =wavelet_level )
+
+            thresh =np .std (wcoeff [-1 ])*_thselect (wcoeff ,wavelet_threshold_sub_type )
+            wcoeff [1 :]=[pywt .threshold (wc ,thresh ,wavelet_threshold_type )for wc in wcoeff [1 :]]
+
+            filtered_data =pywt .waverec (wcoeff ,wavelet_type ,mode ='sym')
+            return filtered_data 
+    else :
+        msg =QMessageBox ()
+        msg .setIcon (QMessageBox .Icon .Critical )
+        msg .setWindowTitle ("Error")
+        msg .setText ("An error has occurred.")
+        msg .setInformativeText (f"The selected cutoff frequency is more than sampling rate/2.")
+        msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+        msg .exec ()
+        return data 
+
+def exponential_weights (window_size ):
+    alpha =2 /(window_size +1 )
+    weights =np .exp (-alpha *np .arange (window_size ))
+    return weights /weights .sum ()
+
+def smooth_threshold (threshold ,window_size ,smoothing_index ,exp_weights =None ):
+    window_size =10 *window_size 
+    if smoothing_index ==0 :
+        smoothed_threshold =sig .fftconvolve (threshold ,np .ones (window_size )/window_size ,mode ='same')
+    elif smoothing_index ==1 :
+        if exp_weights is None :
+            exp_weights =exponential_weights (window_size )
+        smoothed_threshold =sig .fftconvolve (threshold ,exp_weights ,mode ='same')
+    else :
+        raise ValueError ("Invalid smoothing method. Choose 'moving_average' or 'exponential'.")
+    return smoothed_threshold 
+
+def calculate_rolling_stats_window (data ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate_window ):
+    avg_window_size_samples =int ((avg_window_size_in_ms /1000 )*sampling_rate_window )
+    std_window_size_samples =int ((std_window_size_in_ms /1000 )*sampling_rate_window )
+
+    rolling_avg =uniform_filter1d (data ,size =avg_window_size_samples )
+    rolling_std =np .sqrt (uniform_filter1d (data **2 ,size =std_window_size_samples )-uniform_filter1d (data ,size =std_window_size_samples )**2 )
+
+    return rolling_avg ,rolling_std 
+
+
+def find_preliminary_events_window (data ,threshold_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,dips ,sampling_rate_window ):
+    rolling_avg ,rolling_std =calculate_rolling_stats_window (data ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate_window )
+
+    if threshold_method =="multiplier":
+        if dips =="Yes":
+            threshold =rolling_avg -(threshold_multiplier *rolling_std )
+        else :
+            threshold =rolling_avg +(threshold_multiplier *rolling_std )
+    elif threshold_method =="difference":
+        if dips =="Yes":
+            threshold =rolling_avg -(threshold_difference /1000 )
+        else :
+            threshold =rolling_avg +(threshold_difference /1000 )
+    else :
+        raise ValueError ("Unsupported threshold_method. Use 'multiplier' or 'difference'.")
+
+
+    events =[]
+    in_event =False 
+    for i in range (1 ,len (data )):
+        if not in_event and data [i ]<threshold [i ]and data [i -1 ]>=threshold [i -1 ]:
+            in_event =True 
+            event_start =i 
+        elif in_event and data [i ]>=threshold [i ]and data [i -1 ]<threshold [i -1 ]:
+            event_end =i 
+            events .append ((event_start ,event_end ))
+            in_event =False 
+    return events 
+
+
+def exclude_events_and_recalculate_stats_window (data ,events ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate_window ):
+    data_without_events =np .copy (data )
+    for start ,end in events :
+        data_without_events [start :end ]=np .nan 
+
+
+    nan_indices =np .where (np .isnan (data_without_events ))[0 ]
+    for idx in nan_indices :
+        if idx >0 and idx <len (data_without_events )-1 :
+            data_without_events [idx ]=np .nanmean (data_without_events [idx -1 :idx +2 ])
+
+    rolling_avg ,rolling_std =calculate_rolling_stats_window (data ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate_window )
+    return rolling_avg ,rolling_std 
+
+
+def find_events_refined_window (data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,dips ,sampling_rate_window ):
+
+    preliminary_events =find_preliminary_events_window (data ,threshold_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,dips ,sampling_rate_window )
+
+
+    rolling_avg_refined ,rolling_std_refined =exclude_events_and_recalculate_stats_window (data ,preliminary_events ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate_window )
+
+
+    adjusted_baseline_start =rolling_avg_refined -start_multiplier *rolling_std_refined 
+    adjusted_baseline_end =rolling_avg_refined -end_multiplier *rolling_std_refined 
+
+    if threshold_method =="multiplier":
+        if dips =="Yes":
+            threshold_refined =rolling_avg_refined -(threshold_multiplier *rolling_std_refined )
+        else :
+            threshold_refined =rolling_avg_refined +(threshold_multiplier *rolling_std_refined )
+    elif threshold_method =="difference":
+        if dips =="Yes":
+            threshold_refined =rolling_avg_refined -(threshold_difference /1000 )
+        else :
+            threshold_refined =rolling_avg_refined +(threshold_difference /1000 )
+
+    all_refined_events =[]
+    in_event =False 
+    for i in range (1 ,len (data )):
+        if not in_event and data [i ]<threshold_refined [i ]and data [i -1 ]>=threshold_refined [i -1 ]:
+            in_event =True 
+            event_start =i 
+
+            while event_start >0 and not (data [event_start ]<adjusted_baseline_start [event_start ]and data [event_start -1 ]>=adjusted_baseline_start [event_start -1 ]):
+                event_start -=1 
+        elif in_event and data [i ]>=adjusted_baseline_end [i ]and data [i -1 ]<adjusted_baseline_end [i -1 ]:
+            event_end =i 
+            all_refined_events .append ((event_start ,event_end ))
+            in_event =False 
+
+
+    filtered_events =[]
+    for start ,end in all_refined_events :
+        event_width_in_seconds =(end -start )/sampling_rate_window 
+        if min_event_width <=event_width_in_seconds <=max_event_width :
+            filtered_events .append ((start ,end ))
+
+    return filtered_events 
+
+def process_chunk_window_abf (file_path ,desired_duration ,chunk_index ,chunk_size ,step ,channel_index ,signal_size ,sampling_rate ,filter_type ,cutoff_freq ,threshold_method ,dips ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,min_event_width ,max_event_width ,start_index ):
     """
     Process a single chunk of the file.
     This function is intended to be executed in a thread pool.
     """
-    adjusted_sampling_rate = sampling_rate / step
-    i_start = max(int(chunk_index * chunk_size * step), int(start_index))
-    i_stop = min(int((chunk_index + 1) * chunk_size * step), int(signal_size), int(start_index + desired_duration * sampling_rate))
-    i_stop = min(i_stop, int(signal_size))  # Ensure not exceeding the signal size  
-    
-    # Initialize AxonRawIO for each worker to avoid sharing state
-    raw_io = AxonRawIO(filename=file_path)
-    raw_io.parse_header()
-    
-    raw_chunk = raw_io.get_analogsignal_chunk(block_index=0, seg_index=0, i_start=i_start, i_stop=i_stop, channel_indexes=[channel_index])
-    chunk_data = raw_io.rescale_signal_raw_to_float(raw_chunk, dtype='float64', channel_indexes=[channel_index]).flatten()
-    selected_chunk_data = chunk_data[::step]
+    adjusted_sampling_rate =sampling_rate /step 
+    i_start =max (int (chunk_index *chunk_size *step ),int (start_index ))
+    i_stop =min (int ((chunk_index +1 )*chunk_size *step ),int (signal_size ),int (start_index +desired_duration *sampling_rate ))
+    i_stop =min (i_stop ,int (signal_size ))
+
 
-    chunk_data =  apply_low_pass_filter_window(selected_chunk_data, cutoff_freq, filter_type, adjusted_sampling_rate)
+    raw_io =AxonRawIO (filename =file_path )
+    raw_io .parse_header ()
 
-    events =  find_events_refined_window(chunk_data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, dips, adjusted_sampling_rate)
-    rolling_avg_refined, rolling_std_refined = exclude_events_and_recalculate_stats_window(chunk_data, events, avg_window_size_in_ms, std_window_size_in_ms, adjusted_sampling_rate)
-    return events, rolling_avg_refined, rolling_std_refined
+    raw_chunk =raw_io .get_analogsignal_chunk (block_index =0 ,seg_index =0 ,i_start =i_start ,i_stop =i_stop ,channel_indexes =[channel_index ])
+    chunk_data =raw_io .rescale_signal_raw_to_float (raw_chunk ,dtype ='float64',channel_indexes =[channel_index ]).flatten ()
+    selected_chunk_data =chunk_data [::step ]
 
+    chunk_data =apply_low_pass_filter_window (selected_chunk_data ,cutoff_freq ,filter_type ,adjusted_sampling_rate )
 
-def process_chunk_window_abf_with_data(file_path, desired_duration, chunk_index, chunk_size, step, channel_index, signal_size, sampling_rate, filter_type, cutoff_freq, threshold_method, dips, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference,avg_window_size_in_ms, std_window_size_in_ms, min_event_width, max_event_width, start_index):
+    events =find_events_refined_window (chunk_data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,dips ,adjusted_sampling_rate )
+    rolling_avg_refined ,rolling_std_refined =exclude_events_and_recalculate_stats_window (chunk_data ,events ,avg_window_size_in_ms ,std_window_size_in_ms ,adjusted_sampling_rate )
+    return events ,rolling_avg_refined ,rolling_std_refined 
+
+
+def process_chunk_window_abf_with_data (file_path ,desired_duration ,chunk_index ,chunk_size ,step ,channel_index ,signal_size ,sampling_rate ,filter_type ,cutoff_freq ,threshold_method ,dips ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,min_event_width ,max_event_width ,start_index ):
     """
     Process a single chunk of the file and return events, rolling averages, rolling standard deviations, and chunk data.
     This function is intended to be executed in a thread pool.
     """
-    adjusted_sampling_rate = sampling_rate / step
-    i_start = max(int(chunk_index * chunk_size * step), int(start_index))
-    i_stop = min(int((chunk_index + 1) * chunk_size * step), int(signal_size), int(start_index + desired_duration * sampling_rate))
-    i_stop = min(i_stop, int(signal_size))  # Ensure not exceeding the signal size  
-    
-    # Initialize AxonRawIO for each worker to avoid sharing state
-    raw_io = AxonRawIO(filename=file_path)
-    raw_io.parse_header()
-    
-    raw_chunk = raw_io.get_analogsignal_chunk(block_index=0, seg_index=0, i_start=i_start, i_stop=i_stop, channel_indexes=[channel_index])
-    chunk_data = raw_io.rescale_signal_raw_to_float(raw_chunk, dtype='float64', channel_indexes=[channel_index]).flatten()
-    selected_chunk_data = chunk_data[::step]
+    adjusted_sampling_rate =sampling_rate /step 
+    i_start =max (int (chunk_index *chunk_size *step ),int (start_index ))
+    i_stop =min (int ((chunk_index +1 )*chunk_size *step ),int (signal_size ),int (start_index +desired_duration *sampling_rate ))
+    i_stop =min (i_stop ,int (signal_size ))
+
+
+    raw_io =AxonRawIO (filename =file_path )
+    raw_io .parse_header ()
+
+    raw_chunk =raw_io .get_analogsignal_chunk (block_index =0 ,seg_index =0 ,i_start =i_start ,i_stop =i_stop ,channel_indexes =[channel_index ])
+    chunk_data =raw_io .rescale_signal_raw_to_float (raw_chunk ,dtype ='float64',channel_indexes =[channel_index ]).flatten ()
+    selected_chunk_data =chunk_data [::step ]
 
-    chunk_data =  apply_low_pass_filter_window(selected_chunk_data, cutoff_freq, filter_type, adjusted_sampling_rate)
+    chunk_data =apply_low_pass_filter_window (selected_chunk_data ,cutoff_freq ,filter_type ,adjusted_sampling_rate )
 
-    events =  find_events_refined_window(chunk_data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, dips, adjusted_sampling_rate)
-    rolling_avg_refined, rolling_std_refined = exclude_events_and_recalculate_stats_window(chunk_data, events, avg_window_size_in_ms, std_window_size_in_ms, adjusted_sampling_rate)
-    return events, rolling_avg_refined, rolling_std_refined, chunk_data
+    events =find_events_refined_window (chunk_data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,dips ,adjusted_sampling_rate )
+    rolling_avg_refined ,rolling_std_refined =exclude_events_and_recalculate_stats_window (chunk_data ,events ,avg_window_size_in_ms ,std_window_size_in_ms ,adjusted_sampling_rate )
+    return events ,rolling_avg_refined ,rolling_std_refined ,chunk_data 
 
 
 
-def process_chunk_window_hdf5(file_path, dataset_name, desired_duration, chunk_index, chunk_size, step, signal_size, sampling_rate, filter_type, cutoff_freq, threshold_method, dips, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, min_event_width, max_event_width, start_index):
+def process_chunk_window_hdf5 (file_path ,dataset_name ,desired_duration ,chunk_index ,chunk_size ,step ,signal_size ,sampling_rate ,filter_type ,cutoff_freq ,threshold_method ,dips ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,min_event_width ,max_event_width ,start_index ):
     """
     Process a single chunk of the HDF5 dataset.
     This function is intended to be executed in a thread pool.
     """
-    adjusted_sampling_rate = sampling_rate / step
-    i_start = max(chunk_index * chunk_size * step, start_index)
-    i_stop = min((chunk_index + 1) * chunk_size * step, signal_size, start_index + desired_duration * sampling_rate)
-    i_stop = min(i_stop, signal_size)  # Ensure not exceeding the signal size
+    adjusted_sampling_rate =sampling_rate /step 
+    i_start =max (chunk_index *chunk_size *step ,start_index )
+    i_stop =min ((chunk_index +1 )*chunk_size *step ,signal_size ,start_index +desired_duration *sampling_rate )
+    i_stop =min (i_stop ,signal_size )
 
-    with h5py.File(file_path, 'r') as f:
-        chunk_data = f[dataset_name][i_start:i_stop:step]
+    with h5py .File (file_path ,'r')as f :
+        chunk_data =f [dataset_name ][i_start :i_stop :step ]
 
-    chunk_data = apply_low_pass_filter_window(chunk_data, cutoff_freq, filter_type, adjusted_sampling_rate)
+    chunk_data =apply_low_pass_filter_window (chunk_data ,cutoff_freq ,filter_type ,adjusted_sampling_rate )
 
-    events = find_events_refined_window(chunk_data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, dips, adjusted_sampling_rate)
-    rolling_avg_refined, rolling_std_refined = exclude_events_and_recalculate_stats_window(chunk_data, events, avg_window_size_in_ms, std_window_size_in_ms, adjusted_sampling_rate)
-    return events, rolling_avg_refined, rolling_std_refined
+    events =find_events_refined_window (chunk_data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,dips ,adjusted_sampling_rate )
+    rolling_avg_refined ,rolling_std_refined =exclude_events_and_recalculate_stats_window (chunk_data ,events ,avg_window_size_in_ms ,std_window_size_in_ms ,adjusted_sampling_rate )
+    return events ,rolling_avg_refined ,rolling_std_refined 
 
 
-def process_chunk_window_hdf5_with_data(file_path, dataset_name, desired_duration, chunk_index, chunk_size, step, signal_size, sampling_rate, filter_type, cutoff_freq, threshold_method, dips, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, min_event_width, max_event_width, start_index):
+def process_chunk_window_hdf5_with_data (file_path ,dataset_name ,desired_duration ,chunk_index ,chunk_size ,step ,signal_size ,sampling_rate ,filter_type ,cutoff_freq ,threshold_method ,dips ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,min_event_width ,max_event_width ,start_index ):
     """
     Process a single chunk of the HDF5 dataset.
     This function is intended to be executed in a thread pool.
     """
-    adjusted_sampling_rate = sampling_rate / step
-    i_start = max(chunk_index * chunk_size * step, start_index)
-    i_stop = min((chunk_index + 1) * chunk_size * step, signal_size, start_index + desired_duration * sampling_rate)
-    i_stop = min(i_stop, signal_size)  # Ensure not exceeding the signal size
-
-    with h5py.File(file_path, 'r') as f:
-        chunk_data = f[dataset_name][i_start:i_stop:step]
-
-    chunk_data = apply_low_pass_filter_window(chunk_data, cutoff_freq, filter_type, adjusted_sampling_rate)
-
-    events = find_events_refined_window(chunk_data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, dips, adjusted_sampling_rate)
-    rolling_avg_refined, rolling_std_refined = exclude_events_and_recalculate_stats_window(chunk_data, events, avg_window_size_in_ms, std_window_size_in_ms, adjusted_sampling_rate)
-    return events, rolling_avg_refined, rolling_std_refined, chunk_data
-    
-
-def apply_low_pass_filter(data, cutoff_frequency, type, sampling_rate):
-    if cutoff_frequency < sampling_rate / 2:
-        if type == 'Butterworth':
-            nyquist_rate = sampling_rate / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            sos = butter(N=8, Wn=cutoff, btype='low', analog=False, output='sos')
-            zi = sosfilt_zi(sos) * data[0]
-            filtered_data, _ = sosfilt(sos, data, zi=zi)
-            return filtered_data
-        elif type == 'Bessel':
-            nyquist_rate = sampling_rate / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            sos = bessel(N=8, Wn=cutoff, btype='low', analog=False, output='sos')
-            zi = sosfilt_zi(sos) * data[0]
-            filtered_data, _ = sosfilt(sos, data, zi=zi)
-            return filtered_data
-        elif type == 'Chebyshev I':
-            nyquist_rate = sampling_rate / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            sos = cheby1(N=8, rp=0.1, Wn=cutoff, btype='low', analog=False, output='sos')
-            zi = sosfilt_zi(sos) * data[0]
-            filtered_data, _ = sosfilt(sos, data, zi=zi)
-            return filtered_data
-        elif type == 'Chebyshev II':
-            nyquist_rate = sampling_rate / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            sos = cheby2(N=8, rs=40, Wn=cutoff, btype='low', analog=False, output='sos')
-            zi = sosfilt_zi(sos) * data[0]
-            filtered_data, _ = sosfilt(sos, data, zi=zi)
-            return filtered_data
-        elif type == 'Elliptic':
-            nyquist_rate = sampling_rate / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            sos = ellip(N=8, rp=0.1, rs=40, Wn=cutoff, btype='low', analog=False, output='sos')
-            zi = sosfilt_zi(sos) * data[0]
-            filtered_data, _ = sosfilt(sos, data, zi=zi)
-            return filtered_data
-        elif type == 'FIR':
-            nyquist_rate = sampling_rate / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            taps = firwin(101, cutoff)
-            filtered_data = lfilter(taps, 1, data)
-            return filtered_data
-        elif type == 'IIR':
-            nyquist_rate = sampling_rate / 2.0
-            cutoff = cutoff_frequency / nyquist_rate
-            b, a = butter(N=8, Wn=cutoff, btype='low', analog=False)
-            filtered_data = lfilter(b, a, data)
-            return filtered_data
-        elif type == 'Wavelet':
-            wavelet_type = 'db4'
-            wavelet_level = None
-            wavelet_threshold_sub_type = 'sqtwolog'
-            wavelet_threshold_type = 'soft'
-            w = pywt.Wavelet(wavelet_type)
-            max_level = pywt.dwt_max_level(len(data), filter_len=w.dec_len)
-            if wavelet_level is None:
-                wavelet_level = max_level
-            wcoeff = pywt.wavedec(data, w, mode='sym', level=wavelet_level)
-            thresh = np.std(wcoeff[-1]) * _thselect(wcoeff, wavelet_threshold_sub_type)
-            wcoeff[1:] = [pywt.threshold(wc, thresh, wavelet_threshold_type) for wc in wcoeff[1:]]
-            filtered_data = pywt.waverec(wcoeff, wavelet_type, mode='sym')
-            return filtered_data
-        elif type == 'Kalman':
+    adjusted_sampling_rate =sampling_rate /step 
+    i_start =max (chunk_index *chunk_size *step ,start_index )
+    i_stop =min ((chunk_index +1 )*chunk_size *step ,signal_size ,start_index +desired_duration *sampling_rate )
+    i_stop =min (i_stop ,signal_size )
+
+    with h5py .File (file_path ,'r')as f :
+        chunk_data =f [dataset_name ][i_start :i_stop :step ]
+
+    chunk_data =apply_low_pass_filter_window (chunk_data ,cutoff_freq ,filter_type ,adjusted_sampling_rate )
+
+    events =find_events_refined_window (chunk_data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,dips ,adjusted_sampling_rate )
+    rolling_avg_refined ,rolling_std_refined =exclude_events_and_recalculate_stats_window (chunk_data ,events ,avg_window_size_in_ms ,std_window_size_in_ms ,adjusted_sampling_rate )
+    return events ,rolling_avg_refined ,rolling_std_refined ,chunk_data 
+
+
+def apply_low_pass_filter (data ,cutoff_frequency ,type ,sampling_rate ):
+    if cutoff_frequency <sampling_rate /2 :
+        if type =='Butterworth':
+            nyquist_rate =sampling_rate /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            sos =butter (N =8 ,Wn =cutoff ,btype ='low',analog =False ,output ='sos')
+            zi =sosfilt_zi (sos )*data [0 ]
+            filtered_data ,_ =sosfilt (sos ,data ,zi =zi )
+            return filtered_data 
+        elif type =='Bessel':
+            nyquist_rate =sampling_rate /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            sos =bessel (N =8 ,Wn =cutoff ,btype ='low',analog =False ,output ='sos')
+            zi =sosfilt_zi (sos )*data [0 ]
+            filtered_data ,_ =sosfilt (sos ,data ,zi =zi )
+            return filtered_data 
+        elif type =='Chebyshev I':
+            nyquist_rate =sampling_rate /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            sos =cheby1 (N =8 ,rp =0.1 ,Wn =cutoff ,btype ='low',analog =False ,output ='sos')
+            zi =sosfilt_zi (sos )*data [0 ]
+            filtered_data ,_ =sosfilt (sos ,data ,zi =zi )
+            return filtered_data 
+        elif type =='Chebyshev II':
+            nyquist_rate =sampling_rate /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            sos =cheby2 (N =8 ,rs =40 ,Wn =cutoff ,btype ='low',analog =False ,output ='sos')
+            zi =sosfilt_zi (sos )*data [0 ]
+            filtered_data ,_ =sosfilt (sos ,data ,zi =zi )
+            return filtered_data 
+        elif type =='Elliptic':
+            nyquist_rate =sampling_rate /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            sos =ellip (N =8 ,rp =0.1 ,rs =40 ,Wn =cutoff ,btype ='low',analog =False ,output ='sos')
+            zi =sosfilt_zi (sos )*data [0 ]
+            filtered_data ,_ =sosfilt (sos ,data ,zi =zi )
+            return filtered_data 
+        elif type =='FIR':
+            nyquist_rate =sampling_rate /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            taps =firwin (101 ,cutoff )
+            filtered_data =lfilter (taps ,1 ,data )
+            return filtered_data 
+        elif type =='IIR':
+            nyquist_rate =sampling_rate /2.0 
+            cutoff =cutoff_frequency /nyquist_rate 
+            b ,a =butter (N =8 ,Wn =cutoff ,btype ='low',analog =False )
+            filtered_data =lfilter (b ,a ,data )
+            return filtered_data 
+        elif type =='Wavelet':
+            wavelet_type ='db4'
+            wavelet_level =None 
+            wavelet_threshold_sub_type ='sqtwolog'
+            wavelet_threshold_type ='soft'
+            w =pywt .Wavelet (wavelet_type )
+            max_level =pywt .dwt_max_level (len (data ),filter_len =w .dec_len )
+            if wavelet_level is None :
+                wavelet_level =max_level 
+            wcoeff =pywt .wavedec (data ,w ,mode ='sym',level =wavelet_level )
+            thresh =np .std (wcoeff [-1 ])*_thselect (wcoeff ,wavelet_threshold_sub_type )
+            wcoeff [1 :]=[pywt .threshold (wc ,thresh ,wavelet_threshold_type )for wc in wcoeff [1 :]]
+            filtered_data =pywt .waverec (wcoeff ,wavelet_type ,mode ='sym')
+            return filtered_data 
+        elif type =='Kalman':
             '''
             The user isn't given an option for this yet!
 
             process_noise:
             The process noise represents the uncertainty or variability in the system model.
             It quantifies how much the true state of the system can deviate from the predicted state based on the system model.
             In the Kalman filter, the process noise is modeled as a Gaussian distribution with zero mean and a specified covariance matrix.
@@ -564,3611 +564,3599 @@
             initial_covariance:
             The initial covariance represents the uncertainty or confidence in the initial state estimate.
             It is a matrix that quantifies the initial variances and covariances of the state variables.
             A higher initial covariance indicates more uncertainty in the initial state estimate, while a lower initial covariance suggests more confidence in the initial estimate.
             The initial covariance matrix is typically denoted as P in the Kalman filter equations.
             In the provided code, the initial covariance is set to an identity matrix multiplied by a small value (1e-3), assuming a relatively low initial uncertainty.
             '''
-            process_noise = 1e-4
-            measurement_noise = 1e-2
-            initial_state = np.zeros(2)
-            initial_covariance = np.eye(2) * 1e-3
-            
-            num_samples = len(data)
-            state_size = len(initial_state)
+            process_noise =1e-4 
+            measurement_noise =1e-2 
+            initial_state =np .zeros (2 )
+            initial_covariance =np .eye (2 )*1e-3 
 
-            state = np.zeros((state_size, num_samples))
-            state[:, 0] = initial_state
-            covariance = initial_covariance
-
-            transition_matrix = np.eye(state_size)
-            observation_matrix = np.ones((1, state_size))
-            process_noise_covariance = np.eye(state_size) * process_noise
-            measurement_noise_covariance = np.ones((1, 1)) * measurement_noise
-
-            for t in range(1, num_samples):
-                predicted_state = transition_matrix @ state[:, t-1]
-                predicted_covariance = transition_matrix @ covariance @ transition_matrix.T + process_noise_covariance
-
-                innovation = data[t] - observation_matrix @ predicted_state
-                innovation_covariance = observation_matrix @ predicted_covariance @ observation_matrix.T + measurement_noise_covariance
-                kalman_gain = predicted_covariance @ observation_matrix.T @ np.linalg.inv(innovation_covariance)
-
-                state[:, t] = predicted_state + kalman_gain @ innovation
-                covariance = (np.eye(state_size) - kalman_gain @ observation_matrix) @ predicted_covariance
-
-            filtered_data = state[0, :]
-            return filtered_data
-        
-    else:
-        msg = QMessageBox()
-        msg.setIcon(QMessageBox.Icon.Critical)
-        msg.setWindowTitle("Error")
-        msg.setText("An error has occurred.")
-        msg.setInformativeText(f"The selected cutoff frequency is more than sampling rate/2.")
-        msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-        msg.exec()
-        return data
-
-def calculate_rolling_stats(data, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate):
-    avg_window_size_samples = int((avg_window_size_in_ms / 1000) * sampling_rate)
-    std_window_size_samples = int((std_window_size_in_ms / 1000) * sampling_rate)
-    
-    rolling_avg = uniform_filter1d(data, size=avg_window_size_samples)
-    rolling_std = np.sqrt(uniform_filter1d(data**2, size=std_window_size_samples) - uniform_filter1d(data, size=std_window_size_samples)**2)
-    
-    return rolling_avg, rolling_std
+            num_samples =len (data )
+            state_size =len (initial_state )
 
+            state =np .zeros ((state_size ,num_samples ))
+            state [:,0 ]=initial_state 
+            covariance =initial_covariance 
 
-def find_preliminary_events(data, threshold_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, dips,smoothing, smoothing_index, sampling_rate):
-    rolling_avg, rolling_std = calculate_rolling_stats(data, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate)
-    
-    if threshold_method == "multiplier":
-        if dips == "Yes":
-            threshold = rolling_avg - (threshold_multiplier * rolling_std)
-        else:
-            threshold = rolling_avg + (threshold_multiplier * rolling_std)
-    elif threshold_method == "difference":
-        if dips == "Yes":
-            threshold = rolling_avg - (threshold_difference / 1000)
-        else:
-            threshold = rolling_avg + (threshold_difference / 1000)
-    else:
-        raise ValueError("Unsupported threshold_method. Use 'multiplier' or 'difference'.")
-    if smoothing == "Yes":
-        threshold = smooth_threshold(threshold,int((std_window_size_in_ms / 1000) * sampling_rate),smoothing_index)
-    
-    events = []
-    in_event = False
-    for i in range(1, len(data)):
-        if not in_event and data[i] < threshold[i] and data[i-1] >= threshold[i-1]:
-            in_event = True
-            event_start = i
-        elif in_event and data[i] >= threshold[i] and data[i-1] < threshold[i-1]:
-            event_end = i  # Mark the event end at the first crossing
-            events.append((event_start, event_end))
-            in_event = False
-    return events
-
-
-def exclude_events_and_recalculate_stats(data, events, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate):
-    data_without_events = np.copy(data)
-    for start, end in events:
-        data_without_events[start:end] = np.nan  # Exclude event data by setting it to NaN
-
-    # Replace NaNs with the mean of their neighboring values for a smooth transition
-    nan_indices = np.where(np.isnan(data_without_events))[0]
-    for idx in nan_indices:
-        if idx > 0 and idx < len(data_without_events) - 1:
-            data_without_events[idx] = np.nanmean(data_without_events[idx - 1:idx + 2])
-
-    rolling_avg, rolling_std = calculate_rolling_stats(data, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate)
-    return rolling_avg, rolling_std
-
-
-def find_events_refined(data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, dips, smoothing, smoothing_index, sampling_rate):
-    # Step 1: Find preliminary events
-    preliminary_events = find_preliminary_events(data, threshold_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, dips, smoothing, smoothing_index, sampling_rate)
-
-    # Step 2: Recalculate statistics excluding preliminary events
-    rolling_avg_refined, rolling_std_refined = exclude_events_and_recalculate_stats(data, preliminary_events, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate)
-
-    # Step 3: Use the refined statistics to find events again
-    adjusted_baseline_start = rolling_avg_refined - start_multiplier * rolling_std_refined
-    adjusted_baseline_end = rolling_avg_refined - end_multiplier * rolling_std_refined
-
-    if threshold_method == "multiplier":
-        if dips == "Yes":
-            threshold_refined = rolling_avg_refined - (threshold_multiplier * rolling_std_refined)
-        else:
-            threshold_refined = rolling_avg_refined + (threshold_multiplier * rolling_std_refined)
-    elif threshold_method == "difference":
-        if dips == "Yes":
-            threshold_refined = rolling_avg_refined - (threshold_difference / 1000)   
-        else:
-            threshold_refined = rolling_avg_refined + (threshold_difference / 1000)   
-    if smoothing ==  "Yes":
-        threshold_refined = smooth_threshold(threshold_refined,int((std_window_size_in_ms / 1000) * sampling_rate),smoothing_index)
-
-    all_refined_events = []
-    in_event = False
-    for i in range(1, len(data)):
-        if not in_event and data[i] < threshold_refined[i] and data[i-1] >= threshold_refined[i-1]:
-            in_event = True
-            event_start = i
-            # Backtrack to refine event start
-            while event_start > 0 and not (data[event_start] < adjusted_baseline_start[event_start] and data[event_start-1] >= adjusted_baseline_start[event_start-1]):
-                event_start -= 1
-        elif in_event and data[i] >= adjusted_baseline_end[i] and data[i-1] < adjusted_baseline_end[i-1]:
-            event_end = i  # Mark the event end at the first crossing
-            all_refined_events.append((event_start, event_end))
-            in_event = False
-
-    # Step 4: Filter events based on their width (duration)
-    filtered_events = []
-    for start, end in all_refined_events:
-        event_width_in_seconds = (end - start) / sampling_rate
-        if min_event_width <= event_width_in_seconds <= max_event_width:
-            filtered_events.append((start, end))
-    
-    return filtered_events
+            transition_matrix =np .eye (state_size )
+            observation_matrix =np .ones ((1 ,state_size ))
+            process_noise_covariance =np .eye (state_size )*process_noise 
+            measurement_noise_covariance =np .ones ((1 ,1 ))*measurement_noise 
 
+            for t in range (1 ,num_samples ):
+                predicted_state =transition_matrix @state [:,t -1 ]
+                predicted_covariance =transition_matrix @covariance @transition_matrix .T +process_noise_covariance 
 
+                innovation =data [t ]-observation_matrix @predicted_state 
+                innovation_covariance =observation_matrix @predicted_covariance @observation_matrix .T +measurement_noise_covariance 
+                kalman_gain =predicted_covariance @observation_matrix .T @np .linalg .inv (innovation_covariance )
 
-def find_events_refined_parallel(data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, chunk_size,  dips, sampling_rate, smoothing, smoothing_index, n_jobs):
-    # Calculate the number of chunks
-    n_chunks = int(np.ceil(len(data) / chunk_size))
+                state [:,t ]=predicted_state +kalman_gain @innovation 
+                covariance =(np .eye (state_size )-kalman_gain @observation_matrix )@predicted_covariance 
 
-    # Define a helper function to process each chunk
-    def process_chunk(start_index, end_index):
-        chunk_data = data[start_index:end_index]
-        return find_events_refined(chunk_data, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, threshold_method, min_event_width, max_event_width, dips, smoothing, smoothing_index, sampling_rate)
-    
-    # Parallel execution
-    results = Parallel(n_jobs=n_jobs)(
-        delayed(process_chunk)(i * chunk_size, min((i + 1) * chunk_size, len(data)))
-        for i in range(n_chunks)
+            filtered_data =state [0 ,:]
+            return filtered_data 
+
+    else :
+        msg =QMessageBox ()
+        msg .setIcon (QMessageBox .Icon .Critical )
+        msg .setWindowTitle ("Error")
+        msg .setText ("An error has occurred.")
+        msg .setInformativeText (f"The selected cutoff frequency is more than sampling rate/2.")
+        msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+        msg .exec ()
+        return data 
+
+def calculate_rolling_stats (data ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate ):
+    avg_window_size_samples =int ((avg_window_size_in_ms /1000 )*sampling_rate )
+    std_window_size_samples =int ((std_window_size_in_ms /1000 )*sampling_rate )
+
+    rolling_avg =uniform_filter1d (data ,size =avg_window_size_samples )
+    rolling_std =np .sqrt (uniform_filter1d (data **2 ,size =std_window_size_samples )-uniform_filter1d (data ,size =std_window_size_samples )**2 )
+
+    return rolling_avg ,rolling_std 
+
+
+def find_preliminary_events (data ,threshold_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,dips ,smoothing ,smoothing_index ,sampling_rate ):
+    rolling_avg ,rolling_std =calculate_rolling_stats (data ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate )
+
+    if threshold_method =="multiplier":
+        if dips =="Yes":
+            threshold =rolling_avg -(threshold_multiplier *rolling_std )
+        else :
+            threshold =rolling_avg +(threshold_multiplier *rolling_std )
+    elif threshold_method =="difference":
+        if dips =="Yes":
+            threshold =rolling_avg -(threshold_difference /1000 )
+        else :
+            threshold =rolling_avg +(threshold_difference /1000 )
+    else :
+        raise ValueError ("Unsupported threshold_method. Use 'multiplier' or 'difference'.")
+    if smoothing =="Yes":
+        threshold =smooth_threshold (threshold ,int ((std_window_size_in_ms /1000 )*sampling_rate ),smoothing_index )
+
+    events =[]
+    in_event =False 
+    for i in range (1 ,len (data )):
+        if not in_event and data [i ]<threshold [i ]and data [i -1 ]>=threshold [i -1 ]:
+            in_event =True 
+            event_start =i 
+        elif in_event and data [i ]>=threshold [i ]and data [i -1 ]<threshold [i -1 ]:
+            event_end =i 
+            events .append ((event_start ,event_end ))
+            in_event =False 
+    return events 
+
+
+def exclude_events_and_recalculate_stats (data ,events ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate ):
+    data_without_events =np .copy (data )
+    for start ,end in events :
+        data_without_events [start :end ]=np .nan 
+
+
+    nan_indices =np .where (np .isnan (data_without_events ))[0 ]
+    for idx in nan_indices :
+        if idx >0 and idx <len (data_without_events )-1 :
+            data_without_events [idx ]=np .nanmean (data_without_events [idx -1 :idx +2 ])
+
+    rolling_avg ,rolling_std =calculate_rolling_stats (data ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate )
+    return rolling_avg ,rolling_std 
+
+
+def find_events_refined (data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,dips ,smoothing ,smoothing_index ,sampling_rate ):
+
+    preliminary_events =find_preliminary_events (data ,threshold_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,dips ,smoothing ,smoothing_index ,sampling_rate )
+
+
+    rolling_avg_refined ,rolling_std_refined =exclude_events_and_recalculate_stats (data ,preliminary_events ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate )
+
+
+    adjusted_baseline_start =rolling_avg_refined -start_multiplier *rolling_std_refined 
+    adjusted_baseline_end =rolling_avg_refined -end_multiplier *rolling_std_refined 
+
+    if threshold_method =="multiplier":
+        if dips =="Yes":
+            threshold_refined =rolling_avg_refined -(threshold_multiplier *rolling_std_refined )
+        else :
+            threshold_refined =rolling_avg_refined +(threshold_multiplier *rolling_std_refined )
+    elif threshold_method =="difference":
+        if dips =="Yes":
+            threshold_refined =rolling_avg_refined -(threshold_difference /1000 )
+        else :
+            threshold_refined =rolling_avg_refined +(threshold_difference /1000 )
+    if smoothing =="Yes":
+        threshold_refined =smooth_threshold (threshold_refined ,int ((std_window_size_in_ms /1000 )*sampling_rate ),smoothing_index )
+
+    all_refined_events =[]
+    in_event =False 
+    for i in range (1 ,len (data )):
+        if not in_event and data [i ]<threshold_refined [i ]and data [i -1 ]>=threshold_refined [i -1 ]:
+            in_event =True 
+            event_start =i 
+
+            while event_start >0 and not (data [event_start ]<adjusted_baseline_start [event_start ]and data [event_start -1 ]>=adjusted_baseline_start [event_start -1 ]):
+                event_start -=1 
+        elif in_event and data [i ]>=adjusted_baseline_end [i ]and data [i -1 ]<adjusted_baseline_end [i -1 ]:
+            event_end =i 
+            all_refined_events .append ((event_start ,event_end ))
+            in_event =False 
+
+
+    filtered_events =[]
+    for start ,end in all_refined_events :
+        event_width_in_seconds =(end -start )/sampling_rate 
+        if min_event_width <=event_width_in_seconds <=max_event_width :
+            filtered_events .append ((start ,end ))
+
+    return filtered_events 
+
+
+
+def find_events_refined_parallel (data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,chunk_size ,dips ,sampling_rate ,smoothing ,smoothing_index ,n_jobs ):
+
+    n_chunks =int (np .ceil (len (data )/chunk_size ))
+
+
+    def process_chunk (start_index ,end_index ):
+        chunk_data =data [start_index :end_index ]
+        return find_events_refined (chunk_data ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,threshold_method ,min_event_width ,max_event_width ,dips ,smoothing ,smoothing_index ,sampling_rate )
+
+
+    results =Parallel (n_jobs =n_jobs )(
+    delayed (process_chunk )(i *chunk_size ,min ((i +1 )*chunk_size ,len (data )))
+    for i in range (n_chunks )
     )
-    
-    # Combine results from all chunks
-    combined_results = [event for chunk in results for event in chunk]
 
-    # Adjust event indices based on their chunk offsets and filter out those crossing chunk boundaries
-    adjusted_results = []
-    for chunk_index, chunk in enumerate(results):
-        chunk_start_index = chunk_index * chunk_size
-        for start, end in chunk:
-            if start + chunk_start_index < (chunk_index + 1) * chunk_size and end + chunk_start_index <= min((chunk_index + 1) * chunk_size, len(data)):
-                adjusted_results.append((start + chunk_start_index, end + chunk_start_index))
-    
-    rolling_avg_refined, rolling_std_refined = calculate_rolling_stats(data, avg_window_size_in_ms, std_window_size_in_ms, sampling_rate)
-    
-    if threshold_method == "multiplier":
-        if dips == "Yes":
-            threshold_refined = rolling_avg_refined - (threshold_multiplier * rolling_std_refined)
-        else:
-            threshold_refined = rolling_avg_refined + (threshold_multiplier * rolling_std_refined)
-    elif threshold_method == "difference":
-        if dips == "Yes":
-            threshold_refined = rolling_avg_refined - (threshold_difference / 1000)   
-        else:
-            threshold_refined = rolling_avg_refined + (threshold_difference / 1000)  
-    if smoothing == "Yes":
-        threshold_refined = smooth_threshold(threshold_refined,int((std_window_size_in_ms / 1000) * sampling_rate),smoothing_index)      
-
-    return adjusted_results, rolling_avg_refined, threshold_refined
 
+    combined_results =[event for chunk in results for event in chunk ]
 
 
-def calculate_delta_I1(l, sigma, V, i0, i01, delta_I):
-    d = (i0 + np.sqrt(i0 * (i0 + (16 * l * V * sigma) / math.pi))) / (2 * V * sigma)
-    d1 = (i01 + np.sqrt(i01 * (i01 + (16 * l * V * sigma) / math.pi))) / (2 * V * sigma)
-    delta_G = delta_I / V
-    
-    term1 = (d1**2 * math.pi * sigma) / (4 * l + d1 * math.pi)
-    
-    sqrt_term = (4 * l * delta_G + d * math.pi * (delta_G - d * sigma))**3 * (-64 * l**2 * sigma + 4 * l * math.pi * (delta_G - 4 * d * sigma) + d * math.pi**2 * (delta_G - d * sigma))
-    sqrt_term = np.where(sqrt_term >= 0, sqrt_term, np.nan)
-    
-    term2_numerator = (
-        -d**2 * math.pi**3 * delta_G**2 +
-        128 * l**3 * delta_G * sigma +
-        2 * d**3 * math.pi**3 * delta_G * sigma +
-        d**4 * math.pi**3 * sigma**2 -
-        2 * d**2 * d1**2 * math.pi**3 * sigma**2 -
-        16 * l**2 * math.pi * (delta_G**2 - 4 * d * delta_G * sigma + 2 * d1**2 * sigma**2) +
-        8 * d * l * math.pi**2 * (-delta_G**2 + 2 * d * delta_G * sigma + (d**2 - 2 * d1**2) * sigma**2) -
-        np.sqrt(math.pi) * np.sqrt(sqrt_term)
+    adjusted_results =[]
+    for chunk_index ,chunk in enumerate (results ):
+        chunk_start_index =chunk_index *chunk_size 
+        for start ,end in chunk :
+            if start +chunk_start_index <(chunk_index +1 )*chunk_size and end +chunk_start_index <=min ((chunk_index +1 )*chunk_size ,len (data )):
+                adjusted_results .append ((start +chunk_start_index ,end +chunk_start_index ))
+
+    rolling_avg_refined ,rolling_std_refined =calculate_rolling_stats (data ,avg_window_size_in_ms ,std_window_size_in_ms ,sampling_rate )
+
+    if threshold_method =="multiplier":
+        if dips =="Yes":
+            threshold_refined =rolling_avg_refined -(threshold_multiplier *rolling_std_refined )
+        else :
+            threshold_refined =rolling_avg_refined +(threshold_multiplier *rolling_std_refined )
+    elif threshold_method =="difference":
+        if dips =="Yes":
+            threshold_refined =rolling_avg_refined -(threshold_difference /1000 )
+        else :
+            threshold_refined =rolling_avg_refined +(threshold_difference /1000 )
+    if smoothing =="Yes":
+        threshold_refined =smooth_threshold (threshold_refined ,int ((std_window_size_in_ms /1000 )*sampling_rate ),smoothing_index )
+
+    return adjusted_results ,rolling_avg_refined ,threshold_refined 
+
+
+
+def calculate_delta_I1 (l ,sigma ,V ,i0 ,i01 ,delta_I ):
+    d =(i0 +np .sqrt (i0 *(i0 +(16 *l *V *sigma )/math .pi )))/(2 *V *sigma )
+    d1 =(i01 +np .sqrt (i01 *(i01 +(16 *l *V *sigma )/math .pi )))/(2 *V *sigma )
+    delta_G =delta_I /V 
+
+    term1 =(d1 **2 *math .pi *sigma )/(4 *l +d1 *math .pi )
+
+    sqrt_term =(4 *l *delta_G +d *math .pi *(delta_G -d *sigma ))**3 *(-64 *l **2 *sigma +4 *l *math .pi *(delta_G -4 *d *sigma )+d *math .pi **2 *(delta_G -d *sigma ))
+    sqrt_term =np .where (sqrt_term >=0 ,sqrt_term ,np .nan )
+
+    term2_numerator =(
+    -d **2 *math .pi **3 *delta_G **2 +
+    128 *l **3 *delta_G *sigma +
+    2 *d **3 *math .pi **3 *delta_G *sigma +
+    d **4 *math .pi **3 *sigma **2 -
+    2 *d **2 *d1 **2 *math .pi **3 *sigma **2 -
+    16 *l **2 *math .pi *(delta_G **2 -4 *d *delta_G *sigma +2 *d1 **2 *sigma **2 )+
+    8 *d *l *math .pi **2 *(-delta_G **2 +2 *d *delta_G *sigma +(d **2 -2 *d1 **2 )*sigma **2 )-
+    np .sqrt (math .pi )*np .sqrt (sqrt_term )
+    )
+
+    term2_denominator =(
+    (4 *l +d *math .pi )**2 *sigma *(
+    8 *l +np .sqrt (2 *math .pi )*np .sqrt (
+    1 /((4 *l +d *math .pi )**2 *sigma **2 )*(
+    d **2 *math .pi **3 *delta_G **2 -
+    128 *l **3 *delta_G *sigma -
+    2 *d **3 *math .pi **3 *delta_G *sigma -
+    d **4 *math .pi **3 *sigma **2 +
+    2 *d **2 *d1 **2 *math .pi **3 *sigma **2 +
+    16 *l **2 *math .pi *(delta_G **2 -4 *d *delta_G *sigma +2 *d1 **2 *sigma **2 )-
+    8 *d *l *math .pi **2 *(-delta_G **2 +2 *d *delta_G *sigma +(d **2 -2 *d1 **2 )*sigma **2 )+
+    np .sqrt (math .pi )*np .sqrt (sqrt_term )
+    )
+    )
     )
-    
-    term2_denominator = (
-        (4 * l + d * math.pi)**2 * sigma * (
-            8 * l + np.sqrt(2 * math.pi) * np.sqrt(
-                1 / ((4 * l + d * math.pi)**2 * sigma**2) * (
-                    d**2 * math.pi**3 * delta_G**2 -
-                    128 * l**3 * delta_G * sigma -
-                    2 * d**3 * math.pi**3 * delta_G * sigma -
-                    d**4 * math.pi**3 * sigma**2 +
-                    2 * d**2 * d1**2 * math.pi**3 * sigma**2 +
-                    16 * l**2 * math.pi * (delta_G**2 - 4 * d * delta_G * sigma + 2 * d1**2 * sigma**2) -
-                    8 * d * l * math.pi**2 * (-delta_G**2 + 2 * d * delta_G * sigma + (d**2 - 2 * d1**2) * sigma**2) +
-                    np.sqrt(math.pi) * np.sqrt(sqrt_term)
-                )
-            )
-        )
     )
-    
-    term2 = term2_numerator / term2_denominator
-    
-    delta_I1 = V * (term1 + term2)
-    
-    return np.where(np.isnan(delta_I1), np.nan, delta_I1)
 
+    term2 =term2_numerator /term2_denominator 
 
+    delta_I1 =V *(term1 +term2 )
 
-def normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean):
-    normalized_signal = calculate_delta_I1(
-        standard_length_nm * 10**(-9),
-        standard_conductivity_S_m,
-        standard_voltage_applied_mV / 1000,
-        standard_open_pore_current_nA* 10**(-9),
-        event_baseline_mean* 10**(-9),
-        signal* 10**(-9)
+    return np .where (np .isnan (delta_I1 ),np .nan ,delta_I1 )
+
+
+
+def normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean ):
+    normalized_signal =calculate_delta_I1 (
+    standard_length_nm *10 **(-9 ),
+    standard_conductivity_S_m ,
+    standard_voltage_applied_mV /1000 ,
+    standard_open_pore_current_nA *10 **(-9 ),
+    event_baseline_mean *10 **(-9 ),
+    signal *10 **(-9 )
     )
-    return normalized_signal/10**(-9)
+    return normalized_signal /10 **(-9 )
 
 
-def analyze_event_for_CUSUM(event_signal, baseline, ML_standardisation_settings):
-    standard, ML_enabled, ML_standard,  standard_power, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, sampling_rate =  ML_standardisation_settings['standard'],  ML_standardisation_settings['ML_enabled'],  ML_standardisation_settings['ML_standard'],  ML_standardisation_settings['standard_power'], ML_standardisation_settings['standard_length_nm'], ML_standardisation_settings['standard_conductivity_S_m'], ML_standardisation_settings['standard_voltage_applied_mV'], ML_standardisation_settings['standard_open_pore_current_nA'], ML_standardisation_settings['sampling_rate']
+def analyze_event_for_CUSUM (event_signal ,baseline ,ML_standardisation_settings ):
+    standard ,ML_enabled ,ML_standard ,standard_power ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,sampling_rate =ML_standardisation_settings ['standard'],ML_standardisation_settings ['ML_enabled'],ML_standardisation_settings ['ML_standard'],ML_standardisation_settings ['standard_power'],ML_standardisation_settings ['standard_length_nm'],ML_standardisation_settings ['standard_conductivity_S_m'],ML_standardisation_settings ['standard_voltage_applied_mV'],ML_standardisation_settings ['standard_open_pore_current_nA'],ML_standardisation_settings ['sampling_rate']
 
-    if ML_enabled == "False":
-        signal = np.abs(event_signal-baseline)    # Flip the event signal if necessary
-        event_baseline_mean = np.mean(baseline)
-        if standard == "Normal":
-            signal = signal
-        elif standard == "ΔI/I₀":
-            signal = signal/event_baseline_mean
-        elif standard == "(ΔI*I₀)⁰·⁵":
-            signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-        elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-            signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-        elif standard == "Dutt Standardisation":
-            signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-        else:
-            signal = signal 
-
-        sample_period = 1 / sampling_rate
-        width = len(signal) * sample_period
-        area = np.sum(signal) * sample_period
-        peaks, _ = sig.find_peaks(signal)
-        if len(peaks) == 0:
-            return [np.nan, np.nan, np.nan, area, width, np.nan, np.nan, np.nan]
-        highest_peak = max(peaks, key=lambda peak: signal[peak])
-        height = signal[highest_peak]
-        fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-        fwhm = fwhm_[0] * sample_period
-        heightatfwhm = heightatfwhm_[0]
-        skew = stats.skew(signal)
-        kurt = stats.kurtosis(signal)
-        return [height, fwhm, heightatfwhm, area, width, skew, kurt, event_baseline_mean]
-        
-    else:
-        if ML_standard == "Scheme 1":
-            signal = np.abs(event_signal-baseline)    # Flip the event signal if necessary
-            event_baseline_mean = np.mean(baseline)
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 10  # Number of parts to divide the signal into
-            if n>len(signal):
-                n = len(signal)
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n
-
-            # Calculate the width of each part
-            part_width = width / n
-
-            # Initialize an array to store the average values of each part
-            part_averages = np.zeros(n)
-
-            # Iterate over each part
-            for i in range(n):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            # Create the result array in the desired form
-            return np.append(part_averages, part_width)
-        
-        elif ML_standard == "Scheme 2":
-            signal = np.abs(event_signal-baseline)   # Flip the event signal if necessary
-            event_baseline_mean = np.mean(baseline)
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 10  # Number of parts to divide the signal into
-            if n>len(signal):
-                n = len(signal)
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n
-
-            # Calculate the width of each part
-            part_width = width / n
-
-            # Initialize an array to store the average values of each part
-            part_averages = np.zeros(n)
-
-            # Iterate over each part
-            for i in range(n):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            area = np.sum(signal) * sample_period
-            peaks, _ = sig.find_peaks(signal)
-            if len(peaks) == 0:
-                return np.append(part_averages, [np.nan, np.nan, np.nan, np.nan, area, width])
-            highest_peak = max(peaks, key=lambda peak: signal[peak])
-            height = signal[highest_peak]
-            fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-            fwhm = fwhm_[0] * sample_period
-            heightatfwhm = heightatfwhm_[0]
-            return np.append(part_averages, [part_width, height, fwhm, heightatfwhm, area, width])
-        
-        elif ML_standard == "Scheme 3":
-            signal = np.abs(event_signal-baseline)   # Flip the event signal if necessary
-            event_baseline_mean = np.mean(baseline)
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 10  # Number of parts to divide the signal into
-            if n>len(signal):
-                n = len(signal)
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n
-
-            # Calculate the width of each part
-            part_width = width / n
-
-            # Initialize an array to store the average values of each part
-            part_averages = np.zeros(n)
-
-            # Iterate over each part
-            for i in range(n):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            area = np.sum(signal) * sample_period
-            peaks, _ = sig.find_peaks(signal)
-            if len(peaks) == 0:
-                return np.append(part_averages, [np.nan, np.nan, np.nan, np.nan, area, width, np.nan, np.nan])
-            highest_peak = max(peaks, key=lambda peak: signal[peak])
-            height = signal[highest_peak]
-            fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-            fwhm = fwhm_[0] * sample_period
-            heightatfwhm = heightatfwhm_[0]
-            skew = stats.skew(signal)
-            kurt = stats.kurtosis(signal)
-            return np.append(part_averages, [part_width, height, fwhm, heightatfwhm, area, width, skew, kurt])
-        
-        elif ML_standard == "Scheme 4":
-            signal = np.abs(event_signal-baseline)   # Flip the event signal if necessary
-            event_baseline_mean = np.mean(baseline)
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 50  # Number of parts to divide the signal into
-            if n>len(signal):
-                n = len(signal)
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n
-
-            # Calculate the width of each part
-            part_width = width / n
-
-            # Initialize an array to store the average values of each part
-            part_averages = np.zeros(n)
-
-            # Iterate over each part
-            for i in range(n):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            area = np.sum(signal) * sample_period
-            peaks, _ = sig.find_peaks(signal)
-            if len(peaks) == 0:
-                return np.append(part_averages, [np.nan, np.nan, np.nan, np.nan, area, width, np.nan, np.nan])
-            highest_peak = max(peaks, key=lambda peak: signal[peak])
-            height = signal[highest_peak]
-            fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-            fwhm = fwhm_[0] * sample_period
-            heightatfwhm = heightatfwhm_[0]
-            skew = stats.skew(signal)
-            kurt = stats.kurtosis(signal)
-            return np.append(part_averages, [part_width, height, fwhm, heightatfwhm, area, width, skew, kurt])
-        
-        elif ML_standard == "Scheme 5":
-            signal = np.abs(event_signal-baseline)    # Flip the event signal if necessary
-            event_baseline_mean = np.mean(baseline)
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-        width = len(signal) * sample_period
-        area = np.sum(signal) * sample_period
-        peaks, _ = sig.find_peaks(signal)
-        if len(peaks) == 0:
-            return np.append(signal,[np.nan, np.nan, np.nan, area, width, np.nan, np.nan])
-        highest_peak = max(peaks, key=lambda peak: signal[peak])
-        height = signal[highest_peak]
-        fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-        fwhm = fwhm_[0] * sample_period
-        heightatfwhm = heightatfwhm_[0]
-        skew = stats.skew(signal)
-        kurt = stats.kurtosis(signal)
-        return np.append(signal, [height, fwhm, heightatfwhm, area, width, skew, kurt])
-    
-    # if standard == "Normal":
-    #     signal = np.abs(event_signal-baseline)  
+    if ML_enabled =="False":
+        signal =np .abs (event_signal -baseline )
+        event_baseline_mean =np .mean (baseline )
+        if standard =="Normal":
+            signal =signal 
+        elif standard =="ΔI/I₀":
+            signal =signal /event_baseline_mean 
+        elif standard =="(ΔI*I₀)⁰·⁵":
+            signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+        elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+            signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+        elif standard =="Dutt Standardisation":
+            signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+        else :
+            signal =signal 
 
-    #     sample_period = 1 / sampling_rate
-    #     width = len(signal) * sample_period
-    #     area = np.sum(signal) * sample_period
-        
-    #     peaks, _ = sig.find_peaks(signal)
-    #     if len(peaks) == 0:
-    #         return [np.nan, np.nan,np.nan,  area, width, np.nan,  np.nan]
-        
-    #     highest_peak = max(peaks, key=lambda peak: signal[peak])
-    #     height = signal[highest_peak]
-    #     fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-    #     fwhm = fwhm_[0] * sample_period
-    #     heightatfwhm = heightatfwhm_[0]
-        
-    #     skew = stats.skew(signal)
-    #     kurt = stats.kurtosis(signal)
-    #     return [height, fwhm, heightatfwhm, area, width, skew, kurt, np.mean(baseline)]
-
-def analyze_event(event_signal, data, rolling_avg_refined, sampling_rate, ML_standardisation_settings):
-    standard, ML_enabled, ML_standard,  standard_power, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA =  ML_standardisation_settings['standard'],  ML_standardisation_settings['ML_enabled'],  ML_standardisation_settings['ML_standard'],  ML_standardisation_settings['standard_power'], ML_standardisation_settings['standard_length_nm'], ML_standardisation_settings['standard_conductivity_S_m'], ML_standardisation_settings['standard_voltage_applied_mV'], ML_standardisation_settings['standard_open_pore_current_nA']
-
-    if ML_enabled == "False":
-        event_data = data[event_signal[0]:event_signal[1]]
-        event_baseline = rolling_avg_refined[event_signal[0]:event_signal[1]]
-        event_baseline_mean = np.mean(event_baseline)
-        #print(event_baseline_mean)
-        signal = np.abs(event_data - event_baseline)  # Flip the event signal if necessary
-        if standard == "Normal":
-            signal = signal
-        elif standard == "ΔI/I₀":
-            signal = signal/event_baseline_mean
-        elif standard == "(ΔI*I₀)⁰·⁵":
-            signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-        elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-            signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-        elif standard == "Dutt Standardisation":
-            signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-        else:
-            signal = signal 
-
-        sample_period = 1 / sampling_rate
-        width = len(signal) * sample_period
-        area = np.sum(signal) * sample_period
-        peaks, _ = sig.find_peaks(signal)
-        if len(peaks) == 0:
-            return [np.nan, np.nan, np.nan, area, width, np.nan, np.nan, np.nan, np.nan]
-        highest_peak = max(peaks, key=lambda peak: signal[peak])
-        height = signal[highest_peak]
-        fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-        fwhm = fwhm_[0] * sample_period
-        heightatfwhm = heightatfwhm_[0]
-        skew = stats.skew(signal)
-        kurt = stats.kurtosis(signal)
-        # Calculate the actual time of the event occurrence
-        event_time = event_signal[0] / sampling_rate
-        #if standard == "Dutt Standardisation":
-        #    height = normalize_signal(height, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-        #    heightatfwhm = normalize_signal(heightatfwhm, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-        return [height, fwhm, heightatfwhm, area, width, skew, kurt, event_baseline_mean, event_time]
-        
-    else:
-        if ML_standard == "Scheme 1":
-            event_data = data[event_signal[0]:event_signal[1]]
-            event_baseline = rolling_avg_refined[event_signal[0]:event_signal[1]]
-            event_baseline_mean = np.mean(event_baseline)
-            signal = np.abs(event_data - event_baseline)  # Flip the event signal if necessary
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 10  # Number of parts to divide the signal into
-            part_averages = np.full(n, np.nan)  
-
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n if n > 0 else 0
-
-            # Calculate the number of parts that can be used based on the signal length
-            num_parts = min(n, len(signal) // samples_per_part) if samples_per_part > 0 else 0
-
-            # Calculate the width of each part based on the actual number of parts used
-            part_width = width / num_parts if num_parts > 0 else width
-
-            # Iterate over each part
-            for i in range(num_parts):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            # Create the result array in the desired form
-            return np.append(part_averages, part_width)
-        
-        elif ML_standard == "Scheme 2":
-            event_data = data[event_signal[0]:event_signal[1]]
-            event_baseline = rolling_avg_refined[event_signal[0]:event_signal[1]]
-            event_baseline_mean = np.mean(event_baseline)
-            signal = np.abs(event_data - event_baseline)  # Flip the event signal if necessary
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 10  # Number of parts to divide the signal into
-            part_averages = np.full(n, np.nan)  
-
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n if n > 0 else 0
-
-            # Calculate the number of parts that can be used based on the signal length
-            num_parts = min(n, len(signal) // samples_per_part) if samples_per_part > 0 else 0
-
-            # Calculate the width of each part based on the actual number of parts used
-            part_width = width / num_parts if num_parts > 0 else width
-
-            # Iterate over each part
-            for i in range(num_parts):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            area = np.sum(signal) * sample_period
-            peaks, _ = sig.find_peaks(signal)
-            if len(peaks) == 0:
-                return np.full(16, np.nan)
-            highest_peak = max(peaks, key=lambda peak: signal[peak])
-            height = signal[highest_peak]
-            fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-            fwhm = fwhm_[0] * sample_period
-            heightatfwhm = heightatfwhm_[0]
-            return np.append(part_averages, [part_width, height, fwhm, heightatfwhm, area, width])
-        
-        elif ML_standard == "Scheme 3":
-            event_data = data[event_signal[0]:event_signal[1]]
-            event_baseline = rolling_avg_refined[event_signal[0]:event_signal[1]]
-            event_baseline_mean = np.mean(event_baseline)
-            signal = np.abs(event_data - event_baseline)  # Flip the event signal if necessary
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 10  # Number of parts to divide the signal into
-            part_averages = np.full(n, np.nan)  
-
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n if n > 0 else 0
-
-            # Calculate the number of parts that can be used based on the signal length
-            num_parts = min(n, len(signal) // samples_per_part) if samples_per_part > 0 else 0
-
-            # Calculate the width of each part based on the actual number of parts used
-            part_width = width / num_parts if num_parts > 0 else width
-
-            # Iterate over each part
-            for i in range(num_parts):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            area = np.sum(signal) * sample_period
-            peaks, _ = sig.find_peaks(signal)
-            if len(peaks) == 0:
-                return np.full(18, np.nan)
-            highest_peak = max(peaks, key=lambda peak: signal[peak])
-            height = signal[highest_peak]
-            fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-            fwhm = fwhm_[0] * sample_period
-            heightatfwhm = heightatfwhm_[0]
-            skew = stats.skew(signal)
-            kurt = stats.kurtosis(signal)
-            return np.append(part_averages, [part_width, height, fwhm, heightatfwhm, area, width, skew, kurt])
-        
-        elif ML_standard == "Scheme 4":
-            event_data = data[event_signal[0]:event_signal[1]]
-            event_baseline = rolling_avg_refined[event_signal[0]:event_signal[1]]
-            event_baseline_mean = np.mean(event_baseline)
-            signal = np.abs(event_data - event_baseline)  # Flip the event signal if necessary
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-            sample_period = 1 / sampling_rate
-            width = len(signal) * sample_period
-            n = 0  # Number of parts to divide the signal into
-            part_averages = np.full(n, np.nan)  
-
-            # Calculate the number of samples in each part
-            samples_per_part = len(signal) // n if n > 0 else 0
-
-            # Calculate the number of parts that can be used based on the signal length
-            num_parts = min(n, len(signal) // samples_per_part) if samples_per_part > 0 else 0
-
-            # Calculate the width of each part based on the actual number of parts used
-            part_width = width / num_parts if num_parts > 0 else width
-
-            # Iterate over each part
-            for i in range(num_parts):
-                start_index = i * samples_per_part
-                end_index = (i + 1) * samples_per_part
-                # Extract the samples for the current part
-                part_samples = signal[start_index:end_index]
-                # Calculate the average value of the current part
-                part_averages[i] = np.mean(part_samples)
-
-            area = np.sum(signal) * sample_period
-            peaks, _ = sig.find_peaks(signal)
-            if len(peaks) == 0:
-                return np.full(58, np.nan)
-            highest_peak = max(peaks, key=lambda peak: signal[peak])
-            height = signal[highest_peak]
-            fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-            fwhm = fwhm_[0] * sample_period
-            heightatfwhm = heightatfwhm_[0]
-            skew = stats.skew(signal)
-            kurt = stats.kurtosis(signal)
-            return np.append(part_averages, [part_width, height, fwhm, heightatfwhm, area, width, skew, kurt])
-        
-        elif ML_standard == "Scheme 5":
-            event_data = data[event_signal[0]:event_signal[1]]
-            event_baseline = rolling_avg_refined[event_signal[0]:event_signal[1]]
-            event_baseline_mean = np.mean(event_baseline)
-            signal = np.abs(event_data - event_baseline)  # Flip the event signal if necessary
-            if standard == "Normal":
-                signal = signal
-            elif standard == "ΔI/I₀":
-                signal = signal/event_baseline_mean
-            elif standard == "(ΔI*I₀)⁰·⁵":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**0.5
-            elif standard == "(ΔI*I₀)ᵖᵒʷᵉʳ":
-                signal = (np.abs(signal)*np.abs(event_baseline_mean))**standard_power
-            elif standard == "Dutt Standardisation":
-                signal = normalize_signal(signal, standard_length_nm, standard_conductivity_S_m, standard_voltage_applied_mV, standard_open_pore_current_nA, event_baseline_mean)
-            else:
-                signal = signal 
-            
-                sample_period = 1 / sampling_rate
-                width = len(signal) * sample_period
-                area = np.sum(signal) * sample_period
-                peaks, _ = sig.find_peaks(signal)
-
-                max_points = int(sampling_rate / 1000) + 8
-                result = np.full(max_points, np.nan)
-
-                if len(peaks) == 0:
-                    result[-8:] = [np.nan, np.nan, np.nan, area, width, np.nan, np.nan, event_baseline_mean]
-                    return result
-
-                highest_peak = max(peaks, key=lambda peak: signal[peak])
-                height = signal[highest_peak]
-                fwhm_, heightatfwhm_, _, _ = sig.peak_widths(signal, [highest_peak], rel_height=0.5)
-                fwhm = fwhm_[0] * sample_period
-                heightatfwhm = heightatfwhm_[0]
-                skew = stats.skew(signal)
-                kurt = stats.kurtosis(signal)
-
-                signal_length = min(len(signal), max_points - 8)
-                result[:signal_length] = signal[:signal_length]
-                result[-8:] = [height, fwhm, heightatfwhm, area, width, skew, kurt, event_baseline_mean]
-
-                return result
-
-def analyze_events_chunk(chunk, data, rolling_avg_refined, sampling_rate, ML_standardisation_settings):
-    return [analyze_event(event_signal, data, rolling_avg_refined, sampling_rate, ML_standardisation_settings) for event_signal in chunk]
-
-def save_chunked_event_analysis_to_npz(chunk_size, data, events, rolling_avg_refined, sampling_rate, ML_standardisation_settings):
-    event_chunks = np.array_split(events, max(1, len(events) // chunk_size))
-    analysis_results = Parallel(n_jobs=-1)(
-        delayed(analyze_events_chunk)(chunk, data, rolling_avg_refined, sampling_rate,ML_standardisation_settings) for chunk in event_chunks
+        sample_period =1 /sampling_rate 
+        width =len (signal )*sample_period 
+        area =np .sum (signal )*sample_period 
+        peaks ,_ =sig .find_peaks (signal )
+        if len (peaks )==0 :
+            return [np .nan ,np .nan ,np .nan ,area ,width ,np .nan ,np .nan ,np .nan ]
+        highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+        height =signal [highest_peak ]
+        fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+        fwhm =fwhm_ [0 ]*sample_period 
+        heightatfwhm =heightatfwhm_ [0 ]
+        skew =stats .skew (signal )
+        kurt =stats .kurtosis (signal )
+        return [height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ,event_baseline_mean ]
+
+    else :
+        if ML_standard =="Scheme 1":
+            signal =np .abs (event_signal -baseline )
+            event_baseline_mean =np .mean (baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =10 
+            if n >len (signal ):
+                n =len (signal )
+
+            samples_per_part =len (signal )//n 
+
+
+            part_width =width /n 
+
+
+            part_averages =np .zeros (n )
+
+
+            for i in range (n ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+
+                part_samples =signal [start_index :end_index ]
+
+
+                part_averages [i ]=np .mean (part_samples )
+
+
+            return np .append (part_averages ,part_width )
+
+        elif ML_standard =="Scheme 2":
+            signal =np .abs (event_signal -baseline )
+            event_baseline_mean =np .mean (baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =10 
+            if n >len (signal ):
+                n =len (signal )
+
+            samples_per_part =len (signal )//n 
+
+
+            part_width =width /n 
+
+
+            part_averages =np .zeros (n )
+
+
+            for i in range (n ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+
+                part_samples =signal [start_index :end_index ]
+
+
+                part_averages [i ]=np .mean (part_samples )
+
+            area =np .sum (signal )*sample_period 
+            peaks ,_ =sig .find_peaks (signal )
+            if len (peaks )==0 :
+                return np .append (part_averages ,[np .nan ,np .nan ,np .nan ,np .nan ,area ,width ])
+            highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+            height =signal [highest_peak ]
+            fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+            fwhm =fwhm_ [0 ]*sample_period 
+            heightatfwhm =heightatfwhm_ [0 ]
+            return np .append (part_averages ,[part_width ,height ,fwhm ,heightatfwhm ,area ,width ])
+
+        elif ML_standard =="Scheme 3":
+            signal =np .abs (event_signal -baseline )
+            event_baseline_mean =np .mean (baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =10 
+            if n >len (signal ):
+                n =len (signal )
+
+            samples_per_part =len (signal )//n 
+
+
+            part_width =width /n 
+
+
+            part_averages =np .zeros (n )
+
+
+            for i in range (n ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+
+                part_samples =signal [start_index :end_index ]
+
+
+                part_averages [i ]=np .mean (part_samples )
+
+            area =np .sum (signal )*sample_period 
+            peaks ,_ =sig .find_peaks (signal )
+            if len (peaks )==0 :
+                return np .append (part_averages ,[np .nan ,np .nan ,np .nan ,np .nan ,area ,width ,np .nan ,np .nan ])
+            highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+            height =signal [highest_peak ]
+            fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+            fwhm =fwhm_ [0 ]*sample_period 
+            heightatfwhm =heightatfwhm_ [0 ]
+            skew =stats .skew (signal )
+            kurt =stats .kurtosis (signal )
+            return np .append (part_averages ,[part_width ,height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ])
+
+        elif ML_standard =="Scheme 4":
+            signal =np .abs (event_signal -baseline )
+            event_baseline_mean =np .mean (baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =50 
+            if n >len (signal ):
+                n =len (signal )
+
+            samples_per_part =len (signal )//n 
+
+
+            part_width =width /n 
+
+
+            part_averages =np .zeros (n )
+
+
+            for i in range (n ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+
+                part_samples =signal [start_index :end_index ]
+
+
+                part_averages [i ]=np .mean (part_samples )
+
+            area =np .sum (signal )*sample_period 
+            peaks ,_ =sig .find_peaks (signal )
+            if len (peaks )==0 :
+                return np .append (part_averages ,[np .nan ,np .nan ,np .nan ,np .nan ,area ,width ,np .nan ,np .nan ])
+            highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+            height =signal [highest_peak ]
+            fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+            fwhm =fwhm_ [0 ]*sample_period 
+            heightatfwhm =heightatfwhm_ [0 ]
+            skew =stats .skew (signal )
+            kurt =stats .kurtosis (signal )
+            return np .append (part_averages ,[part_width ,height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ])
+
+        elif ML_standard =="Scheme 5":
+            signal =np .abs (event_signal -baseline )
+            event_baseline_mean =np .mean (baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+        width =len (signal )*sample_period 
+        area =np .sum (signal )*sample_period 
+        peaks ,_ =sig .find_peaks (signal )
+        if len (peaks )==0 :
+            return np .append (signal ,[np .nan ,np .nan ,np .nan ,area ,width ,np .nan ,np .nan ])
+        highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+        height =signal [highest_peak ]
+        fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+        fwhm =fwhm_ [0 ]*sample_period 
+        heightatfwhm =heightatfwhm_ [0 ]
+        skew =stats .skew (signal )
+        kurt =stats .kurtosis (signal )
+        return np .append (signal ,[height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ])
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+def analyze_event (event_signal ,data ,rolling_avg_refined ,sampling_rate ,ML_standardisation_settings ):
+    standard ,ML_enabled ,ML_standard ,standard_power ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA =ML_standardisation_settings ['standard'],ML_standardisation_settings ['ML_enabled'],ML_standardisation_settings ['ML_standard'],ML_standardisation_settings ['standard_power'],ML_standardisation_settings ['standard_length_nm'],ML_standardisation_settings ['standard_conductivity_S_m'],ML_standardisation_settings ['standard_voltage_applied_mV'],ML_standardisation_settings ['standard_open_pore_current_nA']
+
+    if ML_enabled =="False":
+        event_data =data [event_signal [0 ]:event_signal [1 ]]
+        event_baseline =rolling_avg_refined [event_signal [0 ]:event_signal [1 ]]
+        event_baseline_mean =np .mean (event_baseline )
+
+        signal =np .abs (event_data -event_baseline )
+        if standard =="Normal":
+            signal =signal 
+        elif standard =="ΔI/I₀":
+            signal =signal /event_baseline_mean 
+        elif standard =="(ΔI*I₀)⁰·⁵":
+            signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+        elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+            signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+        elif standard =="Dutt Standardisation":
+            signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+        else :
+            signal =signal 
+
+        sample_period =1 /sampling_rate 
+        width =len (signal )*sample_period 
+        area =np .sum (signal )*sample_period 
+        peaks ,_ =sig .find_peaks (signal )
+        if len (peaks )==0 :
+            return [np .nan ,np .nan ,np .nan ,area ,width ,np .nan ,np .nan ,np .nan ,np .nan ]
+        highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+        height =signal [highest_peak ]
+        fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+        fwhm =fwhm_ [0 ]*sample_period 
+        heightatfwhm =heightatfwhm_ [0 ]
+        skew =stats .skew (signal )
+        kurt =stats .kurtosis (signal )
+
+        event_time =event_signal [0 ]/sampling_rate 
+
+
+
+        return [height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ,event_baseline_mean ,event_time ]
+
+    else :
+        if ML_standard =="Scheme 1":
+            event_data =data [event_signal [0 ]:event_signal [1 ]]
+            event_baseline =rolling_avg_refined [event_signal [0 ]:event_signal [1 ]]
+            event_baseline_mean =np .mean (event_baseline )
+            signal =np .abs (event_data -event_baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =10 
+            part_averages =np .full (n ,np .nan )
+
+
+            samples_per_part =len (signal )//n if n >0 else 0 
+
+
+            num_parts =min (n ,len (signal )//samples_per_part )if samples_per_part >0 else 0 
+
+
+            part_width =width /num_parts if num_parts >0 else width 
+
+
+            for i in range (num_parts ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+                part_samples =signal [start_index :end_index ]
+
+                part_averages [i ]=np .mean (part_samples )
+
+
+            return np .append (part_averages ,part_width )
+
+        elif ML_standard =="Scheme 2":
+            event_data =data [event_signal [0 ]:event_signal [1 ]]
+            event_baseline =rolling_avg_refined [event_signal [0 ]:event_signal [1 ]]
+            event_baseline_mean =np .mean (event_baseline )
+            signal =np .abs (event_data -event_baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =10 
+            part_averages =np .full (n ,np .nan )
+
+
+            samples_per_part =len (signal )//n if n >0 else 0 
+
+
+            num_parts =min (n ,len (signal )//samples_per_part )if samples_per_part >0 else 0 
+
+
+            part_width =width /num_parts if num_parts >0 else width 
+
+
+            for i in range (num_parts ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+                part_samples =signal [start_index :end_index ]
+
+                part_averages [i ]=np .mean (part_samples )
+
+            area =np .sum (signal )*sample_period 
+            peaks ,_ =sig .find_peaks (signal )
+            if len (peaks )==0 :
+                return np .full (16 ,np .nan )
+            highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+            height =signal [highest_peak ]
+            fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+            fwhm =fwhm_ [0 ]*sample_period 
+            heightatfwhm =heightatfwhm_ [0 ]
+            return np .append (part_averages ,[part_width ,height ,fwhm ,heightatfwhm ,area ,width ])
+
+        elif ML_standard =="Scheme 3":
+            event_data =data [event_signal [0 ]:event_signal [1 ]]
+            event_baseline =rolling_avg_refined [event_signal [0 ]:event_signal [1 ]]
+            event_baseline_mean =np .mean (event_baseline )
+            signal =np .abs (event_data -event_baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =10 
+            part_averages =np .full (n ,np .nan )
+
+
+            samples_per_part =len (signal )//n if n >0 else 0 
+
+
+            num_parts =min (n ,len (signal )//samples_per_part )if samples_per_part >0 else 0 
+
+
+            part_width =width /num_parts if num_parts >0 else width 
+
+
+            for i in range (num_parts ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+                part_samples =signal [start_index :end_index ]
+
+                part_averages [i ]=np .mean (part_samples )
+
+            area =np .sum (signal )*sample_period 
+            peaks ,_ =sig .find_peaks (signal )
+            if len (peaks )==0 :
+                return np .full (18 ,np .nan )
+            highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+            height =signal [highest_peak ]
+            fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+            fwhm =fwhm_ [0 ]*sample_period 
+            heightatfwhm =heightatfwhm_ [0 ]
+            skew =stats .skew (signal )
+            kurt =stats .kurtosis (signal )
+            return np .append (part_averages ,[part_width ,height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ])
+
+        elif ML_standard =="Scheme 4":
+            event_data =data [event_signal [0 ]:event_signal [1 ]]
+            event_baseline =rolling_avg_refined [event_signal [0 ]:event_signal [1 ]]
+            event_baseline_mean =np .mean (event_baseline )
+            signal =np .abs (event_data -event_baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+            sample_period =1 /sampling_rate 
+            width =len (signal )*sample_period 
+            n =0 
+            part_averages =np .full (n ,np .nan )
+
+
+            samples_per_part =len (signal )//n if n >0 else 0 
+
+
+            num_parts =min (n ,len (signal )//samples_per_part )if samples_per_part >0 else 0 
+
+
+            part_width =width /num_parts if num_parts >0 else width 
+
+
+            for i in range (num_parts ):
+                start_index =i *samples_per_part 
+                end_index =(i +1 )*samples_per_part 
+
+                part_samples =signal [start_index :end_index ]
+
+                part_averages [i ]=np .mean (part_samples )
+
+            area =np .sum (signal )*sample_period 
+            peaks ,_ =sig .find_peaks (signal )
+            if len (peaks )==0 :
+                return np .full (58 ,np .nan )
+            highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+            height =signal [highest_peak ]
+            fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+            fwhm =fwhm_ [0 ]*sample_period 
+            heightatfwhm =heightatfwhm_ [0 ]
+            skew =stats .skew (signal )
+            kurt =stats .kurtosis (signal )
+            return np .append (part_averages ,[part_width ,height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ])
+
+        elif ML_standard =="Scheme 5":
+            event_data =data [event_signal [0 ]:event_signal [1 ]]
+            event_baseline =rolling_avg_refined [event_signal [0 ]:event_signal [1 ]]
+            event_baseline_mean =np .mean (event_baseline )
+            signal =np .abs (event_data -event_baseline )
+            if standard =="Normal":
+                signal =signal 
+            elif standard =="ΔI/I₀":
+                signal =signal /event_baseline_mean 
+            elif standard =="(ΔI*I₀)⁰·⁵":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**0.5 
+            elif standard =="(ΔI*I₀)ᵖᵒʷᵉʳ":
+                signal =(np .abs (signal )*np .abs (event_baseline_mean ))**standard_power 
+            elif standard =="Dutt Standardisation":
+                signal =normalize_signal (signal ,standard_length_nm ,standard_conductivity_S_m ,standard_voltage_applied_mV ,standard_open_pore_current_nA ,event_baseline_mean )
+            else :
+                signal =signal 
+
+                sample_period =1 /sampling_rate 
+                width =len (signal )*sample_period 
+                area =np .sum (signal )*sample_period 
+                peaks ,_ =sig .find_peaks (signal )
+
+                max_points =int (sampling_rate /1000 )+8 
+                result =np .full (max_points ,np .nan )
+
+                if len (peaks )==0 :
+                    result [-8 :]=[np .nan ,np .nan ,np .nan ,area ,width ,np .nan ,np .nan ,event_baseline_mean ]
+                    return result 
+
+                highest_peak =max (peaks ,key =lambda peak :signal [peak ])
+                height =signal [highest_peak ]
+                fwhm_ ,heightatfwhm_ ,_ ,_ =sig .peak_widths (signal ,[highest_peak ],rel_height =0.5 )
+                fwhm =fwhm_ [0 ]*sample_period 
+                heightatfwhm =heightatfwhm_ [0 ]
+                skew =stats .skew (signal )
+                kurt =stats .kurtosis (signal )
+
+                signal_length =min (len (signal ),max_points -8 )
+                result [:signal_length ]=signal [:signal_length ]
+                result [-8 :]=[height ,fwhm ,heightatfwhm ,area ,width ,skew ,kurt ,event_baseline_mean ]
+
+                return result 
+
+def analyze_events_chunk (chunk ,data ,rolling_avg_refined ,sampling_rate ,ML_standardisation_settings ):
+    return [analyze_event (event_signal ,data ,rolling_avg_refined ,sampling_rate ,ML_standardisation_settings )for event_signal in chunk ]
+
+def save_chunked_event_analysis_to_npz (chunk_size ,data ,events ,rolling_avg_refined ,sampling_rate ,ML_standardisation_settings ):
+    event_chunks =np .array_split (events ,max (1 ,len (events )//chunk_size ))
+    analysis_results =Parallel (n_jobs =-1 )(
+    delayed (analyze_events_chunk )(chunk ,data ,rolling_avg_refined ,sampling_rate ,ML_standardisation_settings )for chunk in event_chunks 
     )
-    # print("Analysis results shapes:")
-    # for i, chunk_result in enumerate(analysis_results):
-    #     print(f"Chunk {i+1}: {[arr.shape for arr in chunk_result]}")
-    flattened_results = np.array([item for sublist in analysis_results for item in sublist], dtype=np.float64)
-    #flattened_results = np.concatenate(analysis_results)
-    return flattened_results
-
-def autostepfinder(data, acceptance_threshold, max_iterations=100):
-    plateaus = [data]
-    change_points = []
-
-    for _ in range(max_iterations):
-        best_split_idx = None
-        best_reduction = 0
-
-        for i, plateau in enumerate(plateaus):
-            split_idx = find_best_split(plateau)
-            if split_idx is not None:
-                left_plateau, right_plateau = split_plateau(plateau, split_idx)
-                reduction = np.sum((plateau - np.mean(plateau)) **2) - (
-                    np.sum((left_plateau - np.mean(left_plateau))** 2) +
-                    np.sum((right_plateau - np.mean(right_plateau)) ** 2)
+
+
+
+    flattened_results =np .array ([item for sublist in analysis_results for item in sublist ],dtype =np .float64 )
+
+    return flattened_results 
+
+def autostepfinder (data ,acceptance_threshold ,max_iterations =100 ):
+    plateaus =[data ]
+    change_points =[]
+
+    for _ in range (max_iterations ):
+        best_split_idx =None 
+        best_reduction =0 
+
+        for i ,plateau in enumerate (plateaus ):
+            split_idx =find_best_split (plateau )
+            if split_idx is not None :
+                left_plateau ,right_plateau =split_plateau (plateau ,split_idx )
+                reduction =np .sum ((plateau -np .mean (plateau ))**2 )-(
+                np .sum ((left_plateau -np .mean (left_plateau ))**2 )+
+                np .sum ((right_plateau -np .mean (right_plateau ))**2 )
                 )
-                if reduction > best_reduction:
-                    best_reduction = reduction
-                    best_split_idx = (i, split_idx)
-
-        if best_split_idx is None:
-            break
-
-        plateau_idx, split_idx = best_split_idx
-        left_plateau, right_plateau = split_plateau(plateaus[plateau_idx], split_idx)
-        plateaus[plateau_idx] = left_plateau
-        plateaus.insert(plateau_idx + 1, right_plateau)
-
-        change_points.append(sum(len(p) for p in plateaus[:plateau_idx]) + split_idx)
-
-        counter_plateaus = counter_fit(plateaus)
-        s_score = calculate_s_score(plateaus, counter_plateaus)
-
-        if s_score < acceptance_threshold:
-            break
-
-    change_points.sort()
-    return change_points
-
-def find_best_split(plateau):
-    best_split_idx = None
-    best_reduction = 0
-
-    for i in range(1, len(plateau) - 1):
-        left_plateau = plateau[:i]
-        right_plateau = plateau[i:]
-        left_mean = np.mean(left_plateau)
-        right_mean = np.mean(right_plateau)
-        reduction = np.sum((left_plateau - left_mean) **2) + np.sum((right_plateau - right_mean)** 2)
-
-        if reduction > best_reduction:
-            best_reduction = reduction
-            best_split_idx = i
-
-    return best_split_idx
-
-def split_plateau(plateau, split_idx):
-    left_plateau = plateau[:split_idx]
-    right_plateau = plateau[split_idx:]
-    return left_plateau, right_plateau
-
-def counter_fit(plateaus):
-    counter_plateaus = []
-    for plateau in plateaus:
-        split_idx = find_best_split(plateau)
-        if split_idx is not None:
-            left_plateau, right_plateau = split_plateau(plateau, split_idx)
-            counter_plateaus.append(left_plateau)
-            counter_plateaus.append(right_plateau)
-        else:
-            counter_plateaus.append(plateau)
-    return counter_plateaus
-
-def calculate_s_score(plateaus, counter_plateaus):
-    plateaus_var = sum(np.var(plateau) for plateau in plateaus)
-    counter_plateaus_var = sum(np.var(plateau) for plateau in counter_plateaus)
-    s_score = counter_plateaus_var / plateaus_var
-    return s_score
-
-# def analyze_event_chunk_with_padding(event_chunk, padding, library, model, num_components, penalty, data, dips, ML_standardisation_settings):
-#     chunk_results = []
-#     sampling_rate = ML_standardisation_settings['sampling_rate']
-#     for start, end in event_chunk:
-#         padded_start = max(start - padding, 0)
-#         padded_end = min(end + padding, len(data))
-#         padded_event_data = data[padded_start:padded_end]
-#         event_data = data[start:end]
-#         #try:
-#         if len(event_data) > 1:
-#             if library == "ruptures":
-#                 algo = rpt.Pelt(model=model).fit(event_data)
-#                 change_points = algo.predict(pen=penalty)
-#             elif library == "detecta":
-#                 if model == "cusum":
-#                     _, change_points, _, _ = detect_cusum(event_data, threshold=penalty, drift=0, ending=False, show=False)
-#             elif library == "lmfit":
-#                 change_points = autostepfinder(event_data,penalty)
-#             elif library == "hmm":
-#                 hmm_model = hmm.GaussianHMM(n_components=num_components).fit(event_data.reshape(-1, 1))
-#                 _, change_points = hmm_model.decode(event_data.reshape(-1, 1))
-#             elif library == "gmm":
-#                 gmm_model = GaussianMixture(n_components=num_components).fit(event_data.reshape(-1, 1))
-#                 change_points = np.where(np.diff(gmm_model.predict(event_data.reshape(-1, 1))))[0]
-#             else:
-#                 raise ValueError(f"Unsupported library: {library}")
-
-#             segments = [0] + list(change_points) + [len(event_data)]
-
-#             mean_values = []
-#             cusum_segments = []
-#             segment_widths_time = []
-#             segment_mean_diffs = []
-
-#             baseline_value = np.mean(data[padded_start:padded_end])
-#             number_of_segments = len(segments) - 2
-
-#             for i in range(1, len(segments)):
-#                 segment_start, segment_end = segments[i-1], segments[i]
-#                 segment_length = segment_end - segment_start
-#                 if segment_end > segment_start:
-#                     if segment_length >3:
-#                         rate_of_change = np.gradient(event_data[segment_start:segment_end])
-#                         min_rate_of_change = -0.5
-
-#                         is_sharp_decrease = np.any(rate_of_change < min_rate_of_change)
-#                     else:
-#                         is_sharp_decrease = False
-#                     if number_of_segments < 2:
-#                         if dips == "Yes":
-#                             segment_value = np.min(event_data)
-#                         else:
-#                             segment_value = np.max(event_data)
-#                     elif is_sharp_decrease:
-#                         if dips == "Yes":
-#                             segment_value = np.min(event_data[segment_start:segment_end])
-#                         else:
-#                             segment_value = np.max(event_data[segment_start:segment_end])
-#                     else:
-#                         if segment_length > 3:
-#                             elements_to_remove = int(np.ceil(segment_length * 0.2))
-
-#                             adjusted_start = segment_start + elements_to_remove
-#                             adjusted_end = segment_end - elements_to_remove
-
-#                             if adjusted_start < adjusted_end:
-#                                 segment_value = np.mean(event_data[adjusted_start:adjusted_end])
-#                             else:
-#                                 segment_value = np.mean(event_data)
-#                         else:
-#                             if dips == "Yes":
-#                                 segment_value = np.min(event_data[segment_start:segment_end])
-#                             else:
-#                                 segment_value = np.max(event_data[segment_start:segment_end])
-
-#                     mean_values.append(segment_value)
-
-#                     cusum_segments.append((segment_start + start, segment_end + start))
-#                     segment_widths_time.append((segment_end - segment_start) / sampling_rate)
-#                     segment_mean_diffs.append(baseline_value - segment_value)
-
-#             mean_values_continuous = np.zeros(len(event_data))
-#             for i, (segment_start, segment_end) in enumerate(cusum_segments):
-#                 mean_values_continuous[segment_start - start:segment_end - start] = mean_values[i]
-
-#             # mean_values_connected_with_baseline = np.full(len(padded_event_data), np.nan)
-#             # mean_values_connected_with_baseline[start-padded_start:end-padded_start] = mean_values_continuous
-
-#             # if padded_start < start:
-#             #     mean_values_connected_with_baseline[:start-padded_start] = baseline_value
-#             # if padded_end > end:
-#             #     mean_values_connected_with_baseline[end-padded_start:] = baseline_value
-
-#             mean_values_connected_with_baseline = np.full(len(padded_event_data), np.nan)
-#             mean_values_connected_with_baseline[start-padded_start:end-padded_start] = mean_values_continuous
-
-#             if padded_start < start:
-#                 mean_before = np.mean(padded_event_data[:start-padded_start])
-#                 mean_values_connected_with_baseline[:start-padded_start] = mean_before
-#             if padded_end > end:
-#                 mean_after = np.mean(padded_event_data[end-padded_start:])
-#                 mean_values_connected_with_baseline[end-padded_start:] = mean_after
-
-#             time_points_padded = np.linspace(padded_start / sampling_rate, padded_end / sampling_rate, len(padded_event_data))
-#             time_points_event = np.linspace(start / sampling_rate, end / sampling_rate, len(event_data))
-
-#             segment_info = {
-#                 "number_of_segments": len(cusum_segments),
-#                 "segment_mean_diffs": segment_mean_diffs,
-#                 "segment_widths_time": segment_widths_time,
-#                 "event_width": sum(segment_widths_time),
-#             }
-
-#             # Append additional event analysis
-#             event_analysis = np.append(analyze_event_for_CUSUM(event_data, baseline_value, ML_standardisation_settings),start/sampling_rate)
-                                       
-#             chunk_results.append({
-#                 "time_points_padded": time_points_padded,
-#                 "time_points_event": time_points_event,
-#                 "padded_event_data": padded_event_data,
-#                 "event_time_start_end": np.array([start/sampling_rate, end/sampling_rate]),
-#                 "baseline_value": baseline_value,
-#                 "mean_values": mean_values,
-#                 "mean_values_connected": mean_values_continuous,
-#                 "mean_values_connected_with_baseline": mean_values_connected_with_baseline,
-#                 "cusum_segments": cusum_segments,
-#                 "segment_info": segment_info,
-#                 "event_analysis": event_analysis,
-#             })
-
-#     return chunk_results
-
-
-
-
-# def analyze_event_chunk_with_padding(event_chunk, padding, library, model, num_components, penalty, data, dips, ML_standardisation_settings):
-#     segment_rate_threshold = 0.2
-#     chunk_results = []
-#     sampling_rate = ML_standardisation_settings['sampling_rate']
-    
-#     def detect_change_points(event_data, threshold):
-#         if library == "ruptures":
-#             algo = rpt.Pelt(model=model).fit(event_data)
-#             change_points = algo.predict(pen=penalty * threshold)
-#         elif library == "detecta":
-#             if model == "cusum":
-#                 _, change_points, _, _ = detect_cusum(event_data, threshold=penalty * threshold, drift=0, ending=False, show=False)
-#         elif library == "lmfit":
-#             change_points = autostepfinder(event_data, penalty * threshold)
-#         elif library == "hmm":
-#             hmm_model = hmm.GaussianHMM(n_components=num_components).fit(event_data.reshape(-1, 1))
-#             _, change_points = hmm_model.decode(event_data.reshape(-1, 1))
-#         elif library == "gmm":
-#             gmm_model = GaussianMixture(n_components=num_components).fit(event_data.reshape(-1, 1))
-#             change_points = np.where(np.diff(gmm_model.predict(event_data.reshape(-1, 1))))[0]
-#         else:
-#             raise ValueError(f"Unsupported library: {library}")
-#         return change_points
-    
-#     def compare_segment_rates(event_data, change_points, threshold):
-#         segments = [0] + list(change_points) + [len(event_data)]
-#         segment_rates = []
-        
-#         for i in range(len(segments) - 1):
-#             segment_start, segment_end = segments[i], segments[i + 1]
-#             segment_data = event_data[segment_start:segment_end]
-#             if len(segment_data) == 0:
-#                 continue
-#             segment_rate = np.mean(np.abs(np.diff(segment_data)))
-#             segment_rates.append(segment_rate)
-        
-#         merged_change_points = []
-#         merged_segment_rates = []
-        
-#         for i in range(len(segment_rates)):
-#             if i == 0 or abs(segment_rates[i] - merged_segment_rates[-1]) > threshold:
-#                 merged_change_points.append(change_points[i])
-#                 merged_segment_rates.append(segment_rates[i])
-        
-#         return merged_change_points
-    
-#     def adaptive_threshold(event_data):
-#         mean_val = np.mean(event_data)
-#         std_dev = np.std(event_data)
-#         return mean_val + 2 * std_dev  # Example adaptive threshold using mean and standard deviation
-    
-#     for start, end in event_chunk:
-#         padded_start = max(start - padding, 0)
-#         padded_end = min(end + padding, len(data))
-#         padded_event_data = data[padded_start:padded_end]
-#         event_data = data[start:end]
-        
-#         if len(event_data) > 1:
-#             event_duration_points = len(event_data)
-#             change_point_threshold = np.log(event_duration_points + 1)
-            
-#             num_passes = 3
-#             change_points_all = []
-#             for pass_idx in range(num_passes):
-#                 threshold = adaptive_threshold(event_data) / (pass_idx + 1)
-#                 change_points = detect_change_points(event_data, threshold)
-#                 change_points_all.extend(change_points)
-            
-#             change_points_all = sorted(set(change_points_all))
-            
-#             # Compare adjacent segments and merge if necessary
-#             merged_change_points = compare_segment_rates(event_data, change_points_all, segment_rate_threshold)
-            
-#             segments = [0] + list(merged_change_points) + [len(event_data)]
-#             mean_values = []
-#             cusum_segments = []
-#             segment_widths_time = []
-#             segment_mean_diffs = []
-
-#             baseline_value = np.median(data[padded_start:padded_end])
-#             number_of_segments = len(segments) - 1
-
-#             for i in range(1, len(segments)):
-#                 segment_start, segment_end = segments[i-1], segments[i]
-#                 segment_length = segment_end - segment_start
-#                 if segment_end > segment_start:
-#                     if segment_length > 3:
-#                         rate_of_change = np.gradient(event_data[segment_start:segment_end])
-#                         min_rate_of_change = -0.5
-#                         is_sharp_decrease = np.any(rate_of_change < min_rate_of_change)
-#                     else:
-#                         is_sharp_decrease = False
-#                     if number_of_segments < 2:
-                        
-#                         segment_value = np.min(event_data)
-
-#                     elif is_sharp_decrease:
-                        
-#                         segment_value = np.min(event_data[segment_start:segment_end])
-                        
-#                     else:
-#                         if segment_length > 3:
-#                             elements_to_remove = int(np.ceil(segment_length * 0.2))
-
-#                             adjusted_start = segment_start + elements_to_remove
-#                             adjusted_end = segment_end - elements_to_remove
-
-#                             if adjusted_start < adjusted_end:
-#                                 segment_value = np.min(event_data[adjusted_start:adjusted_end])
-#                             else:
-#                                 segment_value = np.min(event_data)
-#                         else:
-                            
-#                             segment_value = np.min(event_data[segment_start:segment_end])
-
-#                     mean_values.append(segment_value)
-
-#                     cusum_segments.append((segment_start + start, segment_end + start))
-#                     segment_widths_time.append((segment_end - segment_start) / sampling_rate)
-#                     segment_mean_diffs.append(baseline_value - segment_value)
-
-#             mean_values_continuous = np.zeros(len(event_data))
-#             for i, (segment_start, segment_end) in enumerate(cusum_segments):
-#                 mean_values_continuous[segment_start - start:segment_end - start] = mean_values[i]
-
-#             mean_values_connected_with_baseline = np.full(len(padded_event_data), baseline_value)
-#             mean_values_connected_with_baseline[start - padded_start:end - padded_start] = mean_values_continuous
-
-#             time_points_padded = np.linspace(padded_start / sampling_rate, padded_end / sampling_rate, len(padded_event_data))
-#             time_points_event = np.linspace(start / sampling_rate, end / sampling_rate, len(event_data))
-
-#             segment_info = {
-#                 "number_of_segments": number_of_segments,
-#                 "segment_mean_diffs": segment_mean_diffs,
-#                 "segment_widths_time": segment_widths_time,
-#                 "event_width": sum(segment_widths_time),
-#             }
-
-#             event_analysis = np.append(analyze_event_for_CUSUM(event_data, baseline_value, ML_standardisation_settings), start / sampling_rate)
-                                       
-#             chunk_results.append({
-#                 "time_points_padded": time_points_padded,
-#                 "time_points_event": time_points_event,
-#                 "padded_event_data": padded_event_data,
-#                 "event_time_start_end": np.array([start / sampling_rate, end / sampling_rate]),
-#                 "baseline_value": baseline_value,
-#                 "mean_values": mean_values,
-#                 "mean_values_connected": mean_values_continuous,
-#                 "mean_values_connected_with_baseline": mean_values_connected_with_baseline,
-#                 "cusum_segments": cusum_segments,
-#                 "segment_info": segment_info,
-#                 "event_analysis": event_analysis,
-#             })
-
-#     return chunk_results
-def analyze_event_chunk_with_padding(event_chunk, padding, library, model, num_components, penalty, data, dips, ML_standardisation_settings):
-    segment_rate_threshold = ML_standardisation_settings['segment_rate_threshold']
-    chunk_results = []
-    sampling_rate = ML_standardisation_settings['sampling_rate']
-    
-    def detect_change_points(event_data, threshold):
-        if library == "ruptures":
-            algo = rpt.Pelt(model=model).fit(event_data)
-            change_points = algo.predict(pen=penalty * threshold)
-        elif library == "detecta":
-            if model == "cusum":
-                _, change_points, _, _ = detect_cusum(event_data, threshold=penalty * threshold, drift=0, ending=False, show=False)
-        elif library == "lmfit":
-            change_points = autostepfinder(event_data, penalty * threshold)
-        elif library == "hmm":
-            hmm_model = hmm.GaussianHMM(n_components=num_components).fit(event_data.reshape(-1, 1))
-            _, change_points = hmm_model.decode(event_data.reshape(-1, 1))
-        elif library == "gmm":
-            gmm_model = GaussianMixture(n_components=num_components).fit(event_data.reshape(-1, 1))
-            change_points = np.where(np.diff(gmm_model.predict(event_data.reshape(-1, 1))))[0]
-        else:
-            raise ValueError(f"Unsupported library: {library}")
-        return change_points
-    
-    def compare_segment_rates(event_data, change_points, threshold):
-        segments = [0] + list(change_points) + [len(event_data)]
-        segment_rates = []
-        segment_mins = []
-        
-        for i in range(len(segments) - 1):
-            segment_start, segment_end = segments[i], segments[i + 1]
-            segment_data = event_data[segment_start:segment_end]
-            if len(segment_data) == 0:
-                continue
-            segment_rate = np.mean(np.abs(np.diff(segment_data)))
-            segment_rates.append(segment_rate)
-            segment_mins.append(np.min(segment_data))
-        
-        merged_change_points = []
-        merged_segment_rates = []
-        merged_segment_mins = []
-        merged_segments = []
-
-        i = 0
-        while i < len(segment_rates):
-            if i == 0 or abs(segment_rates[i] - merged_segment_rates[-1]) > threshold:
-                merged_change_points.append(change_points[i] if i < len(change_points) else segments[i + 1])
-                merged_segment_rates.append(segment_rates[i])
-                merged_segment_mins.append(segment_mins[i])
-                merged_segments.append((segments[i], segments[i + 1]))
-            else:
-                merged_segment_rates[-1] = (merged_segment_rates[-1] * (merged_segments[-1][1] - merged_segments[-1][0]) +
-                                            segment_rates[i] * (segments[i + 1] - segments[i])) / \
-                                           (merged_segments[-1][1] - merged_segments[-1][0] + segments[i + 1] - segments[i])
-                merged_segment_mins[-1] = min(merged_segment_mins[-1], segment_mins[i])
-                merged_segments[-1] = (merged_segments[-1][0], segments[i + 1])
-            i += 1
-        
-        return merged_change_points, merged_segments, merged_segment_mins
-    
-    def adaptive_threshold(event_data):
-        mean_val = np.mean(event_data)
-        std_dev = np.std(event_data)
-        return mean_val + 2 * std_dev  # Example adaptive threshold using mean and standard deviation
-    
-    for start, end in event_chunk:
-        padded_start = max(start - padding, 0)
-        padded_end = min(end + padding, len(data))
-        padded_event_data = data[padded_start:padded_end]
-        event_data = data[start:end]
-        
-        if len(event_data) > 1:
-            event_duration_points = len(event_data)
-            change_point_threshold = np.log(event_duration_points + 1)
-            
-            num_passes = 3
-            change_points_all = []
-            for pass_idx in range(num_passes):
-                threshold = adaptive_threshold(event_data) / (pass_idx + 1)
-                change_points = detect_change_points(event_data, threshold)
-                change_points_all.extend(change_points)
-            
-            change_points_all = sorted(set(change_points_all))
-            
-            # Compare adjacent segments and merge if necessary
-            merged_change_points, merged_segments, merged_segment_mins = compare_segment_rates(event_data, change_points_all, segment_rate_threshold)
-            
-            mean_values = []
-            cusum_segments = []
-            segment_widths_time = []
-            segment_mean_diffs = []
-
-            baseline_value = np.median(data[padded_start:start])
-            number_of_segments = len(merged_segments)
-
-            rate_of_change_threshold = 0.5
-
-            for i, (segment_start, segment_end) in enumerate(merged_segments):
-                segment_length = segment_end - segment_start
-                if segment_end > segment_start:
-                    if segment_length > 3:
-                        rate_of_change = np.gradient(event_data[segment_start:segment_end])
-                        is_sharp_change = np.any(np.abs(rate_of_change) > rate_of_change_threshold)
-                    else:
-                        is_sharp_change = False
-                    if number_of_segments < 2:
-                        segment_value = merged_segment_mins[i]
-                    elif is_sharp_change:
-                        segment_value = merged_segment_mins[i]
-                    else:
-                        if segment_length > 3:
-                            elements_to_remove = int(np.ceil(segment_length * 0.2))
-                            adjusted_start = segment_start + elements_to_remove
-                            adjusted_end = segment_end - elements_to_remove
-                            if adjusted_start < adjusted_end:
-                                segment_value = np.min(event_data[adjusted_start:adjusted_end])
-                            else:
-                                segment_value = merged_segment_mins[i]
-                        else:
-                            segment_value = merged_segment_mins[i]
-                    mean_values.append(segment_value)
-                    cusum_segments.append((segment_start + start, segment_end + start))
-                    segment_widths_time.append((segment_end - segment_start) / sampling_rate)
-                    segment_mean_diffs.append(baseline_value - segment_value)
-
-            mean_values_continuous = np.zeros(len(event_data))
-            for i, (segment_start, segment_end) in enumerate(cusum_segments):
-                mean_values_continuous[segment_start - start:segment_end - start] = mean_values[i]
-
-            mean_values_connected_with_baseline = np.full(len(padded_event_data), baseline_value)
-            mean_values_connected_with_baseline[start - padded_start:end - padded_start] = mean_values_continuous
-
-            time_points_padded = np.linspace(padded_start / sampling_rate, padded_end / sampling_rate, len(padded_event_data))
-            time_points_event = np.linspace(start / sampling_rate, end / sampling_rate, len(event_data))
-
-            segment_info = {
-                "number_of_segments": number_of_segments,
-                "segment_mean_diffs": segment_mean_diffs,
-                "segment_widths_time": segment_widths_time,
-                "event_width": sum(segment_widths_time),
+                if reduction >best_reduction :
+                    best_reduction =reduction 
+                    best_split_idx =(i ,split_idx )
+
+        if best_split_idx is None :
+            break 
+
+        plateau_idx ,split_idx =best_split_idx 
+        left_plateau ,right_plateau =split_plateau (plateaus [plateau_idx ],split_idx )
+        plateaus [plateau_idx ]=left_plateau 
+        plateaus .insert (plateau_idx +1 ,right_plateau )
+
+        change_points .append (sum (len (p )for p in plateaus [:plateau_idx ])+split_idx )
+
+        counter_plateaus =counter_fit (plateaus )
+        s_score =calculate_s_score (plateaus ,counter_plateaus )
+
+        if s_score <acceptance_threshold :
+            break 
+
+    change_points .sort ()
+    return change_points 
+
+def find_best_split (plateau ):
+    best_split_idx =None 
+    best_reduction =0 
+
+    for i in range (1 ,len (plateau )-1 ):
+        left_plateau =plateau [:i ]
+        right_plateau =plateau [i :]
+        left_mean =np .mean (left_plateau )
+        right_mean =np .mean (right_plateau )
+        reduction =np .sum ((left_plateau -left_mean )**2 )+np .sum ((right_plateau -right_mean )**2 )
+
+        if reduction >best_reduction :
+            best_reduction =reduction 
+            best_split_idx =i 
+
+    return best_split_idx 
+
+def split_plateau (plateau ,split_idx ):
+    left_plateau =plateau [:split_idx ]
+    right_plateau =plateau [split_idx :]
+    return left_plateau ,right_plateau 
+
+def counter_fit (plateaus ):
+    counter_plateaus =[]
+    for plateau in plateaus :
+        split_idx =find_best_split (plateau )
+        if split_idx is not None :
+            left_plateau ,right_plateau =split_plateau (plateau ,split_idx )
+            counter_plateaus .append (left_plateau )
+            counter_plateaus .append (right_plateau )
+        else :
+            counter_plateaus .append (plateau )
+    return counter_plateaus 
+
+def calculate_s_score (plateaus ,counter_plateaus ):
+    plateaus_var =sum (np .var (plateau )for plateau in plateaus )
+    counter_plateaus_var =sum (np .var (plateau )for plateau in counter_plateaus )
+    s_score =counter_plateaus_var /plateaus_var 
+    return s_score 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+def analyze_event_chunk_with_padding (event_chunk ,padding ,library ,model ,num_components ,penalty ,data ,dips ,ML_standardisation_settings ):
+    segment_rate_threshold =ML_standardisation_settings ['segment_rate_threshold']
+    chunk_results =[]
+    sampling_rate =ML_standardisation_settings ['sampling_rate']
+
+    def detect_change_points (event_data ,threshold ):
+        if library =="ruptures":
+            algo =rpt .Pelt (model =model ).fit (event_data )
+            change_points =algo .predict (pen =penalty *threshold )
+        elif library =="detecta":
+            if model =="cusum":
+                _ ,change_points ,_ ,_ =detect_cusum (event_data ,threshold =penalty *threshold ,drift =0 ,ending =False ,show =False )
+        elif library =="lmfit":
+            change_points =autostepfinder (event_data ,penalty *threshold )
+        elif library =="hmm":
+            hmm_model =hmm .GaussianHMM (n_components =num_components ).fit (event_data .reshape (-1 ,1 ))
+            _ ,change_points =hmm_model .decode (event_data .reshape (-1 ,1 ))
+        elif library =="gmm":
+            gmm_model =GaussianMixture (n_components =num_components ).fit (event_data .reshape (-1 ,1 ))
+            change_points =np .where (np .diff (gmm_model .predict (event_data .reshape (-1 ,1 ))))[0 ]
+        else :
+            raise ValueError (f"Unsupported library: {library}")
+        return change_points 
+
+    def compare_segment_rates (event_data ,change_points ,threshold ):
+        segments =[0 ]+list (change_points )+[len (event_data )]
+        segment_rates =[]
+        segment_mins =[]
+
+        for i in range (len (segments )-1 ):
+            segment_start ,segment_end =segments [i ],segments [i +1 ]
+            segment_data =event_data [segment_start :segment_end ]
+            if len (segment_data )==0 :
+                continue 
+            segment_rate =np .mean (np .abs (np .diff (segment_data )))
+            segment_rates .append (segment_rate )
+            segment_mins .append (np .min (segment_data ))
+
+        merged_change_points =[]
+        merged_segment_rates =[]
+        merged_segment_mins =[]
+        merged_segments =[]
+
+        i =0 
+        while i <len (segment_rates ):
+            if i ==0 or abs (segment_rates [i ]-merged_segment_rates [-1 ])>threshold :
+                merged_change_points .append (change_points [i ]if i <len (change_points )else segments [i +1 ])
+                merged_segment_rates .append (segment_rates [i ])
+                merged_segment_mins .append (segment_mins [i ])
+                merged_segments .append ((segments [i ],segments [i +1 ]))
+            else :
+                merged_segment_rates [-1 ]=(merged_segment_rates [-1 ]*(merged_segments [-1 ][1 ]-merged_segments [-1 ][0 ])+
+                segment_rates [i ]*(segments [i +1 ]-segments [i ]))/(merged_segments [-1 ][1 ]-merged_segments [-1 ][0 ]+segments [i +1 ]-segments [i ])
+                merged_segment_mins [-1 ]=min (merged_segment_mins [-1 ],segment_mins [i ])
+                merged_segments [-1 ]=(merged_segments [-1 ][0 ],segments [i +1 ])
+            i +=1 
+
+        return merged_change_points ,merged_segments ,merged_segment_mins 
+
+    def adaptive_threshold (event_data ):
+        mean_val =np .mean (event_data )
+        std_dev =np .std (event_data )
+        return mean_val +2 *std_dev 
+
+    for start ,end in event_chunk :
+        padded_start =max (start -padding ,0 )
+        padded_end =min (end +padding ,len (data ))
+        padded_event_data =data [padded_start :padded_end ]
+        event_data =data [start :end ]
+
+        if len (event_data )>1 :
+            event_duration_points =len (event_data )
+            change_point_threshold =np .log (event_duration_points +1 )
+
+            num_passes =3 
+            change_points_all =[]
+            for pass_idx in range (num_passes ):
+                threshold =adaptive_threshold (event_data )/(pass_idx +1 )
+                change_points =detect_change_points (event_data ,threshold )
+                change_points_all .extend (change_points )
+
+            change_points_all =sorted (set (change_points_all ))
+
+
+            merged_change_points ,merged_segments ,merged_segment_mins =compare_segment_rates (event_data ,change_points_all ,segment_rate_threshold )
+
+            mean_values =[]
+            cusum_segments =[]
+            segment_widths_time =[]
+            segment_mean_diffs =[]
+
+            baseline_value =np .median (data [padded_start :start ])
+            number_of_segments =len (merged_segments )
+
+            rate_of_change_threshold =0.5 
+
+            for i ,(segment_start ,segment_end )in enumerate (merged_segments ):
+                segment_length =segment_end -segment_start 
+                if segment_end >segment_start :
+                    if segment_length >3 :
+                        rate_of_change =np .gradient (event_data [segment_start :segment_end ])
+                        is_sharp_change =np .any (np .abs (rate_of_change )>rate_of_change_threshold )
+                    else :
+                        is_sharp_change =False 
+                    if number_of_segments <2 :
+                        segment_value =merged_segment_mins [i ]
+                    elif is_sharp_change :
+                        segment_value =merged_segment_mins [i ]
+                    else :
+                        if segment_length >3 :
+                            elements_to_remove =int (np .ceil (segment_length *0.2 ))
+                            adjusted_start =segment_start +elements_to_remove 
+                            adjusted_end =segment_end -elements_to_remove 
+                            if adjusted_start <adjusted_end :
+                                segment_value =np .min (event_data [adjusted_start :adjusted_end ])
+                            else :
+                                segment_value =merged_segment_mins [i ]
+                        else :
+                            segment_value =merged_segment_mins [i ]
+                    mean_values .append (segment_value )
+                    cusum_segments .append ((segment_start +start ,segment_end +start ))
+                    segment_widths_time .append ((segment_end -segment_start )/sampling_rate )
+                    segment_mean_diffs .append (baseline_value -segment_value )
+
+            mean_values_continuous =np .zeros (len (event_data ))
+            for i ,(segment_start ,segment_end )in enumerate (cusum_segments ):
+                mean_values_continuous [segment_start -start :segment_end -start ]=mean_values [i ]
+
+            mean_values_connected_with_baseline =np .full (len (padded_event_data ),baseline_value )
+            mean_values_connected_with_baseline [start -padded_start :end -padded_start ]=mean_values_continuous 
+
+            time_points_padded =np .linspace (padded_start /sampling_rate ,padded_end /sampling_rate ,len (padded_event_data ))
+            time_points_event =np .linspace (start /sampling_rate ,end /sampling_rate ,len (event_data ))
+
+            segment_info ={
+            "number_of_segments":number_of_segments ,
+            "segment_mean_diffs":segment_mean_diffs ,
+            "segment_widths_time":segment_widths_time ,
+            "event_width":sum (segment_widths_time ),
             }
 
-            event_analysis = np.append(analyze_event_for_CUSUM(event_data, baseline_value, ML_standardisation_settings), start / sampling_rate)
-                                       
-            chunk_results.append({
-                "time_points_padded": time_points_padded,
-                "time_points_event": time_points_event,
-                "padded_event_data": padded_event_data,
-                "event_time_start_end": np.array([start / sampling_rate, end / sampling_rate]),
-                "baseline_value": baseline_value,
-                "mean_values": mean_values,
-                "mean_values_connected": mean_values_continuous,
-                "mean_values_connected_with_baseline": mean_values_connected_with_baseline,
-                "cusum_segments": cusum_segments,
-                "segment_info": segment_info,
-                "event_analysis": event_analysis,
+            event_analysis =np .append (analyze_event_for_CUSUM (event_data ,baseline_value ,ML_standardisation_settings ),start /sampling_rate )
+
+            chunk_results .append ({
+            "time_points_padded":time_points_padded ,
+            "time_points_event":time_points_event ,
+            "padded_event_data":padded_event_data ,
+            "event_time_start_end":np .array ([start /sampling_rate ,end /sampling_rate ]),
+            "baseline_value":baseline_value ,
+            "mean_values":mean_values ,
+            "mean_values_connected":mean_values_continuous ,
+            "mean_values_connected_with_baseline":mean_values_connected_with_baseline ,
+            "cusum_segments":cusum_segments ,
+            "segment_info":segment_info ,
+            "event_analysis":event_analysis ,
             })
 
-    return chunk_results
+    return chunk_results 
 
-def multi_level_fitting_events(padding, chunk_size_events,library, model,num_components, penalty, data,events, dips, ML_standardisation_settings):
-    event_chunks = [events[i:i + chunk_size_events] for i in range(0, len(events), chunk_size_events)]
-    prepared_data_chunks = Parallel(n_jobs=-1)(
-        delayed(analyze_event_chunk_with_padding)(chunk, padding,library, model,num_components,penalty,data, dips, ML_standardisation_settings) for chunk in event_chunks
+def multi_level_fitting_events (padding ,chunk_size_events ,library ,model ,num_components ,penalty ,data ,events ,dips ,ML_standardisation_settings ):
+    event_chunks =[events [i :i +chunk_size_events ]for i in range (0 ,len (events ),chunk_size_events )]
+    prepared_data_chunks =Parallel (n_jobs =-1 )(
+    delayed (analyze_event_chunk_with_padding )(chunk ,padding ,library ,model ,num_components ,penalty ,data ,dips ,ML_standardisation_settings )for chunk in event_chunks 
     )
 
-    # Initialize a dictionary to hold all the data to be saved
-    npz_dict = {}
 
-    # Initialize a list to collect all the event_analysis arrays
-    all_event_analyses = []
+    npz_dict ={}
+
+
+    all_event_analyses =[]
+
+    event_counter =0 
+    for chunk_data in prepared_data_chunks :
+        for event_data in chunk_data :
+
+            event_key =f'EVENT_DATA_{event_counter}'
+            segment_info_key =f'SEGMENT_INFO_{event_counter}'
+            event_analysis_key =f'EVENT_ANALYSIS_{event_counter}'
+
 
-    event_counter = 0
-    for chunk_data in prepared_data_chunks:
-        for event_data in chunk_data:
-            # Construct keys for each data type
-            event_key = f'EVENT_DATA_{event_counter}'
-            segment_info_key = f'SEGMENT_INFO_{event_counter}'
-            event_analysis_key = f'EVENT_ANALYSIS_{event_counter}'
-
-            # Prepare the EVENT_DATA
-            event_data_formatted = [
-                np.array(event_data['time_points_padded'], dtype=np.float64),
-                np.array(event_data['padded_event_data'], dtype=np.float64),
-                np.array(event_data['event_time_start_end'], dtype=np.float64),
-                np.array(event_data['mean_values_connected_with_baseline'], dtype=np.float64),
-                np.full(len(event_data['padded_event_data']), event_data['baseline_value'], dtype=np.float64)
+            event_data_formatted =[
+            np .array (event_data ['time_points_padded'],dtype =np .float64 ),
+            np .array (event_data ['padded_event_data'],dtype =np .float64 ),
+            np .array (event_data ['event_time_start_end'],dtype =np .float64 ),
+            np .array (event_data ['mean_values_connected_with_baseline'],dtype =np .float64 ),
+            np .full (len (event_data ['padded_event_data']),event_data ['baseline_value'],dtype =np .float64 )
             ]
 
-            # Save each piece of data separately to handle varying lengths
-            for i, arr in enumerate(event_data_formatted):
-                npz_dict[f'{event_key}_part_{i}'] = arr
-
-            # Prepare and save SEGMENT_INFO
-            segment_info_formatted = {
-                'number_of_segments': np.array([event_data['segment_info']['number_of_segments']], dtype=np.float64),
-                'segment_mean_diffs': np.array(event_data['segment_info']['segment_mean_diffs'], dtype=np.float64),
-                'segment_widths_time': np.array(event_data['segment_info']['segment_widths_time'], dtype=np.float64),
-                'event_width': np.array([event_data['segment_info']['event_width']], dtype=np.float64),
+
+            for i ,arr in enumerate (event_data_formatted ):
+                npz_dict [f'{event_key}_part_{i}']=arr 
+
+
+            segment_info_formatted ={
+            'number_of_segments':np .array ([event_data ['segment_info']['number_of_segments']],dtype =np .float64 ),
+            'segment_mean_diffs':np .array (event_data ['segment_info']['segment_mean_diffs'],dtype =np .float64 ),
+            'segment_widths_time':np .array (event_data ['segment_info']['segment_widths_time'],dtype =np .float64 ),
+            'event_width':np .array ([event_data ['segment_info']['event_width']],dtype =np .float64 ),
             }
 
-            for key, value in segment_info_formatted.items():
-                npz_dict[f'{segment_info_key}_{key}'] = value
+            for key ,value in segment_info_formatted .items ():
+                npz_dict [f'{segment_info_key}_{key}']=value 
 
-            #Since event_analysis is a list, directly convert it to a numpy array
-            event_analysis_array = np.array(event_data['event_analysis'], dtype=np.float64)
-            npz_dict[f'EVENT_ANALYSIS_{event_counter}'] = event_analysis_array
-            # Append the numpy array to the all_event_analyses list
-            all_event_analyses.append(event_analysis_array)
-
-            event_counter += 1
-
-    # Convert the list of all event analyses into a numpy array
-    all_event_analyses_array = np.array(all_event_analyses, dtype=object)
-
-    return npz_dict, all_event_analyses_array
-
-class FileLoadError(Exception):
-    pass
-
-class CustomNavigationToolbar(NavigationToolbar):
-    def __init__(self, canvas, parent):
-        super().__init__(canvas, parent)
-        self.setIconSize(QSize(17, 17))  # Set the icon size to 17x17 pixels
-
-class MplWidget(QWidget):
-    def __init__(self, parent=None):
-        super(MplWidget, self).__init__(parent)
-        self.canvas = MplCanvas()
-        layout = QVBoxLayout()
-        layout.addWidget(self.canvas)
-        self.setLayout(layout)
-
-class MplCanvas(FigureCanvas):
-    def __init__(self, width=5, height=4, dpi=100):
-        fig = Figure(figsize=(width, height), dpi=dpi)
-        self.axes = fig.add_subplot(111)
-        super(MplCanvas, self).__init__(fig)
-
-
-class MainWindow(QMainWindow):
-    def __init__(self):
-        super().__init__()
-        self.setWindowTitle("SD Data Reduction App")
-        self.setGeometry(100, 100, 1200, 800)  # x, y, width, height
-        
-        # Main widget and layout
-        main_widget = QWidget()
-        self.setCentralWidget(main_widget)
-        main_layout = QHBoxLayout(main_widget)
-        
-        # Splitter for adjustable layouts
-        splitter = QSplitter(Qt.Orientation.Horizontal)
-        settings_widget = QWidget()
-        settings_layout = QVBoxLayout(settings_widget)
-        display_widget = QWidget()
-        display_layout = QVBoxLayout(display_widget)
-        
-        # Splitting the layout with splitter
-        splitter.addWidget(settings_widget)
-        splitter.addWidget(display_widget)
-        splitter.setSizes([350, 900])  # Adjusted sizes for left and right side
-        
-        main_layout.addWidget(splitter)
-        
-        # Add app name and email at the top of settings
-        self.setupTopLabels(settings_layout)
-        
-        # Setup tabs in settings_layout
-        self.setupTabs(settings_layout)
-        
-        # Setup the right side (display area)
-        self.setupDisplayArea(display_layout)
-        self.current_event_index = 0  # Starting at the first event
-        self.total_events = 0
-        self.sampling_rate = None
-        self.save_file_path = None
-
-    def setupTopLabels(self, layout):
-        self.app_name_label = QLabel("SD Data Reduction App")
-        self.app_name_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.app_name_label.setStyleSheet("font-size: 22px; font-weight: bold;")
-        self.email_label = QLabel("shankar.dutt@anu.edu.au")
-        self.email_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        layout.addWidget(self.app_name_label)
-        layout.addWidget(self.email_label)
-
-    def setupTabs(self, layout):
-        tab_widget = QTabWidget()
-        layout.addWidget(tab_widget)
-        
-        # Tabs
-        self.load_options_tab = LoadOptionsTab()
-        self.event_settings_tab = EventSettingsTab()
-        self.fitting_settings_tab = FittingSettingsTab()
-        self.ml_tab = MLTab()
-        
-        tab_widget.addTab(self.load_options_tab, "Load Options")
-        tab_widget.addTab(self.event_settings_tab, "Event Options")
-        tab_widget.addTab(self.fitting_settings_tab, "Fitting Options")
-        tab_widget.addTab(self.ml_tab, "ML")
-
-        #Connections Here!!
-        self.load_options_tab.test_settings_btn.clicked.connect(self.on_test_settings_clicked)
-        self.load_options_tab.perform_data_reduction_btn.clicked.connect(self.on_perform_data_reduction_clicked)
-        self.load_options_tab.plot_data_btn.clicked.connect(self.Plot_Entire_Data)
-        self.load_options_tab.save_file_path_btn.clicked.connect(self.specify_file_name)
-        
-    def setupDisplayArea(self, layout):
-        # Vertical splitter to separate the main plot area and the information area
-        vertical_splitter = QSplitter(Qt.Orientation.Vertical)
-        
-        # Top tab widget for Analysis and Plots
-        top_tab_widget = QTabWidget()
-        
-        # Analysis tab
-        analysis_tab = QWidget()
-        analysis_layout = QVBoxLayout(analysis_tab)
-        analysis_layout.setSpacing(0)
-        analysis_layout.setContentsMargins(0, 0, 0, 0)
-        self.data_visualization_widget = MplWidget()
-        self.data_visualization_toolbar = CustomNavigationToolbar(self.data_visualization_widget.canvas, self)
-        analysis_layout.addWidget(self.data_visualization_widget)
-        analysis_layout.addWidget(self.data_visualization_toolbar)
-        top_tab_widget.addTab(analysis_tab, "Analysis")
-        
-        # Plots tab
-        plots_tab = QWidget()
-        plots_layout = QHBoxLayout(plots_tab)
-        plots_layout.setSpacing(0)
-        plots_layout.setContentsMargins(0, 0, 0, 0)
-        self.plot_widgets = []
-        for i in range(2):
-            plot_widget = MplWidget()
-            plot_toolbar = CustomNavigationToolbar(plot_widget.canvas, self)
-            plot_layout = QVBoxLayout()
-            plot_layout.addWidget(plot_widget)
-            plot_layout.addWidget(plot_toolbar)
-            plots_layout.addLayout(plot_layout)
-            self.plot_widgets.append(plot_widget)
-        top_tab_widget.addTab(plots_tab, "Plots")
-        
-        # Bottom splitter for the table, event details, and second plot with navigation
-        bottom_splitter = QSplitter(Qt.Orientation.Horizontal)
-        
-        # Widget for the table and event information
-        table_and_info_widget = QWidget()
-        table_and_info_layout = QVBoxLayout(table_and_info_widget)
-        table_and_info_layout.setSpacing(0)
-        table_and_info_layout.setContentsMargins(0, 0, 0, 0)
-        self.table_widget = QTableWidget()
-        self.event_info_text_edit = QTextEdit()
-        self.event_info_text_edit.setReadOnly(True)
-        table_and_info_layout.addWidget(self.table_widget)
-        table_and_info_layout.addWidget(self.event_info_text_edit)
-        
-        # Widget for the second plot and navigation
-        event_plot_and_navigation_widget = QWidget()
-        event_plot_and_navigation_layout = QVBoxLayout(event_plot_and_navigation_widget)
-        event_plot_and_navigation_layout.setSpacing(0)
-        event_plot_and_navigation_layout.setContentsMargins(0, 0, 0, 0)
-        self.event_visualization_widget = MplWidget()
-        self.event_visualization_toolbar = CustomNavigationToolbar(self.event_visualization_widget.canvas, self)
-        event_plot_and_navigation_layout.addWidget(self.event_visualization_widget)
-        event_plot_and_navigation_layout.addWidget(self.event_visualization_toolbar)
-        self.setupEventNavigationButtons(event_plot_and_navigation_layout)
-
-        # Add widgets to the bottom splitter and set their sizes
-        bottom_splitter.addWidget(table_and_info_widget)
-        bottom_splitter.addWidget(event_plot_and_navigation_widget)
-        bottom_splitter.setSizes([int(self.width() * 0.55), int(self.width() * 0.45)])
-        
-        # Add top tab widget and bottom splitter to the vertical splitter
-        vertical_splitter.addWidget(top_tab_widget)
-        vertical_splitter.addWidget(bottom_splitter)
-        
-        # Set the sizes of the vertical splitter. 
-        vertical_splitter.setSizes([int(self.height() * 0.5), int(self.height() * 0.5)])
-        
-        # Finally, add the vertical splitter to the main layout
-        layout.addWidget(vertical_splitter)
-
-
-    def setupEventNavigationButtons(self, layout):
-        # Event navigation buttons (Previous, Next, Jump To)
-        event_navigation_layout = QHBoxLayout()
-        event_navigation_layout.setSpacing(0)
-        event_navigation_layout.setContentsMargins(0, 0, 0, 0)
-        self.previous_button = QPushButton("Previous")
-        self.next_button = QPushButton("Next")
-        self.jump_to_label = QLabel("Jump To (index):")
-        self.jump_to_spinbox = QSpinBox()
-        self.jump_button = QPushButton("Jump")
-        event_navigation_layout.addWidget(self.previous_button)
-        event_navigation_layout.addWidget(self.next_button)
-        event_navigation_layout.addWidget(self.jump_to_label)
-        event_navigation_layout.addWidget(self.jump_to_spinbox)
-        event_navigation_layout.addWidget(self.jump_button)
-        layout.addLayout(event_navigation_layout)
-        self.previous_button.clicked.connect(self.navigate_to_previous_event)
-        self.next_button.clicked.connect(self.navigate_to_next_event)
-        self.jump_button.clicked.connect(self.jump_to_event)
-
-    def specify_file_name(self):
-        # Inform the user to select a folder
-        #QMessageBox.information(self, "Select Folder", "Please select a folder to save the file.")
-
-        # Step 1: Let the user select a directory with a clear instruction in the dialog title
-        folder_path = QFileDialog.getExistingDirectory(self, "Select Folder to Save File")
-        if folder_path:  # Ensure the user selected a folder
-            # Step 2: Prompt the user to specify a file name
-            file_name, ok = QInputDialog.getText(self, "Specify File Name", "Enter only the file name (without extension):")
-            if ok and file_name:  # Ensure the user entered a file name and pressed OK
-                # Combine the folder path and file name to form the full file path
-                self.save_file_path = f"{folder_path}/{file_name}"
-                #print(f"File path specified: {self.save_file_path}") # For checking
 
-    
-    def on_test_settings_clicked(self):
-        start_time = time.time()
-        # Get selected items from the list
-        selected_items = self.load_options_tab.files_list_widget.selectedItems()
-        if selected_items:
-            
-            # Use only the first selected file
-            file_path = selected_items[0].data(Qt.ItemDataRole.UserRole)
+            event_analysis_array =np .array (event_data ['event_analysis'],dtype =np .float64 )
+            npz_dict [f'EVENT_ANALYSIS_{event_counter}']=event_analysis_array 
+
+            all_event_analyses .append (event_analysis_array )
+
+            event_counter +=1 
+
+
+    all_event_analyses_array =np .array (all_event_analyses ,dtype =object )
+
+    return npz_dict ,all_event_analyses_array 
+
+class FileLoadError (Exception ):
+    pass 
+
+class CustomNavigationToolbar (NavigationToolbar ):
+    def __init__ (self ,canvas ,parent ):
+        super ().__init__ (canvas ,parent )
+        self .setIconSize (QSize (17 ,17 ))
+
+class MplWidget (QWidget ):
+    def __init__ (self ,parent =None ):
+        super (MplWidget ,self ).__init__ (parent )
+        self .canvas =MplCanvas ()
+        layout =QVBoxLayout ()
+        layout .addWidget (self .canvas )
+        self .setLayout (layout )
+
+class MplCanvas (FigureCanvas ):
+    def __init__ (self ,width =5 ,height =4 ,dpi =100 ):
+        fig =Figure (figsize =(width ,height ),dpi =dpi )
+        self .axes =fig .add_subplot (111 )
+        super (MplCanvas ,self ).__init__ (fig )
+
+
+class MainWindow (QMainWindow ):
+    def __init__ (self ):
+        super ().__init__ ()
+        self .setWindowTitle ("SD Data Reduction App")
+        self .setGeometry (100 ,100 ,1200 ,800 )
+
+
+        main_widget =QWidget ()
+        self .setCentralWidget (main_widget )
+        main_layout =QHBoxLayout (main_widget )
+
+
+        splitter =QSplitter (Qt .Orientation .Horizontal )
+        settings_widget =QWidget ()
+        settings_layout =QVBoxLayout (settings_widget )
+        display_widget =QWidget ()
+        display_layout =QVBoxLayout (display_widget )
+
+
+        splitter .addWidget (settings_widget )
+        splitter .addWidget (display_widget )
+        splitter .setSizes ([350 ,900 ])
+
+        main_layout .addWidget (splitter )
+
+
+        self .setupTopLabels (settings_layout )
+
+
+        self .setupTabs (settings_layout )
+
+
+        self .setupDisplayArea (display_layout )
+        self .current_event_index =0 
+        self .total_events =0 
+        self .sampling_rate =None 
+        self .save_file_path =None 
+
+    def setupTopLabels (self ,layout ):
+        self .app_name_label =QLabel ("SD Data Reduction App")
+        self .app_name_label .setAlignment (Qt .AlignmentFlag .AlignCenter )
+        self .app_name_label .setStyleSheet ("font-size: 22px; font-weight: bold;")
+        self .email_label =QLabel ("shankar.dutt@anu.edu.au")
+        self .email_label .setAlignment (Qt .AlignmentFlag .AlignCenter )
+        layout .addWidget (self .app_name_label )
+        layout .addWidget (self .email_label )
+
+    def setupTabs (self ,layout ):
+        tab_widget =QTabWidget ()
+        layout .addWidget (tab_widget )
+
+
+        self .load_options_tab =LoadOptionsTab ()
+        self .event_settings_tab =EventSettingsTab ()
+        self .fitting_settings_tab =FittingSettingsTab ()
+        self .ml_tab =MLTab ()
+
+        tab_widget .addTab (self .load_options_tab ,"Load Options")
+        tab_widget .addTab (self .event_settings_tab ,"Event Options")
+        tab_widget .addTab (self .fitting_settings_tab ,"Fitting Options")
+        tab_widget .addTab (self .ml_tab ,"ML")
+
+
+        self .load_options_tab .test_settings_btn .clicked .connect (self .on_test_settings_clicked )
+        self .load_options_tab .perform_data_reduction_btn .clicked .connect (self .on_perform_data_reduction_clicked )
+        self .load_options_tab .plot_data_btn .clicked .connect (self .Plot_Entire_Data )
+        self .load_options_tab .save_file_path_btn .clicked .connect (self .specify_file_name )
+
+    def setupDisplayArea (self ,layout ):
+
+        vertical_splitter =QSplitter (Qt .Orientation .Vertical )
+
+
+        top_tab_widget =QTabWidget ()
+
+
+        analysis_tab =QWidget ()
+        analysis_layout =QVBoxLayout (analysis_tab )
+        analysis_layout .setSpacing (0 )
+        analysis_layout .setContentsMargins (0 ,0 ,0 ,0 )
+        self .data_visualization_widget =MplWidget ()
+        self .data_visualization_toolbar =CustomNavigationToolbar (self .data_visualization_widget .canvas ,self )
+        analysis_layout .addWidget (self .data_visualization_widget )
+        analysis_layout .addWidget (self .data_visualization_toolbar )
+        top_tab_widget .addTab (analysis_tab ,"Analysis")
+
+
+        plots_tab =QWidget ()
+        plots_layout =QHBoxLayout (plots_tab )
+        plots_layout .setSpacing (0 )
+        plots_layout .setContentsMargins (0 ,0 ,0 ,0 )
+        self .plot_widgets =[]
+        for i in range (2 ):
+            plot_widget =MplWidget ()
+            plot_toolbar =CustomNavigationToolbar (plot_widget .canvas ,self )
+            plot_layout =QVBoxLayout ()
+            plot_layout .addWidget (plot_widget )
+            plot_layout .addWidget (plot_toolbar )
+            plots_layout .addLayout (plot_layout )
+            self .plot_widgets .append (plot_widget )
+        top_tab_widget .addTab (plots_tab ,"Plots")
+
+
+        bottom_splitter =QSplitter (Qt .Orientation .Horizontal )
+
+
+        table_and_info_widget =QWidget ()
+        table_and_info_layout =QVBoxLayout (table_and_info_widget )
+        table_and_info_layout .setSpacing (0 )
+        table_and_info_layout .setContentsMargins (0 ,0 ,0 ,0 )
+        self .table_widget =QTableWidget ()
+        self .event_info_text_edit =QTextEdit ()
+        self .event_info_text_edit .setReadOnly (True )
+        table_and_info_layout .addWidget (self .table_widget )
+        table_and_info_layout .addWidget (self .event_info_text_edit )
+
+
+        event_plot_and_navigation_widget =QWidget ()
+        event_plot_and_navigation_layout =QVBoxLayout (event_plot_and_navigation_widget )
+        event_plot_and_navigation_layout .setSpacing (0 )
+        event_plot_and_navigation_layout .setContentsMargins (0 ,0 ,0 ,0 )
+        self .event_visualization_widget =MplWidget ()
+        self .event_visualization_toolbar =CustomNavigationToolbar (self .event_visualization_widget .canvas ,self )
+        event_plot_and_navigation_layout .addWidget (self .event_visualization_widget )
+        event_plot_and_navigation_layout .addWidget (self .event_visualization_toolbar )
+        self .setupEventNavigationButtons (event_plot_and_navigation_layout )
+
+
+        bottom_splitter .addWidget (table_and_info_widget )
+        bottom_splitter .addWidget (event_plot_and_navigation_widget )
+        bottom_splitter .setSizes ([int (self .width ()*0.55 ),int (self .width ()*0.45 )])
+
+
+        vertical_splitter .addWidget (top_tab_widget )
+        vertical_splitter .addWidget (bottom_splitter )
+
+
+        vertical_splitter .setSizes ([int (self .height ()*0.5 ),int (self .height ()*0.5 )])
+
+
+        layout .addWidget (vertical_splitter )
+
 
-            if self.event_settings_tab.enable_window_loading.isChecked():
-                if file_path.endswith('.abf'):
-                    #Load the sampling rate and length of the file in seconds
-                    length_in_seconds,sampling_rate = get_abf_file_info(file_path)
-                    # Load data and sampling rate from the file
-                    if self.event_settings_tab.enable_nth_data_point_loading.isChecked():
-                        msg = QMessageBox()
-                        msg.setIcon(QMessageBox.Icon.Critical)
-                        msg.setWindowTitle("Error")
-                        msg.setText("An error has occurred.")
-                        msg.setInformativeText(f"Loading of nth data point has not yet been implemented. Loading every single point.")
-                        msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-                        msg.exec()
-                        step = 1
-                    else:
-                        step = 1
-                    
-                    raw_io = AxonRawIO(filename=file_path)
-                    raw_io.parse_header()
-                    signal_size = raw_io.get_signal_size(block_index=0, seg_index=0)
-
-                    if self.event_settings_tab.apply_filter_combo.currentText() == "Yes":
-                        if self.event_settings_tab.filter_type_combo.currentText() == "Wavelet":
-                            filter_type = "Wavelet"
-                            cutoff_freq = 10000
-                        else:
-                            filter_type = self.event_settings_tab.low_pass_filter_type_combo.currentText()
-                            cutoff_freq = self.event_settings_tab.cutoff_frequency_spinbox.value()*1000
-                    if self.event_settings_tab.type_of_threshold_combo.currentText() == "ΔI":
-                        threshold_method = "difference"
-                    else:
-                        threshold_method = "multiplier"
-                    if self.event_settings_tab.dips_or_peaks_combo.currentText()=="Dips":
-                        dips = "Yes"
-                    else:
-                        dips = "No"
-                    
-                    threshold_multiplier, start_multiplier, end_multiplier, threshold_difference =  self.event_settings_tab.threshold_value_multiplier_spinbox.value(),  self.event_settings_tab.start_of_event_threshold_spinbox.value(), self.event_settings_tab.end_of_event_threshold_spinbox.value(), self.event_settings_tab.threshold_value_multiplier_spinbox.value()
-                    avg_window_size_in_ms, std_window_size_in_ms = self.event_settings_tab.mean_window_size_spinbox.value(), self.event_settings_tab.std_window_size_spinbox.value()
-                    min_event_width, max_event_width = self.event_settings_tab.minimum_event_width_spinbox.value()/1000, self.event_settings_tab.maximum_event_width_spinbox.value()/1000
-                    channel_index = 0
-                    chunk_size = max(avg_window_size_in_ms,std_window_size_in_ms)*self.event_settings_tab.window_size_multiple_spinbox.value()*sampling_rate
-
-                    start_testing_duration = self.load_options_tab.testing_duration_start_spinbox.value()
-                    end_testing_duration = self.load_options_tab.testing_duration_end_spinbox.value()  # in seconds
-                    desired_duration = end_testing_duration
-                    start_index = int(start_testing_duration * sampling_rate)
-                    start_chunk_index = int(start_index // (chunk_size * step))
-                    num_chunks = int((signal_size - start_index) // (chunk_size * step)) + (0 if (signal_size - start_index) % (chunk_size * step) == 0 else 1)
-
-                    results = Parallel(n_jobs=-1)(
-                        delayed(process_chunk_window_abf_with_data)(file_path, desired_duration, chunk_index, chunk_size, step, channel_index, signal_size, sampling_rate, filter_type, cutoff_freq, threshold_method, dips, threshold_multiplier, start_multiplier, end_multiplier, threshold_difference, avg_window_size_in_ms, std_window_size_in_ms, min_event_width, max_event_width, start_index)
-                        for chunk_index in range(start_chunk_index, start_chunk_index + num_chunks)
+    def setupEventNavigationButtons (self ,layout ):
+
+        event_navigation_layout =QHBoxLayout ()
+        event_navigation_layout .setSpacing (0 )
+        event_navigation_layout .setContentsMargins (0 ,0 ,0 ,0 )
+        self .previous_button =QPushButton ("Previous")
+        self .next_button =QPushButton ("Next")
+        self .jump_to_label =QLabel ("Jump To (index):")
+        self .jump_to_spinbox =QSpinBox ()
+        self .jump_button =QPushButton ("Jump")
+        event_navigation_layout .addWidget (self .previous_button )
+        event_navigation_layout .addWidget (self .next_button )
+        event_navigation_layout .addWidget (self .jump_to_label )
+        event_navigation_layout .addWidget (self .jump_to_spinbox )
+        event_navigation_layout .addWidget (self .jump_button )
+        layout .addLayout (event_navigation_layout )
+        self .previous_button .clicked .connect (self .navigate_to_previous_event )
+        self .next_button .clicked .connect (self .navigate_to_next_event )
+        self .jump_button .clicked .connect (self .jump_to_event )
+
+    def specify_file_name (self ):
+
+
+
+
+        folder_path =QFileDialog .getExistingDirectory (self ,"Select Folder to Save File")
+        if folder_path :
+
+            file_name ,ok =QInputDialog .getText (self ,"Specify File Name","Enter only the file name (without extension):")
+            if ok and file_name :
+
+                self .save_file_path =f"{folder_path}/{file_name}"
+
+
+
+    def on_test_settings_clicked (self ):
+        start_time =time .time ()
+
+        selected_items =self .load_options_tab .files_list_widget .selectedItems ()
+        if selected_items :
+
+
+            file_path =selected_items [0 ].data (Qt .ItemDataRole .UserRole )
+
+            if self .event_settings_tab .enable_window_loading .isChecked ():
+                if file_path .endswith ('.abf'):
+
+                    length_in_seconds ,sampling_rate =get_abf_file_info (file_path )
+
+                    if self .event_settings_tab .enable_nth_data_point_loading .isChecked ():
+                        msg =QMessageBox ()
+                        msg .setIcon (QMessageBox .Icon .Critical )
+                        msg .setWindowTitle ("Error")
+                        msg .setText ("An error has occurred.")
+                        msg .setInformativeText (f"Loading of nth data point has not yet been implemented. Loading every single point.")
+                        msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+                        msg .exec ()
+                        step =1 
+                    else :
+                        step =1 
+
+                    raw_io =AxonRawIO (filename =file_path )
+                    raw_io .parse_header ()
+                    signal_size =raw_io .get_signal_size (block_index =0 ,seg_index =0 )
+
+                    if self .event_settings_tab .apply_filter_combo .currentText ()=="Yes":
+                        if self .event_settings_tab .filter_type_combo .currentText ()=="Wavelet":
+                            filter_type ="Wavelet"
+                            cutoff_freq =10000 
+                        else :
+                            filter_type =self .event_settings_tab .low_pass_filter_type_combo .currentText ()
+                            cutoff_freq =self .event_settings_tab .cutoff_frequency_spinbox .value ()*1000 
+                    if self .event_settings_tab .type_of_threshold_combo .currentText ()=="ΔI":
+                        threshold_method ="difference"
+                    else :
+                        threshold_method ="multiplier"
+                    if self .event_settings_tab .dips_or_peaks_combo .currentText ()=="Dips":
+                        dips ="Yes"
+                    else :
+                        dips ="No"
+
+                    threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference =self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .start_of_event_threshold_spinbox .value (),self .event_settings_tab .end_of_event_threshold_spinbox .value (),self .event_settings_tab .threshold_value_multiplier_spinbox .value ()
+                    avg_window_size_in_ms ,std_window_size_in_ms =self .event_settings_tab .mean_window_size_spinbox .value (),self .event_settings_tab .std_window_size_spinbox .value ()
+                    min_event_width ,max_event_width =self .event_settings_tab .minimum_event_width_spinbox .value ()/1000 ,self .event_settings_tab .maximum_event_width_spinbox .value ()/1000 
+                    channel_index =0 
+                    chunk_size =max (avg_window_size_in_ms ,std_window_size_in_ms )*self .event_settings_tab .window_size_multiple_spinbox .value ()*sampling_rate 
+
+                    start_testing_duration =self .load_options_tab .testing_duration_start_spinbox .value ()
+                    end_testing_duration =self .load_options_tab .testing_duration_end_spinbox .value ()
+                    desired_duration =end_testing_duration 
+                    start_index =int (start_testing_duration *sampling_rate )
+                    start_chunk_index =int (start_index //(chunk_size *step ))
+                    num_chunks =int ((signal_size -start_index )//(chunk_size *step ))+(0 if (signal_size -start_index )%(chunk_size *step )==0 else 1 )
+
+                    results =Parallel (n_jobs =-1 )(
+                    delayed (process_chunk_window_abf_with_data )(file_path ,desired_duration ,chunk_index ,chunk_size ,step ,channel_index ,signal_size ,sampling_rate ,filter_type ,cutoff_freq ,threshold_method ,dips ,threshold_multiplier ,start_multiplier ,end_multiplier ,threshold_difference ,avg_window_size_in_ms ,std_window_size_in_ms ,min_event_width ,max_event_width ,start_index )
+                    for chunk_index in range (start_chunk_index ,start_chunk_index +num_chunks )
                     )
 
-                   # Unzip the results
-                    chunk_events, chunk_rolling_avgs, chunk_rolling_stds, chunk_data = zip(*results)
 
-                    # After the parallel processing loop
-                    combined_events = [event for chunk_events_tuple in chunk_events for event in chunk_events_tuple]
-                    rolling_avg_refined = np.concatenate(chunk_rolling_avgs)
-                    rolling_std_refined = np.concatenate(chunk_rolling_stds)
-                    data = np.concatenate(chunk_data)
-
-                    # Adjust event indices based on their chunk offsets and filter out those crossing chunk boundaries
-                    adjusted_events = []
-                    for chunk_index, chunk_events_tuple in enumerate(chunk_events):
-                        chunk_start_index = chunk_index * chunk_size * step
-                        for event in chunk_events_tuple:
-                            start, end = event
-                            if start + chunk_start_index < (chunk_index + 1) * chunk_size * step and end + chunk_start_index <= min((chunk_index + 1) * chunk_size * step, signal_size):
-                                adjusted_events.append((start + chunk_start_index, end + chunk_start_index))
-
-                    if threshold_method == "multiplier":
-                        if dips == "Yes":
-                            rolling_threshold_refined = rolling_avg_refined - (threshold_multiplier * rolling_std_refined)
-                        else:
-                            rolling_threshold_refined = rolling_avg_refined + (threshold_multiplier * rolling_std_refined)
-                    elif threshold_method == "difference":
-                        if dips == "Yes":
-                            rolling_threshold_refined = rolling_avg_refined - (threshold_difference / 1000)
-                        else:
-                            rolling_threshold_refined = rolling_avg_refined + (threshold_difference / 1000)
-
-                    if self.event_settings_tab.enable_std_smoothing_checkbox.isChecked():
-                        rolling_threshold_refined = smooth_threshold(rolling_threshold_refined,int((std_window_size_in_ms / 1000) * sampling_rate),self.event_settings_tab.smoothing_type_dropdown.currentIndex())
-                    
-                    events = adjusted_events
-                    end_time = time.time()
-                    time_taken = end_time-start_time
-
-                elif  file_path.endswith('.hdf5') or file_path.endswith('.h5'):
-                    msg = QMessageBox()
-                    msg.setIcon(QMessageBox.Icon.Critical)
-                    msg.setWindowTitle("Error")
-                    msg.setText("An error has occurred.")
-                    msg.setInformativeText(f"Loading of hdf5 files has not yet been implemented with window processing. Please use the normal processing methods.")
-                    msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-                    msg.exec()
-                    
-            else:
-                if file_path.endswith('.abf'):
-                    #Load the sampling rate and length of the file in seconds
-                    length_in_seconds,sampling_rate = get_abf_file_info(file_path)
-                    # Load data and sampling rate from the file
-                    if self.event_settings_tab.enable_nth_data_point_loading.isChecked():
-                        data, sampling_rate = load_abf_file_nth(file_path,self.event_settings_tab.nth_data_point_spinbox.value())
-                    else:
-                        data, sampling_rate = load_abf_file(file_path)
-                elif  file_path.endswith('.hdf5') or file_path.endswith('.h5'):
-                    data,sampling_rate = load_hdf5_file(file_path)
-                    length_in_seconds = len(data)/sampling_rate
-                         
-                if data is not None:
-                    # Determine the number of points to plot based on the testing duration
-                    # This can be removed in main function
-                    start_testing_duration = self.load_options_tab.testing_duration_start_spinbox.value()
-                    end_testing_duration = self.load_options_tab.testing_duration_end_spinbox.value()  # in seconds
-                    start_points = int(start_testing_duration * sampling_rate)
-                    end_points = int(end_testing_duration * sampling_rate)
-                    # Take the slice of data 
-                    data = data[start_points:end_points]
-
-                    # Update the EventSettingsTab with the sampling rate and file duration
-                    self.event_settings_tab.sampling_rate_spinbox.setValue(sampling_rate / 1000)  # Convert to kHz
-                    self.event_settings_tab.analysis_end_duration_spinbox.setValue(length_in_seconds)
-                    self.event_settings_tab.analysis_end_duration_spinbox.setMaximum(length_in_seconds)
-                    self.load_options_tab.testing_duration_end_spinbox.setMaximum(length_in_seconds)
-
-                    if self.event_settings_tab.apply_filter_combo.currentText() == "Yes":
-                        if self.event_settings_tab.filter_type_combo.currentText() == "Wavelet":
-                            data = apply_low_pass_filter(data, 10000, "Wavelet",sampling_rate)
-                        else:
-                            data = apply_low_pass_filter(data, self.event_settings_tab.cutoff_frequency_spinbox.value()*1000, self.event_settings_tab.low_pass_filter_type_combo.currentText(),sampling_rate)
-                    if self.event_settings_tab.type_of_threshold_combo.currentText() == "ΔI":
-                        threshold_method = "difference"
-                    else:
-                        threshold_method = "multiplier"
-                    if self.event_settings_tab.dips_or_peaks_combo.currentText()=="Dips":
-                        dips = "Yes"
-                    else:
-                        dips = "Yes"
-                        data_sent = ne.evaluate("data*(-1)")
-                    if self.event_settings_tab.enable_std_smoothing_checkbox.isChecked():
-                        enable_smoothing = "Yes"
-                    else:
-                        enable_smoothing = "No"
-                    try:
-                        if self.event_settings_tab.dips_or_peaks_combo.currentText()=="Dips":
-                            events,rolling_avg_refined, rolling_threshold_refined = find_events_refined_parallel(data, self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.start_of_event_threshold_spinbox.value(), self.event_settings_tab.end_of_event_threshold_spinbox.value(), self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.mean_window_size_spinbox.value(), self.event_settings_tab.std_window_size_spinbox.value(), threshold_method, self.event_settings_tab.minimum_event_width_spinbox.value()/1000, self.event_settings_tab.maximum_event_width_spinbox.value()/1000, self.fitting_settings_tab.chunk_size_for_event_detection_spinbox.value(), dips, sampling_rate, enable_smoothing, self.event_settings_tab.smoothing_type_dropdown.currentIndex(), n_jobs = -1)
-                        else:
-                            events,rolling_avg_refined, rolling_threshold_refined = find_events_refined_parallel(data_sent, self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.start_of_event_threshold_spinbox.value(), self.event_settings_tab.end_of_event_threshold_spinbox.value(), self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.mean_window_size_spinbox.value(), self.event_settings_tab.std_window_size_spinbox.value(), threshold_method, self.event_settings_tab.minimum_event_width_spinbox.value()/1000, self.event_settings_tab.maximum_event_width_spinbox.value()/1000, self.fitting_settings_tab.chunk_size_for_event_detection_spinbox.value(), dips, sampling_rate, enable_smoothing, self.event_settings_tab.smoothing_type_dropdown.currentIndex(), n_jobs = -1)
-                        end_time = time.time()
-                        time_taken = end_time-start_time
-
-                        if self.event_settings_tab.dips_or_peaks_combo.currentText()!="Dips":
-                            rolling_avg_refined, rolling_threshold_refined = ne.evaluate("rolling_avg_refined*-1"), ne.evaluate("rolling_threshold_refined *-1")
-                    except:
-                        msg = QMessageBox()
-                        msg.setIcon(QMessageBox.Icon.Critical)
-                        msg.setWindowTitle("Error")
-                        msg.setText("An error has occurred.")
-                        msg.setInformativeText(f"I cannot extract any events from the selected file ({file_path}) within the selected duration. \nContact shankar.dutt@anu.edu.au")
-                        msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-                        msg.exec()
-                    
-            # Update information
-            self.update_file_info(file_path, length_in_seconds, len(events), time_taken, file_path, test = "True")
-            # Plot the data
-            self.plot_events(events, data, rolling_avg_refined, rolling_threshold_refined, sampling_rate)
-            # Event Fitting
-            if self.load_options_tab.level_fitting_combo.currentText() == "Yes":
-
-                if self.fitting_settings_tab.enable_standardisation_checkbox.isChecked():
-                    standard = self.fitting_settings_tab.standardisation_type_combo.currentText()
-                else:
-                    standard = "Normal"
-                if self.ml_tab.enable_ml_data_reduction_checkbox.isChecked():
-                    ML_enabled = "True"
-                    ML_tag = self.ml_tab.tag_lineedit.text()
-                    ML_standard = self.ml_tab.data_reduction_type_combo.currentText()
-                    if self.ml_tab.apply_standardisation_checkbox.isChecked():
-                        if self.fitting_settings_tab.enable_standardisation_checkbox.isChecked():
-                            standard = self.fitting_settings_tab.standardisation_type_combo.currentText()
-                    else:
-                        standard = "Normal"
-                else:
-                    ML_enabled = "False"
-                    ML_standard = None
-                    ML_tag = None
-
-                ML_standardisation_settings = {
-                    'standard' : standard,
-                    'ML_enabled' : ML_enabled,
-                    'ML_standard' : ML_standard,
-                    'standard_power' : self.fitting_settings_tab.power_spinbox.value(),
-                    'standard_length_nm' : self.fitting_settings_tab.length_spinbox.value(),
-                    'standard_conductivity_S_m' : self.fitting_settings_tab.conductivity_spinbox.value(),
-                    'standard_voltage_applied_mV' : self.fitting_settings_tab.voltage_spinbox.value(),
-                    'standard_open_pore_current_nA' : self.fitting_settings_tab.open_pore_current_spinbox.value(),
-                    'sampling_rate' : sampling_rate,
-                    'segment_rate_threshold' : self.fitting_settings_tab.segment_rate_threshold_spinbox.value()
+                    chunk_events ,chunk_rolling_avgs ,chunk_rolling_stds ,chunk_data =zip (*results )
+
+
+                    combined_events =[event for chunk_events_tuple in chunk_events for event in chunk_events_tuple ]
+                    rolling_avg_refined =np .concatenate (chunk_rolling_avgs )
+                    rolling_std_refined =np .concatenate (chunk_rolling_stds )
+                    data =np .concatenate (chunk_data )
+
+
+                    adjusted_events =[]
+                    for chunk_index ,chunk_events_tuple in enumerate (chunk_events ):
+                        chunk_start_index =chunk_index *chunk_size *step 
+                        for event in chunk_events_tuple :
+                            start ,end =event 
+                            if start +chunk_start_index <(chunk_index +1 )*chunk_size *step and end +chunk_start_index <=min ((chunk_index +1 )*chunk_size *step ,signal_size ):
+                                adjusted_events .append ((start +chunk_start_index ,end +chunk_start_index ))
+
+                    if threshold_method =="multiplier":
+                        if dips =="Yes":
+                            rolling_threshold_refined =rolling_avg_refined -(threshold_multiplier *rolling_std_refined )
+                        else :
+                            rolling_threshold_refined =rolling_avg_refined +(threshold_multiplier *rolling_std_refined )
+                    elif threshold_method =="difference":
+                        if dips =="Yes":
+                            rolling_threshold_refined =rolling_avg_refined -(threshold_difference /1000 )
+                        else :
+                            rolling_threshold_refined =rolling_avg_refined +(threshold_difference /1000 )
+
+                    if self .event_settings_tab .enable_std_smoothing_checkbox .isChecked ():
+                        rolling_threshold_refined =smooth_threshold (rolling_threshold_refined ,int ((std_window_size_in_ms /1000 )*sampling_rate ),self .event_settings_tab .smoothing_type_dropdown .currentIndex ())
+
+                    events =adjusted_events 
+                    end_time =time .time ()
+                    time_taken =end_time -start_time 
+
+                elif file_path .endswith ('.hdf5')or file_path .endswith ('.h5'):
+                    msg =QMessageBox ()
+                    msg .setIcon (QMessageBox .Icon .Critical )
+                    msg .setWindowTitle ("Error")
+                    msg .setText ("An error has occurred.")
+                    msg .setInformativeText (f"Loading of hdf5 files has not yet been implemented with window processing. Please use the normal processing methods.")
+                    msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+                    msg .exec ()
+
+            else :
+                if file_path .endswith ('.abf'):
+
+                    length_in_seconds ,sampling_rate =get_abf_file_info (file_path )
+
+                    if self .event_settings_tab .enable_nth_data_point_loading .isChecked ():
+                        data ,sampling_rate =load_abf_file_nth (file_path ,self .event_settings_tab .nth_data_point_spinbox .value ())
+                    else :
+                        data ,sampling_rate =load_abf_file (file_path )
+                elif file_path .endswith ('.hdf5')or file_path .endswith ('.h5'):
+                    data ,sampling_rate =load_hdf5_file (file_path )
+                    length_in_seconds =len (data )/sampling_rate 
+
+                if data is not None :
+
+
+                    start_testing_duration =self .load_options_tab .testing_duration_start_spinbox .value ()
+                    end_testing_duration =self .load_options_tab .testing_duration_end_spinbox .value ()
+                    start_points =int (start_testing_duration *sampling_rate )
+                    end_points =int (end_testing_duration *sampling_rate )
+
+                    data =data [start_points :end_points ]
+
+
+                    self .event_settings_tab .sampling_rate_spinbox .setValue (sampling_rate /1000 )
+                    self .event_settings_tab .analysis_end_duration_spinbox .setValue (length_in_seconds )
+                    self .event_settings_tab .analysis_end_duration_spinbox .setMaximum (length_in_seconds )
+                    self .load_options_tab .testing_duration_end_spinbox .setMaximum (length_in_seconds )
+
+                    if self .event_settings_tab .apply_filter_combo .currentText ()=="Yes":
+                        if self .event_settings_tab .filter_type_combo .currentText ()=="Wavelet":
+                            data =apply_low_pass_filter (data ,10000 ,"Wavelet",sampling_rate )
+                        else :
+                            data =apply_low_pass_filter (data ,self .event_settings_tab .cutoff_frequency_spinbox .value ()*1000 ,self .event_settings_tab .low_pass_filter_type_combo .currentText (),sampling_rate )
+                    if self .event_settings_tab .type_of_threshold_combo .currentText ()=="ΔI":
+                        threshold_method ="difference"
+                    else :
+                        threshold_method ="multiplier"
+                    if self .event_settings_tab .dips_or_peaks_combo .currentText ()=="Dips":
+                        dips ="Yes"
+                    else :
+                        dips ="Yes"
+                        data_sent =ne .evaluate ("data*(-1)")
+                    if self .event_settings_tab .enable_std_smoothing_checkbox .isChecked ():
+                        enable_smoothing ="Yes"
+                    else :
+                        enable_smoothing ="No"
+                    try :
+                        if self .event_settings_tab .dips_or_peaks_combo .currentText ()=="Dips":
+                            events ,rolling_avg_refined ,rolling_threshold_refined =find_events_refined_parallel (data ,self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .start_of_event_threshold_spinbox .value (),self .event_settings_tab .end_of_event_threshold_spinbox .value (),self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .mean_window_size_spinbox .value (),self .event_settings_tab .std_window_size_spinbox .value (),threshold_method ,self .event_settings_tab .minimum_event_width_spinbox .value ()/1000 ,self .event_settings_tab .maximum_event_width_spinbox .value ()/1000 ,self .fitting_settings_tab .chunk_size_for_event_detection_spinbox .value (),dips ,sampling_rate ,enable_smoothing ,self .event_settings_tab .smoothing_type_dropdown .currentIndex (),n_jobs =-1 )
+                        else :
+                            events ,rolling_avg_refined ,rolling_threshold_refined =find_events_refined_parallel (data_sent ,self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .start_of_event_threshold_spinbox .value (),self .event_settings_tab .end_of_event_threshold_spinbox .value (),self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .mean_window_size_spinbox .value (),self .event_settings_tab .std_window_size_spinbox .value (),threshold_method ,self .event_settings_tab .minimum_event_width_spinbox .value ()/1000 ,self .event_settings_tab .maximum_event_width_spinbox .value ()/1000 ,self .fitting_settings_tab .chunk_size_for_event_detection_spinbox .value (),dips ,sampling_rate ,enable_smoothing ,self .event_settings_tab .smoothing_type_dropdown .currentIndex (),n_jobs =-1 )
+                        end_time =time .time ()
+                        time_taken =end_time -start_time 
+
+                        if self .event_settings_tab .dips_or_peaks_combo .currentText ()!="Dips":
+                            rolling_avg_refined ,rolling_threshold_refined =ne .evaluate ("rolling_avg_refined*-1"),ne .evaluate ("rolling_threshold_refined *-1")
+                    except :
+                        msg =QMessageBox ()
+                        msg .setIcon (QMessageBox .Icon .Critical )
+                        msg .setWindowTitle ("Error")
+                        msg .setText ("An error has occurred.")
+                        msg .setInformativeText (f"I cannot extract any events from the selected file ({file_path}) within the selected duration. \nContact shankar.dutt@anu.edu.au")
+                        msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+                        msg .exec ()
+
+
+            self .update_file_info (file_path ,length_in_seconds ,len (events ),time_taken ,file_path ,test ="True")
+
+            self .plot_events (events ,data ,rolling_avg_refined ,rolling_threshold_refined ,sampling_rate )
+
+            if self .load_options_tab .level_fitting_combo .currentText ()=="Yes":
+
+                if self .fitting_settings_tab .enable_standardisation_checkbox .isChecked ():
+                    standard =self .fitting_settings_tab .standardisation_type_combo .currentText ()
+                else :
+                    standard ="Normal"
+                if self .ml_tab .enable_ml_data_reduction_checkbox .isChecked ():
+                    ML_enabled ="True"
+                    ML_tag =self .ml_tab .tag_lineedit .text ()
+                    ML_standard =self .ml_tab .data_reduction_type_combo .currentText ()
+                    if self .ml_tab .apply_standardisation_checkbox .isChecked ():
+                        if self .fitting_settings_tab .enable_standardisation_checkbox .isChecked ():
+                            standard =self .fitting_settings_tab .standardisation_type_combo .currentText ()
+                    else :
+                        standard ="Normal"
+                else :
+                    ML_enabled ="False"
+                    ML_standard =None 
+                    ML_tag =None 
+
+                ML_standardisation_settings ={
+                'standard':standard ,
+                'ML_enabled':ML_enabled ,
+                'ML_standard':ML_standard ,
+                'standard_power':self .fitting_settings_tab .power_spinbox .value (),
+                'standard_length_nm':self .fitting_settings_tab .length_spinbox .value (),
+                'standard_conductivity_S_m':self .fitting_settings_tab .conductivity_spinbox .value (),
+                'standard_voltage_applied_mV':self .fitting_settings_tab .voltage_spinbox .value (),
+                'standard_open_pore_current_nA':self .fitting_settings_tab .open_pore_current_spinbox .value (),
+                'sampling_rate':sampling_rate ,
+                'segment_rate_threshold':self .fitting_settings_tab .segment_rate_threshold_spinbox .value ()
                 }
 
-                if self.event_settings_tab.dips_or_peaks_combo.currentText()=="Dips":
-                    self.npz_dict, event_analysis_array = multi_level_fitting_events(self.fitting_settings_tab.padding_spinbox.value(), self.fitting_settings_tab.chunk_size_for_event_fitting_spinbox.value(),self.fitting_settings_tab.library_combo.currentText(),self.fitting_settings_tab.model_combo.currentText(),self.fitting_settings_tab.num_components_spinbox.value(), self.fitting_settings_tab.threshold_spinbox.value(), data, events, dips,ML_standardisation_settings)
-                else:
-                    self.npz_dict, event_analysis_array = multi_level_fitting_events(self.fitting_settings_tab.padding_spinbox.value(), self.fitting_settings_tab.chunk_size_for_event_fitting_spinbox.value(),self.fitting_settings_tab.library_combo.currentText(),self.fitting_settings_tab.model_combo.currentText(),self.fitting_settings_tab.num_components_spinbox.value(), self.fitting_settings_tab.threshold_spinbox.value(), data_sent, events, dips,ML_standardisation_settings)
-                X =[np.array(sublist, dtype=np.float64) for sublist in event_analysis_array]
-                if len(self.npz_dict)>10:
-                    self.total_events = len(self.npz_dict) // 10  
-                    self.jump_to_spinbox.setMaximum(self.total_events - 1)
-                    self.jump_to_spinbox.setValue(0)
-                    self.current_event_index = 0
-                    self.plot_event(0)
-                    self.update_event_info_table(0)
-
-
-    def process_single_file(self,file_path):
-        start_time = time.time()
-        if file_path.endswith('.abf'):
-            #Load the sampling rate and length of the file in seconds
-            length_in_seconds,sampling_rate = get_abf_file_info(file_path)
-            if self.event_settings_tab.enable_nth_data_point_loading.isChecked():
-                data, sampling_rate = load_abf_file_nth(file_path,self.event_settings_tab.nth_data_point_spinbox.value())
-            else:
-                data, sampling_rate = load_abf_file(file_path)
-        elif file_path.endswith('.hdf5') or file_path.endswith('.h5'):
-            data,sampling_rate = load_hdf5_file(file_path)
-            length_in_seconds = len(data)/sampling_rate
-
-        if data is not None:
-            if self.event_settings_tab.analysis_start_duration_spinbox.value() > 0:
-                if self.event_settings_tab.enable_analysis_time_specific.isChecked():
-                    start_testing_duration = self.event_settings_tab.analysis_start_duration_spinbox.value()
-                    start_points = int(start_testing_duration * sampling_rate)
-                else:
-                    start_testing_duration = 0
-                    start_points = 0
-            else:
-                start_testing_duration = 0
-                start_points = 0
-            if self.event_settings_tab.analysis_end_duration_spinbox.value() > 0:
-                if self.event_settings_tab.enable_analysis_time_specific.isChecked():
-                    end_testing_duration = self.event_settings_tab.analysis_end_duration_spinbox.value()
-                    end_points = int(end_testing_duration * sampling_rate)
-                else:
-                    end_testing_duration = length_in_seconds
-                    end_points = int(end_testing_duration * sampling_rate)
-            else:
-                end_points = int(length_in_seconds * sampling_rate)
-                end_testing_duration = length_in_seconds
-
-            # Take the slice of data 
-            data = data[start_points:end_points]
-
-            #Update the EventSettingsTab with the sampling rate and file duration
-            self.event_settings_tab.sampling_rate_spinbox.setValue(sampling_rate / 1000)  # Convert to kHz
-            self.event_settings_tab.analysis_end_duration_spinbox.setMaximum(length_in_seconds)
-            self.load_options_tab.testing_duration_end_spinbox.setMaximum(length_in_seconds)
-            file_duration = length_in_seconds
-
-            if self.event_settings_tab.apply_filter_combo.currentText() == "Yes":
-                if self.event_settings_tab.filter_type_combo.currentText() == "Wavelet":
-                    data = apply_low_pass_filter(data, 10000, "Wavelet",sampling_rate)
-                else:
-                    data = apply_low_pass_filter(data, self.event_settings_tab.cutoff_frequency_spinbox.value()*1000, self.event_settings_tab.low_pass_filter_type_combo.currentText(),sampling_rate)
-            if self.event_settings_tab.type_of_threshold_combo.currentText() == "ΔI":
-                threshold_method = "difference"
-            else:
-                threshold_method = "multiplier"
-            if self.event_settings_tab.dips_or_peaks_combo.currentText()=="Dips":
-                dips = "Yes"
-            else:
-                #dips = "No"
-                dips = "Yes"
-                data = ne.evaluate("data*(-1)")
-            if self.event_settings_tab.enable_std_smoothing_checkbox.isChecked():
-                enable_smoothing = "Yes"
-            else:
-                enable_smoothing = "No"
-            try:
-                events,rolling_avg_refined, rolling_threshold_refined = find_events_refined_parallel(data, self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.start_of_event_threshold_spinbox.value(), self.event_settings_tab.end_of_event_threshold_spinbox.value(), self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.mean_window_size_spinbox.value(), self.event_settings_tab.std_window_size_spinbox.value(), threshold_method, self.event_settings_tab.minimum_event_width_spinbox.value()/1000, self.event_settings_tab.maximum_event_width_spinbox.value()/1000, self.fitting_settings_tab.chunk_size_for_event_detection_spinbox.value(), dips, sampling_rate, enable_smoothing, self.event_settings_tab.smoothing_type_dropdown.currentIndex(), n_jobs = -1)
-            except:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Icon.Critical)
-                msg.setWindowTitle("Error")
-                msg.setText("An error has occurred.")
-                msg.setInformativeText(f"I cannot extract any events from the selected file ({file_path}). Change your settings or \nContact shankar.dutt@anu.edu.au")
-                msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-                msg.exec()
-            
-            if len(events)<1:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Icon.Critical)
-                msg.setWindowTitle("No Events Detected!")
-                msg.setText("No Events Detected!")
-                msg.setInformativeText(f"I cannot extract any events from the selected file ({file_path}). Change your settings or \nContact shankar.dutt@anu.edu.au")
-                msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-                msg.exec()
-            else:               
-                if self.load_options_tab.save_event_chk.isChecked():
-                    # Organize the event information
-                    event_info = {
-                        'sampling_rate': sampling_rate,
-                        'events': [],
+                if self .event_settings_tab .dips_or_peaks_combo .currentText ()=="Dips":
+                    self .npz_dict ,event_analysis_array =multi_level_fitting_events (self .fitting_settings_tab .padding_spinbox .value (),self .fitting_settings_tab .chunk_size_for_event_fitting_spinbox .value (),self .fitting_settings_tab .library_combo .currentText (),self .fitting_settings_tab .model_combo .currentText (),self .fitting_settings_tab .num_components_spinbox .value (),self .fitting_settings_tab .threshold_spinbox .value (),data ,events ,dips ,ML_standardisation_settings )
+                else :
+                    self .npz_dict ,event_analysis_array =multi_level_fitting_events (self .fitting_settings_tab .padding_spinbox .value (),self .fitting_settings_tab .chunk_size_for_event_fitting_spinbox .value (),self .fitting_settings_tab .library_combo .currentText (),self .fitting_settings_tab .model_combo .currentText (),self .fitting_settings_tab .num_components_spinbox .value (),self .fitting_settings_tab .threshold_spinbox .value (),data_sent ,events ,dips ,ML_standardisation_settings )
+                X =[np .array (sublist ,dtype =np .float64 )for sublist in event_analysis_array ]
+                if len (self .npz_dict )>10 :
+                    self .total_events =len (self .npz_dict )//10 
+                    self .jump_to_spinbox .setMaximum (self .total_events -1 )
+                    self .jump_to_spinbox .setValue (0 )
+                    self .current_event_index =0 
+                    self .plot_event (0 )
+                    self .update_event_info_table (0 )
+
+
+    def process_single_file (self ,file_path ):
+        start_time =time .time ()
+        if file_path .endswith ('.abf'):
+
+            length_in_seconds ,sampling_rate =get_abf_file_info (file_path )
+            if self .event_settings_tab .enable_nth_data_point_loading .isChecked ():
+                data ,sampling_rate =load_abf_file_nth (file_path ,self .event_settings_tab .nth_data_point_spinbox .value ())
+            else :
+                data ,sampling_rate =load_abf_file (file_path )
+        elif file_path .endswith ('.hdf5')or file_path .endswith ('.h5'):
+            data ,sampling_rate =load_hdf5_file (file_path )
+            length_in_seconds =len (data )/sampling_rate 
+
+        if data is not None :
+            if self .event_settings_tab .analysis_start_duration_spinbox .value ()>0 :
+                if self .event_settings_tab .enable_analysis_time_specific .isChecked ():
+                    start_testing_duration =self .event_settings_tab .analysis_start_duration_spinbox .value ()
+                    start_points =int (start_testing_duration *sampling_rate )
+                else :
+                    start_testing_duration =0 
+                    start_points =0 
+            else :
+                start_testing_duration =0 
+                start_points =0 
+            if self .event_settings_tab .analysis_end_duration_spinbox .value ()>0 :
+                if self .event_settings_tab .enable_analysis_time_specific .isChecked ():
+                    end_testing_duration =self .event_settings_tab .analysis_end_duration_spinbox .value ()
+                    end_points =int (end_testing_duration *sampling_rate )
+                else :
+                    end_testing_duration =length_in_seconds 
+                    end_points =int (end_testing_duration *sampling_rate )
+            else :
+                end_points =int (length_in_seconds *sampling_rate )
+                end_testing_duration =length_in_seconds 
+
+
+            data =data [start_points :end_points ]
+
+
+            self .event_settings_tab .sampling_rate_spinbox .setValue (sampling_rate /1000 )
+            self .event_settings_tab .analysis_end_duration_spinbox .setMaximum (length_in_seconds )
+            self .load_options_tab .testing_duration_end_spinbox .setMaximum (length_in_seconds )
+            file_duration =length_in_seconds 
+
+            if self .event_settings_tab .apply_filter_combo .currentText ()=="Yes":
+                if self .event_settings_tab .filter_type_combo .currentText ()=="Wavelet":
+                    data =apply_low_pass_filter (data ,10000 ,"Wavelet",sampling_rate )
+                else :
+                    data =apply_low_pass_filter (data ,self .event_settings_tab .cutoff_frequency_spinbox .value ()*1000 ,self .event_settings_tab .low_pass_filter_type_combo .currentText (),sampling_rate )
+            if self .event_settings_tab .type_of_threshold_combo .currentText ()=="ΔI":
+                threshold_method ="difference"
+            else :
+                threshold_method ="multiplier"
+            if self .event_settings_tab .dips_or_peaks_combo .currentText ()=="Dips":
+                dips ="Yes"
+            else :
+
+                dips ="Yes"
+                data =ne .evaluate ("data*(-1)")
+            if self .event_settings_tab .enable_std_smoothing_checkbox .isChecked ():
+                enable_smoothing ="Yes"
+            else :
+                enable_smoothing ="No"
+            try :
+                events ,rolling_avg_refined ,rolling_threshold_refined =find_events_refined_parallel (data ,self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .start_of_event_threshold_spinbox .value (),self .event_settings_tab .end_of_event_threshold_spinbox .value (),self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .mean_window_size_spinbox .value (),self .event_settings_tab .std_window_size_spinbox .value (),threshold_method ,self .event_settings_tab .minimum_event_width_spinbox .value ()/1000 ,self .event_settings_tab .maximum_event_width_spinbox .value ()/1000 ,self .fitting_settings_tab .chunk_size_for_event_detection_spinbox .value (),dips ,sampling_rate ,enable_smoothing ,self .event_settings_tab .smoothing_type_dropdown .currentIndex (),n_jobs =-1 )
+            except :
+                msg =QMessageBox ()
+                msg .setIcon (QMessageBox .Icon .Critical )
+                msg .setWindowTitle ("Error")
+                msg .setText ("An error has occurred.")
+                msg .setInformativeText (f"I cannot extract any events from the selected file ({file_path}). Change your settings or \nContact shankar.dutt@anu.edu.au")
+                msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+                msg .exec ()
+
+            if len (events )<1 :
+                msg =QMessageBox ()
+                msg .setIcon (QMessageBox .Icon .Critical )
+                msg .setWindowTitle ("No Events Detected!")
+                msg .setText ("No Events Detected!")
+                msg .setInformativeText (f"I cannot extract any events from the selected file ({file_path}). Change your settings or \nContact shankar.dutt@anu.edu.au")
+                msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+                msg .exec ()
+            else :
+                if self .load_options_tab .save_event_chk .isChecked ():
+
+                    event_info ={
+                    'sampling_rate':sampling_rate ,
+                    'events':[],
                     }
 
-                    for idx, (start, end) in enumerate(events):
-                        event_data = data[start:end]
-                        event_baseline = rolling_avg_refined[start:end]
-                        event_info_data = {
-                            'event_id': idx,
-                            'start_time': start / sampling_rate,
-                            'end_time': end / sampling_rate,
-                            'event_data': event_data-event_baseline,
-                            'baseline_value': np.mean(event_baseline)
+                    for idx ,(start ,end )in enumerate (events ):
+                        event_data =data [start :end ]
+                        event_baseline =rolling_avg_refined [start :end ]
+                        event_info_data ={
+                        'event_id':idx ,
+                        'start_time':start /sampling_rate ,
+                        'end_time':end /sampling_rate ,
+                        'event_data':event_data -event_baseline ,
+                        'baseline_value':np .mean (event_baseline )
                         }
-                        event_info['events'].append(event_info_data)
+                        event_info ['events'].append (event_info_data )
 
-                    date_time_str = datetime.now().strftime("%Y_%m_%d__%H_%M_%S")
-                    if self.save_file_path is not None:
-                        np.savez_compressed(self.save_file_path + '_' + date_time_str + '.event_data', 
-                                            sampling_rate=event_info['sampling_rate'],
-                                            events=event_info['events'])
-                                            
-                    else:
-                        file_path, _ = os.path.splitext(file_path)
-                        np.savez_compressed(file_path + '_' + date_time_str + '.event_data',
-                                            sampling_rate=event_info['sampling_rate'],
-                                            events=event_info['events'])
-                                            
-                    
-                if self.fitting_settings_tab.enable_standardisation_checkbox.isChecked():
-                    standard = self.fitting_settings_tab.standardisation_type_combo.currentText()
-                else:
-                    standard = "Normal"
-                if self.ml_tab.enable_ml_data_reduction_checkbox.isChecked():
-                    ML_enabled = "True"
-                    ML_tag = self.ml_tab.tag_lineedit.text()
-                    ML_standard = self.ml_tab.data_reduction_type_combo.currentText()
-                    if self.ml_tab.apply_standardisation_checkbox.isChecked():
-                        if self.fitting_settings_tab.enable_standardisation_checkbox.isChecked():
-                            standard = self.fitting_settings_tab.standardisation_type_combo.currentText()
-                    else:
-                        standard = "Normal"
-                else:
-                    ML_enabled = "False"
-                    ML_standard = None
-                    ML_tag = None
-
-                ML_standardisation_settings = {
-                    'standard' : standard,
-                    'ML_enabled' : ML_enabled,
-                    'ML_standard' : ML_standard,
-                    'standard_power' : self.fitting_settings_tab.power_spinbox.value(),
-                    'standard_length_nm' : self.fitting_settings_tab.length_spinbox.value(),
-                    'standard_conductivity_S_m' : self.fitting_settings_tab.conductivity_spinbox.value(),
-                    'standard_voltage_applied_mV' : self.fitting_settings_tab.voltage_spinbox.value(),
-                    'standard_open_pore_current_nA' : self.fitting_settings_tab.open_pore_current_spinbox.value(),
-                    'sampling_rate' : sampling_rate,
-                    'segment_rate_threshold' : self.fitting_settings_tab.segment_rate_threshold_spinbox.value()
+                    date_time_str =datetime .now ().strftime ("%Y_%m_%d__%H_%M_%S")
+                    if self .save_file_path is not None :
+                        np .savez_compressed (self .save_file_path +'_'+date_time_str +'.event_data',
+                        sampling_rate =event_info ['sampling_rate'],
+                        events =event_info ['events'])
+
+                    else :
+                        file_path ,_ =os .path .splitext (file_path )
+                        np .savez_compressed (file_path +'_'+date_time_str +'.event_data',
+                        sampling_rate =event_info ['sampling_rate'],
+                        events =event_info ['events'])
+
+
+                if self .fitting_settings_tab .enable_standardisation_checkbox .isChecked ():
+                    standard =self .fitting_settings_tab .standardisation_type_combo .currentText ()
+                else :
+                    standard ="Normal"
+                if self .ml_tab .enable_ml_data_reduction_checkbox .isChecked ():
+                    ML_enabled ="True"
+                    ML_tag =self .ml_tab .tag_lineedit .text ()
+                    ML_standard =self .ml_tab .data_reduction_type_combo .currentText ()
+                    if self .ml_tab .apply_standardisation_checkbox .isChecked ():
+                        if self .fitting_settings_tab .enable_standardisation_checkbox .isChecked ():
+                            standard =self .fitting_settings_tab .standardisation_type_combo .currentText ()
+                    else :
+                        standard ="Normal"
+                else :
+                    ML_enabled ="False"
+                    ML_standard =None 
+                    ML_tag =None 
+
+                ML_standardisation_settings ={
+                'standard':standard ,
+                'ML_enabled':ML_enabled ,
+                'ML_standard':ML_standard ,
+                'standard_power':self .fitting_settings_tab .power_spinbox .value (),
+                'standard_length_nm':self .fitting_settings_tab .length_spinbox .value (),
+                'standard_conductivity_S_m':self .fitting_settings_tab .conductivity_spinbox .value (),
+                'standard_voltage_applied_mV':self .fitting_settings_tab .voltage_spinbox .value (),
+                'standard_open_pore_current_nA':self .fitting_settings_tab .open_pore_current_spinbox .value (),
+                'sampling_rate':sampling_rate ,
+                'segment_rate_threshold':self .fitting_settings_tab .segment_rate_threshold_spinbox .value ()
                 }
 
-                settings = {
-                    "file_name": file_path,
-                    "sampling_rate": sampling_rate,
-                    "start_testing_duration": start_testing_duration,
-                    "end_testing_duration": end_testing_duration,
-                    "threshold_method": threshold_method,
-                    "dips": dips,
-                    "low_pass_filter_applied": self.event_settings_tab.apply_filter_combo.currentText(),
-                    "low_pass_filter_cutoff": self.event_settings_tab.cutoff_frequency_spinbox.value() * 1000,
-                    "low_pass_filter_type": self.event_settings_tab.low_pass_filter_type_combo.currentText(),
-                    "threshold_value_multiplier": self.event_settings_tab.threshold_value_multiplier_spinbox.value(),
-                    "start_of_event_threshold": self.event_settings_tab.start_of_event_threshold_spinbox.value(),
-                    "end_of_event_threshold": self.event_settings_tab.end_of_event_threshold_spinbox.value(),
-                    "mean_window_size": self.event_settings_tab.mean_window_size_spinbox.value(),
-                    "std_window_size": self.event_settings_tab.std_window_size_spinbox.value(),
-                    "minimum_event_width": self.event_settings_tab.minimum_event_width_spinbox.value() / 1000,
-                    "maximum_event_width": self.event_settings_tab.maximum_event_width_spinbox.value() / 1000,
-                    "chunk_size_for_event_detection": self.fitting_settings_tab.chunk_size_for_event_detection_spinbox.value(),
-                    "standard": standard,
-                    "ML_enabled": ML_enabled,
-                    "ML_tag": ML_tag,
-                    "ML_standard": ML_standard,
-                    'standard_power' : self.fitting_settings_tab.power_spinbox.value(),
-                    'standard_length_nm' : self.fitting_settings_tab.length_spinbox.value(),
-                    'standard_conductivity_S_m' : self.fitting_settings_tab.conductivity_spinbox.value(),
-                    'standard_voltage_applied_mV' : self.fitting_settings_tab.voltage_spinbox.value(),
-                    'standard_open_pore_current_nA' : self.fitting_settings_tab.open_pore_current_spinbox.value()
+                settings ={
+                "file_name":file_path ,
+                "sampling_rate":sampling_rate ,
+                "start_testing_duration":start_testing_duration ,
+                "end_testing_duration":end_testing_duration ,
+                "threshold_method":threshold_method ,
+                "dips":dips ,
+                "low_pass_filter_applied":self .event_settings_tab .apply_filter_combo .currentText (),
+                "low_pass_filter_cutoff":self .event_settings_tab .cutoff_frequency_spinbox .value ()*1000 ,
+                "low_pass_filter_type":self .event_settings_tab .low_pass_filter_type_combo .currentText (),
+                "threshold_value_multiplier":self .event_settings_tab .threshold_value_multiplier_spinbox .value (),
+                "start_of_event_threshold":self .event_settings_tab .start_of_event_threshold_spinbox .value (),
+                "end_of_event_threshold":self .event_settings_tab .end_of_event_threshold_spinbox .value (),
+                "mean_window_size":self .event_settings_tab .mean_window_size_spinbox .value (),
+                "std_window_size":self .event_settings_tab .std_window_size_spinbox .value (),
+                "minimum_event_width":self .event_settings_tab .minimum_event_width_spinbox .value ()/1000 ,
+                "maximum_event_width":self .event_settings_tab .maximum_event_width_spinbox .value ()/1000 ,
+                "chunk_size_for_event_detection":self .fitting_settings_tab .chunk_size_for_event_detection_spinbox .value (),
+                "standard":standard ,
+                "ML_enabled":ML_enabled ,
+                "ML_tag":ML_tag ,
+                "ML_standard":ML_standard ,
+                'standard_power':self .fitting_settings_tab .power_spinbox .value (),
+                'standard_length_nm':self .fitting_settings_tab .length_spinbox .value (),
+                'standard_conductivity_S_m':self .fitting_settings_tab .conductivity_spinbox .value (),
+                'standard_voltage_applied_mV':self .fitting_settings_tab .voltage_spinbox .value (),
+                'standard_open_pore_current_nA':self .fitting_settings_tab .open_pore_current_spinbox .value ()
                 }
 
-                # Serialize the settings dictionary to a JSON string
-                settings = json.dumps(settings)
 
-                # Event Fitting
-                if self.load_options_tab.level_fitting_combo.currentText() == "Yes":   
-                    self.npz_dict, event_analysis_array = multi_level_fitting_events(self.fitting_settings_tab.padding_spinbox.value(), self.fitting_settings_tab.chunk_size_for_event_fitting_spinbox.value(),self.fitting_settings_tab.library_combo.currentText(),self.fitting_settings_tab.model_combo.currentText(),self.fitting_settings_tab.num_components_spinbox.value(), self.fitting_settings_tab.threshold_spinbox.value(), data, events, dips, ML_standardisation_settings)
-                    X =[np.array(sublist, dtype=np.float64) for sublist in event_analysis_array]
-                    end_time = time.time()
-                    time_taken = end_time-start_time
-
-                    # Update information
-                    if len(self.npz_dict)>10:
-                        date_time_str = datetime.now().strftime("%Y_%m_%d__%H_%M_%S")
-                        if self.save_file_path is not None:
-                            file_123 = self.save_file_path+'_'+date_time_str
-                            np.savez_compressed(self.save_file_path+'_'+date_time_str+'.event_fitting', **self.npz_dict)
-                            if ML_enabled == "True":
-                                np.savez_compressed(self.save_file_path+'_'+date_time_str+'.MLdataset',settings=settings, X=X)
-                            else:
-                                np.savez_compressed(self.save_file_path+'_'+date_time_str+'.dataset', settings=settings, X=X)
-                        else:
-                            file_path, _ = os.path.splitext(file_path)
-                            file_123 = file_path+'_'+date_time_str
-                            np.savez_compressed(file_path+'_'+date_time_str+'.event_fitting', **self.npz_dict)
-                            if ML_enabled == "True":
-                                np.savez_compressed(file_path+'_'+date_time_str+'.MLdataset',settings=settings, X=X)
-                            else:
-                                np.savez_compressed(file_path+'_'+date_time_str+'.dataset', settings=settings, X=X)
-                        
-                        self.update_file_info(file_path, file_duration, len(events),time_taken, file_123, test = "False")
-                        self.total_events = len(self.npz_dict) // 10  # Assuming 10 parts per event
-                        self.jump_to_spinbox.setMaximum(self.total_events - 1)
-                        self.jump_to_spinbox.setValue(0)
-                        self.current_event_index = 0
-                        self.plot_event(0)
-                        self.update_event_info_table(0)
-                        
-                else:
-                    self.npz_dict = [ ]
-                    X = save_chunked_event_analysis_to_npz(self.fitting_settings_tab.chunk_size_for_peak_fitting_spinbox.value(),data,events, rolling_avg_refined, sampling_rate, ML_standardisation_settings)
-                    date_time_str = datetime.now().strftime("%Y_%m_%d__%H_%M_%S")
-                    if self.save_file_path is not None:
-                        file_123 = self.save_file_path+'_'+date_time_str
-                        if ML_enabled == "True":
-                            np.savez_compressed(self.save_file_path+'_'+date_time_str+'.MLdataset',settings=settings, X=X)
-                        else:
-                            np.savez_compressed(self.save_file_path+'_'+date_time_str+'.dataset', settings=settings, X=X)
-                    else:
-                        file_path, _ = os.path.splitext(file_path)
-                        file_123 = file_path+'_'+date_time_str
-                        if ML_enabled == "True":
-                            np.savez_compressed(file_path+'_'+date_time_str+'.MLdataset',settings=settings, X=X)
-                        else:
-                            np.savez_compressed(file_path+'_'+date_time_str+'.dataset', settings=settings, X=X)
-                    self.jump_to_spinbox.setMaximum(0)
-                    self.jump_to_spinbox.setValue(0)
-                    self.current_event_index = 0
-                    end_time = time.time()
-                    time_taken = end_time-start_time
-                    # Update information
-                    self.update_file_info(file_path, file_duration, len(events),time_taken, file_123, test = "False")
-
-                if self.event_settings_tab.enable_plots.isChecked():
-                    # Assuming X is already defined and populated with your event data as described
-                    
-                    if ML_enabled == "False":
-                        dI = np.array([x[0] for x in X]) 
-                        dt = np.array([x[4] for x in X])*1e3 
-                    else:
-                        if ML_standard == "Scheme 2" or ML_standard == "Scheme 3":
-                            dI = np.array([x[11] for x in X])  
-                            dt = np.array([x[15] for x in X])*1e3 
-                        elif ML_standard == "Scheme 4":
-                            dI = np.array([x[51] for x in X]) 
-                            dt = np.array([x[55] for x in X])*1e3  
-                        else:
-                            dI = np.array([x[0] for x in X]) 
-                            dt = np.array([x[4] for x in X])*1e3 
-
-                    if ML_standard == "Scheme 1" or ML_standard == "Scheme 2" or ML_standard == "Scheme 3" or ML_enabled == "False":
-
-                        dt =  dt[~np.isnan(dI)]
-                        dI =  dI[~np.isnan(dI)]
-                        
-
-                        # Plotting the histogram of dI on the first canvas
-                        self.plot_widgets[0].canvas.axes.clear()  # Clear existing plot
-                        self.plot_widgets[0].canvas.axes.hist(dI, bins=100, color='blue', alpha=0.7)  # Adjust 'bins' as necessary
-                        self.plot_widgets[0].canvas.axes.set_title(f'Histogram of dI | Counts:{len(dI)}')
-                        self.plot_widgets[0].canvas.axes.set_xlabel('dI (nA)')
-                        self.plot_widgets[0].canvas.axes.set_ylabel('Frequency')
-                        self.plot_widgets[0].canvas.draw()  # Redraw the canvas
-
-                        # Save the histogram plot
-                        date_time_str = datetime.now().strftime("%Y%m%d_%H%M%S")
-                        plot_title = f'Histogram of dI | Counts:{len(dI)}'
-                        if self.save_file_path is not None:
-                            filename = f"{self.save_file_path}_dI_{date_time_str}.png"
-                        else:
-                            file_path, _ = os.path.splitext(file_path)
-                            filename = f"{file_path}_dI_{date_time_str}.png"
-                        self.plot_widgets[0].canvas.figure.savefig(filename, dpi=300, transparent=True)
-
-                        # Plotting the scatter plot of dI vs log(dt*1e3) on the second canvas
-                        #log_dt = np.log(np.array(dt) * 1e3)  # Calculate the logarithm of dt*1e3
-                        log_dt = np.log(dt)  # Calculate the logarithm of dt*1e3
-                        self.plot_widgets[1].canvas.axes.clear()
-                        self.plot_widgets[1].canvas.axes.scatter(log_dt, dI, color='red', alpha=0.5, s = 2)  # Plot dI vs. log(dt*1e3)
-                        self.plot_widgets[1].canvas.axes.set_title('Scatter Plot of ΔI vs. log(Δt*1e3)')
-                        self.plot_widgets[1].canvas.axes.set_ylabel('ΔI (nA)')
-                        self.plot_widgets[1].canvas.axes.set_xlabel('log(Δt (ms))')
-                        self.plot_widgets[1].canvas.draw()  
-                        # Save the scatter plot
-                        plot_title = 'Scatter_Plot_of_dI_vs_log_dt'
-                        if self.save_file_path is not None:
-                            filename = f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
-                        else:
-                            file_path, _ = os.path.splitext(file_path)
-                            filename = f"{file_path}_{plot_title}_{date_time_str}.png"
-                        self.plot_widgets[1].canvas.figure.savefig(filename, dpi=300, transparent=True)
-                    
-
-
-                msgBox = QMessageBox()
-                msgBox.setIcon(QMessageBox.Icon.Information)
-                msgBox.setWindowTitle("Success")
-                msgBox.setText("Data Reduction performed successfully!")
-                msgBox.setInformativeText(f"Number of Events Detected: {len(events)}")
-                msgBox.setStandardButtons(QMessageBox.StandardButton.Ok)
-                msgBox.exec()
-    
+                settings =json .dumps (settings )
 
-    def process_multiple_files(self,file_path):
-        start_time = time.time()
-        # Load data and sampling rate from the file
-        #Load the sampling rate and length of the file in seconds
-
-        if file_path.endswith('.abf'):
-
-            length_in_seconds,sampling_rate = get_abf_file_info(file_path)
-            if self.event_settings_tab.enable_nth_data_point_loading.isChecked():
-                data, sampling_rate = load_abf_file_nth(file_path,self.event_settings_tab.nth_data_point_spinbox.value())
-            else:
-                data, sampling_rate = load_abf_file(file_path)
-        elif  file_path.endswith('.hdf5') or file_path.endswith('.h5'):
-                data,sampling_rate = load_hdf5_file(file_path)
-                length_in_seconds = len(data)/sampling_rate
-
-        if data is not None:
-            if self.event_settings_tab.analysis_start_duration_spinbox.value() > 0:
-                if self.event_settings_tab.enable_analysis_time_specific.isChecked():
-                    start_testing_duration = self.event_settings_tab.analysis_start_duration_spinbox.value()
-                    start_points = int(start_testing_duration * sampling_rate)
-                else:
-                    start_testing_duration = 0
-                    start_points = 0
-            else:
-                start_testing_duration = 0
-                start_points = 0
-            if self.event_settings_tab.analysis_end_duration_spinbox.value() > 0:
-                if self.event_settings_tab.enable_analysis_time_specific.isChecked():
-                    end_testing_duration = self.event_settings_tab.analysis_end_duration_spinbox.value()
-                    end_points = int(end_testing_duration * sampling_rate)
-                else:
-                    end_testing_duration = length_in_seconds
-                    end_points = int(end_testing_duration * sampling_rate)
-            else:
-                end_points = int(length_in_seconds * sampling_rate)
-                end_testing_duration = length_in_seconds
-
-            # Take the slice of data 
-            data = data[start_points:end_points]
-
-            #Update the EventSettingsTab with the sampling rate and file duration
-            self.event_settings_tab.sampling_rate_spinbox.setValue(sampling_rate / 1000)  # Convert to kHz
-            self.event_settings_tab.analysis_end_duration_spinbox.setMaximum(length_in_seconds)
-            self.load_options_tab.testing_duration_end_spinbox.setMaximum(length_in_seconds)
-            file_duration = length_in_seconds
-
-            if self.event_settings_tab.apply_filter_combo.currentText() == "Yes":
-                if self.event_settings_tab.filter_type_combo.currentText() == "Wavelet":
-                    data = apply_low_pass_filter(data, 10000, "Wavelet",sampling_rate)
-                else:
-                    data = apply_low_pass_filter(data, self.event_settings_tab.cutoff_frequency_spinbox.value()*1000, self.event_settings_tab.low_pass_filter_type_combo.currentText(),sampling_rate)
-            if self.event_settings_tab.type_of_threshold_combo.currentText() == "ΔI":
-                threshold_method = "difference"
-            else:
-                threshold_method = "multiplier"
-            if self.event_settings_tab.dips_or_peaks_combo.currentText()=="Dips":
-                dips = "Yes"
-            else:
-                dips = "Yes"
-                data = ne.evaluate("data*(-1)")
-                
-            if self.event_settings_tab.enable_std_smoothing_checkbox.isChecked():
-                enable_smoothing = "Yes"
-            else:
-                enable_smoothing = "No"
-            try:
-                events,rolling_avg_refined, rolling_threshold_refined = find_events_refined_parallel(data, self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.start_of_event_threshold_spinbox.value(), self.event_settings_tab.end_of_event_threshold_spinbox.value(), self.event_settings_tab.threshold_value_multiplier_spinbox.value(), self.event_settings_tab.mean_window_size_spinbox.value(), self.event_settings_tab.std_window_size_spinbox.value(), threshold_method, self.event_settings_tab.minimum_event_width_spinbox.value()/1000, self.event_settings_tab.maximum_event_width_spinbox.value()/1000, self.fitting_settings_tab.chunk_size_for_event_detection_spinbox.value(), dips, sampling_rate, enable_smoothing, self.event_settings_tab.smoothing_type_dropdown.currentIndex(), n_jobs = -1)
-            except:
-                pass
-            if self.load_options_tab.save_event_chk.isChecked():
-                # Organize the event information
-                event_info = {
-                    'sampling_rate': sampling_rate,
-                    'events': []
+
+                if self .load_options_tab .level_fitting_combo .currentText ()=="Yes":
+                    self .npz_dict ,event_analysis_array =multi_level_fitting_events (self .fitting_settings_tab .padding_spinbox .value (),self .fitting_settings_tab .chunk_size_for_event_fitting_spinbox .value (),self .fitting_settings_tab .library_combo .currentText (),self .fitting_settings_tab .model_combo .currentText (),self .fitting_settings_tab .num_components_spinbox .value (),self .fitting_settings_tab .threshold_spinbox .value (),data ,events ,dips ,ML_standardisation_settings )
+                    X =[np .array (sublist ,dtype =np .float64 )for sublist in event_analysis_array ]
+                    end_time =time .time ()
+                    time_taken =end_time -start_time 
+
+
+                    if len (self .npz_dict )>10 :
+                        date_time_str =datetime .now ().strftime ("%Y_%m_%d__%H_%M_%S")
+                        if self .save_file_path is not None :
+                            file_123 =self .save_file_path +'_'+date_time_str 
+                            np .savez_compressed (self .save_file_path +'_'+date_time_str +'.event_fitting',**self .npz_dict )
+                            if ML_enabled =="True":
+                                np .savez_compressed (self .save_file_path +'_'+date_time_str +'.MLdataset',settings =settings ,X =X )
+                            else :
+                                np .savez_compressed (self .save_file_path +'_'+date_time_str +'.dataset',settings =settings ,X =X )
+                        else :
+                            file_path ,_ =os .path .splitext (file_path )
+                            file_123 =file_path +'_'+date_time_str 
+                            np .savez_compressed (file_path +'_'+date_time_str +'.event_fitting',**self .npz_dict )
+                            if ML_enabled =="True":
+                                np .savez_compressed (file_path +'_'+date_time_str +'.MLdataset',settings =settings ,X =X )
+                            else :
+                                np .savez_compressed (file_path +'_'+date_time_str +'.dataset',settings =settings ,X =X )
+
+                        self .update_file_info (file_path ,file_duration ,len (events ),time_taken ,file_123 ,test ="False")
+                        self .total_events =len (self .npz_dict )//10 
+                        self .jump_to_spinbox .setMaximum (self .total_events -1 )
+                        self .jump_to_spinbox .setValue (0 )
+                        self .current_event_index =0 
+                        self .plot_event (0 )
+                        self .update_event_info_table (0 )
+
+                else :
+                    self .npz_dict =[]
+                    X =save_chunked_event_analysis_to_npz (self .fitting_settings_tab .chunk_size_for_peak_fitting_spinbox .value (),data ,events ,rolling_avg_refined ,sampling_rate ,ML_standardisation_settings )
+                    date_time_str =datetime .now ().strftime ("%Y_%m_%d__%H_%M_%S")
+                    if self .save_file_path is not None :
+                        file_123 =self .save_file_path +'_'+date_time_str 
+                        if ML_enabled =="True":
+                            np .savez_compressed (self .save_file_path +'_'+date_time_str +'.MLdataset',settings =settings ,X =X )
+                        else :
+                            np .savez_compressed (self .save_file_path +'_'+date_time_str +'.dataset',settings =settings ,X =X )
+                    else :
+                        file_path ,_ =os .path .splitext (file_path )
+                        file_123 =file_path +'_'+date_time_str 
+                        if ML_enabled =="True":
+                            np .savez_compressed (file_path +'_'+date_time_str +'.MLdataset',settings =settings ,X =X )
+                        else :
+                            np .savez_compressed (file_path +'_'+date_time_str +'.dataset',settings =settings ,X =X )
+                    self .jump_to_spinbox .setMaximum (0 )
+                    self .jump_to_spinbox .setValue (0 )
+                    self .current_event_index =0 
+                    end_time =time .time ()
+                    time_taken =end_time -start_time 
+
+                    self .update_file_info (file_path ,file_duration ,len (events ),time_taken ,file_123 ,test ="False")
+
+                if self .event_settings_tab .enable_plots .isChecked ():
+
+
+                    if ML_enabled =="False":
+                        dI =np .array ([x [0 ]for x in X ])
+                        dt =np .array ([x [4 ]for x in X ])*1e3 
+                    else :
+                        if ML_standard =="Scheme 2"or ML_standard =="Scheme 3":
+                            dI =np .array ([x [11 ]for x in X ])
+                            dt =np .array ([x [15 ]for x in X ])*1e3 
+                        elif ML_standard =="Scheme 4":
+                            dI =np .array ([x [51 ]for x in X ])
+                            dt =np .array ([x [55 ]for x in X ])*1e3 
+                        else :
+                            dI =np .array ([x [0 ]for x in X ])
+                            dt =np .array ([x [4 ]for x in X ])*1e3 
+
+                    if ML_standard =="Scheme 1"or ML_standard =="Scheme 2"or ML_standard =="Scheme 3"or ML_enabled =="False":
+
+                        dt =dt [~np .isnan (dI )]
+                        dI =dI [~np .isnan (dI )]
+
+
+
+                        self .plot_widgets [0 ].canvas .axes .clear ()
+                        self .plot_widgets [0 ].canvas .axes .hist (dI ,bins =100 ,color ='blue',alpha =0.7 )
+                        self .plot_widgets [0 ].canvas .axes .set_title (f'Histogram of dI | Counts:{len(dI)}')
+                        self .plot_widgets [0 ].canvas .axes .set_xlabel ('dI (nA)')
+                        self .plot_widgets [0 ].canvas .axes .set_ylabel ('Frequency')
+                        self .plot_widgets [0 ].canvas .draw ()
+
+
+                        date_time_str =datetime .now ().strftime ("%Y%m%d_%H%M%S")
+                        plot_title =f'Histogram of dI | Counts:{len(dI)}'
+                        if self .save_file_path is not None :
+                            filename =f"{self.save_file_path}_dI_{date_time_str}.png"
+                        else :
+                            file_path ,_ =os .path .splitext (file_path )
+                            filename =f"{file_path}_dI_{date_time_str}.png"
+                        self .plot_widgets [0 ].canvas .figure .savefig (filename ,dpi =300 ,transparent =True )
+
+
+
+                        log_dt =np .log (dt )
+                        self .plot_widgets [1 ].canvas .axes .clear ()
+                        self .plot_widgets [1 ].canvas .axes .scatter (log_dt ,dI ,color ='red',alpha =0.5 ,s =2 )
+                        self .plot_widgets [1 ].canvas .axes .set_title ('Scatter Plot of ΔI vs. log(Δt*1e3)')
+                        self .plot_widgets [1 ].canvas .axes .set_ylabel ('ΔI (nA)')
+                        self .plot_widgets [1 ].canvas .axes .set_xlabel ('log(Δt (ms))')
+                        self .plot_widgets [1 ].canvas .draw ()
+
+                        plot_title ='Scatter_Plot_of_dI_vs_log_dt'
+                        if self .save_file_path is not None :
+                            filename =f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
+                        else :
+                            file_path ,_ =os .path .splitext (file_path )
+                            filename =f"{file_path}_{plot_title}_{date_time_str}.png"
+                        self .plot_widgets [1 ].canvas .figure .savefig (filename ,dpi =300 ,transparent =True )
+
+
+
+                msgBox =QMessageBox ()
+                msgBox .setIcon (QMessageBox .Icon .Information )
+                msgBox .setWindowTitle ("Success")
+                msgBox .setText ("Data Reduction performed successfully!")
+                msgBox .setInformativeText (f"Number of Events Detected: {len(events)}")
+                msgBox .setStandardButtons (QMessageBox .StandardButton .Ok )
+                msgBox .exec ()
+
+
+    def process_multiple_files (self ,file_path ):
+        start_time =time .time ()
+
+
+
+        if file_path .endswith ('.abf'):
+
+            length_in_seconds ,sampling_rate =get_abf_file_info (file_path )
+            if self .event_settings_tab .enable_nth_data_point_loading .isChecked ():
+                data ,sampling_rate =load_abf_file_nth (file_path ,self .event_settings_tab .nth_data_point_spinbox .value ())
+            else :
+                data ,sampling_rate =load_abf_file (file_path )
+        elif file_path .endswith ('.hdf5')or file_path .endswith ('.h5'):
+                data ,sampling_rate =load_hdf5_file (file_path )
+                length_in_seconds =len (data )/sampling_rate 
+
+        if data is not None :
+            if self .event_settings_tab .analysis_start_duration_spinbox .value ()>0 :
+                if self .event_settings_tab .enable_analysis_time_specific .isChecked ():
+                    start_testing_duration =self .event_settings_tab .analysis_start_duration_spinbox .value ()
+                    start_points =int (start_testing_duration *sampling_rate )
+                else :
+                    start_testing_duration =0 
+                    start_points =0 
+            else :
+                start_testing_duration =0 
+                start_points =0 
+            if self .event_settings_tab .analysis_end_duration_spinbox .value ()>0 :
+                if self .event_settings_tab .enable_analysis_time_specific .isChecked ():
+                    end_testing_duration =self .event_settings_tab .analysis_end_duration_spinbox .value ()
+                    end_points =int (end_testing_duration *sampling_rate )
+                else :
+                    end_testing_duration =length_in_seconds 
+                    end_points =int (end_testing_duration *sampling_rate )
+            else :
+                end_points =int (length_in_seconds *sampling_rate )
+                end_testing_duration =length_in_seconds 
+
+
+            data =data [start_points :end_points ]
+
+
+            self .event_settings_tab .sampling_rate_spinbox .setValue (sampling_rate /1000 )
+            self .event_settings_tab .analysis_end_duration_spinbox .setMaximum (length_in_seconds )
+            self .load_options_tab .testing_duration_end_spinbox .setMaximum (length_in_seconds )
+            file_duration =length_in_seconds 
+
+            if self .event_settings_tab .apply_filter_combo .currentText ()=="Yes":
+                if self .event_settings_tab .filter_type_combo .currentText ()=="Wavelet":
+                    data =apply_low_pass_filter (data ,10000 ,"Wavelet",sampling_rate )
+                else :
+                    data =apply_low_pass_filter (data ,self .event_settings_tab .cutoff_frequency_spinbox .value ()*1000 ,self .event_settings_tab .low_pass_filter_type_combo .currentText (),sampling_rate )
+            if self .event_settings_tab .type_of_threshold_combo .currentText ()=="ΔI":
+                threshold_method ="difference"
+            else :
+                threshold_method ="multiplier"
+            if self .event_settings_tab .dips_or_peaks_combo .currentText ()=="Dips":
+                dips ="Yes"
+            else :
+                dips ="Yes"
+                data =ne .evaluate ("data*(-1)")
+
+            if self .event_settings_tab .enable_std_smoothing_checkbox .isChecked ():
+                enable_smoothing ="Yes"
+            else :
+                enable_smoothing ="No"
+            try :
+                events ,rolling_avg_refined ,rolling_threshold_refined =find_events_refined_parallel (data ,self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .start_of_event_threshold_spinbox .value (),self .event_settings_tab .end_of_event_threshold_spinbox .value (),self .event_settings_tab .threshold_value_multiplier_spinbox .value (),self .event_settings_tab .mean_window_size_spinbox .value (),self .event_settings_tab .std_window_size_spinbox .value (),threshold_method ,self .event_settings_tab .minimum_event_width_spinbox .value ()/1000 ,self .event_settings_tab .maximum_event_width_spinbox .value ()/1000 ,self .fitting_settings_tab .chunk_size_for_event_detection_spinbox .value (),dips ,sampling_rate ,enable_smoothing ,self .event_settings_tab .smoothing_type_dropdown .currentIndex (),n_jobs =-1 )
+            except :
+                pass 
+            if self .load_options_tab .save_event_chk .isChecked ():
+
+                event_info ={
+                'sampling_rate':sampling_rate ,
+                'events':[]
                 }
 
-                for idx, (start, end) in enumerate(events):
-                    event_data = data[start:end]
-                    event_baseline = rolling_avg_refined[start:end]
-                    event_info_data = {
-                        'event_id': idx,
-                        'start_time': start / sampling_rate,
-                        'end_time': end / sampling_rate,
-                        'event_data': event_data,
-                        'baseline_value': np.mean(event_baseline)
+                for idx ,(start ,end )in enumerate (events ):
+                    event_data =data [start :end ]
+                    event_baseline =rolling_avg_refined [start :end ]
+                    event_info_data ={
+                    'event_id':idx ,
+                    'start_time':start /sampling_rate ,
+                    'end_time':end /sampling_rate ,
+                    'event_data':event_data ,
+                    'baseline_value':np .mean (event_baseline )
                     }
-                    event_info['events'].append(event_info_data)
+                    event_info ['events'].append (event_info_data )
 
-                date_time_str = datetime.now().strftime("%Y_%m_%d__%H_%M_%S")
-                if self.save_file_path is not None:
-                    np.savez_compressed(self.save_file_path + '_' + date_time_str + '.event_data', 
-                                        sampling_rate=event_info['sampling_rate'],
-                                        events=event_info['events'])
-                else:
-                    file_path, _ = os.path.splitext(file_path)
-                    np.savez_compressed(file_path + '_' + date_time_str + '.event_data',
-                                        sampling_rate=event_info['sampling_rate'],
-                                        events=event_info['events'])
-            
-            if self.fitting_settings_tab.enable_standardisation_checkbox.isChecked():
-                standard = self.fitting_settings_tab.standardisation_type_combo.currentText()
-            else:
-                standard = "Normal"
-            if self.ml_tab.enable_ml_data_reduction_checkbox.isChecked():
-                ML_enabled = "True"
-                ML_tag = self.ml_tab.tag_lineedit.text()
-                ML_standard = self.ml_tab.data_reduction_type_combo.currentText()
-                if self.ml_tab.apply_standardisation_checkbox.isChecked():
-                    if self.fitting_settings_tab.enable_standardisation_checkbox.isChecked():
-                        standard = self.fitting_settings_tab.standardisation_type_combo.currentText()
-                else:
-                    standard = "Normal"
-            else:
-                ML_enabled = "False"
-                ML_standard = None
-                ML_tag = None
-
-            ML_standardisation_settings = {
-                'standard' : standard,
-                'ML_enabled' : ML_enabled,
-                'ML_standard' : ML_standard,
-                'standard_power' : self.fitting_settings_tab.power_spinbox.value(),
-                'standard_length_nm' : self.fitting_settings_tab.length_spinbox.value(),
-                'standard_conductivity_S_m' : self.fitting_settings_tab.conductivity_spinbox.value(),
-                'standard_voltage_applied_mV' : self.fitting_settings_tab.voltage_spinbox.value(),
-                'standard_open_pore_current_nA' : self.fitting_settings_tab.open_pore_current_spinbox.value(),
-                'sampling_rate' : sampling_rate,
-                'segment_rate_threshold' : self.fitting_settings_tab.segment_rate_threshold_spinbox.value()
+                date_time_str =datetime .now ().strftime ("%Y_%m_%d__%H_%M_%S")
+                if self .save_file_path is not None :
+                    np .savez_compressed (self .save_file_path +'_'+date_time_str +'.event_data',
+                    sampling_rate =event_info ['sampling_rate'],
+                    events =event_info ['events'])
+                else :
+                    file_path ,_ =os .path .splitext (file_path )
+                    np .savez_compressed (file_path +'_'+date_time_str +'.event_data',
+                    sampling_rate =event_info ['sampling_rate'],
+                    events =event_info ['events'])
+
+            if self .fitting_settings_tab .enable_standardisation_checkbox .isChecked ():
+                standard =self .fitting_settings_tab .standardisation_type_combo .currentText ()
+            else :
+                standard ="Normal"
+            if self .ml_tab .enable_ml_data_reduction_checkbox .isChecked ():
+                ML_enabled ="True"
+                ML_tag =self .ml_tab .tag_lineedit .text ()
+                ML_standard =self .ml_tab .data_reduction_type_combo .currentText ()
+                if self .ml_tab .apply_standardisation_checkbox .isChecked ():
+                    if self .fitting_settings_tab .enable_standardisation_checkbox .isChecked ():
+                        standard =self .fitting_settings_tab .standardisation_type_combo .currentText ()
+                else :
+                    standard ="Normal"
+            else :
+                ML_enabled ="False"
+                ML_standard =None 
+                ML_tag =None 
+
+            ML_standardisation_settings ={
+            'standard':standard ,
+            'ML_enabled':ML_enabled ,
+            'ML_standard':ML_standard ,
+            'standard_power':self .fitting_settings_tab .power_spinbox .value (),
+            'standard_length_nm':self .fitting_settings_tab .length_spinbox .value (),
+            'standard_conductivity_S_m':self .fitting_settings_tab .conductivity_spinbox .value (),
+            'standard_voltage_applied_mV':self .fitting_settings_tab .voltage_spinbox .value (),
+            'standard_open_pore_current_nA':self .fitting_settings_tab .open_pore_current_spinbox .value (),
+            'sampling_rate':sampling_rate ,
+            'segment_rate_threshold':self .fitting_settings_tab .segment_rate_threshold_spinbox .value ()
             }
 
-            settings = {
-                "file_name": file_path,
-                "sampling_rate": sampling_rate,
-                "start_testing_duration": start_testing_duration,
-                "end_testing_duration": end_testing_duration,
-                "threshold_method": threshold_method,
-                "dips": dips,
-                "low_pass_filter_applied": self.event_settings_tab.apply_filter_combo.currentText(),
-                "low_pass_filter_cutoff": self.event_settings_tab.cutoff_frequency_spinbox.value() * 1000,
-                "low_pass_filter_type": self.event_settings_tab.low_pass_filter_type_combo.currentText(),
-                "threshold_value_multiplier": self.event_settings_tab.threshold_value_multiplier_spinbox.value(),
-                "start_of_event_threshold": self.event_settings_tab.start_of_event_threshold_spinbox.value(),
-                "end_of_event_threshold": self.event_settings_tab.end_of_event_threshold_spinbox.value(),
-                "mean_window_size": self.event_settings_tab.mean_window_size_spinbox.value(),
-                "std_window_size": self.event_settings_tab.std_window_size_spinbox.value(),
-                "minimum_event_width": self.event_settings_tab.minimum_event_width_spinbox.value() / 1000,
-                "maximum_event_width": self.event_settings_tab.maximum_event_width_spinbox.value() / 1000,
-                "chunk_size_for_event_detection": self.fitting_settings_tab.chunk_size_for_event_detection_spinbox.value(),
-                "standard": standard,
-                "ML_enabled": ML_enabled,
-                "ML_tag": ML_tag,
-                "ML_standard": ML_standard,
-                'standard_power' : self.fitting_settings_tab.power_spinbox.value(),
-                'standard_length_nm' : self.fitting_settings_tab.length_spinbox.value(),
-                'standard_conductivity_S_m' : self.fitting_settings_tab.conductivity_spinbox.value(),
-                'standard_voltage_applied_mV' : self.fitting_settings_tab.voltage_spinbox.value(),
-                'standard_open_pore_current_nA' : self.fitting_settings_tab.open_pore_current_spinbox.value()
+            settings ={
+            "file_name":file_path ,
+            "sampling_rate":sampling_rate ,
+            "start_testing_duration":start_testing_duration ,
+            "end_testing_duration":end_testing_duration ,
+            "threshold_method":threshold_method ,
+            "dips":dips ,
+            "low_pass_filter_applied":self .event_settings_tab .apply_filter_combo .currentText (),
+            "low_pass_filter_cutoff":self .event_settings_tab .cutoff_frequency_spinbox .value ()*1000 ,
+            "low_pass_filter_type":self .event_settings_tab .low_pass_filter_type_combo .currentText (),
+            "threshold_value_multiplier":self .event_settings_tab .threshold_value_multiplier_spinbox .value (),
+            "start_of_event_threshold":self .event_settings_tab .start_of_event_threshold_spinbox .value (),
+            "end_of_event_threshold":self .event_settings_tab .end_of_event_threshold_spinbox .value (),
+            "mean_window_size":self .event_settings_tab .mean_window_size_spinbox .value (),
+            "std_window_size":self .event_settings_tab .std_window_size_spinbox .value (),
+            "minimum_event_width":self .event_settings_tab .minimum_event_width_spinbox .value ()/1000 ,
+            "maximum_event_width":self .event_settings_tab .maximum_event_width_spinbox .value ()/1000 ,
+            "chunk_size_for_event_detection":self .fitting_settings_tab .chunk_size_for_event_detection_spinbox .value (),
+            "standard":standard ,
+            "ML_enabled":ML_enabled ,
+            "ML_tag":ML_tag ,
+            "ML_standard":ML_standard ,
+            'standard_power':self .fitting_settings_tab .power_spinbox .value (),
+            'standard_length_nm':self .fitting_settings_tab .length_spinbox .value (),
+            'standard_conductivity_S_m':self .fitting_settings_tab .conductivity_spinbox .value (),
+            'standard_voltage_applied_mV':self .fitting_settings_tab .voltage_spinbox .value (),
+            'standard_open_pore_current_nA':self .fitting_settings_tab .open_pore_current_spinbox .value ()
             }
 
-            # Serialize the settings dictionary to a JSON string
-            settings = json.dumps(settings)
 
-            # Event Fitting
-            if self.load_options_tab.level_fitting_combo.currentText() == "Yes":    
-                self.npz_dict, event_analysis_array = multi_level_fitting_events(self.fitting_settings_tab.padding_spinbox.value(), self.fitting_settings_tab.chunk_size_for_event_fitting_spinbox.value(),self.fitting_settings_tab.library_combo.currentText(),self.fitting_settings_tab.model_combo.currentText(),self.fitting_settings_tab.num_components_spinbox.value(), self.fitting_settings_tab.threshold_spinbox.value(), data, events, dips, ML_standardisation_settings)
-                X =[np.array(sublist, dtype=np.float64) for sublist in event_analysis_array]
-                end_time = time.time()
-                time_taken = end_time-start_time
-                # Update information
-                if len(self.npz_dict)>10:
-                    date_time_str = datetime.now().strftime("%Y_%m_%d__%H_%M_%S")
-
-                    file_path, _ = os.path.splitext(file_path)
-                    file_123 = file_path+'_'+date_time_str
-                    np.savez_compressed(file_path+'_'+date_time_str+'.event_fitting', **self.npz_dict)
-                    if ML_enabled == "True":
-                        np.savez_compressed(file_path+'_'+date_time_str+'.MLdataset',settings=settings, X=X)
-                    else:
-                        np.savez_compressed(file_path+'_'+date_time_str+'.dataset', settings=settings, X=X)
-                    self.update_file_info(file_path, file_duration, len(events),time_taken, file_123, test = "False")
-                    if self.event_settings_tab.enable_plots.isChecked():
-                        if ML_enabled == "False":
-                            dI = np.array([x[0] for x in X]) 
-                            dt = np.array([x[4] for x in X])*1e3 
-                        else:
-                            if ML_standard == "Scheme 2" or ML_standard == "Scheme 3":
-                                dI = np.array([x[11] for x in X])  
-                                dt = np.array([x[15] for x in X])*1e3 
-                            elif ML_standard == "Scheme 4":
-                                dI = np.array([x[51] for x in X]) 
-                                dt = np.array([x[55] for x in X])*1e3  
-                            else:
-                                dI = np.array([x[0] for x in X]) 
-                                dt = np.array([x[4] for x in X])*1e3 
-
-                        if ML_standard == "Scheme 1" or ML_standard == "Scheme 2" or ML_standard == "Scheme 3" or ML_enabled == "False":
-
-                            dt =  dt[~np.isnan(dI)]
-                            dI =  dI[~np.isnan(dI)]
-                            
-                        
-                            # Plotting the histogram of dI on the first canvas
-                            self.plot_widgets[0].canvas.axes.clear()  # Clear existing plot
-                            self.plot_widgets[0].canvas.axes.hist(dI, bins=100, color='blue', alpha=0.7)  # Adjust 'bins' as necessary
-                            self.plot_widgets[0].canvas.axes.set_title('Histogram of dI')
-                            self.plot_widgets[0].canvas.axes.set_xlabel('dI (nA)')
-                            self.plot_widgets[0].canvas.axes.set_ylabel('Frequency')
-                            self.plot_widgets[0].canvas.draw()  # Redraw the canvas
-
-                            # Save the histogram plot
-                            date_time_str = datetime.now().strftime("%Y%m%d_%H%M%S")
-                            plot_title = 'Histogram_of_dI'
-                            if self.save_file_path is not None:
-                                filename = f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
-                            else:
-                                file_path, _ = os.path.splitext(file_path)
-                                filename = f"{file_path}_{plot_title}_{date_time_str}.png"
-                            self.plot_widgets[0].canvas.figure.savefig(filename, dpi=300, transparent=True)
-
-                            # Plotting the scatter plot of dI vs log(dt*1e3) on the second canvas
-                            #log_dt = np.log(np.array(dt) * 1e3)  # Calculate the logarithm of dt*1e3
-                            log_dt = np.log(dt)  # Calculate the logarithm of dt*1e3
-                            self.plot_widgets[1].canvas.axes.clear()
-                            self.plot_widgets[1].canvas.axes.scatter(log_dt, dI, color='red', alpha=0.5, s = 2)  # Plot dI vs. log(dt*1e3)
-                            self.plot_widgets[1].canvas.axes.set_title('Scatter Plot of ΔI vs. log(Δt*1e3)')
-                            self.plot_widgets[1].canvas.axes.set_ylabel('ΔI (nA)')
-                            self.plot_widgets[1].canvas.axes.set_xlabel('log(Δt (ms))')
-                            self.plot_widgets[1].canvas.draw()  
-                            # Save the scatter plot
-                            plot_title = 'Scatter_Plot_of_dI_vs_log_dt'
-                            if self.save_file_path is not None:
-                                filename = f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
-                            else:
-                                file_path, _ = os.path.splitext(file_path)
-                                filename = f"{file_path}_{plot_title}_{date_time_str}.png"
-                            self.plot_widgets[1].canvas.figure.savefig(filename, dpi=300, transparent=True)
-                    
-                    del self.npz_dict,X
-            else:
-                self.npz_dict = [ ]
-                X = save_chunked_event_analysis_to_npz(self.fitting_settings_tab.chunk_size_for_peak_fitting_spinbox.value(),data,events, rolling_avg_refined, sampling_rate, ML_standardisation_settings)
-                date_time_str = datetime.now().strftime("%Y_%m_%d__%H_%M_%S")
-
-                file_path, _ = os.path.splitext(file_path)
-                file_123 = file_path+'_'+date_time_str
-                if ML_enabled == "True":
-                    np.savez_compressed(file_path+'_'+date_time_str+'.MLdataset',settings=settings, X=X)
-                else:
-                    np.savez_compressed(file_path+'_'+date_time_str+'.dataset', settings=settings, X=X)
-                end_time = time.time()
-                time_taken = end_time-start_time
-                # Update information
-                self.update_file_info(file_path, file_duration, len(events),time_taken, file_123, test = "False")
-                if self.event_settings_tab.enable_plots.isChecked():
-                    # Assuming X is already defined and populated with your event data as described
-                    if ML_enabled == "False":
-                        dI = np.array([x[0] for x in X]) 
-                        dt = np.array([x[4] for x in X])*1e3 
-                    else:
-                        if ML_standard == "Scheme 2" or ML_standard == "Scheme 3":
-                            dI = np.array([x[11] for x in X])  
-                            dt = np.array([x[15] for x in X])*1e3 
-                        elif ML_standard == "Scheme 4":
-                            dI = np.array([x[51] for x in X]) 
-                            dt = np.array([x[55] for x in X])*1e3  
-                        else:
-                            dI = np.array([x[0] for x in X]) 
-                            dt = np.array([x[4] for x in X])*1e3 
-
-                    if ML_standard == "Scheme 1" or ML_standard == "Scheme 2" or ML_standard == "Scheme 3" or ML_enabled == "False":
-
-                        dt =  dt[~np.isnan(dI)]
-                        dI =  dI[~np.isnan(dI)]
-                        
-                    
-                        # Plotting the histogram of dI on the first canvas
-                        self.plot_widgets[0].canvas.axes.clear()  # Clear existing plot
-                        self.plot_widgets[0].canvas.axes.hist(dI, bins=100, color='blue', alpha=0.7)  # Adjust 'bins' as necessary
-                        self.plot_widgets[0].canvas.axes.set_title(f'Histogram of dI | Counts:{len(dI)}')
-                        self.plot_widgets[0].canvas.axes.set_xlabel('dI (nA)')
-                        self.plot_widgets[0].canvas.axes.set_ylabel('Frequency')
-                        self.plot_widgets[0].canvas.draw()  # Redraw the canvas
-
-                        # Save the histogram plot
-                        date_time_str = datetime.now().strftime("%Y%m%d_%H%M%S")
-                        plot_title = f'Histogram of dI | Counts:{len(dI)}'
-                        if self.save_file_path is not None:
-                            filename = f"{self.save_file_path}_dI_{date_time_str}.png"
-                        else:
-                            file_path, _ = os.path.splitext(file_path)
-                            filename = f"{file_path}_dI_{date_time_str}.png"
-                        self.plot_widgets[0].canvas.figure.savefig(filename, dpi=300, transparent=True)
-
-                        # Plotting the scatter plot of dI vs log(dt*1e3) on the second canvas
-                        #log_dt = np.log(np.array(dt) * 1e3)  # Calculate the logarithm of dt*1e3
-                        log_dt = np.log(dt)  # Calculate the logarithm of dt*1e3
-                        self.plot_widgets[1].canvas.axes.clear()
-                        self.plot_widgets[1].canvas.axes.scatter(log_dt, dI, color='red', alpha=0.5, s = 2)  # Plot dI vs. log(dt*1e3)
-                        self.plot_widgets[1].canvas.axes.set_title('Scatter Plot of ΔI vs. log(Δt*1e3)')
-                        self.plot_widgets[1].canvas.axes.set_ylabel('ΔI (nA)')
-                        self.plot_widgets[1].canvas.axes.set_xlabel('log(Δt (ms))')
-                        self.plot_widgets[1].canvas.draw()  
-                        # Save the scatter plot
-                        plot_title = 'Scatter_Plot_of_dI_vs_log_dt'
-                        if self.save_file_path is not None:
-                            filename = f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
-                        else:
-                            file_path, _ = os.path.splitext(file_path)
-                            filename = f"{file_path}_{plot_title}_{date_time_str}.png"
-                        self.plot_widgets[1].canvas.figure.savefig(filename, dpi=300, transparent=True)
-                del X
-            
-            del data
+            settings =json .dumps (settings )
 
-    def on_perform_data_reduction_clicked(self):
 
-        # Get selected items from the list
-        selected_items = self.load_options_tab.files_list_widget.selectedItems()       
-        
-        if selected_items:
-            files = [item.data(Qt.ItemDataRole.UserRole) for item in selected_items]
-            if len(files) > 1:
-                # Show custom dialog for multiple files
-                dialog = ProcessingDialog(self)
-                dialog.show()
-
-                # Process events to ensure the dialog is displayed
-                QApplication.processEvents()
-
-                for  file_path in files:
-                    self.process_multiple_files(file_path)
-                    gc.collect()
-
-                # Close the dialog when done
-                dialog.close()
-
-                msgBox = QMessageBox()
-                msgBox.setIcon(QMessageBox.Icon.Information)
-                msgBox.setWindowTitle("Success")
-                msgBox.setText("Data Reduction performed successfully!")
-                msgBox.setInformativeText(f"Number of Files Processed: {len(files)}\n Due to the fact that multiple files were processed, we are not displaying any events.")
-                msgBox.setStandardButtons(QMessageBox.StandardButton.Ok)
-                msgBox.exec()
-            else:
-                # Show custom dialog for single file
-                dialog = ProcessingDialog(self)
-                dialog.show()
-
-                # Process events to ensure the message box is displayed
-                QApplication.processEvents()
-
-                # Process the single file
-                self.process_single_file(files[0])
-
-                # Close the dialog when done
-                dialog.close()
-                    
-
-    def plot_event(self, event_index):
-        try:
-            # Retrieve event data from your npz_dict using the event_index
-            event_data_key = f'EVENT_DATA_{event_index}'
-            segment_info_key = f'SEGMENT_INFO_{event_index}'
-            #print(self.npz_dict)
-            # Assuming npz_dict is accessible within this scope, or passed as an argument
-            time_points_padded = self.npz_dict[f'{event_data_key}_part_0']
-            padded_event_data = self.npz_dict[f'{event_data_key}_part_1']
-            event_time_start_end = self.npz_dict[f'{event_data_key}_part_2']
-            mean_values_connected_with_baseline = self.npz_dict[f'{event_data_key}_part_3']
-
-            # Clear the current plot
-            self.event_visualization_widget.canvas.figure.clear()
-            ax = self.event_visualization_widget.canvas.figure.add_subplot(111)
-
-            # Plot the event data
-            ax.plot(time_points_padded, padded_event_data, label='Event Data')
-                
-            # Highlight event start and end
-            ax.axvline(x=event_time_start_end[0], color='g', linestyle='--', label='Event Start')
-            ax.axvline(x=event_time_start_end[1], color='g', linestyle='--', label='Event End')
-            
-            # Plot mean values connected with baseline
-            ax.plot(time_points_padded, mean_values_connected_with_baseline, label='Mean Values with Baseline', color='red', linestyle='--')
-            
-            # Set x-axis limits based on the minimum and maximum of the time points
-            ax.set_xlim(min(time_points_padded), max(time_points_padded))
+            if self .load_options_tab .level_fitting_combo .currentText ()=="Yes":
+                self .npz_dict ,event_analysis_array =multi_level_fitting_events (self .fitting_settings_tab .padding_spinbox .value (),self .fitting_settings_tab .chunk_size_for_event_fitting_spinbox .value (),self .fitting_settings_tab .library_combo .currentText (),self .fitting_settings_tab .model_combo .currentText (),self .fitting_settings_tab .num_components_spinbox .value (),self .fitting_settings_tab .threshold_spinbox .value (),data ,events ,dips ,ML_standardisation_settings )
+                X =[np .array (sublist ,dtype =np .float64 )for sublist in event_analysis_array ]
+                end_time =time .time ()
+                time_taken =end_time -start_time 
 
-            self.event_visualization_widget.canvas.figure.tight_layout()
-            self.event_visualization_widget.canvas.draw()
-        except:
-            msg = QMessageBox()
-            msg.setIcon(QMessageBox.Icon.Critical)
-            msg.setWindowTitle("Error")
-            msg.setText("An error has occurred.")
-            msg.setInformativeText(f"No fitted events found!")
-            msg.setStandardButtons(QMessageBox.StandardButton.Ok)
-            msg.exec()
-            
+                if len (self .npz_dict )>10 :
+                    date_time_str =datetime .now ().strftime ("%Y_%m_%d__%H_%M_%S")
 
-    def update_event_info_table(self, event_index):
-        try:
-            segment_info_key = f'SEGMENT_INFO_{event_index}'
-            number_of_segments = int(self.npz_dict[f'{segment_info_key}_number_of_segments'][0])
-            segment_mean_diffs = self.npz_dict[f'{segment_info_key}_segment_mean_diffs']
-            segment_widths_time = self.npz_dict[f'{segment_info_key}_segment_widths_time']
-            event_width = self.npz_dict[f'{segment_info_key}_event_width'][0]
-
-            # Adjust row count to include segments + extra rows for event info
-            self.table_widget.setRowCount(number_of_segments + 3)  # Corrected row count
-            self.table_widget.setColumnCount(3)
-            self.table_widget.setHorizontalHeaderLabels(["Segment #", "ΔI (nA)", "Width (μs)"])
-
-            # Fill segment rows
-            for i in range(number_of_segments):
-                self.table_widget.setItem(i, 0, QTableWidgetItem(str(i + 1)))
-                self.table_widget.setItem(i, 1, QTableWidgetItem(f"{segment_mean_diffs[i]:.3g}"))
-                self.table_widget.setItem(i, 2, QTableWidgetItem(f"{segment_widths_time[i]*1e6:.3g}"))
-
-            # Insert an empty row as a separator
-            # Corrected by removing setSpan, simply leaving an empty row for visual separation
-            separator_index = number_of_segments
-            self.table_widget.setItem(separator_index, 0, QTableWidgetItem(""))
-            self.table_widget.setItem(separator_index, 1, QTableWidgetItem(""))
-            self.table_widget.setItem(separator_index, 2, QTableWidgetItem(""))
-
-            # Event Number Row
-            event_number_index = number_of_segments + 1
-            self.table_widget.setItem(event_number_index, 0, QTableWidgetItem("Event Index"))
-            self.table_widget.setItem(event_number_index, 1, QTableWidgetItem(""))  # Adjust if you want the number in a different column
-            self.table_widget.setItem(event_number_index, 2, QTableWidgetItem(f"{event_index}"))
-
-            # Event Width Row
-            event_width_index = number_of_segments + 2
-            self.table_widget.setItem(event_width_index, 0, QTableWidgetItem("Event Width (μs)"))
-            self.table_widget.setItem(event_width_index, 1, QTableWidgetItem(""))  # Adjust if you want the width in a different column
-            self.table_widget.setItem(event_width_index, 2, QTableWidgetItem(f"{event_width*1e6:.3g}"))
-
-            # Adjusting appearance
-            self.table_widget.resizeColumnsToContents()
-        except:
-            pass
-                  
-       
-    def Plot_Entire_Data(self):
-        selected_items = self.load_options_tab.files_list_widget.selectedItems()
-        if selected_items:
-            # Use only the first selected file
-            file_path = selected_items[0].data(Qt.ItemDataRole.UserRole)
-            if file_path.endswith('.abf'):
-                # Load data and sampling rate from the file
-                if self.event_settings_tab.enable_nth_data_point_loading.isChecked():
-                    data, sampling_rate = load_abf_file_nth(file_path,self.event_settings_tab.nth_data_point_spinbox.value())
-                else:
-                    data, sampling_rate = load_abf_file(file_path)
-            elif  file_path.endswith('.hdf5') or file_path.endswith('.h5'):
-                data,sampling_rate = load_hdf5_file(file_path)
-                length_in_seconds = len(data)/sampling_rate
-            
-            if data is not None:
-                time_axis = np.arange(len(data)) / sampling_rate
+                    file_path ,_ =os .path .splitext (file_path )
+                    file_123 =file_path +'_'+date_time_str 
+                    np .savez_compressed (file_path +'_'+date_time_str +'.event_fitting',**self .npz_dict )
+                    if ML_enabled =="True":
+                        np .savez_compressed (file_path +'_'+date_time_str +'.MLdataset',settings =settings ,X =X )
+                    else :
+                        np .savez_compressed (file_path +'_'+date_time_str +'.dataset',settings =settings ,X =X )
+                    self .update_file_info (file_path ,file_duration ,len (events ),time_taken ,file_123 ,test ="False")
+                    if self .event_settings_tab .enable_plots .isChecked ():
+                        if ML_enabled =="False":
+                            dI =np .array ([x [0 ]for x in X ])
+                            dt =np .array ([x [4 ]for x in X ])*1e3 
+                        else :
+                            if ML_standard =="Scheme 2"or ML_standard =="Scheme 3":
+                                dI =np .array ([x [11 ]for x in X ])
+                                dt =np .array ([x [15 ]for x in X ])*1e3 
+                            elif ML_standard =="Scheme 4":
+                                dI =np .array ([x [51 ]for x in X ])
+                                dt =np .array ([x [55 ]for x in X ])*1e3 
+                            else :
+                                dI =np .array ([x [0 ]for x in X ])
+                                dt =np .array ([x [4 ]for x in X ])*1e3 
+
+                        if ML_standard =="Scheme 1"or ML_standard =="Scheme 2"or ML_standard =="Scheme 3"or ML_enabled =="False":
+
+                            dt =dt [~np .isnan (dI )]
+                            dI =dI [~np .isnan (dI )]
+
+
+
+                            self .plot_widgets [0 ].canvas .axes .clear ()
+                            self .plot_widgets [0 ].canvas .axes .hist (dI ,bins =100 ,color ='blue',alpha =0.7 )
+                            self .plot_widgets [0 ].canvas .axes .set_title ('Histogram of dI')
+                            self .plot_widgets [0 ].canvas .axes .set_xlabel ('dI (nA)')
+                            self .plot_widgets [0 ].canvas .axes .set_ylabel ('Frequency')
+                            self .plot_widgets [0 ].canvas .draw ()
+
+
+                            date_time_str =datetime .now ().strftime ("%Y%m%d_%H%M%S")
+                            plot_title ='Histogram_of_dI'
+                            if self .save_file_path is not None :
+                                filename =f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
+                            else :
+                                file_path ,_ =os .path .splitext (file_path )
+                                filename =f"{file_path}_{plot_title}_{date_time_str}.png"
+                            self .plot_widgets [0 ].canvas .figure .savefig (filename ,dpi =300 ,transparent =True )
+
+
+
+                            log_dt =np .log (dt )
+                            self .plot_widgets [1 ].canvas .axes .clear ()
+                            self .plot_widgets [1 ].canvas .axes .scatter (log_dt ,dI ,color ='red',alpha =0.5 ,s =2 )
+                            self .plot_widgets [1 ].canvas .axes .set_title ('Scatter Plot of ΔI vs. log(Δt*1e3)')
+                            self .plot_widgets [1 ].canvas .axes .set_ylabel ('ΔI (nA)')
+                            self .plot_widgets [1 ].canvas .axes .set_xlabel ('log(Δt (ms))')
+                            self .plot_widgets [1 ].canvas .draw ()
+
+                            plot_title ='Scatter_Plot_of_dI_vs_log_dt'
+                            if self .save_file_path is not None :
+                                filename =f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
+                            else :
+                                file_path ,_ =os .path .splitext (file_path )
+                                filename =f"{file_path}_{plot_title}_{date_time_str}.png"
+                            self .plot_widgets [1 ].canvas .figure .savefig (filename ,dpi =300 ,transparent =True )
+
+                    del self .npz_dict ,X 
+            else :
+                self .npz_dict =[]
+                X =save_chunked_event_analysis_to_npz (self .fitting_settings_tab .chunk_size_for_peak_fitting_spinbox .value (),data ,events ,rolling_avg_refined ,sampling_rate ,ML_standardisation_settings )
+                date_time_str =datetime .now ().strftime ("%Y_%m_%d__%H_%M_%S")
+
+                file_path ,_ =os .path .splitext (file_path )
+                file_123 =file_path +'_'+date_time_str 
+                if ML_enabled =="True":
+                    np .savez_compressed (file_path +'_'+date_time_str +'.MLdataset',settings =settings ,X =X )
+                else :
+                    np .savez_compressed (file_path +'_'+date_time_str +'.dataset',settings =settings ,X =X )
+                end_time =time .time ()
+                time_taken =end_time -start_time 
+
+                self .update_file_info (file_path ,file_duration ,len (events ),time_taken ,file_123 ,test ="False")
+                if self .event_settings_tab .enable_plots .isChecked ():
+
+                    if ML_enabled =="False":
+                        dI =np .array ([x [0 ]for x in X ])
+                        dt =np .array ([x [4 ]for x in X ])*1e3 
+                    else :
+                        if ML_standard =="Scheme 2"or ML_standard =="Scheme 3":
+                            dI =np .array ([x [11 ]for x in X ])
+                            dt =np .array ([x [15 ]for x in X ])*1e3 
+                        elif ML_standard =="Scheme 4":
+                            dI =np .array ([x [51 ]for x in X ])
+                            dt =np .array ([x [55 ]for x in X ])*1e3 
+                        else :
+                            dI =np .array ([x [0 ]for x in X ])
+                            dt =np .array ([x [4 ]for x in X ])*1e3 
+
+                    if ML_standard =="Scheme 1"or ML_standard =="Scheme 2"or ML_standard =="Scheme 3"or ML_enabled =="False":
+
+                        dt =dt [~np .isnan (dI )]
+                        dI =dI [~np .isnan (dI )]
+
+
+
+                        self .plot_widgets [0 ].canvas .axes .clear ()
+                        self .plot_widgets [0 ].canvas .axes .hist (dI ,bins =100 ,color ='blue',alpha =0.7 )
+                        self .plot_widgets [0 ].canvas .axes .set_title (f'Histogram of dI | Counts:{len(dI)}')
+                        self .plot_widgets [0 ].canvas .axes .set_xlabel ('dI (nA)')
+                        self .plot_widgets [0 ].canvas .axes .set_ylabel ('Frequency')
+                        self .plot_widgets [0 ].canvas .draw ()
+
+
+                        date_time_str =datetime .now ().strftime ("%Y%m%d_%H%M%S")
+                        plot_title =f'Histogram of dI | Counts:{len(dI)}'
+                        if self .save_file_path is not None :
+                            filename =f"{self.save_file_path}_dI_{date_time_str}.png"
+                        else :
+                            file_path ,_ =os .path .splitext (file_path )
+                            filename =f"{file_path}_dI_{date_time_str}.png"
+                        self .plot_widgets [0 ].canvas .figure .savefig (filename ,dpi =300 ,transparent =True )
+
+
+
+                        log_dt =np .log (dt )
+                        self .plot_widgets [1 ].canvas .axes .clear ()
+                        self .plot_widgets [1 ].canvas .axes .scatter (log_dt ,dI ,color ='red',alpha =0.5 ,s =2 )
+                        self .plot_widgets [1 ].canvas .axes .set_title ('Scatter Plot of ΔI vs. log(Δt*1e3)')
+                        self .plot_widgets [1 ].canvas .axes .set_ylabel ('ΔI (nA)')
+                        self .plot_widgets [1 ].canvas .axes .set_xlabel ('log(Δt (ms))')
+                        self .plot_widgets [1 ].canvas .draw ()
 
-                if self.event_settings_tab.apply_filter_combo.currentText() == "Yes":
-                    if self.event_settings_tab.filter_type_combo.currentText() == "Wavelet":
-                        data = apply_low_pass_filter(data, 10000, "Wavelet", sampling_rate)
-                    else:
-                        data = apply_low_pass_filter(data, self.event_settings_tab.cutoff_frequency_spinbox.value()*1000, self.event_settings_tab.low_pass_filter_type_combo.currentText(), sampling_rate)
-                
-
-                # Clear the current figure and plot the new data
-                self.data_visualization_widget.canvas.axes.clear()
-                self.data_visualization_widget.canvas.axes.plot(time_axis, data, label='Signal', linewidth=0.5)
-                self.data_visualization_widget.canvas.axes.set_xlabel('Time (s)')
-                self.data_visualization_widget.canvas.axes.set_ylabel('Current (nA)')
-
-                #Adjust Limits
-                self.data_visualization_widget.canvas.axes.set_xlim(min(time_axis), max(time_axis))
-
-                # Adjust layout
-                self.data_visualization_widget.canvas.figure.tight_layout()
-
-                self.data_visualization_widget.canvas.draw()
-
-                self.event_settings_tab.sampling_rate_spinbox.setValue(sampling_rate / 1000)  # Convert to kHz
-
-                file_duration = len(data) / sampling_rate
-
-                self.event_settings_tab.analysis_end_duration_spinbox.setValue(file_duration)
-
-    def plot_events(self, events, data, rolling_avg_refined, rolling_std_refined, sampling_rate):
-        time_axis = np.arange(len(data)) / sampling_rate
-        self.data_visualization_widget.canvas.axes.clear()
-
-        # Plot the main signal
-        self.data_visualization_widget.canvas.axes.plot(time_axis, data, label='Signal', linewidth=0.5)
-        # Plot the rolling average (baseline)
-        self.data_visualization_widget.canvas.axes.plot(time_axis, rolling_avg_refined, label='Baseline', color='orange')
-        # Plot the rolling standard deviation (threshold)
-        self.data_visualization_widget.canvas.axes.plot(time_axis, rolling_std_refined, label='Threshold', color='green', linestyle='--')
-
-        # Highlight events, but limit to the first 20 for performance
-        events_to_highlight = events[:20]  # Only highlight the first 20 events
-        for start, end in events_to_highlight:
-            # Calculate the bottom and height for the rectangle
-            bottom = min(data)
-            height = max(data) - bottom
-            # Add a rectangle patch for the event duration
-            self.data_visualization_widget.canvas.axes.add_patch(patches.Rectangle(
-                (start / sampling_rate, bottom),  # (x, y)
-                (end - start) / sampling_rate,    # width
-                height,                           # height
-                color='yellow', alpha=0.5))       # rectangle color and transparency
-
-        if len(events) > 20:
-            # If more than 20 events, show a message box to the user
-            if not hasattr(self, 'events_message_shown') or not self.events_message_shown:
-                # If more than 20 events and the message hasn't been shown before
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Icon.Information)
-                msg.setText("We are highlighting the first 20 events only for performance reasons.")
-                msg.setInformativeText("Contact shankar.dutt@anu.edu.au for any further changes.")
-                msg.setWindowTitle("Notice")
-
-                # Add a checkbox to the message box for muting future messages
-                mute_checkbox = QCheckBox("Mute future messages")
-                msg.setCheckBox(mute_checkbox)
-
-                msg.exec()
-
-                # Update the flag to indicate that the message has been shown
-                self.events_message_shown = True
-
-                # Check if the user has chosen to mute future messages
-                if mute_checkbox.isChecked():
-                    self.events_message_muted = True
-
-            elif not hasattr(self, 'events_message_muted') or not self.events_message_muted:
-                # If the message has been shown before but not muted
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Icon.Information)
-                msg.setText("We are highlighting the first 20 events only for performance reasons.")
-                msg.setInformativeText("Contact shankar.dutt@anu.edu.au for any further changes.")
-                msg.setWindowTitle("Notice")
-
-                # Add a checkbox to the message box for muting future messages
-                mute_checkbox = QCheckBox("Mute future messages")
-                msg.setCheckBox(mute_checkbox)
-
-                msg.exec()
-
-                # Check if the user has chosen to mute future messages
-                if mute_checkbox.isChecked():
-                    self.events_message_muted = True
-
-        # Set labels and title
-        self.data_visualization_widget.canvas.axes.set_xlabel('Time (s)')
-        self.data_visualization_widget.canvas.axes.set_ylabel('Current (nA)')
-        self.data_visualization_widget.canvas.axes.set_title('Signal with Identified Events')
-        self.data_visualization_widget.canvas.axes.legend(loc='lower right')
-
-        # Set x-axis limits to minimum and maximum of the time axis
-        self.data_visualization_widget.canvas.axes.set_xlim(min(time_axis), max(time_axis))
-
-        # Adjust layout
-        self.data_visualization_widget.canvas.figure.tight_layout()
-
-        # Refresh the canvas to display the updated plot
-        self.data_visualization_widget.canvas.draw()
-
-    def navigate_to_previous_event(self):
-        if self.current_event_index > 0:
-            self.current_event_index -= 1
-            self.plot_event(self.current_event_index)
-            self.update_event_info_table(self.current_event_index)
-        else:
-            QMessageBox.information(self, "Navigation", "Already at the first event.")
-
-    def navigate_to_next_event(self):
-        if self.current_event_index < self.total_events - 1:
-            self.current_event_index += 1
-            self.plot_event(self.current_event_index)
-            self.update_event_info_table(self.current_event_index)
-        else:
-            QMessageBox.information(self, "Navigation", "Already at the last event.")
-
-    def jump_to_event(self):
-        jump_index = self.jump_to_spinbox.value()
-        if 0 <= jump_index < self.total_events:
-            self.current_event_index = jump_index
-            self.plot_event(self.current_event_index)
-            self.update_event_info_table(self.current_event_index)
-        else:
-            QMessageBox.warning(self, "Invalid Event Number", "The specified event number is out of bounds.")
+                        plot_title ='Scatter_Plot_of_dI_vs_log_dt'
+                        if self .save_file_path is not None :
+                            filename =f"{self.save_file_path}_{plot_title}_{date_time_str}.png"
+                        else :
+                            file_path ,_ =os .path .splitext (file_path )
+                            filename =f"{file_path}_{plot_title}_{date_time_str}.png"
+                        self .plot_widgets [1 ].canvas .figure .savefig (filename ,dpi =300 ,transparent =True )
+                del X 
 
+            del data 
 
-    def update_file_info(self, file_name, file_duration, event_count,  time_taken, file_path, test):
+    def on_perform_data_reduction_clicked (self ):
+
+
+        selected_items =self .load_options_tab .files_list_widget .selectedItems ()
+
+        if selected_items :
+            files =[item .data (Qt .ItemDataRole .UserRole )for item in selected_items ]
+            if len (files )>1 :
+
+                dialog =ProcessingDialog (self )
+                dialog .show ()
+
+
+                QApplication .processEvents ()
+
+                for file_path in files :
+                    self .process_multiple_files (file_path )
+                    gc .collect ()
+
+
+                dialog .close ()
+
+                msgBox =QMessageBox ()
+                msgBox .setIcon (QMessageBox .Icon .Information )
+                msgBox .setWindowTitle ("Success")
+                msgBox .setText ("Data Reduction performed successfully!")
+                msgBox .setInformativeText (f"Number of Files Processed: {len(files)}\n Due to the fact that multiple files were processed, we are not displaying any events.")
+                msgBox .setStandardButtons (QMessageBox .StandardButton .Ok )
+                msgBox .exec ()
+            else :
+
+                dialog =ProcessingDialog (self )
+                dialog .show ()
+
+
+                QApplication .processEvents ()
+
+
+                self .process_single_file (files [0 ])
+
+
+                dialog .close ()
+
+
+    def plot_event (self ,event_index ):
+        try :
+
+            event_data_key =f'EVENT_DATA_{event_index}'
+            segment_info_key =f'SEGMENT_INFO_{event_index}'
+
+
+            time_points_padded =self .npz_dict [f'{event_data_key}_part_0']
+            padded_event_data =self .npz_dict [f'{event_data_key}_part_1']
+            event_time_start_end =self .npz_dict [f'{event_data_key}_part_2']
+            mean_values_connected_with_baseline =self .npz_dict [f'{event_data_key}_part_3']
+
+
+            self .event_visualization_widget .canvas .figure .clear ()
+            ax =self .event_visualization_widget .canvas .figure .add_subplot (111 )
+
+
+            ax .plot (time_points_padded ,padded_event_data ,label ='Event Data')
+
+
+            ax .axvline (x =event_time_start_end [0 ],color ='g',linestyle ='--',label ='Event Start')
+            ax .axvline (x =event_time_start_end [1 ],color ='g',linestyle ='--',label ='Event End')
+
+
+            ax .plot (time_points_padded ,mean_values_connected_with_baseline ,label ='Mean Values with Baseline',color ='red',linestyle ='--')
+
+
+            ax .set_xlim (min (time_points_padded ),max (time_points_padded ))
+
+            self .event_visualization_widget .canvas .figure .tight_layout ()
+            self .event_visualization_widget .canvas .draw ()
+        except :
+            msg =QMessageBox ()
+            msg .setIcon (QMessageBox .Icon .Critical )
+            msg .setWindowTitle ("Error")
+            msg .setText ("An error has occurred.")
+            msg .setInformativeText (f"No fitted events found!")
+            msg .setStandardButtons (QMessageBox .StandardButton .Ok )
+            msg .exec ()
+
+
+    def update_event_info_table (self ,event_index ):
+        try :
+            segment_info_key =f'SEGMENT_INFO_{event_index}'
+            number_of_segments =int (self .npz_dict [f'{segment_info_key}_number_of_segments'][0 ])
+            segment_mean_diffs =self .npz_dict [f'{segment_info_key}_segment_mean_diffs']
+            segment_widths_time =self .npz_dict [f'{segment_info_key}_segment_widths_time']
+            event_width =self .npz_dict [f'{segment_info_key}_event_width'][0 ]
+
+
+            self .table_widget .setRowCount (number_of_segments +3 )
+            self .table_widget .setColumnCount (3 )
+            self .table_widget .setHorizontalHeaderLabels (["Segment #","ΔI (nA)","Width (μs)"])
+
+
+            for i in range (number_of_segments ):
+                self .table_widget .setItem (i ,0 ,QTableWidgetItem (str (i +1 )))
+                self .table_widget .setItem (i ,1 ,QTableWidgetItem (f"{segment_mean_diffs[i]:.3g}"))
+                self .table_widget .setItem (i ,2 ,QTableWidgetItem (f"{segment_widths_time[i]*1e6:.3g}"))
+
+
+
+            separator_index =number_of_segments 
+            self .table_widget .setItem (separator_index ,0 ,QTableWidgetItem (""))
+            self .table_widget .setItem (separator_index ,1 ,QTableWidgetItem (""))
+            self .table_widget .setItem (separator_index ,2 ,QTableWidgetItem (""))
+
+
+            event_number_index =number_of_segments +1 
+            self .table_widget .setItem (event_number_index ,0 ,QTableWidgetItem ("Event Index"))
+            self .table_widget .setItem (event_number_index ,1 ,QTableWidgetItem (""))
+            self .table_widget .setItem (event_number_index ,2 ,QTableWidgetItem (f"{event_index}"))
+
+
+            event_width_index =number_of_segments +2 
+            self .table_widget .setItem (event_width_index ,0 ,QTableWidgetItem ("Event Width (μs)"))
+            self .table_widget .setItem (event_width_index ,1 ,QTableWidgetItem (""))
+            self .table_widget .setItem (event_width_index ,2 ,QTableWidgetItem (f"{event_width*1e6:.3g}"))
+
+
+            self .table_widget .resizeColumnsToContents ()
+        except :
+            pass 
+
+
+    def Plot_Entire_Data (self ):
+        selected_items =self .load_options_tab .files_list_widget .selectedItems ()
+        if selected_items :
+
+            file_path =selected_items [0 ].data (Qt .ItemDataRole .UserRole )
+            if file_path .endswith ('.abf'):
+
+                if self .event_settings_tab .enable_nth_data_point_loading .isChecked ():
+                    data ,sampling_rate =load_abf_file_nth (file_path ,self .event_settings_tab .nth_data_point_spinbox .value ())
+                else :
+                    data ,sampling_rate =load_abf_file (file_path )
+            elif file_path .endswith ('.hdf5')or file_path .endswith ('.h5'):
+                data ,sampling_rate =load_hdf5_file (file_path )
+                length_in_seconds =len (data )/sampling_rate 
+
+            if data is not None :
+                time_axis =np .arange (len (data ))/sampling_rate 
+
+                if self .event_settings_tab .apply_filter_combo .currentText ()=="Yes":
+                    if self .event_settings_tab .filter_type_combo .currentText ()=="Wavelet":
+                        data =apply_low_pass_filter (data ,10000 ,"Wavelet",sampling_rate )
+                    else :
+                        data =apply_low_pass_filter (data ,self .event_settings_tab .cutoff_frequency_spinbox .value ()*1000 ,self .event_settings_tab .low_pass_filter_type_combo .currentText (),sampling_rate )
+
+
+
+                self .data_visualization_widget .canvas .axes .clear ()
+                self .data_visualization_widget .canvas .axes .plot (time_axis ,data ,label ='Signal',linewidth =0.5 )
+                self .data_visualization_widget .canvas .axes .set_xlabel ('Time (s)')
+                self .data_visualization_widget .canvas .axes .set_ylabel ('Current (nA)')
+
+
+                self .data_visualization_widget .canvas .axes .set_xlim (min (time_axis ),max (time_axis ))
+
+
+                self .data_visualization_widget .canvas .figure .tight_layout ()
+
+                self .data_visualization_widget .canvas .draw ()
+
+                self .event_settings_tab .sampling_rate_spinbox .setValue (sampling_rate /1000 )
+
+                file_duration =len (data )/sampling_rate 
+
+                self .event_settings_tab .analysis_end_duration_spinbox .setValue (file_duration )
+
+    def plot_events (self ,events ,data ,rolling_avg_refined ,rolling_std_refined ,sampling_rate ):
+        time_axis =np .arange (len (data ))/sampling_rate 
+        self .data_visualization_widget .canvas .axes .clear ()
+
+
+        self .data_visualization_widget .canvas .axes .plot (time_axis ,data ,label ='Signal',linewidth =0.5 )
+
+        self .data_visualization_widget .canvas .axes .plot (time_axis ,rolling_avg_refined ,label ='Baseline',color ='orange')
+
+        self .data_visualization_widget .canvas .axes .plot (time_axis ,rolling_std_refined ,label ='Threshold',color ='green',linestyle ='--')
+
+
+        events_to_highlight =events [:20 ]
+        for start ,end in events_to_highlight :
+
+            bottom =min (data )
+            height =max (data )-bottom 
+
+            self .data_visualization_widget .canvas .axes .add_patch (patches .Rectangle (
+            (start /sampling_rate ,bottom ),
+            (end -start )/sampling_rate ,
+            height ,
+            color ='yellow',alpha =0.5 ))
+
+        if len (events )>20 :
+
+            if not hasattr (self ,'events_message_shown')or not self .events_message_shown :
+
+                msg =QMessageBox ()
+                msg .setIcon (QMessageBox .Icon .Information )
+                msg .setText ("We are highlighting the first 20 events only for performance reasons.")
+                msg .setInformativeText ("Contact shankar.dutt@anu.edu.au for any further changes.")
+                msg .setWindowTitle ("Notice")
+
+
+                mute_checkbox =QCheckBox ("Mute future messages")
+                msg .setCheckBox (mute_checkbox )
+
+                msg .exec ()
+
+
+                self .events_message_shown =True 
+
+
+                if mute_checkbox .isChecked ():
+                    self .events_message_muted =True 
+
+            elif not hasattr (self ,'events_message_muted')or not self .events_message_muted :
+
+                msg =QMessageBox ()
+                msg .setIcon (QMessageBox .Icon .Information )
+                msg .setText ("We are highlighting the first 20 events only for performance reasons.")
+                msg .setInformativeText ("Contact shankar.dutt@anu.edu.au for any further changes.")
+                msg .setWindowTitle ("Notice")
+
+
+                mute_checkbox =QCheckBox ("Mute future messages")
+                msg .setCheckBox (mute_checkbox )
+
+                msg .exec ()
+
+
+                if mute_checkbox .isChecked ():
+                    self .events_message_muted =True 
+
+
+        self .data_visualization_widget .canvas .axes .set_xlabel ('Time (s)')
+        self .data_visualization_widget .canvas .axes .set_ylabel ('Current (nA)')
+        self .data_visualization_widget .canvas .axes .set_title ('Signal with Identified Events')
+        self .data_visualization_widget .canvas .axes .legend (loc ='lower right')
+
+
+        self .data_visualization_widget .canvas .axes .set_xlim (min (time_axis ),max (time_axis ))
+
+
+        self .data_visualization_widget .canvas .figure .tight_layout ()
+
+
+        self .data_visualization_widget .canvas .draw ()
+
+    def navigate_to_previous_event (self ):
+        if self .current_event_index >0 :
+            self .current_event_index -=1 
+            self .plot_event (self .current_event_index )
+            self .update_event_info_table (self .current_event_index )
+        else :
+            QMessageBox .information (self ,"Navigation","Already at the first event.")
+
+    def navigate_to_next_event (self ):
+        if self .current_event_index <self .total_events -1 :
+            self .current_event_index +=1 
+            self .plot_event (self .current_event_index )
+            self .update_event_info_table (self .current_event_index )
+        else :
+            QMessageBox .information (self ,"Navigation","Already at the last event.")
+
+    def jump_to_event (self ):
+        jump_index =self .jump_to_spinbox .value ()
+        if 0 <=jump_index <self .total_events :
+            self .current_event_index =jump_index 
+            self .plot_event (self .current_event_index )
+            self .update_event_info_table (self .current_event_index )
+        else :
+            QMessageBox .warning (self ,"Invalid Event Number","The specified event number is out of bounds.")
+
+
+    def update_file_info (self ,file_name ,file_duration ,event_count ,time_taken ,file_path ,test ):
         """
         Clears the existing content of the event_info_text_edit and updates it 
         with information about the loaded file, its duration, and the number of detected events.
 
         Not clearing it anymore though. We can clear by uncommenting the line below. 
 
         Parameters:
         - file_name: str, name of the loaded file.
         - file_duration: float, duration of the file in seconds.
         - event_count: int, number of detected events.
         """
-        # Clear the existing content
-        # self.event_info_text_edit.clear()
 
-        # Get the current date and time
-        now = datetime.now()
-        date_time_str = now.strftime("%Y-%m-%d %H:%M:%S")
-
-        if test == "True":
-            # Create the information text
-            info_text = (
-                f"TEST SETTINGS ON THE FOLLOWING FILE\n\n"
-                f"File Information:\n\n"
-                f"Path: {file_name}\n\n"
-                f"Duration Analysed: {file_duration:.2f} seconds\n"
-                f"Detected Events: {event_count}\n"
-                f"Date and Time of Analysis: {date_time_str}\n"
-                f"Time taken for Analysis: {round(time_taken, 3)} s\n"
-                f"_________________________________________________________________________________"
+
+
+
+        now =datetime .now ()
+        date_time_str =now .strftime ("%Y-%m-%d %H:%M:%S")
+
+        if test =="True":
+
+            info_text =(
+            f"TEST SETTINGS ON THE FOLLOWING FILE\n\n"
+            f"File Information:\n\n"
+            f"Path: {file_name}\n\n"
+            f"Duration Analysed: {file_duration:.2f} seconds\n"
+            f"Detected Events: {event_count}\n"
+            f"Date and Time of Analysis: {date_time_str}\n"
+            f"Time taken for Analysis: {round(time_taken, 3)} s\n"
+            f"_________________________________________________________________________________"
             )
 
-        else:
-            # Create the information text
-            info_text = (
-                f"File Information:\n\n"
-                f"Path: {file_name}\n\n"
-                f"Duration: {file_duration:.2f} seconds\n"
-                f"Detected Events: {event_count}\n"
-                f"Date and Time of Analysis: {date_time_str}\n"
-                f"Time taken for Analysis: {round(time_taken, 3)} s\n"
-                f"File Saved to: {file_path} \n" 
-                f"_________________________________________________________________________________"
+        else :
+
+            info_text =(
+            f"File Information:\n\n"
+            f"Path: {file_name}\n\n"
+            f"Duration: {file_duration:.2f} seconds\n"
+            f"Detected Events: {event_count}\n"
+            f"Date and Time of Analysis: {date_time_str}\n"
+            f"Time taken for Analysis: {round(time_taken, 3)} s\n"
+            f"File Saved to: {file_path} \n"
+            f"_________________________________________________________________________________"
             )
-                
-       # Ensure the cursor is at the end and append the new information text
-        self.event_info_text_edit.moveCursor(QTextCursor.MoveOperation.End)
-        self.event_info_text_edit.append(info_text)
-
-class MLTab(QWidget):
-    def __init__(self):
-        super().__init__()
-        layout = QVBoxLayout(self)
-        layout.setContentsMargins(0, 0, 0, 0)
-        
-        group = QGroupBox("Data Reduction for ML")
-        group_layout = QFormLayout(group)
-        
-        self.enable_ml_data_reduction_checkbox = QCheckBox("Enable ML Data Reduction")
-        self.enable_ml_data_reduction_checkbox.stateChanged.connect(self.toggle_ml_widgets)
-        group_layout.addRow(self.enable_ml_data_reduction_checkbox)
-        
-        self.tag_label = QLabel("Tag:")
-        self.tag_lineedit = QLineEdit()
-        self.tag_lineedit.setText("BSA")
-        group_layout.addRow(self.tag_label, self.tag_lineedit)
-        
-        self.apply_standardisation_checkbox = QCheckBox("Apply Standardisation?")
-        self.apply_standardisation_checkbox.stateChanged.connect(self.toggle_standardisation_label)
-        group_layout.addRow(self.apply_standardisation_checkbox)
-        
-        self.standardisation_label = QLabel("Please choose standardisation settings in the Fitting Options tab. If not chosen, results may not be correct.")
-        self.standardisation_label.setWordWrap(True)
-        self.standardisation_label.setVisible(False)
-        group_layout.addRow(self.standardisation_label)
-        
-        self.data_reduction_type_label = QLabel("Type of Data Reduction:")
-        self.data_reduction_type_combo = QComboBox()
-        self.data_reduction_type_combo.addItems(["Scheme 1", "Scheme 2", "Scheme 3", "Scheme 4", "Scheme 5"])
-        group_layout.addRow(self.data_reduction_type_label, self.data_reduction_type_combo)
-        
-        self.scheme_table = QTableWidget()
-        self.scheme_table.setRowCount(5)
-        self.scheme_table.setColumnCount(2)
-        self.scheme_table.setHorizontalHeaderLabels(["Feature Extraction Scheme", "Features/Details"])
-        self.scheme_table.setItem(0, 0, QTableWidgetItem("Scheme 1"))
-        self.scheme_table.setItem(0, 1, QTableWidgetItem("Δi1, Δi2, … Δi10, Δt0/10"))
-        self.scheme_table.setItem(1, 0, QTableWidgetItem("Scheme 2"))
-        self.scheme_table.setItem(1, 1, QTableWidgetItem("Δi1, Δi2, … Δi10, Δt0/10, Δtfwhm, area, Δifwhm, Δimax"))
-        self.scheme_table.setItem(2, 0, QTableWidgetItem("Scheme 3"))
-        self.scheme_table.setItem(2, 1, QTableWidgetItem("Δi1, Δi2, … Δi10, Δt0/10, Δtfwhm, area, Δifwhm, Δimax , skew, kurtosis"))
-        self.scheme_table.setItem(3, 0, QTableWidgetItem("Scheme 4"))
-        self.scheme_table.setItem(3, 1, QTableWidgetItem("Δi1, Δi2, … Δi50, Δt0/50, Δtfwhm, area, Δifwhm, Δimax , skew, kurtosis"))
-        self.scheme_table.setItem(4, 0, QTableWidgetItem("Scheme 5"))
-        self.scheme_table.setItem(4, 1, QTableWidgetItem("Full signal, Δtfwhm, area, Δifwhm, Δimax , skew, kurtosis"))
-        self.scheme_table.resizeColumnsToContents()
-        group_layout.addRow(self.scheme_table)
-        
-        layout.addWidget(group)
-        
-        self.ml_widgets = [self.tag_label, self.tag_lineedit, self.apply_standardisation_checkbox, self.data_reduction_type_label, self.data_reduction_type_combo, self.scheme_table]
-        self.toggle_ml_widgets()
-        
-    def toggle_ml_widgets(self):
-        for widget in self.ml_widgets:
-            widget.setVisible(self.enable_ml_data_reduction_checkbox.isChecked())
-        
-    def toggle_standardisation_label(self):
-        self.standardisation_label.setVisible(self.apply_standardisation_checkbox.isChecked())
-        
-
-class LoadOptionsTab(QWidget):
-    def __init__(self):
-        super().__init__()
-        layout = QVBoxLayout(self)
-        layout.setContentsMargins(0, 0, 0, 0)  # Adjust margins as needed
-
-        # Scroll Area Setup
-        scroll_area = QScrollArea()
-        scroll_area.setWidgetResizable(True)
-        scroll_widget = QWidget()
-        scroll_layout = QVBoxLayout(scroll_widget)
-        scroll_layout.setSpacing(10)
-        
-        # Button to select folder
-        self.select_folder_btn = QPushButton("Select Folder")
-        self.select_folder_btn.clicked.connect(self.selectFolder)
-        
-        # Include subfolders checkbox
-        self.include_subfolders_chk = QCheckBox("Include Subfolders")
-        
-        # List widget to display .abf files
-        self.files_list_widget = QListWidget()
-        self.files_list_widget.setSelectionMode(QListWidget.SelectionMode.MultiSelection)
-        
-        # Path display
-        self.folder_path_label = QLabel(" ")
-        self.folder_path_label.setWordWrap(True)
-
-        # Select All checkbox
-        self.select_all_chk = QCheckBox("Select All")
-        self.select_all_chk.stateChanged.connect(self.selectAllFiles)
-        self.select_all_chk.setTristate(False)
-        
-        # Testing duration setup with new layout structure
-        testing_duration_main_layout = QVBoxLayout()  # Main vertical layout for the testing duration section
-
-        # Label for Testing Duration, centered
-        testing_duration_label = QLabel("Testing Duration")
-        testing_duration_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        testing_duration_main_layout.addWidget(testing_duration_label)
-
-        testing_duration_start_layout = QHBoxLayout()
-        start_label = QLabel("Start:")
-        testing_duration_start_layout.addWidget(start_label)  # Add Start label
-
-        self.testing_duration_start_spinbox = QDoubleSpinBox()  # Make it an attribute of the class
-        self.testing_duration_start_spinbox.setRange(0, 1000)  # Example range
-        self.testing_duration_start_spinbox.setValue(0.0)  # Example start value
-        self.testing_duration_start_spinbox.setSuffix(" s")  # Unit
-        testing_duration_start_layout.addWidget(self.testing_duration_start_spinbox)
-
-        # Horizontal layout for End Duration label and spinbox
-        testing_duration_end_layout = QHBoxLayout()
-        end_label = QLabel("End:")
-        testing_duration_end_layout.addWidget(end_label)  # Add End label
-
-        self.testing_duration_end_spinbox = QDoubleSpinBox()  # Make it an attribute of the class
-        self.testing_duration_end_spinbox.setRange(0, 1000)  # Example range
-        self.testing_duration_end_spinbox.setValue(1)  # Example end value
-        self.testing_duration_end_spinbox.setSuffix(" s")  # Unit
-        testing_duration_end_layout.addWidget(self.testing_duration_end_spinbox)
-
-        # Adding the start and end layouts to the main vertical layout
-        testing_duration_main_layout.addLayout(testing_duration_start_layout)
-        testing_duration_main_layout.addLayout(testing_duration_end_layout)
-        
-        # Save Event Data
-        self.save_event_chk = QCheckBox("Save Events individually for Clustering")
-        self.save_event_chk.setTristate(False)
-        testing_duration_main_layout.addWidget(self.save_event_chk)
-
-        # Level Fitting DropDown
-        level_fitting_layout = QHBoxLayout()
-        level_fitting_layout.addWidget(QLabel("Do you want Level Fitting?"))
-        self.level_fitting_combo = QComboBox()
-        self.level_fitting_combo.addItems(["Yes", "No"])
-        self.level_fitting_combo.setCurrentText("No")  # Default to "No"
-        level_fitting_layout.addWidget(self.level_fitting_combo)
-
-
-        self.test_settings_btn = QPushButton("Test Settings on File")
-        #Create the Plot Data button 
-        self.plot_data_btn = QPushButton("Plot Data")
-
-        self.perform_data_reduction_btn = QPushButton("Perform Data Reduction")
-        self.save_file_path_btn = QPushButton("Specify File Name (Saved Data)")
-        
-
-        #Adjust the layout to place the new button to the left of the Test Settings on File button
-        button_layout = QHBoxLayout()  # Create a horizontal layout
-        button_layout.addWidget(self.plot_data_btn)  # Add the Plot Data button first
-        button_layout.addWidget(self.test_settings_btn)  # Then add the Test Settings on File button
-
-
-        #Adjust the layout to place the new button to the left of the Test Settings on File button
-        button_layout_2 = QHBoxLayout()  # Create a horizontal layout
-        button_layout_2.addWidget(self.save_file_path_btn)  # Add the Plot Data button first
-        button_layout_2.addWidget(self.perform_data_reduction_btn)  # Then add the Test Settings on File button
-        
-        # Adding widgets to layout
-        scroll_layout.addWidget(self.select_folder_btn)
-        scroll_layout.addWidget(self.include_subfolders_chk)
-        scroll_layout.addWidget(self.folder_path_label)
-        scroll_layout.addWidget(self.files_list_widget)
-        scroll_layout.addWidget(self.select_all_chk)
-        scroll_layout.addLayout(testing_duration_main_layout)
-        scroll_layout.addLayout(level_fitting_layout)
-        scroll_layout.addLayout(button_layout)
-        scroll_layout.addLayout(button_layout_2)
-        scroll_area.setWidget(scroll_widget)
-        layout.addWidget(scroll_area)
-        
-    def selectFolder(self):
-        options = QFileDialog.Option.ShowDirsOnly
-        directory = QFileDialog.getExistingDirectory(self, "Select Folder", "", options=options)
-        if directory:
-            # Set text with word wrap for long paths
-            self.folder_path_label.setText(f"Selected folder: {directory}")
-            self.populateFileList(directory, self.include_subfolders_chk.isChecked())
-
-    def populateFileList(self, directory, include_subfolders):
-        self.files_list_widget.clear()  # Clear the existing list
-        for root, dirs, files in os.walk(directory):
-            for file in files:
-                if file.endswith('.abf') or file.endswith('.hdf5')or file.endswith('.h5'):
-                    # Get the relative path
-                    rel_path = os.path.relpath(os.path.join(root, file), start=directory)
-                    item = QListWidgetItem(rel_path)  # Create a new QListWidgetItem
-                    item.setData(Qt.ItemDataRole.UserRole, os.path.join(root, file))  # Store the full path
-                    self.files_list_widget.addItem(item)  # Add the item to the list
-            if not include_subfolders:
-                # If we don't want to include subfolders, break after the first iteration
-                break
-
-    def selectAllFiles(self):
-        is_checked = self.select_all_chk.isChecked()  # Directly check if the checkbox is checked
-        for index in range(self.files_list_widget.count()):
-            item = self.files_list_widget.item(index)
-            item.setSelected(is_checked)
-
-class EventSettingsTab(QWidget):
-    def __init__(self):
-        super().__init__()
-        layout = QVBoxLayout(self)
-        layout.setContentsMargins(0, 0, 0, 0)  # Adjust margins as needed
-
-        scroll_area = QScrollArea()
-        scroll_area.setWidgetResizable(True)
-        scroll_widget = QWidget()
-        scroll_layout = QVBoxLayout(scroll_widget)
-        scroll_layout.setSpacing(10)
-        scroll_area.setWidget(scroll_widget)      
-
-        # Group 1: File settings
-        file_settings_group = QGroupBox("File Settings")
-        file_settings_layout = QFormLayout(file_settings_group)
-        self.sampling_rate_spinbox = QDoubleSpinBox()
-        self.sampling_rate_spinbox.setRange(1, 100000)  # 
-        self.sampling_rate_spinbox.setValue(200)  # Default value
-        self.sampling_rate_spinbox.setSuffix(" kHz")  # Unit
-        self.analysis_start_duration_spinbox = QDoubleSpinBox()
-        self.analysis_start_duration_spinbox.setRange(0, 100000)
-        self.analysis_start_duration_spinbox.setValue(0)  # Default value
-        self.analysis_start_duration_spinbox.setSuffix(" s")  # Unit
-        self.analysis_end_duration_spinbox = QDoubleSpinBox()
-        self.analysis_end_duration_spinbox.setRange(0, 100000)
-        self.analysis_end_duration_spinbox.setValue(0)  # Default value
-        self.analysis_end_duration_spinbox.setSuffix(" s")  # Unit
-        self.dips_or_peaks_combo = QComboBox()
-        self.dips_or_peaks_combo.addItems(["Dips","Peaks"])
-        self.dips_or_peaks_combo.setCurrentIndex(0) #Default to "Dips"
-
-        
-
-        self.enable_nth_data_point_loading = QCheckBox("Enable Nth Data Point Loading")
-        self.enable_nth_data_point_loading.stateChanged.connect(self.toggle_nth_data_point_loading_widgets)
-        
-        file_settings_layout.addRow("Sampling Rate:", self.sampling_rate_spinbox)
-        file_settings_layout.addRow("Analysis Start Duration:", self.analysis_start_duration_spinbox)
-        file_settings_layout.addRow("Analysis End Duration:", self.analysis_end_duration_spinbox)
-        file_settings_layout.addRow("Dips or Peaks:", self.dips_or_peaks_combo)
-        self.enable_analysis_time_specific = QCheckBox("Enable Analysis between the time specified above")
-        file_settings_layout.addRow(self.enable_analysis_time_specific)
-        file_settings_layout.addRow(self.enable_nth_data_point_loading)
-        
-    
 
-        self.nth_data_point_spinbox = QDoubleSpinBox()
-        self.nth_data_point_spinbox.setRange(1,1000)
-        self.nth_data_point_spinbox.setValue(10)
-        self.nth_data_point_label = QLabel("Load every nth point:")
-        file_settings_layout.addRow(self.nth_data_point_label,self.nth_data_point_spinbox)
-        self.nth_data_point_loading_widgets = [self.nth_data_point_spinbox,self.nth_data_point_label]
-        self.toggle_nth_data_point_loading_widgets()
-
-
-        self.enable_window_loading = QCheckBox("Enable Window Loading")
-        self.enable_window_loading.stateChanged.connect(self.toggle_window_loading_widgets)
-        file_settings_layout.addRow(self.enable_window_loading)
-        self.window_size_multiple_spinbox = QDoubleSpinBox()
-        self.window_size_multiple_spinbox.setRange(1,1000)
-        self.window_size_multiple_spinbox.setValue(10)
-        self.window_size_multiple_label = QLabel("Multiple of avg/std Window Size(whichever is higher):")
-        file_settings_layout.addRow(self.window_size_multiple_label, self.window_size_multiple_spinbox)
-        self.window_loading_widgets = [self.window_size_multiple_label, self.window_size_multiple_spinbox]
-        self.toggle_window_loading_widgets()
-
-        self.enable_plots = QCheckBox("Enable Plots after Data Reduction")
-        self.enable_plots.setChecked(True)  # Set the checkbox checked by default
-        self.enable_plots.stateChanged.connect(self.toggle_enable_plots_widgets)
-        file_settings_layout.addRow(self.enable_plots)
-        self.enable_plots_label = QLabel("NOTE: This option only works when you reduce single file!")
-        file_settings_layout.addRow(self.enable_plots_label)
-        self.enable_plots_widgets = [self.enable_plots_label]
-        self.toggle_enable_plots_widgets()
-
-        self.save_plots = QCheckBox("Save Plots after Data Reduction")
-        self.save_plots.setChecked(True)  # Set the checkbox checked by default
-        self.save_plots.stateChanged.connect(self.toggle_enable_plots_widgets)
-        file_settings_layout.addRow(self.save_plots)
-        
-
-
-        # Group 2: Low Pass Filter
-        filtering_group = QGroupBox("Filtering Options")
-        filtering_layout = QFormLayout(filtering_group)
-
-        self.apply_filter_combo = QComboBox()
-        self.apply_filter_combo.addItems(["Yes", "No"])
-        self.apply_filter_combo.setCurrentIndex(0)  # Default to "Yes"
-        filtering_layout.addRow("Apply Filter:", self.apply_filter_combo)
-
-        self.filter_type_combo = QComboBox()
-        self.filter_type_combo.addItems(["Low Pass Filter", "Wavelet"])
-        self.filter_type_combo.setCurrentIndex(0)  # Default to "Low Pass Filter"
-        filtering_layout.addRow("Filter Type:", self.filter_type_combo)
-
-        # Labels for additional options
-        self.type_of_low_pass_filter_label = QLabel("Type of Low Pass Filter:")
-        self.low_pass_filter_type_combo = QComboBox()
-        self.low_pass_filter_type_combo.addItems(["Bessel", "Butterworth", "Chebyshev I", "Chebyshev II", "Elliptic", "FIR", "IIR"])
-        self.low_pass_filter_type_combo.setCurrentIndex(1)  # Default to "Butterworth"
-
-        self.cutoff_frequency_label = QLabel("Cutoff Frequency:")
-        self.cutoff_frequency_spinbox = QDoubleSpinBox()
-        self.cutoff_frequency_spinbox.setRange(1, 5000)  # Example range, adjust as needed
-        self.cutoff_frequency_spinbox.setValue(35)
-        self.cutoff_frequency_spinbox.setSuffix(" kHz")
-
-        # Add labels and widgets but hide them initially
-        filtering_layout.addRow(self.type_of_low_pass_filter_label, self.low_pass_filter_type_combo)
-        filtering_layout.addRow(self.cutoff_frequency_label, self.cutoff_frequency_spinbox)
-
-        self.low_pass_filter_type_combo.hide()
-        self.cutoff_frequency_spinbox.hide()
-        self.type_of_low_pass_filter_label.hide()
-        self.cutoff_frequency_label.hide()
-
-        def update_filter_options():
-            # Show or hide low pass filter options based on the filter type selection
-            if self.filter_type_combo.currentText() == "Low Pass Filter":
-                self.low_pass_filter_type_combo.show()
-                self.cutoff_frequency_spinbox.show()
-                self.type_of_low_pass_filter_label.show()
-                self.cutoff_frequency_label.show()
-            else:
-                self.low_pass_filter_type_combo.hide()
-                self.cutoff_frequency_spinbox.hide()
-                self.type_of_low_pass_filter_label.hide()
-                self.cutoff_frequency_label.hide()
-
-        self.filter_type_combo.currentTextChanged.connect(update_filter_options)
-
-        # Initial call to ensure the UI is correctly set up for the default selection
-        update_filter_options()
-
-        # Group 3: Thresholds - Dynamic adjustment for threshold value will be implemented in its handler
-        thresholds_group = QGroupBox("Thresholds")
-        thresholds_layout = QFormLayout(thresholds_group)
-        self.type_of_threshold_combo = QComboBox()
-        self.type_of_threshold_combo.addItems(["ΔI", "std multiplier"])
-        self.type_of_threshold_combo.setCurrentIndex(1)  # Set the second index as default
-        self.threshold_value_multiplier_spinbox = QDoubleSpinBox()
-        # Default values and ranges set dynamically in a handler
-        self.start_of_event_threshold_spinbox = QDoubleSpinBox()
-        self.start_of_event_threshold_spinbox.setValue(0.1)  # Default value
-        self.end_of_event_threshold_spinbox = QDoubleSpinBox()
-        self.end_of_event_threshold_spinbox.setValue(0.1)  # Default value
-        thresholds_layout.addRow("Type of Threshold:", self.type_of_threshold_combo)
-        thresholds_layout.addRow("Threshold Value/Multiplier:", self.threshold_value_multiplier_spinbox)
-        thresholds_layout.addRow("Start of Event Threshold:", self.start_of_event_threshold_spinbox)
-        thresholds_layout.addRow("End of Event Threshold:", self.end_of_event_threshold_spinbox)
-
-        # Handlers for dynamic value adjustments
-        self.type_of_threshold_combo.currentTextChanged.connect(self.updateThresholdValueRange)
-        self.updateThresholdValueRange(self.type_of_threshold_combo.currentText())  # Initial update
-
-        # Group 4: Window Sizes
-        window_sizes_group = QGroupBox("Window Sizes")
-        window_sizes_layout = QFormLayout(window_sizes_group)
-
-        self.mean_window_size_spinbox = QDoubleSpinBox()
-        self.mean_window_size_spinbox.setRange(0.1, 10000)  # Min and max
-        self.mean_window_size_spinbox.setValue(10)  # Default value
-        self.mean_window_size_spinbox.setSuffix(" ms")  # Unit
-
-        self.std_window_size_label = QLabel("Std Window Size:")
-        self.std_window_size_spinbox = QDoubleSpinBox()
-        self.std_window_size_spinbox.setRange(0.1, 10000)  # Min and max
-        self.std_window_size_spinbox.setValue(250)  # Default value
-        self.std_window_size_spinbox.setSuffix(" ms")  # Unit
-
-        self.enable_std_smoothing_checkbox = QCheckBox("Enable Std Smoothing")
-        self.enable_std_smoothing_checkbox.setChecked(False)
-        self.enable_std_smoothing_checkbox.stateChanged.connect(lambda state: self.update_std_smoothing_options(state))
-
-        self.smoothing_type_label = QLabel("Type of smoothing:")
-        self.smoothing_type_dropdown = QComboBox()
-        self.smoothing_type_dropdown.addItems(["Moving Mean Smoothing", "Exponential Smoothing"])
-        self.smoothing_type_dropdown.setCurrentIndex(1)
-
-        window_sizes_layout.addRow("Mean Window Size:", self.mean_window_size_spinbox)
-        window_sizes_layout.addRow(self.std_window_size_label, self.std_window_size_spinbox)
-        window_sizes_layout.addRow(self.enable_std_smoothing_checkbox)
-        window_sizes_layout.addRow(self.smoothing_type_label, self.smoothing_type_dropdown)
-
-        self.smoothing_type_label.setVisible(False)
-        self.smoothing_type_dropdown.setVisible(False)
-
-        # Group 5: Min, Max Event Widths
-        event_widths_group = QGroupBox("Min, Max Event Widths")
-        event_widths_layout = QFormLayout(event_widths_group)
-        self.minimum_event_width_spinbox = QDoubleSpinBox()
-        self.minimum_event_width_spinbox.setRange(0.000001, 100)  # Min and max
-        self.minimum_event_width_spinbox.setDecimals(6)  # Increase precision for small values
-        self.minimum_event_width_spinbox.setValue(0.001)  # Default value
-        self.minimum_event_width_spinbox.setSuffix(" ms")  # Unit
-        self.maximum_event_width_spinbox = QDoubleSpinBox()
-        self.maximum_event_width_spinbox.setRange(1e-3, 10000)  # Min and max
-        self.maximum_event_width_spinbox.setDecimals(6)  # Allow precision for large values
-        self.maximum_event_width_spinbox.setValue(3)  # Default value
-        self.maximum_event_width_spinbox.setSuffix(" ms")  # Unit
-        event_widths_layout.addRow("Minimum Event Width:", self.minimum_event_width_spinbox)
-        event_widths_layout.addRow("Maximum Event Width:", self.maximum_event_width_spinbox)
-
-        # Adjusting layout for all groups to ensure alignment
-        self.adjustGroupLayout(file_settings_group)
-        self.adjustGroupLayout(filtering_group)  # Explicit adjustment might help
-        self.adjustGroupLayout(thresholds_group)
-        self.adjustGroupLayout(window_sizes_group)
-        self.adjustGroupLayout(event_widths_group)
-
-        # Add all groups to the main layout
-        scroll_layout.addWidget(file_settings_group)
-        scroll_layout.addWidget(filtering_group)
-        scroll_layout.addWidget(thresholds_group)
-        scroll_layout.addWidget(window_sizes_group)
-        scroll_layout.addWidget(event_widths_group)
-        layout.addWidget(scroll_area)
-    
-    def update_std_smoothing_options(self, state):
-        if state == 2:
-            self.smoothing_type_label.setVisible(True)
-            self.smoothing_type_dropdown.setVisible(True)
-            self.std_window_size_spinbox.setValue(10)  # Reset to default value
-        else:
-            self.smoothing_type_label.setVisible(False)
-            self.smoothing_type_dropdown.setVisible(False)
-            self.std_window_size_spinbox.setValue(250)  # Reset to default value
-
-    def toggle_nth_data_point_loading_widgets(self):
-        for widget in self.nth_data_point_loading_widgets:
-            widget.setVisible(self.enable_nth_data_point_loading.isChecked())
-    
-    def toggle_window_loading_widgets(self):
-        for widget in self.window_loading_widgets:
-            widget.setVisible(self.enable_window_loading.isChecked())
-
-    def toggle_enable_plots_widgets(self):
-        for widget in self.enable_plots_widgets:
-            widget.setVisible(self.enable_plots.isChecked())
-
-    def updateThresholdValueRange(self, threshold_type):
-        if threshold_type == "ΔI":
-            self.threshold_value_multiplier_spinbox.setRange(100, 20000)
-            self.threshold_value_multiplier_spinbox.setValue(2000)
-            self.threshold_value_multiplier_spinbox.setSuffix(" pA")  # Unit
-        else:  # std multiplier
-            self.threshold_value_multiplier_spinbox.setRange(1, 20)
-            self.threshold_value_multiplier_spinbox.setValue(4)
-            self.threshold_value_multiplier_spinbox.setSuffix(" ")  # Unit
 
-    
-    def adjustGroupLayout(self, group_box):
-        group_box.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Preferred)
-        layout = group_box.layout()
-        if layout:
-            layout.setAlignment(Qt.AlignmentFlag.AlignLeft)  # Align content to the left
-            
-            for i in range(layout.count()):
-                item = layout.itemAt(i).widget()
-                if item:
-                    item.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Fixed)            
-
-class FittingSettingsTab(QWidget):
-    def __init__(self):
-        super().__init__()
-        layout = QVBoxLayout(self)
-        layout.setContentsMargins(0, 0, 0, 0)  # Adjust margins as needed
-
-        scroll_area = QScrollArea()
-        scroll_area.setWidgetResizable(True)
-        scroll_widget = QWidget()
-        scroll_layout = QVBoxLayout(scroll_widget)
-        scroll_layout.setSpacing(10)
-        scroll_area.setWidget(scroll_widget)
-
-        # Setting groups
-        settings_group = QGroupBox("Fitting Settings")
-        settings_layout = QFormLayout(settings_group)
-        scroll_layout.addWidget(settings_group)
-
-        self.padding_spinbox = QSpinBox()
-        self.padding_spinbox.setRange(0, 10000)  # Min and max values
-        self.padding_spinbox.setValue(100)  # Default value
-
-        self.chunk_size_for_event_detection_spinbox = QSpinBox()
-        self.chunk_size_for_event_detection_spinbox.setRange(1, 1000000000)  # Min and max values
-        self.chunk_size_for_event_detection_spinbox.setValue(4000000)  # Default value
-
-        self.chunk_size_for_event_fitting_spinbox = QSpinBox()
-        self.chunk_size_for_event_fitting_spinbox.setRange(1, 100000)  # Min and max values
-        self.chunk_size_for_event_fitting_spinbox.setValue(30)  # Default value
-
-        self.chunk_size_for_peak_fitting_spinbox = QSpinBox()
-        self.chunk_size_for_peak_fitting_spinbox.setRange(1, 100000)  # Min and max values
-        self.chunk_size_for_peak_fitting_spinbox.setValue(30)  # Default value
-
-        self.library_combo = QComboBox()
-        self.library_combo.addItems(["ruptures",  "detecta", "lmfit", "hmm", "gmm"])
-        self.library_combo.currentIndexChanged.connect(self.update_model_combo)
-
-        self.model_combo = QComboBox()
-        self.model_label = QLabel("Model:")
-
-        self.num_components_spinbox = QSpinBox()
-        self.num_components_spinbox.setRange(2, 10)  # Min and max values
-        self.num_components_spinbox.setValue(2)  # Default value
-        self.num_components_label = QLabel("Number of Components:")
-
-        self.threshold_spinbox = QDoubleSpinBox()
-        self.threshold_spinbox.setRange(0.1, 100)  # Min and max values
-        self.threshold_spinbox.setValue(3)  # Default value
-        self.threshold_spinbox.setDecimals(2)  # Allows for fractional thresholds
-
-
-        self.segment_rate_threshold_spinbox = QDoubleSpinBox()
-        self.segment_rate_threshold_spinbox.setRange(0.001, 100)  # Min and max values
-        self.segment_rate_threshold_spinbox.setValue(0.2)  # Default value
-        self.segment_rate_threshold_spinbox.setDecimals(3)  # Allows for fractional thresholds
-
-        settings_layout.addRow("Padding (in number of samples):", self.padding_spinbox)
-        settings_layout.addRow("Chunk Size for Event Detection:", self.chunk_size_for_event_detection_spinbox)
-        settings_layout.addRow("Chunk Size for Event Fitting:", self.chunk_size_for_event_fitting_spinbox)
-        settings_layout.addRow("Chunk Size for Peak Fitting:", self.chunk_size_for_peak_fitting_spinbox)
-        settings_layout.addRow("Library:", self.library_combo)
-        settings_layout.addRow(self.model_label, self.model_combo)
-        settings_layout.addRow(self.num_components_label, self.num_components_spinbox)
-        settings_layout.addRow("Threshold:", self.threshold_spinbox)
-        settings_layout.addRow("Segment Rate Threshold:", self.segment_rate_threshold_spinbox)
-
-        layout.addWidget(scroll_area)
-
-        standardisation_group = QGroupBox("Standardisation during Data Reduction")
-        group_layout = QFormLayout(standardisation_group)
-        scroll_layout.addWidget(standardisation_group)
-
-        self.enable_standardisation_checkbox = QCheckBox("Enable Standardisation")
-        self.enable_standardisation_checkbox.stateChanged.connect(self.toggle_standardisation_widgets)
-        group_layout.addRow(self.enable_standardisation_checkbox)
-
-        self.standardisation_type_label = QLabel("Which Standardisation to use:")
-        self.standardisation_type_combo = QComboBox()
-        self.standardisation_type_combo.addItems(["ΔI/I₀", "(ΔI*I₀)⁰·⁵", "(ΔI*I₀)ᵖᵒʷᵉʳ", "Dutt Standardisation"])
-        self.standardisation_type_combo.currentIndexChanged.connect(self.update_standardisation_explanation)
-        group_layout.addRow(self.standardisation_type_label, self.standardisation_type_combo)
-
-        self.standardisation_explanation_label = QLabel()
-        self.standardisation_explanation_label.setWordWrap(True)
-        group_layout.addRow(self.standardisation_explanation_label)
-
-        self.power_label = QLabel("Power:")
-        self.power_spinbox = QDoubleSpinBox()
-        self.power_spinbox.setRange(0.01, 10)
-        self.power_spinbox.setValue(0.5)
-        self.power_spinbox.setSingleStep(0.01)
-        self.power_label.setVisible(False)
-        self.power_spinbox.setVisible(False)
-        group_layout.addRow(self.power_label, self.power_spinbox)
-
-        self.length_label = QLabel("Length of the nanopore (L) (nm):")
-        self.length_spinbox = QDoubleSpinBox()
-        self.length_spinbox.setRange(1, 100)
-        self.length_spinbox.setValue(7)
-        self.length_spinbox.setSingleStep(0.1)
-        self.length_label.setVisible(False)
-        self.length_spinbox.setVisible(False)
-        group_layout.addRow(self.length_label, self.length_spinbox)
-
-        self.conductivity_label = QLabel("σ (Conductivity of the solution) (S/m):")
-        self.conductivity_spinbox = QDoubleSpinBox()
-        self.conductivity_spinbox.setRange(0.1, 100)
-        self.conductivity_spinbox.setValue(10.5)
-        self.conductivity_spinbox.setSingleStep(0.1)
-        self.conductivity_label.setVisible(False)
-        self.conductivity_spinbox.setVisible(False)
-        group_layout.addRow(self.conductivity_label, self.conductivity_spinbox)
-
-        self.voltage_label = QLabel("V (Voltage Applied) (mV):")
-        self.voltage_spinbox = QDoubleSpinBox()
-        self.voltage_spinbox.setRange(10, 2000)
-        self.voltage_spinbox.setValue(400)
-        self.voltage_spinbox.setSingleStep(1)
-        self.voltage_label.setVisible(False)
-        self.voltage_spinbox.setVisible(False)
-        group_layout.addRow(self.voltage_label, self.voltage_spinbox)
-
-        self.open_pore_current_label = QLabel("I₀ (Open Pore Current) (nA):")
-        self.open_pore_current_spinbox = QDoubleSpinBox()
-        self.open_pore_current_spinbox.setRange(-500, 500)
-        self.open_pore_current_spinbox.setValue(25)
-        self.open_pore_current_spinbox.setSingleStep(0.1)
-        self.open_pore_current_label.setVisible(False)
-        self.open_pore_current_spinbox.setVisible(False)
-        group_layout.addRow(self.open_pore_current_label, self.open_pore_current_spinbox)
-
-        check_values_group = QGroupBox("Check Values")
-        check_values_layout = QFormLayout(check_values_group)
-        scroll_layout.addWidget(check_values_group)
-
-        self.delta_i_label = QLabel("ΔI (Change in Current) (nA):")
-        self.delta_i_spinbox = QDoubleSpinBox()
-        self.delta_i_spinbox.setRange(-500, 500)
-        self.delta_i_spinbox.setValue(1)
-        self.delta_i_spinbox.setSingleStep(0.1)
-        check_values_layout.addRow(self.delta_i_label, self.delta_i_spinbox)
-
-        self.check_values_button = QPushButton("Check Values")
-        self.check_values_button.clicked.connect(self.check_values)
-        check_values_layout.addRow(self.check_values_button)
-
-        self.check_values_result_label = QLabel()
-        check_values_layout.addRow(self.check_values_result_label)
-
-        self.check_values_group = check_values_group
-        self.check_values_group.setVisible(False)
-
-        layout.addWidget(scroll_area)
-
-        self.standardisation_widgets = [
-            self.standardisation_type_label,
-            self.standardisation_type_combo,
-            self.standardisation_explanation_label,
-            self.power_label,
-            self.power_spinbox,
-            self.length_label,
-            self.length_spinbox,
-            self.conductivity_label,
-            self.conductivity_spinbox,
-            self.voltage_label,
-            self.voltage_spinbox,
-            self.open_pore_current_label,
-            self.open_pore_current_spinbox
+        self .event_info_text_edit .moveCursor (QTextCursor .MoveOperation .End )
+        self .event_info_text_edit .append (info_text )
+
+class MLTab (QWidget ):
+    def __init__ (self ):
+        super ().__init__ ()
+        layout =QVBoxLayout (self )
+        layout .setContentsMargins (0 ,0 ,0 ,0 )
+
+        group =QGroupBox ("Data Reduction for ML")
+        group_layout =QFormLayout (group )
+
+        self .enable_ml_data_reduction_checkbox =QCheckBox ("Enable ML Data Reduction")
+        self .enable_ml_data_reduction_checkbox .stateChanged .connect (self .toggle_ml_widgets )
+        group_layout .addRow (self .enable_ml_data_reduction_checkbox )
+
+        self .tag_label =QLabel ("Tag:")
+        self .tag_lineedit =QLineEdit ()
+        self .tag_lineedit .setText ("BSA")
+        group_layout .addRow (self .tag_label ,self .tag_lineedit )
+
+        self .apply_standardisation_checkbox =QCheckBox ("Apply Standardisation?")
+        self .apply_standardisation_checkbox .stateChanged .connect (self .toggle_standardisation_label )
+        group_layout .addRow (self .apply_standardisation_checkbox )
+
+        self .standardisation_label =QLabel ("Please choose standardisation settings in the Fitting Options tab. If not chosen, results may not be correct.")
+        self .standardisation_label .setWordWrap (True )
+        self .standardisation_label .setVisible (False )
+        group_layout .addRow (self .standardisation_label )
+
+        self .data_reduction_type_label =QLabel ("Type of Data Reduction:")
+        self .data_reduction_type_combo =QComboBox ()
+        self .data_reduction_type_combo .addItems (["Scheme 1","Scheme 2","Scheme 3","Scheme 4","Scheme 5"])
+        group_layout .addRow (self .data_reduction_type_label ,self .data_reduction_type_combo )
+
+        self .scheme_table =QTableWidget ()
+        self .scheme_table .setRowCount (5 )
+        self .scheme_table .setColumnCount (2 )
+        self .scheme_table .setHorizontalHeaderLabels (["Feature Extraction Scheme","Features/Details"])
+        self .scheme_table .setItem (0 ,0 ,QTableWidgetItem ("Scheme 1"))
+        self .scheme_table .setItem (0 ,1 ,QTableWidgetItem ("Δi1, Δi2, … Δi10, Δt0/10"))
+        self .scheme_table .setItem (1 ,0 ,QTableWidgetItem ("Scheme 2"))
+        self .scheme_table .setItem (1 ,1 ,QTableWidgetItem ("Δi1, Δi2, … Δi10, Δt0/10, Δtfwhm, area, Δifwhm, Δimax"))
+        self .scheme_table .setItem (2 ,0 ,QTableWidgetItem ("Scheme 3"))
+        self .scheme_table .setItem (2 ,1 ,QTableWidgetItem ("Δi1, Δi2, … Δi10, Δt0/10, Δtfwhm, area, Δifwhm, Δimax , skew, kurtosis"))
+        self .scheme_table .setItem (3 ,0 ,QTableWidgetItem ("Scheme 4"))
+        self .scheme_table .setItem (3 ,1 ,QTableWidgetItem ("Δi1, Δi2, … Δi50, Δt0/50, Δtfwhm, area, Δifwhm, Δimax , skew, kurtosis"))
+        self .scheme_table .setItem (4 ,0 ,QTableWidgetItem ("Scheme 5"))
+        self .scheme_table .setItem (4 ,1 ,QTableWidgetItem ("Full signal, Δtfwhm, area, Δifwhm, Δimax , skew, kurtosis"))
+        self .scheme_table .resizeColumnsToContents ()
+        group_layout .addRow (self .scheme_table )
+
+        layout .addWidget (group )
+
+        self .ml_widgets =[self .tag_label ,self .tag_lineedit ,self .apply_standardisation_checkbox ,self .data_reduction_type_label ,self .data_reduction_type_combo ,self .scheme_table ]
+        self .toggle_ml_widgets ()
+
+    def toggle_ml_widgets (self ):
+        for widget in self .ml_widgets :
+            widget .setVisible (self .enable_ml_data_reduction_checkbox .isChecked ())
+
+    def toggle_standardisation_label (self ):
+        self .standardisation_label .setVisible (self .apply_standardisation_checkbox .isChecked ())
+
+
+class LoadOptionsTab (QWidget ):
+    def __init__ (self ):
+        super ().__init__ ()
+        layout =QVBoxLayout (self )
+        layout .setContentsMargins (0 ,0 ,0 ,0 )
+
+
+        scroll_area =QScrollArea ()
+        scroll_area .setWidgetResizable (True )
+        scroll_widget =QWidget ()
+        scroll_layout =QVBoxLayout (scroll_widget )
+        scroll_layout .setSpacing (10 )
+
+
+        self .select_folder_btn =QPushButton ("Select Folder")
+        self .select_folder_btn .clicked .connect (self .selectFolder )
+
+
+        self .include_subfolders_chk =QCheckBox ("Include Subfolders")
+
+
+        self .files_list_widget =QListWidget ()
+        self .files_list_widget .setSelectionMode (QListWidget .SelectionMode .MultiSelection )
+
+
+        self .folder_path_label =QLabel (" ")
+        self .folder_path_label .setWordWrap (True )
+
+
+        self .select_all_chk =QCheckBox ("Select All")
+        self .select_all_chk .stateChanged .connect (self .selectAllFiles )
+        self .select_all_chk .setTristate (False )
+
+
+        testing_duration_main_layout =QVBoxLayout ()
+
+
+        testing_duration_label =QLabel ("Testing Duration")
+        testing_duration_label .setAlignment (Qt .AlignmentFlag .AlignCenter )
+        testing_duration_main_layout .addWidget (testing_duration_label )
+
+        testing_duration_start_layout =QHBoxLayout ()
+        start_label =QLabel ("Start:")
+        testing_duration_start_layout .addWidget (start_label )
+
+        self .testing_duration_start_spinbox =QDoubleSpinBox ()
+        self .testing_duration_start_spinbox .setRange (0 ,10000 )
+        self .testing_duration_start_spinbox .setValue (0.0 )
+        self .testing_duration_start_spinbox .setSuffix (" s")
+        testing_duration_start_layout .addWidget (self .testing_duration_start_spinbox )
+
+
+        testing_duration_end_layout =QHBoxLayout ()
+        end_label =QLabel ("End:")
+        testing_duration_end_layout .addWidget (end_label )
+
+        self .testing_duration_end_spinbox =QDoubleSpinBox ()
+        self .testing_duration_end_spinbox .setRange (0 ,10000 )
+        self .testing_duration_end_spinbox .setValue (1 )
+        self .testing_duration_end_spinbox .setSuffix (" s")
+        testing_duration_end_layout .addWidget (self .testing_duration_end_spinbox )
+
+
+        testing_duration_main_layout .addLayout (testing_duration_start_layout )
+        testing_duration_main_layout .addLayout (testing_duration_end_layout )
+
+
+        self .save_event_chk =QCheckBox ("Save Events individually for Clustering")
+        self .save_event_chk .setTristate (False )
+        testing_duration_main_layout .addWidget (self .save_event_chk )
+
+
+        level_fitting_layout =QHBoxLayout ()
+        level_fitting_layout .addWidget (QLabel ("Do you want Level Fitting?"))
+        self .level_fitting_combo =QComboBox ()
+        self .level_fitting_combo .addItems (["Yes","No"])
+        self .level_fitting_combo .setCurrentText ("No")
+        level_fitting_layout .addWidget (self .level_fitting_combo )
+
+
+        self .test_settings_btn =QPushButton ("Test Settings on File")
+
+        self .plot_data_btn =QPushButton ("Plot Data")
+
+        self .perform_data_reduction_btn =QPushButton ("Perform Data Reduction")
+        self .save_file_path_btn =QPushButton ("Specify File Name (Saved Data)")
+
+
+
+        button_layout =QHBoxLayout ()
+        button_layout .addWidget (self .plot_data_btn )
+        button_layout .addWidget (self .test_settings_btn )
+
+
+
+        button_layout_2 =QHBoxLayout ()
+        button_layout_2 .addWidget (self .save_file_path_btn )
+        button_layout_2 .addWidget (self .perform_data_reduction_btn )
+
+
+        scroll_layout .addWidget (self .select_folder_btn )
+        scroll_layout .addWidget (self .include_subfolders_chk )
+        scroll_layout .addWidget (self .folder_path_label )
+        scroll_layout .addWidget (self .files_list_widget )
+        scroll_layout .addWidget (self .select_all_chk )
+        scroll_layout .addLayout (testing_duration_main_layout )
+        scroll_layout .addLayout (level_fitting_layout )
+        scroll_layout .addLayout (button_layout )
+        scroll_layout .addLayout (button_layout_2 )
+        scroll_area .setWidget (scroll_widget )
+        layout .addWidget (scroll_area )
+
+    def selectFolder (self ):
+        options =QFileDialog .Option .ShowDirsOnly 
+        directory =QFileDialog .getExistingDirectory (self ,"Select Folder","",options =options )
+        if directory :
+
+            self .folder_path_label .setText (f"Selected folder: {directory}")
+            self .populateFileList (directory ,self .include_subfolders_chk .isChecked ())
+
+    def populateFileList (self ,directory ,include_subfolders ):
+        self .files_list_widget .clear ()
+        for root ,dirs ,files in os .walk (directory ):
+            for file in files :
+                if file .endswith ('.abf')or file .endswith ('.hdf5')or file .endswith ('.h5'):
+
+                    rel_path =os .path .relpath (os .path .join (root ,file ),start =directory )
+                    item =QListWidgetItem (rel_path )
+                    item .setData (Qt .ItemDataRole .UserRole ,os .path .join (root ,file ))
+                    self .files_list_widget .addItem (item )
+            if not include_subfolders :
+
+                break 
+
+    def selectAllFiles (self ):
+        is_checked =self .select_all_chk .isChecked ()
+        for index in range (self .files_list_widget .count ()):
+            item =self .files_list_widget .item (index )
+            item .setSelected (is_checked )
+
+class EventSettingsTab (QWidget ):
+    def __init__ (self ):
+        super ().__init__ ()
+        layout =QVBoxLayout (self )
+        layout .setContentsMargins (0 ,0 ,0 ,0 )
+
+        scroll_area =QScrollArea ()
+        scroll_area .setWidgetResizable (True )
+        scroll_widget =QWidget ()
+        scroll_layout =QVBoxLayout (scroll_widget )
+        scroll_layout .setSpacing (10 )
+        scroll_area .setWidget (scroll_widget )
+
+
+        file_settings_group =QGroupBox ("File Settings")
+        file_settings_layout =QFormLayout (file_settings_group )
+        self .sampling_rate_spinbox =QDoubleSpinBox ()
+        self .sampling_rate_spinbox .setRange (1 ,100000 )
+        self .sampling_rate_spinbox .setValue (200 )
+        self .sampling_rate_spinbox .setSuffix (" kHz")
+        self .analysis_start_duration_spinbox =QDoubleSpinBox ()
+        self .analysis_start_duration_spinbox .setRange (0 ,100000 )
+        self .analysis_start_duration_spinbox .setValue (0 )
+        self .analysis_start_duration_spinbox .setSuffix (" s")
+        self .analysis_end_duration_spinbox =QDoubleSpinBox ()
+        self .analysis_end_duration_spinbox .setRange (0 ,100000 )
+        self .analysis_end_duration_spinbox .setValue (0 )
+        self .analysis_end_duration_spinbox .setSuffix (" s")
+        self .dips_or_peaks_combo =QComboBox ()
+        self .dips_or_peaks_combo .addItems (["Dips","Peaks"])
+        self .dips_or_peaks_combo .setCurrentIndex (0 )
+
+
+
+        self .enable_nth_data_point_loading =QCheckBox ("Enable Nth Data Point Loading")
+        self .enable_nth_data_point_loading .stateChanged .connect (self .toggle_nth_data_point_loading_widgets )
+
+        file_settings_layout .addRow ("Sampling Rate:",self .sampling_rate_spinbox )
+        file_settings_layout .addRow ("Analysis Start Duration:",self .analysis_start_duration_spinbox )
+        file_settings_layout .addRow ("Analysis End Duration:",self .analysis_end_duration_spinbox )
+        file_settings_layout .addRow ("Dips or Peaks:",self .dips_or_peaks_combo )
+        self .enable_analysis_time_specific =QCheckBox ("Enable Analysis between the time specified above")
+        file_settings_layout .addRow (self .enable_analysis_time_specific )
+        file_settings_layout .addRow (self .enable_nth_data_point_loading )
+
+
+
+        self .nth_data_point_spinbox =QDoubleSpinBox ()
+        self .nth_data_point_spinbox .setRange (1 ,1000 )
+        self .nth_data_point_spinbox .setValue (10 )
+        self .nth_data_point_label =QLabel ("Load every nth point:")
+        file_settings_layout .addRow (self .nth_data_point_label ,self .nth_data_point_spinbox )
+        self .nth_data_point_loading_widgets =[self .nth_data_point_spinbox ,self .nth_data_point_label ]
+        self .toggle_nth_data_point_loading_widgets ()
+
+
+        self .enable_window_loading =QCheckBox ("Enable Window Loading")
+        self .enable_window_loading .stateChanged .connect (self .toggle_window_loading_widgets )
+        file_settings_layout .addRow (self .enable_window_loading )
+        self .window_size_multiple_spinbox =QDoubleSpinBox ()
+        self .window_size_multiple_spinbox .setRange (1 ,1000 )
+        self .window_size_multiple_spinbox .setValue (10 )
+        self .window_size_multiple_label =QLabel ("Multiple of avg/std Window Size(whichever is higher):")
+        file_settings_layout .addRow (self .window_size_multiple_label ,self .window_size_multiple_spinbox )
+        self .window_loading_widgets =[self .window_size_multiple_label ,self .window_size_multiple_spinbox ]
+        self .toggle_window_loading_widgets ()
+
+        self .enable_plots =QCheckBox ("Enable Plots after Data Reduction")
+        self .enable_plots .setChecked (True )
+        self .enable_plots .stateChanged .connect (self .toggle_enable_plots_widgets )
+        file_settings_layout .addRow (self .enable_plots )
+        self .enable_plots_label =QLabel ("NOTE: This option only works when you reduce single file!")
+        file_settings_layout .addRow (self .enable_plots_label )
+        self .enable_plots_widgets =[self .enable_plots_label ]
+        self .toggle_enable_plots_widgets ()
+
+        self .save_plots =QCheckBox ("Save Plots after Data Reduction")
+        self .save_plots .setChecked (True )
+        self .save_plots .stateChanged .connect (self .toggle_enable_plots_widgets )
+        file_settings_layout .addRow (self .save_plots )
+
+
+
+
+        filtering_group =QGroupBox ("Filtering Options")
+        filtering_layout =QFormLayout (filtering_group )
+
+        self .apply_filter_combo =QComboBox ()
+        self .apply_filter_combo .addItems (["Yes","No"])
+        self .apply_filter_combo .setCurrentIndex (0 )
+        filtering_layout .addRow ("Apply Filter:",self .apply_filter_combo )
+
+        self .filter_type_combo =QComboBox ()
+        self .filter_type_combo .addItems (["Low Pass Filter","Wavelet"])
+        self .filter_type_combo .setCurrentIndex (0 )
+        filtering_layout .addRow ("Filter Type:",self .filter_type_combo )
+
+
+        self .type_of_low_pass_filter_label =QLabel ("Type of Low Pass Filter:")
+        self .low_pass_filter_type_combo =QComboBox ()
+        self .low_pass_filter_type_combo .addItems (["Bessel","Butterworth","Chebyshev I","Chebyshev II","Elliptic","FIR","IIR"])
+        self .low_pass_filter_type_combo .setCurrentIndex (1 )
+
+        self .cutoff_frequency_label =QLabel ("Cutoff Frequency:")
+        self .cutoff_frequency_spinbox =QDoubleSpinBox ()
+        self .cutoff_frequency_spinbox .setRange (1 ,5000 )
+        self .cutoff_frequency_spinbox .setValue (35 )
+        self .cutoff_frequency_spinbox .setSuffix (" kHz")
+
+
+        filtering_layout .addRow (self .type_of_low_pass_filter_label ,self .low_pass_filter_type_combo )
+        filtering_layout .addRow (self .cutoff_frequency_label ,self .cutoff_frequency_spinbox )
+
+        self .low_pass_filter_type_combo .hide ()
+        self .cutoff_frequency_spinbox .hide ()
+        self .type_of_low_pass_filter_label .hide ()
+        self .cutoff_frequency_label .hide ()
+
+        def update_filter_options ():
+
+            if self .filter_type_combo .currentText ()=="Low Pass Filter":
+                self .low_pass_filter_type_combo .show ()
+                self .cutoff_frequency_spinbox .show ()
+                self .type_of_low_pass_filter_label .show ()
+                self .cutoff_frequency_label .show ()
+            else :
+                self .low_pass_filter_type_combo .hide ()
+                self .cutoff_frequency_spinbox .hide ()
+                self .type_of_low_pass_filter_label .hide ()
+                self .cutoff_frequency_label .hide ()
+
+        self .filter_type_combo .currentTextChanged .connect (update_filter_options )
+
+
+        update_filter_options ()
+
+
+        thresholds_group =QGroupBox ("Thresholds")
+        thresholds_layout =QFormLayout (thresholds_group )
+        self .type_of_threshold_combo =QComboBox ()
+        self .type_of_threshold_combo .addItems (["ΔI","std multiplier"])
+        self .type_of_threshold_combo .setCurrentIndex (1 )
+        self .threshold_value_multiplier_spinbox =QDoubleSpinBox ()
+
+        self .start_of_event_threshold_spinbox =QDoubleSpinBox ()
+        self .start_of_event_threshold_spinbox .setValue (0.1 )
+        self .end_of_event_threshold_spinbox =QDoubleSpinBox ()
+        self .end_of_event_threshold_spinbox .setValue (0.1 )
+        thresholds_layout .addRow ("Type of Threshold:",self .type_of_threshold_combo )
+        thresholds_layout .addRow ("Threshold Value/Multiplier:",self .threshold_value_multiplier_spinbox )
+        thresholds_layout .addRow ("Start of Event Threshold:",self .start_of_event_threshold_spinbox )
+        thresholds_layout .addRow ("End of Event Threshold:",self .end_of_event_threshold_spinbox )
+
+
+        self .type_of_threshold_combo .currentTextChanged .connect (self .updateThresholdValueRange )
+        self .updateThresholdValueRange (self .type_of_threshold_combo .currentText ())
+
+
+        window_sizes_group =QGroupBox ("Window Sizes")
+        window_sizes_layout =QFormLayout (window_sizes_group )
+
+        self .mean_window_size_spinbox =QDoubleSpinBox ()
+        self .mean_window_size_spinbox .setRange (0.1 ,10000 )
+        self .mean_window_size_spinbox .setValue (10 )
+        self .mean_window_size_spinbox .setSuffix (" ms")
+
+        self .std_window_size_label =QLabel ("Std Window Size:")
+        self .std_window_size_spinbox =QDoubleSpinBox ()
+        self .std_window_size_spinbox .setRange (0.1 ,10000 )
+        self .std_window_size_spinbox .setValue (250 )
+        self .std_window_size_spinbox .setSuffix (" ms")
+
+        self .enable_std_smoothing_checkbox =QCheckBox ("Enable Std Smoothing")
+        self .enable_std_smoothing_checkbox .setChecked (False )
+        self .enable_std_smoothing_checkbox .stateChanged .connect (lambda state :self .update_std_smoothing_options (state ))
+
+        self .smoothing_type_label =QLabel ("Type of smoothing:")
+        self .smoothing_type_dropdown =QComboBox ()
+        self .smoothing_type_dropdown .addItems (["Moving Mean Smoothing","Exponential Smoothing"])
+        self .smoothing_type_dropdown .setCurrentIndex (1 )
+
+        window_sizes_layout .addRow ("Mean Window Size:",self .mean_window_size_spinbox )
+        window_sizes_layout .addRow (self .std_window_size_label ,self .std_window_size_spinbox )
+        window_sizes_layout .addRow (self .enable_std_smoothing_checkbox )
+        window_sizes_layout .addRow (self .smoothing_type_label ,self .smoothing_type_dropdown )
+
+        self .smoothing_type_label .setVisible (False )
+        self .smoothing_type_dropdown .setVisible (False )
+
+
+        event_widths_group =QGroupBox ("Min, Max Event Widths")
+        event_widths_layout =QFormLayout (event_widths_group )
+        self .minimum_event_width_spinbox =QDoubleSpinBox ()
+        self .minimum_event_width_spinbox .setRange (0.000001 ,100 )
+        self .minimum_event_width_spinbox .setDecimals (6 )
+        self .minimum_event_width_spinbox .setValue (0.001 )
+        self .minimum_event_width_spinbox .setSuffix (" ms")
+        self .maximum_event_width_spinbox =QDoubleSpinBox ()
+        self .maximum_event_width_spinbox .setRange (1e-3 ,10000 )
+        self .maximum_event_width_spinbox .setDecimals (6 )
+        self .maximum_event_width_spinbox .setValue (3 )
+        self .maximum_event_width_spinbox .setSuffix (" ms")
+        event_widths_layout .addRow ("Minimum Event Width:",self .minimum_event_width_spinbox )
+        event_widths_layout .addRow ("Maximum Event Width:",self .maximum_event_width_spinbox )
+
+
+        self .adjustGroupLayout (file_settings_group )
+        self .adjustGroupLayout (filtering_group )
+        self .adjustGroupLayout (thresholds_group )
+        self .adjustGroupLayout (window_sizes_group )
+        self .adjustGroupLayout (event_widths_group )
+
+
+        scroll_layout .addWidget (file_settings_group )
+        scroll_layout .addWidget (filtering_group )
+        scroll_layout .addWidget (thresholds_group )
+        scroll_layout .addWidget (window_sizes_group )
+        scroll_layout .addWidget (event_widths_group )
+        layout .addWidget (scroll_area )
+
+    def update_std_smoothing_options (self ,state ):
+        if state ==2 :
+            self .smoothing_type_label .setVisible (True )
+            self .smoothing_type_dropdown .setVisible (True )
+            self .std_window_size_spinbox .setValue (10 )
+        else :
+            self .smoothing_type_label .setVisible (False )
+            self .smoothing_type_dropdown .setVisible (False )
+            self .std_window_size_spinbox .setValue (250 )
+
+    def toggle_nth_data_point_loading_widgets (self ):
+        for widget in self .nth_data_point_loading_widgets :
+            widget .setVisible (self .enable_nth_data_point_loading .isChecked ())
+
+    def toggle_window_loading_widgets (self ):
+        for widget in self .window_loading_widgets :
+            widget .setVisible (self .enable_window_loading .isChecked ())
+
+    def toggle_enable_plots_widgets (self ):
+        for widget in self .enable_plots_widgets :
+            widget .setVisible (self .enable_plots .isChecked ())
+
+    def updateThresholdValueRange (self ,threshold_type ):
+        if threshold_type =="ΔI":
+            self .threshold_value_multiplier_spinbox .setRange (100 ,20000 )
+            self .threshold_value_multiplier_spinbox .setValue (2000 )
+            self .threshold_value_multiplier_spinbox .setSuffix (" pA")
+        else :
+            self .threshold_value_multiplier_spinbox .setRange (1 ,20 )
+            self .threshold_value_multiplier_spinbox .setValue (4 )
+            self .threshold_value_multiplier_spinbox .setSuffix (" ")
+
+
+    def adjustGroupLayout (self ,group_box ):
+        group_box .setSizePolicy (QSizePolicy .Policy .Preferred ,QSizePolicy .Policy .Preferred )
+        layout =group_box .layout ()
+        if layout :
+            layout .setAlignment (Qt .AlignmentFlag .AlignLeft )
+
+            for i in range (layout .count ()):
+                item =layout .itemAt (i ).widget ()
+                if item :
+                    item .setSizePolicy (QSizePolicy .Policy .Preferred ,QSizePolicy .Policy .Fixed )
+
+class FittingSettingsTab (QWidget ):
+    def __init__ (self ):
+        super ().__init__ ()
+        layout =QVBoxLayout (self )
+        layout .setContentsMargins (0 ,0 ,0 ,0 )
+
+        scroll_area =QScrollArea ()
+        scroll_area .setWidgetResizable (True )
+        scroll_widget =QWidget ()
+        scroll_layout =QVBoxLayout (scroll_widget )
+        scroll_layout .setSpacing (10 )
+        scroll_area .setWidget (scroll_widget )
+
+
+        settings_group =QGroupBox ("Fitting Settings")
+        settings_layout =QFormLayout (settings_group )
+        scroll_layout .addWidget (settings_group )
+
+        self .padding_spinbox =QSpinBox ()
+        self .padding_spinbox .setRange (0 ,10000 )
+        self .padding_spinbox .setValue (100 )
+
+        self .chunk_size_for_event_detection_spinbox =QSpinBox ()
+        self .chunk_size_for_event_detection_spinbox .setRange (1 ,1000000000 )
+        self .chunk_size_for_event_detection_spinbox .setValue (4000000 )
+
+        self .chunk_size_for_event_fitting_spinbox =QSpinBox ()
+        self .chunk_size_for_event_fitting_spinbox .setRange (1 ,100000 )
+        self .chunk_size_for_event_fitting_spinbox .setValue (30 )
+
+        self .chunk_size_for_peak_fitting_spinbox =QSpinBox ()
+        self .chunk_size_for_peak_fitting_spinbox .setRange (1 ,100000 )
+        self .chunk_size_for_peak_fitting_spinbox .setValue (30 )
+
+        self .library_combo =QComboBox ()
+        self .library_combo .addItems (["ruptures","detecta","lmfit","hmm","gmm"])
+        self .library_combo .currentIndexChanged .connect (self .update_model_combo )
+
+        self .model_combo =QComboBox ()
+        self .model_label =QLabel ("Model:")
+
+        self .num_components_spinbox =QSpinBox ()
+        self .num_components_spinbox .setRange (2 ,10 )
+        self .num_components_spinbox .setValue (2 )
+        self .num_components_label =QLabel ("Number of Components:")
+
+        self .threshold_spinbox =QDoubleSpinBox ()
+        self .threshold_spinbox .setRange (0.1 ,100 )
+        self .threshold_spinbox .setValue (3 )
+        self .threshold_spinbox .setDecimals (2 )
+
+
+        self .segment_rate_threshold_spinbox =QDoubleSpinBox ()
+        self .segment_rate_threshold_spinbox .setRange (0.001 ,100 )
+        self .segment_rate_threshold_spinbox .setValue (0.2 )
+        self .segment_rate_threshold_spinbox .setDecimals (3 )
+
+        settings_layout .addRow ("Padding (in number of samples):",self .padding_spinbox )
+        settings_layout .addRow ("Chunk Size for Event Detection:",self .chunk_size_for_event_detection_spinbox )
+        settings_layout .addRow ("Chunk Size for Event Fitting:",self .chunk_size_for_event_fitting_spinbox )
+        settings_layout .addRow ("Chunk Size for Peak Fitting:",self .chunk_size_for_peak_fitting_spinbox )
+        settings_layout .addRow ("Library:",self .library_combo )
+        settings_layout .addRow (self .model_label ,self .model_combo )
+        settings_layout .addRow (self .num_components_label ,self .num_components_spinbox )
+        settings_layout .addRow ("Threshold:",self .threshold_spinbox )
+        settings_layout .addRow ("Segment Rate Threshold:",self .segment_rate_threshold_spinbox )
+
+        layout .addWidget (scroll_area )
+
+        standardisation_group =QGroupBox ("Standardisation during Data Reduction")
+        group_layout =QFormLayout (standardisation_group )
+        scroll_layout .addWidget (standardisation_group )
+
+        self .enable_standardisation_checkbox =QCheckBox ("Enable Standardisation")
+        self .enable_standardisation_checkbox .stateChanged .connect (self .toggle_standardisation_widgets )
+        group_layout .addRow (self .enable_standardisation_checkbox )
+
+        self .standardisation_type_label =QLabel ("Which Standardisation to use:")
+        self .standardisation_type_combo =QComboBox ()
+        self .standardisation_type_combo .addItems (["ΔI/I₀","(ΔI*I₀)⁰·⁵","(ΔI*I₀)ᵖᵒʷᵉʳ","Dutt Standardisation"])
+        self .standardisation_type_combo .currentIndexChanged .connect (self .update_standardisation_explanation )
+        group_layout .addRow (self .standardisation_type_label ,self .standardisation_type_combo )
+
+        self .standardisation_explanation_label =QLabel ()
+        self .standardisation_explanation_label .setWordWrap (True )
+        group_layout .addRow (self .standardisation_explanation_label )
+
+        self .power_label =QLabel ("Power:")
+        self .power_spinbox =QDoubleSpinBox ()
+        self .power_spinbox .setRange (0.01 ,10 )
+        self .power_spinbox .setValue (0.5 )
+        self .power_spinbox .setSingleStep (0.01 )
+        self .power_label .setVisible (False )
+        self .power_spinbox .setVisible (False )
+        group_layout .addRow (self .power_label ,self .power_spinbox )
+
+        self .length_label =QLabel ("Length of the nanopore (L) (nm):")
+        self .length_spinbox =QDoubleSpinBox ()
+        self .length_spinbox .setRange (1 ,100 )
+        self .length_spinbox .setValue (7 )
+        self .length_spinbox .setSingleStep (0.1 )
+        self .length_label .setVisible (False )
+        self .length_spinbox .setVisible (False )
+        group_layout .addRow (self .length_label ,self .length_spinbox )
+
+        self .conductivity_label =QLabel ("σ (Conductivity of the solution) (S/m):")
+        self .conductivity_spinbox =QDoubleSpinBox ()
+        self .conductivity_spinbox .setRange (0.1 ,100 )
+        self .conductivity_spinbox .setValue (10.5 )
+        self .conductivity_spinbox .setSingleStep (0.1 )
+        self .conductivity_label .setVisible (False )
+        self .conductivity_spinbox .setVisible (False )
+        group_layout .addRow (self .conductivity_label ,self .conductivity_spinbox )
+
+        self .voltage_label =QLabel ("V (Voltage Applied) (mV):")
+        self .voltage_spinbox =QDoubleSpinBox ()
+        self .voltage_spinbox .setRange (10 ,2000 )
+        self .voltage_spinbox .setValue (400 )
+        self .voltage_spinbox .setSingleStep (1 )
+        self .voltage_label .setVisible (False )
+        self .voltage_spinbox .setVisible (False )
+        group_layout .addRow (self .voltage_label ,self .voltage_spinbox )
+
+        self .open_pore_current_label =QLabel ("I₀ (Open Pore Current) (nA):")
+        self .open_pore_current_spinbox =QDoubleSpinBox ()
+        self .open_pore_current_spinbox .setRange (-500 ,500 )
+        self .open_pore_current_spinbox .setValue (25 )
+        self .open_pore_current_spinbox .setSingleStep (0.1 )
+        self .open_pore_current_label .setVisible (False )
+        self .open_pore_current_spinbox .setVisible (False )
+        group_layout .addRow (self .open_pore_current_label ,self .open_pore_current_spinbox )
+
+        check_values_group =QGroupBox ("Check Values")
+        check_values_layout =QFormLayout (check_values_group )
+        scroll_layout .addWidget (check_values_group )
+
+        self .delta_i_label =QLabel ("ΔI (Change in Current) (nA):")
+        self .delta_i_spinbox =QDoubleSpinBox ()
+        self .delta_i_spinbox .setRange (-500 ,500 )
+        self .delta_i_spinbox .setValue (1 )
+        self .delta_i_spinbox .setSingleStep (0.1 )
+        check_values_layout .addRow (self .delta_i_label ,self .delta_i_spinbox )
+
+        self .check_values_button =QPushButton ("Check Values")
+        self .check_values_button .clicked .connect (self .check_values )
+        check_values_layout .addRow (self .check_values_button )
+
+        self .check_values_result_label =QLabel ()
+        check_values_layout .addRow (self .check_values_result_label )
+
+        self .check_values_group =check_values_group 
+        self .check_values_group .setVisible (False )
+
+        layout .addWidget (scroll_area )
+
+        self .standardisation_widgets =[
+        self .standardisation_type_label ,
+        self .standardisation_type_combo ,
+        self .standardisation_explanation_label ,
+        self .power_label ,
+        self .power_spinbox ,
+        self .length_label ,
+        self .length_spinbox ,
+        self .conductivity_label ,
+        self .conductivity_spinbox ,
+        self .voltage_label ,
+        self .voltage_spinbox ,
+        self .open_pore_current_label ,
+        self .open_pore_current_spinbox 
         ]
-        self.toggle_standardisation_widgets()
+        self .toggle_standardisation_widgets ()
 
-        self.update_model_combo(0)  # Initialize the model combo based on the default library
-        self.update_standardisation_explanation(0)
+        self .update_model_combo (0 )
+        self .update_standardisation_explanation (0 )
 
-    def check_values(self):
-        l = self.length_spinbox.value()*10**(-9)
-        delta_i = self.delta_i_spinbox.value()*10**(-9)
-        v = self.voltage_spinbox.value()/1000
-        sigma = self.conductivity_spinbox.value()
-        i0 = self.open_pore_current_spinbox.value()*10**(-9)
-
-        d = i0 + (i0 * (i0 + 16 * l * v * sigma / np.pi)) ** 0.5 / (2 * v * sigma)
-        condition = sigma > (4 * l * delta_i / v + d * np.pi * delta_i / v) / (d ** 2 * np.pi)
-        condition1  = delta_i<i0
-
-        if condition and condition1:
-            self.check_values_result_label.setText("The entered values should work and you will get a good standardisation.")
-        else:
-            self.check_values_result_label.setText("The entered values will not work. Something is wrong!")
-        self.check_values_result_label.setWordWrap(True)
-
-
-    def update_model_combo(self, index):
-        library = self.library_combo.currentText()
-        self.model_combo.clear()
-
-        if library in ["ruptures", "detecta",  "lmfit"]:
-            self.model_label.setVisible(True)
-            self.model_combo.setVisible(True)
-            self.num_components_label.setVisible(False)
-            self.num_components_spinbox.setVisible(False)
-
-            if library == "ruptures":
-                self.model_combo.addItems(["l1", "l2", "rbf"])
-                self.model_combo.setCurrentIndex(1)
-                self.model_combo.setCurrentIndex(1)
-            elif library == "detecta":
-                self.model_combo.addItems(["cusum"])
-            elif library == "lmfit":
-                self.model_combo.addItems(["autostepfinder"])
-        else:
-            self.model_label.setVisible(False)
-            self.model_combo.setVisible(False)
-            self.num_components_label.setVisible(True)
-            self.num_components_spinbox.setVisible(True)
-
-    def toggle_standardisation_widgets(self):
-        enabled = self.enable_standardisation_checkbox.isChecked()
-        for widget in self.standardisation_widgets:
-            widget.setVisible(enabled)
-
-        if enabled:
-            self.update_standardisation_explanation(self.standardisation_type_combo.currentIndex())
-        else:
-            self.power_label.setVisible(False)
-            self.power_spinbox.setVisible(False)
-            self.length_label.setVisible(False)
-            self.length_spinbox.setVisible(False)
-            self.conductivity_label.setVisible(False)
-            self.conductivity_spinbox.setVisible(False)
-            self.voltage_label.setVisible(False)
-            self.voltage_spinbox.setVisible(False)
-            self.open_pore_current_label.setVisible(False)
-            self.open_pore_current_spinbox.setVisible(False)
-            self.check_values_group.setVisible(False)
-
-    def update_standardisation_explanation(self, index):
-        self.power_label.setVisible(index == 2)
-        self.power_spinbox.setVisible(index == 2)
-        self.length_label.setVisible(index == 3)
-        self.length_spinbox.setVisible(index == 3)
-        self.conductivity_label.setVisible(index == 3)
-        self.conductivity_spinbox.setVisible(index == 3)
-        self.voltage_label.setVisible(index == 3)
-        self.voltage_spinbox.setVisible(index == 3)
-        self.open_pore_current_label.setVisible(index == 3)
-        self.open_pore_current_spinbox.setVisible(index == 3)
-        self.check_values_group.setVisible(index == 3)
-
-
-        if index == 0:
-            self.standardisation_explanation_label.setText("ΔI<sub>new</sub> = ΔI/I<sub>0</sub>")
-        elif index == 1:
-            self.standardisation_explanation_label.setText("ΔI<sub>new</sub> = (ΔI*I<sub>0</sub>)<sup>0.5</sup>")
-        elif index == 2:
-            self.standardisation_explanation_label.setText("ΔI<sub>new</sub> = (ΔI*I<sub>0</sub>)<sup>power</sup><br>"
-                                                        "Beware of using this option as some parts of ΔI<sub>new</sub> would be favoured as compared to others with changing values of power. "
-                                                        "Also beware of the units as except for power = 0.5, the units are not nA.")
-        elif index == 3:
-            self.standardisation_explanation_label.setText("Fo more information on this, talk with Shankar Dutt (shankar.dutt@anu.edu.au)")
-        elif index == 4:
-            explanation = "According to Kowalczyk Model:<br>" \
-                        "I<sub>0</sub> = σ*V*(4*L/(π*d<sup>2</sup>)+1/d)<sup>(-1)</sup><br>" \
-                        " <br>"\
-                        "ΔI = I<sub>0</sub>-(1*V*σ)/((1.27324*L)/(-1* d<sub>bio</sub><sup>2</sup>+(0.25*(I<sub>0</sub>+(I<sub>0</sub>*(I<sub>0</sub>+5.09296*L*V*σ)) <br>"\
-                        "<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup> *σ<sup>2</sup>))+1/((-1* d<sub>bio</sub><sup>2</sup>+(0.25*(I<sub>0</sub>+(I<sub>0</sub>* (I<sub>0</sub>+5.09296*L*V*σ))<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))<sup>0.5</sup>)<br>" \
-                        "<br> "\
-                        "ΔI<sub>new</sub> = ΔI*(I<sub>0_new</sub>-(1*V*σ)/(2.50663/(((3.14159*I<sub>0_new</sub><sup>2</sup>+8*I<sub>0_new</sub>*L*V*σ-6.28319*d<sub>bio</sub><sup>2</sup>*V<sup>2</sup>*σ<sup>2</sup>+ <br>" \
-                        "1.77245*I<sub>0_new</sub>*(I<sub>0_new</sub>*(3.14159*I<sub>0_new</sub>+16*L*V*σ))<sup>0.5</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))<sup>0.5</sup>)+(1.27324*L)/ <br>" \
-                        "(-1*d<sub>bio</sub><sup>2</sup>+ (0.25*(I<sub>0_new</sub>+(I<sub>0_new</sub>*(I<sub>0_new</sub>+5.09296*L*V*σ))<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup> <br> " \
-                        "*σ<sup>2</sup>))))/(I<sub>0</sub>-(1*V*σ)/(2.50663*/(((3.14159*I<sub>0</sub><sup>2</sup>+ 8*I<sub>0</sub>*L*V*σ-6.28319*d<sub>bio</sub><sup>2</sup>*V<sup>2</sup>*σ<sup>2</sup>+ <br> "\
-                        "1.77245*I<sub>0</sub>*(I<sub>0</sub>*(3.14159*I<sub>0</sub>+16*L*V*σ))<sup>0.5</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))<sup>0.5</sup>)+(1.27324*L)/(-1*d<sub>bio</sub><sup>2</sup>+ <br> "\
-                        "(0.25*(i0+(I<sub>0</sub>*(I<sub>0</sub>+5.09296*L*V*σ))<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))))"
-            self.standardisation_explanation_label.setText(explanation)
-        
-
-class ProcessingDialog(QDialog):
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        self.setWindowTitle("SD Data Reduction App")
-        self.setFixedSize(300, 100)
-
-        layout = QVBoxLayout()
-        self.label = QLabel("Please wait, Data Reduction is in progress...")
-        self.label.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        layout.addWidget(self.label)
-        self.setLayout(layout)
-
-
-
-class MplCanvas(FigureCanvas):
-    def __init__(self, width=5, height=4, dpi=100):
-        fig = Figure(figsize=(width, height), dpi=dpi)
-        self.axes = fig.add_subplot(111)
-        super().__init__(fig)
-
-
-
-def main():
-    app = QApplication(sys.argv)
-
-    app.setStyle(QStyleFactory.create('Fusion'))  # Use Fusion or other available styles
-    # Customize the palette for a darker, more modern look
-    palette = QPalette()
-    palette.setColor(QPalette.ColorRole.Window, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.WindowText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Base, QColor(25, 25, 25))
-    palette.setColor(QPalette.ColorRole.AlternateBase, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.ToolTipBase, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.ToolTipText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Text, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Button, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.ButtonText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.BrightText, Qt.GlobalColor.red)
-    palette.setColor(QPalette.ColorRole.Link, QColor(42, 130, 218))
-    palette.setColor(QPalette.ColorRole.Highlight, QColor(42, 130, 218))
-    palette.setColor(QPalette.ColorRole.HighlightedText, Qt.GlobalColor.black)
-    app.setPalette(palette)
-
-
-    main_window = MainWindow()
-    main_window.showMaximized()
-    sys.exit(app.exec())
+    def check_values (self ):
+        l =self .length_spinbox .value ()*10 **(-9 )
+        delta_i =self .delta_i_spinbox .value ()*10 **(-9 )
+        v =self .voltage_spinbox .value ()/1000 
+        sigma =self .conductivity_spinbox .value ()
+        i0 =self .open_pore_current_spinbox .value ()*10 **(-9 )
+
+        d =i0 +(i0 *(i0 +16 *l *v *sigma /np .pi ))**0.5 /(2 *v *sigma )
+        condition =sigma >(4 *l *delta_i /v +d *np .pi *delta_i /v )/(d **2 *np .pi )
+        condition1 =delta_i <i0 
+
+        if condition and condition1 :
+            self .check_values_result_label .setText ("The entered values should work and you will get a good standardisation.")
+        else :
+            self .check_values_result_label .setText ("The entered values will not work. Something is wrong!")
+        self .check_values_result_label .setWordWrap (True )
+
+
+    def update_model_combo (self ,index ):
+        library =self .library_combo .currentText ()
+        self .model_combo .clear ()
+
+        if library in ["ruptures","detecta","lmfit"]:
+            self .model_label .setVisible (True )
+            self .model_combo .setVisible (True )
+            self .num_components_label .setVisible (False )
+            self .num_components_spinbox .setVisible (False )
+
+            if library =="ruptures":
+                self .model_combo .addItems (["l1","l2","rbf"])
+                self .model_combo .setCurrentIndex (1 )
+                self .model_combo .setCurrentIndex (1 )
+            elif library =="detecta":
+                self .model_combo .addItems (["cusum"])
+            elif library =="lmfit":
+                self .model_combo .addItems (["autostepfinder"])
+        else :
+            self .model_label .setVisible (False )
+            self .model_combo .setVisible (False )
+            self .num_components_label .setVisible (True )
+            self .num_components_spinbox .setVisible (True )
+
+    def toggle_standardisation_widgets (self ):
+        enabled =self .enable_standardisation_checkbox .isChecked ()
+        for widget in self .standardisation_widgets :
+            widget .setVisible (enabled )
+
+        if enabled :
+            self .update_standardisation_explanation (self .standardisation_type_combo .currentIndex ())
+        else :
+            self .power_label .setVisible (False )
+            self .power_spinbox .setVisible (False )
+            self .length_label .setVisible (False )
+            self .length_spinbox .setVisible (False )
+            self .conductivity_label .setVisible (False )
+            self .conductivity_spinbox .setVisible (False )
+            self .voltage_label .setVisible (False )
+            self .voltage_spinbox .setVisible (False )
+            self .open_pore_current_label .setVisible (False )
+            self .open_pore_current_spinbox .setVisible (False )
+            self .check_values_group .setVisible (False )
+
+    def update_standardisation_explanation (self ,index ):
+        self .power_label .setVisible (index ==2 )
+        self .power_spinbox .setVisible (index ==2 )
+        self .length_label .setVisible (index ==3 )
+        self .length_spinbox .setVisible (index ==3 )
+        self .conductivity_label .setVisible (index ==3 )
+        self .conductivity_spinbox .setVisible (index ==3 )
+        self .voltage_label .setVisible (index ==3 )
+        self .voltage_spinbox .setVisible (index ==3 )
+        self .open_pore_current_label .setVisible (index ==3 )
+        self .open_pore_current_spinbox .setVisible (index ==3 )
+        self .check_values_group .setVisible (index ==3 )
+
+
+        if index ==0 :
+            self .standardisation_explanation_label .setText ("ΔI<sub>new</sub> = ΔI/I<sub>0</sub>")
+        elif index ==1 :
+            self .standardisation_explanation_label .setText ("ΔI<sub>new</sub> = (ΔI*I<sub>0</sub>)<sup>0.5</sup>")
+        elif index ==2 :
+            self .standardisation_explanation_label .setText ("ΔI<sub>new</sub> = (ΔI*I<sub>0</sub>)<sup>power</sup><br>"
+            "Beware of using this option as some parts of ΔI<sub>new</sub> would be favoured as compared to others with changing values of power. "
+            "Also beware of the units as except for power = 0.5, the units are not nA.")
+        elif index ==3 :
+            self .standardisation_explanation_label .setText ("Fo more information on this, talk with Shankar Dutt (shankar.dutt@anu.edu.au)")
+        elif index ==4 :
+            explanation ="According to Kowalczyk Model:<br>" "I<sub>0</sub> = σ*V*(4*L/(π*d<sup>2</sup>)+1/d)<sup>(-1)</sup><br>" " <br>" "ΔI = I<sub>0</sub>-(1*V*σ)/((1.27324*L)/(-1* d<sub>bio</sub><sup>2</sup>+(0.25*(I<sub>0</sub>+(I<sub>0</sub>*(I<sub>0</sub>+5.09296*L*V*σ)) <br>" "<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup> *σ<sup>2</sup>))+1/((-1* d<sub>bio</sub><sup>2</sup>+(0.25*(I<sub>0</sub>+(I<sub>0</sub>* (I<sub>0</sub>+5.09296*L*V*σ))<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))<sup>0.5</sup>)<br>" "<br> " "ΔI<sub>new</sub> = ΔI*(I<sub>0_new</sub>-(1*V*σ)/(2.50663/(((3.14159*I<sub>0_new</sub><sup>2</sup>+8*I<sub>0_new</sub>*L*V*σ-6.28319*d<sub>bio</sub><sup>2</sup>*V<sup>2</sup>*σ<sup>2</sup>+ <br>" "1.77245*I<sub>0_new</sub>*(I<sub>0_new</sub>*(3.14159*I<sub>0_new</sub>+16*L*V*σ))<sup>0.5</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))<sup>0.5</sup>)+(1.27324*L)/ <br>" "(-1*d<sub>bio</sub><sup>2</sup>+ (0.25*(I<sub>0_new</sub>+(I<sub>0_new</sub>*(I<sub>0_new</sub>+5.09296*L*V*σ))<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup> <br> " "*σ<sup>2</sup>))))/(I<sub>0</sub>-(1*V*σ)/(2.50663*/(((3.14159*I<sub>0</sub><sup>2</sup>+ 8*I<sub>0</sub>*L*V*σ-6.28319*d<sub>bio</sub><sup>2</sup>*V<sup>2</sup>*σ<sup>2</sup>+ <br> " "1.77245*I<sub>0</sub>*(I<sub>0</sub>*(3.14159*I<sub>0</sub>+16*L*V*σ))<sup>0.5</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))<sup>0.5</sup>)+(1.27324*L)/(-1*d<sub>bio</sub><sup>2</sup>+ <br> " "(0.25*(i0+(I<sub>0</sub>*(I<sub>0</sub>+5.09296*L*V*σ))<sup>0.5</sup>)<sup>2</sup>)/(V<sup>2</sup>*σ<sup>2</sup>))))"
+            self .standardisation_explanation_label .setText (explanation )
+
+
+class ProcessingDialog (QDialog ):
+    def __init__ (self ,parent =None ):
+        super ().__init__ (parent )
+        self .setWindowTitle ("SD Data Reduction App")
+        self .setFixedSize (300 ,100 )
+
+        layout =QVBoxLayout ()
+        self .label =QLabel ("Please wait, Data Reduction is in progress...")
+        self .label .setAlignment (Qt .AlignmentFlag .AlignCenter )
+        layout .addWidget (self .label )
+        self .setLayout (layout )
+
+
+
+class MplCanvas (FigureCanvas ):
+    def __init__ (self ,width =5 ,height =4 ,dpi =100 ):
+        fig =Figure (figsize =(width ,height ),dpi =dpi )
+        self .axes =fig .add_subplot (111 )
+        super ().__init__ (fig )
+
+
+
+def main ():
+    app =QApplication (sys .argv )
+
+    app .setStyle (QStyleFactory .create ('Fusion'))
+
+    palette =QPalette ()
+    palette .setColor (QPalette .ColorRole .Window ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .WindowText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Base ,QColor (25 ,25 ,25 ))
+    palette .setColor (QPalette .ColorRole .AlternateBase ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .ToolTipBase ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .ToolTipText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Text ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Button ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .ButtonText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .BrightText ,Qt .GlobalColor .red )
+    palette .setColor (QPalette .ColorRole .Link ,QColor (42 ,130 ,218 ))
+    palette .setColor (QPalette .ColorRole .Highlight ,QColor (42 ,130 ,218 ))
+    palette .setColor (QPalette .ColorRole .HighlightedText ,Qt .GlobalColor .black )
+    app .setPalette (palette )
+
+
+    main_window =MainWindow ()
+    main_window .showMaximized ()
+    sys .exit (app .exec ())
 
-if __name__ == "__main__":
-    main()
+if __name__ =="__main__":
+    main ()
```

### Comparing `nanosense-0.3.1/nanosense/Frequency and multi-plots/main.py` & `nanosense-0.3.2/nanosense/Frequency and multi-plots/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,824 +1,824 @@
-import sys
-import os
-import numpy as np
-from PySide6.QtWidgets import (QApplication, QMainWindow, QWidget, QVBoxLayout, QHBoxLayout, QPushButton, QListWidget, QSpinBox,QDoubleSpinBox, QLabel, QCheckBox, QFileDialog, QTabWidget, QSizePolicy, QGridLayout, QSpinBox, QMessageBox, QLineEdit, QFormLayout, QHBoxLayout, QStyleFactory,)
-from PySide6.QtCore import Qt
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-from matplotlib.figure import Figure
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-from functools import partial
-import seaborn as sns
-import matplotlib.pyplot as plt
-from matplotlib.ticker import ScalarFormatter
-from PySide6.QtGui import QPalette, QColor, QFont
-import math
-
-class MplCanvas(FigureCanvas):
-    def __init__(self, width=5, height=4, dpi=300):
-        fig = Figure(figsize=(width, height), dpi=dpi)
-        self.axes = fig.add_subplot(111)
-        super().__init__(fig)
-
-class PlottingApplication(QMainWindow):
-    def __init__(self):
-        super().__init__()
-        self.setWindowTitle("SD Frequency and multi-plots")
-        self.histogram_bins = 100  # Default number of bins
-        self.scatter_marker_size = 3  # Default scatter marker size
-        self.global_limits = {}
-        self.initUI()
-
-    def initUI(self):
-        # Main widget and layout
-        mainWidget = QWidget()
-        self.setCentralWidget(mainWidget)
-        mainLayout = QHBoxLayout(mainWidget)
-
-        # Left panel for file selection and plot options
-        self.leftPanel = QTabWidget()  # Assign to self to make it accessible class-wide
-        fileSelectionTab = QWidget()
-        self.plotOptionsTab = QWidget()
-        self.leftPanel.addTab(fileSelectionTab, "Files")
-        self.leftPanel.addTab(self.plotOptionsTab, "Options")
-        
-        # Right panel for displaying plots
-        self.rightPanel = QTabWidget()
-
-        mainLayout.addWidget(self.leftPanel, 25)
-        mainLayout.addWidget(self.rightPanel, 75)
-
-        self.setupFileSelectionTab(fileSelectionTab)
-        self.setupPlotOptionsTab(self.plotOptionsTab)
-    
-
-
-    def calculateGridSize(self, numberOfPlots):
-        # Calculate the square root of the number of plots to get an approximation
-        # of the grid size
-        gridSize = math.ceil(math.sqrt(numberOfPlots))
-        
-        # For a perfectly square layout, both the number of rows and columns
-        # would be equal to gridSize. However, depending on your exact needs,
-        # you might want to adjust this to have more rows than columns or vice versa.
-        nrows = gridSize
-        ncols = gridSize
-        
-        # Adjust ncols if there are too many empty spots
-        if gridSize * (gridSize - 1) >= numberOfPlots:
-            ncols -= 1
-        
-        return nrows, ncols
-
-
-
-    def setupFileSelectionTab(self, tab):
-        layout = QVBoxLayout(tab)  # Create a layout for this tab
-
-        headerLabel = QLabel("SD Frequency and multi-plots\nshankar.dutt@anu.edu.au")
-        headerLabel.setWordWrap(True)
-        headerLabel.setAlignment(Qt.AlignmentFlag.AlignCenter)  # Update alignment flag
-        headerLabel.setFont(QFont('Arial', 18, QFont.Weight.Bold))  # Update font weight
-        headerLabel.setStyleSheet("QLabel { color : white; margin-top: 20px; margin-bottom: 20px; }")
+import sys 
+import os 
+import numpy as np 
+from PySide6 .QtWidgets import (QApplication ,QMainWindow ,QWidget ,QVBoxLayout ,QHBoxLayout ,QPushButton ,QListWidget ,QSpinBox ,QDoubleSpinBox ,QLabel ,QCheckBox ,QFileDialog ,QTabWidget ,QSizePolicy ,QGridLayout ,QSpinBox ,QMessageBox ,QLineEdit ,QFormLayout ,QHBoxLayout ,QStyleFactory ,)
+from PySide6 .QtCore import Qt 
+from matplotlib .backends .backend_qt5agg import FigureCanvasQTAgg as FigureCanvas 
+from matplotlib .figure import Figure 
+from matplotlib .backends .backend_qt5agg import NavigationToolbar2QT as NavigationToolbar 
+from functools import partial 
+import seaborn as sns 
+import matplotlib .pyplot as plt 
+from matplotlib .ticker import ScalarFormatter 
+from PySide6 .QtGui import QPalette ,QColor ,QFont 
+import math 
 
-        # Update the stylesheet for QPushButton for PyQt6
-        app.setStyleSheet("""
+class MplCanvas (FigureCanvas ):
+    def __init__ (self ,width =5 ,height =4 ,dpi =300 ):
+        fig =Figure (figsize =(width ,height ),dpi =dpi )
+        self .axes =fig .add_subplot (111 )
+        super ().__init__ (fig )
+
+class PlottingApplication (QMainWindow ):
+    def __init__ (self ):
+        super ().__init__ ()
+        self .setWindowTitle ("SD Frequency and multi-plots")
+        self .histogram_bins =100 
+        self .scatter_marker_size =3 
+        self .global_limits ={}
+        self .initUI ()
+
+    def initUI (self ):
+
+        mainWidget =QWidget ()
+        self .setCentralWidget (mainWidget )
+        mainLayout =QHBoxLayout (mainWidget )
+
+
+        self .leftPanel =QTabWidget ()
+        fileSelectionTab =QWidget ()
+        self .plotOptionsTab =QWidget ()
+        self .leftPanel .addTab (fileSelectionTab ,"Files")
+        self .leftPanel .addTab (self .plotOptionsTab ,"Options")
+
+
+        self .rightPanel =QTabWidget ()
+
+        mainLayout .addWidget (self .leftPanel ,25 )
+        mainLayout .addWidget (self .rightPanel ,75 )
+
+        self .setupFileSelectionTab (fileSelectionTab )
+        self .setupPlotOptionsTab (self .plotOptionsTab )
+
+
+
+    def calculateGridSize (self ,numberOfPlots ):
+
+
+        gridSize =math .ceil (math .sqrt (numberOfPlots ))
+
+
+
+
+        nrows =gridSize 
+        ncols =gridSize 
+
+
+        if gridSize *(gridSize -1 )>=numberOfPlots :
+            ncols -=1 
+
+        return nrows ,ncols 
+
+
+
+    def setupFileSelectionTab (self ,tab ):
+        layout =QVBoxLayout (tab )
+
+        headerLabel =QLabel ("SD Frequency and multi-plots\nshankar.dutt@anu.edu.au")
+        headerLabel .setWordWrap (True )
+        headerLabel .setAlignment (Qt .AlignmentFlag .AlignCenter )
+        headerLabel .setFont (QFont ('Arial',18 ,QFont .Weight .Bold ))
+        headerLabel .setStyleSheet ("QLabel { color : white; margin-top: 20px; margin-bottom: 20px; }")
+
+
+        app .setStyleSheet ("""
         QPushButton {
             background-color: #2b5b84;
             color: white;
             border-radius: 5px;
             padding: 10px;
         }
         QPushButton:hover {
             background-color: #1d4560;
         }
         """)
 
-        layout.addWidget(headerLabel)
+        layout .addWidget (headerLabel )
 
-        selectFolderBtn = QPushButton("Select Folder")
-        selectFolderBtn.clicked.connect(self.selectFolder)
-        layout.addWidget(selectFolderBtn)
-
-        self.fileListWidget = QListWidget()
-        self.fileListWidget.setSelectionMode(QListWidget.SelectionMode.MultiSelection)
-        layout.addWidget(self.fileListWidget)
-
-        self.includeSubfoldersCheckbox = QCheckBox("Include Subfolders")
-        layout.addWidget(self.includeSubfoldersCheckbox)
-
-        plotButton = QPushButton("Plot")
-        plotButton.clicked.connect(self.plotSelectedFiles)
-        layout.addWidget(plotButton)
-
-        # Initialize plot options and add them to the layout
-        self.plotOptions = {
-            'Histogram of dI': QCheckBox('Histogram of dI'),
-            'Histogram of dt': QCheckBox('Histogram of dt'),
-            'Histogram of Area': QCheckBox('Histogram of Area'),
-            'Scatter plot dI vs dt': QCheckBox('Scatter plot dI vs dt'),
-            'Scatter plot area vs dt': QCheckBox('Scatter plot area vs dt'),
-            'Histogram of dt (log)': QCheckBox('Histogram of dt (log)'),
-            'Scatter plot dI vs dt (log)': QCheckBox('Scatter plot dI vs dt (log)'),
-            'Frequency plot': QCheckBox('Frequency plot')
+        selectFolderBtn =QPushButton ("Select Folder")
+        selectFolderBtn .clicked .connect (self .selectFolder )
+        layout .addWidget (selectFolderBtn )
+
+        self .fileListWidget =QListWidget ()
+        self .fileListWidget .setSelectionMode (QListWidget .SelectionMode .MultiSelection )
+        layout .addWidget (self .fileListWidget )
+
+        self .includeSubfoldersCheckbox =QCheckBox ("Include Subfolders")
+        layout .addWidget (self .includeSubfoldersCheckbox )
+
+        plotButton =QPushButton ("Plot")
+        plotButton .clicked .connect (self .plotSelectedFiles )
+        layout .addWidget (plotButton )
+
+
+        self .plotOptions ={
+        'Histogram of dI':QCheckBox ('Histogram of dI'),
+        'Histogram of dt':QCheckBox ('Histogram of dt'),
+        'Histogram of Area':QCheckBox ('Histogram of Area'),
+        'Scatter plot dI vs dt':QCheckBox ('Scatter plot dI vs dt'),
+        'Scatter plot area vs dt':QCheckBox ('Scatter plot area vs dt'),
+        'Histogram of dt (log)':QCheckBox ('Histogram of dt (log)'),
+        'Scatter plot dI vs dt (log)':QCheckBox ('Scatter plot dI vs dt (log)'),
+        'Frequency plot':QCheckBox ('Frequency plot')
         }
-        for option in self.plotOptions.values():
-            layout.addWidget(option)
+        for option in self .plotOptions .values ():
+            layout .addWidget (option )
+
+        syncZoomButton =QPushButton ("Sync Zoom")
+        syncZoomButton .clicked .connect (self .syncZoomAcrossPlots )
+        layout .addWidget (syncZoomButton )
+        self .selectedFilesOrder =[]
+
+
+        self .fileListWidget .itemSelectionChanged .connect (self .updateSelectionOrder )
+
+
+    def setupPlotOptionsTab (self ,tab ):
+        layout =QVBoxLayout (tab )
+
+
+        formLayout =QFormLayout ()
+
+
+        self .histogramBinsSpinBox =QSpinBox ()
+        self .histogramBinsSpinBox .setMinimum (1 )
+        self .histogramBinsSpinBox .setMaximum (1000 )
+        self .histogramBinsSpinBox .setValue (100 )
+        formLayout .addRow ("Histogram Bins:",self .histogramBinsSpinBox )
+
+
+        self .markerSizeSpinBox =QSpinBox ()
+        self .markerSizeSpinBox .setMinimum (1 )
+        self .markerSizeSpinBox .setMaximum (100 )
+        self .markerSizeSpinBox .setValue (3 )
+        formLayout .addRow ("Marker Size:",self .markerSizeSpinBox )
+
+
+        self .linearFitCheckBox =QCheckBox ("Enable Linear Fit in the Frequency Plots")
+        formLayout .addRow (self .linearFitCheckBox )
+
+
+        self .fitBetweenPointsCheckBox =QCheckBox ("Fit Between Two Points")
+        formLayout .addRow (self .fitBetweenPointsCheckBox )
+
+
+        self .fitStartPointSpinBox =QDoubleSpinBox ()
+        self .fitStartPointSpinBox .setMinimum (-np .inf )
+        self .fitStartPointSpinBox .setMaximum (np .inf )
+        self .fitStartPointSpinBox .setValue (0 )
+
+
+        self .fitEndPointSpinBox =QDoubleSpinBox ()
+        self .fitEndPointSpinBox .setMinimum (-np .inf )
+        self .fitEndPointSpinBox .setMaximum (np .inf )
+        self .fitEndPointSpinBox .setValue (1 )
+
+        self .fitRangeLabel =QLabel ("Fit Range:")
+        self .fitRangeLayout =QHBoxLayout ()
+        self .fitRangeLayout .addWidget (self .fitRangeLabel )
+        self .fitRangeLayout .addWidget (self .fitStartPointSpinBox )
+        self .fitRangeLayout .addWidget (self .fitEndPointSpinBox )
+        formLayout .addRow (self .fitRangeLayout )
+
+        self .fitBetweenPointsCheckBox .stateChanged .connect (self .toggleFitRangeVisibility )
+        self .toggleFitRangeVisibility (False )
+
+        self .overlayPlotsCheckBox =QCheckBox ("Overlay Plots")
+        formLayout .addRow (self .overlayPlotsCheckBox )
+
+        self .alphaSpin =QDoubleSpinBox ()
+        self .alphaSpin .setMinimum (0.0 )
+        self .alphaSpin .setMaximum (1.0 )
+        self .alphaSpin .setSingleStep (0.1 )
+        self .alphaSpin .setValue (0.5 )
+        formLayout .addRow ("Alpha:",self .alphaSpin )
+
+
+        self .saveDirectoryLineEdit =QLineEdit ()
+        self .saveDirectoryButton =QPushButton ("Select Save Folder")
+        self .saveDirectoryButton .clicked .connect (self .selectSaveFolder )
+        saveFolderLayout =QHBoxLayout ()
+        saveFolderLayout .addWidget (self .saveDirectoryLineEdit )
+        saveFolderLayout .addWidget (self .saveDirectoryButton )
+        formLayout .addRow ("Save Figures To:",saveFolderLayout )
+
+
+        updatePlotsButton =QPushButton ("Update Plots")
+        updatePlotsButton .clicked .connect (self .updatePlots )
+        formLayout .addRow ("",updatePlotsButton )
+
+
+        saveFiguresButton =QPushButton ("Save Figures")
+        saveFiguresButton .clicked .connect (self .saveAllFigures )
+        formLayout .addRow ("",saveFiguresButton )
+
+        layout .addLayout (formLayout )
+
+
+        layout .setSpacing (10 )
+        tab .setLayout (layout )
+
+    def toggleFitRangeVisibility (self ,visible ):
+        self .fitRangeLabel .setVisible (visible )
+        self .fitStartPointSpinBox .setVisible (visible )
+        self .fitEndPointSpinBox .setVisible (visible )
+
+
+    def selectSaveFolder (self ):
+        folder =QFileDialog .getExistingDirectory (self ,"Select Folder")
+        if folder :
+            self .saveDirectoryLineEdit .setText (folder )
+
+    def saveAllFigures (self ):
+        saveFolder =self .saveDirectoryLineEdit .text ().strip ()
+        if not saveFolder :
+            QMessageBox .information (self ,"Info","Please select a folder to save the figures.")
+            return 
+
+        for i in range (self .rightPanel .count ()):
+            tab =self .rightPanel .widget (i )
+            if hasattr (tab ,"property"):
+                tabCanvases =tab .property ("canvases")
+                if tabCanvases :
+                    tabFolder =os .path .join (saveFolder ,self .rightPanel .tabText (i ))
+                    if not os .path .exists (tabFolder ):
+                        os .makedirs (tabFolder )
+                    for j ,canvas in enumerate (tabCanvases ):
+                        figure =canvas .figure 
+                        figure .savefig (os .path .join (tabFolder ,f"figure_{j+1}.png"),dpi =300 ,bbox_inches ='tight')
+        QMessageBox .information (self ,"Info","Figures saved successfully.")
+
+
+
+    def selectFolder (self ):
+        folderPath =QFileDialog .getExistingDirectory (self ,"Select Folder")
+        if folderPath :
+            self .populateFileList (folderPath ,self .includeSubfoldersCheckbox .isChecked ())
+
+    def populateFileList (self ,folderPath ,includeSubfolders ):
+        self .fileListWidget .clear ()
+        if includeSubfolders :
+            for root ,dirs ,files in os .walk (folderPath ):
+                for file in files :
+                    if file .endswith ('.dataset.npz'):
+                        fullPath =os .path .join (root ,file )
+                        self .fileListWidget .addItem (fullPath )
+        else :
+            for file in os .listdir (folderPath ):
+                if file .endswith ('.dataset.npz'):
+                    fullPath =os .path .join (folderPath ,file )
+                    self .fileListWidget .addItem (fullPath )
+
+    def updateSelectionOrder (self ):
+
+        currentSelection ={self .fileListWidget .item (i ).text ()for i in range (self .fileListWidget .count ())if self .fileListWidget .item (i ).isSelected ()}
+
+
+        self .selectedFilesOrder =[f for f in self .selectedFilesOrder if f in currentSelection ]
+
+
+        for i in range (self .fileListWidget .count ()):
+            itemText =self .fileListWidget .item (i ).text ()
+            if self .fileListWidget .item (i ).isSelected ()and itemText not in self .selectedFilesOrder :
+                self .selectedFilesOrder .append (itemText )
+
+
+    def updatePlots (self ):
+
+        self .histogram_bins =self .histogramBinsSpinBox .value ()
+        self .scatter_marker_size =self .markerSizeSpinBox .value ()
+
+
+        self .plotSelectedFiles ()
+
+
+    @staticmethod 
+    def create_joint_plot (self ,fig ,data_x ,data_y ,min_x ,max_x ,min_y ,max_y ,plotType ,alpha ):
+
+        gs =fig .add_gridspec (4 ,4 )
+
+
+        ax_scatter =fig .add_subplot (gs [1 :4 ,0 :3 ])
+        if data_x is not None and data_y is not None :
+            ax_scatter .scatter (data_x ,data_y ,s =int (self .markerSizeSpinBox .value ()),alpha =alpha )
+        ax_scatter .set_xlim (min_x ,max_x )
+        ax_scatter .set_ylim (min_y ,max_y )
+
+
+        ax_histx =fig .add_subplot (gs [0 ,0 :3 ],sharex =ax_scatter )
+        if data_x is not None :
+            ax_histx .hist (data_x ,bins =self .histogramBinsSpinBox .value ())
+        ax_histx .set_ylabel (' ')
+
+
+        ax_histy =fig .add_subplot (gs [1 :4 ,3 ],sharey =ax_scatter )
+        if data_y is not None :
+            ax_histy .hist (data_y ,bins =self .histogramBinsSpinBox .value (),orientation ='horizontal')
+        ax_histy .set_xlabel (' ')
+
+
+        plt .setp (ax_histx .get_xticklabels (),visible =False )
+        plt .setp (ax_histy .get_yticklabels (),visible =False )
+
+        ax_scatter .xaxis .set_major_formatter (ScalarFormatter (useMathText =True ))
+        ax_scatter .yaxis .set_major_formatter (ScalarFormatter (useMathText =True ))
+        if 'dI vs dt'in plotType and 'log'not in plotType :
+            ax_scatter .set_xlabel ('Δt (ms)')
+            ax_scatter .set_ylabel ('ΔI (nA)')
+        elif 'area vs dt'in plotType :
+            ax_scatter .set_xlabel ('Δt (ms)')
+            ax_scatter .set_ylabel ('Area (C)')
+        elif 'dI vs dt (log)'in plotType :
+            ax_scatter .set_xlabel ('Δt (ms) [log]')
+            ax_scatter .set_ylabel ('ΔI (nA)')
+
+        ax_scatter .ticklabel_format (style ='sci',axis ='both',scilimits =(0 ,0 ))
+        ax_histx .ticklabel_format (style ='sci',axis ='both',scilimits =(0 ,0 ))
+        ax_histy .ticklabel_format (style ='sci',axis ='both',scilimits =(0 ,0 ))
+        fig .tight_layout ()
+
+
+        return {'ax_scatter':ax_scatter ,'ax_histx':ax_histx ,'ax_histy':ax_histy }
 
-        syncZoomButton = QPushButton("Sync Zoom")
-        syncZoomButton.clicked.connect(self.syncZoomAcrossPlots)
-        layout.addWidget(syncZoomButton)
-        self.selectedFilesOrder = []
-        
-        # Connect the selection changed signal
-        self.fileListWidget.itemSelectionChanged.connect(self.updateSelectionOrder)
-
-
-    def setupPlotOptionsTab(self, tab):
-        layout = QVBoxLayout(tab)
-        
-        # Use QFormLayout for a neat alignment of labels and fields including buttons
-        formLayout = QFormLayout()
-
-        # Histogram Bins
-        self.histogramBinsSpinBox = QSpinBox()
-        self.histogramBinsSpinBox.setMinimum(1)
-        self.histogramBinsSpinBox.setMaximum(1000)
-        self.histogramBinsSpinBox.setValue(100)
-        formLayout.addRow("Histogram Bins:", self.histogramBinsSpinBox)
-
-        # Marker Size
-        self.markerSizeSpinBox = QSpinBox()
-        self.markerSizeSpinBox.setMinimum(1)
-        self.markerSizeSpinBox.setMaximum(100)
-        self.markerSizeSpinBox.setValue(3)
-        formLayout.addRow("Marker Size:", self.markerSizeSpinBox)
-
-        # Linear Fit
-        self.linearFitCheckBox = QCheckBox("Enable Linear Fit in the Frequency Plots")
-        formLayout.addRow(self.linearFitCheckBox)
-
-        # Fit between two points
-        self.fitBetweenPointsCheckBox = QCheckBox("Fit Between Two Points")
-        formLayout.addRow(self.fitBetweenPointsCheckBox)
-
-        # Start point for fit
-        self.fitStartPointSpinBox = QDoubleSpinBox()
-        self.fitStartPointSpinBox.setMinimum(-np.inf)
-        self.fitStartPointSpinBox.setMaximum(np.inf)
-        self.fitStartPointSpinBox.setValue(0)
-
-        # End point for fit
-        self.fitEndPointSpinBox = QDoubleSpinBox()
-        self.fitEndPointSpinBox.setMinimum(-np.inf)
-        self.fitEndPointSpinBox.setMaximum(np.inf)
-        self.fitEndPointSpinBox.setValue(1)
-
-        self.fitRangeLabel = QLabel("Fit Range:")
-        self.fitRangeLayout = QHBoxLayout()
-        self.fitRangeLayout.addWidget(self.fitRangeLabel)
-        self.fitRangeLayout.addWidget(self.fitStartPointSpinBox)
-        self.fitRangeLayout.addWidget(self.fitEndPointSpinBox)
-        formLayout.addRow(self.fitRangeLayout)
-
-        self.fitBetweenPointsCheckBox.stateChanged.connect(self.toggleFitRangeVisibility)
-        self.toggleFitRangeVisibility(False)
-
-        self.overlayPlotsCheckBox = QCheckBox("Overlay Plots")
-        formLayout.addRow(self.overlayPlotsCheckBox)
-
-        self.alphaSpin = QDoubleSpinBox()
-        self.alphaSpin.setMinimum(0.0)
-        self.alphaSpin.setMaximum(1.0)
-        self.alphaSpin.setSingleStep(0.1)
-        self.alphaSpin.setValue(0.5)  # Default alpha value
-        formLayout.addRow("Alpha:", self.alphaSpin)
-
-        # Save directory input and button
-        self.saveDirectoryLineEdit = QLineEdit()
-        self.saveDirectoryButton = QPushButton("Select Save Folder")
-        self.saveDirectoryButton.clicked.connect(self.selectSaveFolder)
-        saveFolderLayout = QHBoxLayout()
-        saveFolderLayout.addWidget(self.saveDirectoryLineEdit)
-        saveFolderLayout.addWidget(self.saveDirectoryButton)
-        formLayout.addRow("Save Figures To:", saveFolderLayout)
-
-        # Update plots button
-        updatePlotsButton = QPushButton("Update Plots")
-        updatePlotsButton.clicked.connect(self.updatePlots)
-        formLayout.addRow("", updatePlotsButton)  # Add an empty label for alignment
-
-        # Save figures button
-        saveFiguresButton = QPushButton("Save Figures")
-        saveFiguresButton.clicked.connect(self.saveAllFigures)
-        formLayout.addRow("", saveFiguresButton)  # Add an empty label for alignment
-
-        layout.addLayout(formLayout)
-
-        # Adjust overall layout settings
-        layout.setSpacing(10)  # Adjust the spacing as needed
-        tab.setLayout(layout)
-
-    def toggleFitRangeVisibility(self, visible):
-        self.fitRangeLabel.setVisible(visible)
-        self.fitStartPointSpinBox.setVisible(visible)
-        self.fitEndPointSpinBox.setVisible(visible)
-
-
-    def selectSaveFolder(self):
-        folder = QFileDialog.getExistingDirectory(self, "Select Folder")
-        if folder:
-            self.saveDirectoryLineEdit.setText(folder)
-
-    def saveAllFigures(self):
-        saveFolder = self.saveDirectoryLineEdit.text().strip()
-        if not saveFolder:
-            QMessageBox.information(self, "Info", "Please select a folder to save the figures.")
-            return
-
-        for i in range(self.rightPanel.count()):
-            tab = self.rightPanel.widget(i)
-            if hasattr(tab, "property"):
-                tabCanvases = tab.property("canvases")
-                if tabCanvases:
-                    tabFolder = os.path.join(saveFolder, self.rightPanel.tabText(i))
-                    if not os.path.exists(tabFolder):
-                        os.makedirs(tabFolder)
-                    for j, canvas in enumerate(tabCanvases):
-                        figure = canvas.figure
-                        figure.savefig(os.path.join(tabFolder, f"figure_{j+1}.png"), dpi=300, bbox_inches='tight')
-        QMessageBox.information(self, "Info", "Figures saved successfully.")
-
-
-           
-    def selectFolder(self):
-        folderPath = QFileDialog.getExistingDirectory(self, "Select Folder")
-        if folderPath:
-            self.populateFileList(folderPath,self.includeSubfoldersCheckbox.isChecked() )
-
-    def populateFileList(self, folderPath, includeSubfolders):
-        self.fileListWidget.clear()
-        if includeSubfolders:
-            for root, dirs, files in os.walk(folderPath):
-                for file in files:
-                    if file.endswith('.dataset.npz'):
-                        fullPath = os.path.join(root, file)
-                        self.fileListWidget.addItem(fullPath)
-        else:
-            for file in os.listdir(folderPath):
-                if file.endswith('.dataset.npz'):
-                    fullPath = os.path.join(folderPath, file)
-                    self.fileListWidget.addItem(fullPath)
-    
-    def updateSelectionOrder(self):
-        # Get the current selection
-        currentSelection = {self.fileListWidget.item(i).text() for i in range(self.fileListWidget.count()) if self.fileListWidget.item(i).isSelected()}
-        
-        # Filter out any deselected items
-        self.selectedFilesOrder = [f for f in self.selectedFilesOrder if f in currentSelection]
-        
-        # Add new selections in order
-        for i in range(self.fileListWidget.count()):
-            itemText = self.fileListWidget.item(i).text()
-            if self.fileListWidget.item(i).isSelected() and itemText not in self.selectedFilesOrder:
-                self.selectedFilesOrder.append(itemText)
-    
-
-    def updatePlots(self):
-        # Update the class attributes with the new values from the UI
-        self.histogram_bins = self.histogramBinsSpinBox.value()
-        self.scatter_marker_size = self.markerSizeSpinBox.value()
-
-        # Re-plot all selected files with the new settings
-        self.plotSelectedFiles()
-
-
-    @staticmethod
-    def create_joint_plot(self, fig, data_x, data_y, min_x, max_x, min_y, max_y, plotType, alpha):
-        # Create grid layout for the plots
-        gs = fig.add_gridspec(4, 4)
-        
-        # Main scatter plot with specified axis limits
-        ax_scatter = fig.add_subplot(gs[1:4, 0:3])
-        if data_x is not None and data_y is not None:
-            ax_scatter.scatter(data_x, data_y, s=int(self.markerSizeSpinBox.value()), alpha=alpha)
-        ax_scatter.set_xlim(min_x, max_x)
-        ax_scatter.set_ylim(min_y, max_y)
-        
-        # Histogram for X distribution
-        ax_histx = fig.add_subplot(gs[0, 0:3], sharex=ax_scatter)
-        if data_x is not None:
-            ax_histx.hist(data_x, bins=self.histogramBinsSpinBox.value())
-        ax_histx.set_ylabel(' ')
-        
-        # Histogram for Y distribution
-        ax_histy = fig.add_subplot(gs[1:4, 3], sharey=ax_scatter)
-        if data_y is not None:
-            ax_histy.hist(data_y, bins=self.histogramBinsSpinBox.value(), orientation='horizontal')
-        ax_histy.set_xlabel(' ')
-        
-        # Hide tick labels for histograms to avoid overlap
-        plt.setp(ax_histx.get_xticklabels(), visible=False)
-        plt.setp(ax_histy.get_yticklabels(), visible=False)
-
-        ax_scatter.xaxis.set_major_formatter(ScalarFormatter(useMathText=True))
-        ax_scatter.yaxis.set_major_formatter(ScalarFormatter(useMathText=True))
-        if 'dI vs dt' in plotType and 'log' not in plotType:
-            ax_scatter.set_xlabel('Δt (ms)')
-            ax_scatter.set_ylabel('ΔI (nA)')
-        elif 'area vs dt' in plotType:
-            ax_scatter.set_xlabel('Δt (ms)')
-            ax_scatter.set_ylabel('Area (C)')
-        elif 'dI vs dt (log)' in plotType:
-            ax_scatter.set_xlabel('Δt (ms) [log]')
-            ax_scatter.set_ylabel('ΔI (nA)')
-
-        ax_scatter.ticklabel_format(style='sci', axis='both', scilimits=(0,0))
-        ax_histx.ticklabel_format(style='sci', axis='both', scilimits=(0,0))
-        ax_histy.ticklabel_format(style='sci', axis='both', scilimits=(0,0))
-        fig.tight_layout()
-
-        # Return the axes dictionary
-        return {'ax_scatter': ax_scatter, 'ax_histx': ax_histx, 'ax_histy': ax_histy}
-    
-    def plotSelectedFiles(self):
+    def plotSelectedFiles (self ):
         '''selectedFiles = [self.fileListWidget.item(i).text() for i in range(self.fileListWidget.count()) if self.fileListWidget.item(i).isSelected()]
         plotOptions = {key: option.isChecked() for key, option in self.plotOptions.items() if option.isChecked()}'''
 
-        plotOptions = {key: option.isChecked() for key, option in self.plotOptions.items() if option.isChecked()}
-        self.rightPanel.clear()
+        plotOptions ={key :option .isChecked ()for key ,option in self .plotOptions .items ()if option .isChecked ()}
+        self .rightPanel .clear ()
 
-        self.rightPanel.clear()
+        self .rightPanel .clear ()
 
-        if not self.selectedFilesOrder or not plotOptions:
-            return
+        if not self .selectedFilesOrder or not plotOptions :
+            return 
 
-        data = self.prepareData(self.selectedFilesOrder, plotOptions)
-
-        for plotType, plotData in data.items():
-            tab = QWidget()
-            layout = QVBoxLayout(tab)
-            plotLayout = QGridLayout()
-            alpha = self.alphaSpin.value()
-            tabCanvases = []
-
-            if self.overlayPlotsCheckBox.isChecked():
-                # Create a single figure and canvas for overlaid plots
-                fig = Figure(figsize=(10, 5))
-                canvas = FigureCanvas(fig)
-                tabCanvases.append(canvas)
-
-                min_x, max_x, min_y, max_y = self.calculateGlobalAxisLimits(plotData, plotType)
-
-                if 'Scatter plot dI vs dt' in plotType and 'log' not in plotType:
-                    axes_dict = self.create_joint_plot(self, fig, None, None, min_x, max_x, min_y, max_y, 'dI vs dt', alpha)
-                    ax_scatter = axes_dict['ax_scatter']
-                    ax_histx = axes_dict['ax_histx']
-                    ax_histy = axes_dict['ax_histy']
-
-                    for filePath, values in plotData.items():
-                        alpha = self.alphaSpin.value()
-                        label = os.path.basename(filePath)
-
-                        ax_scatter.scatter(values[0], values[1], s=int(self.markerSizeSpinBox.value()), alpha=alpha, label=label)
-                        ax_histx.hist(values[0], bins=self.histogramBinsSpinBox.value(), alpha=alpha)
-                        ax_histy.hist(values[1], bins=self.histogramBinsSpinBox.value(), orientation='horizontal', alpha=alpha)
-                    fig.tight_layout()
-                    ax_scatter.legend()
-
-                elif 'Scatter plot area vs dt' in plotType:
-                    axes_dict = self.create_joint_plot(self, fig, None, None, min_x, max_x, min_y, max_y, 'area vs dt', alpha)
-                    ax_scatter = axes_dict['ax_scatter']
-                    ax_histx = axes_dict['ax_histx']
-                    ax_histy = axes_dict['ax_histy']
-
-                    for filePath, values in plotData.items():
-                        alpha = self.alphaSpin.value()
-                        label = os.path.basename(filePath)
-
-                        ax_scatter.scatter(values[0], values[1], s=int(self.markerSizeSpinBox.value()), alpha=alpha, label=label)
-                        ax_histx.hist(values[0], bins=self.histogramBinsSpinBox.value(), alpha=alpha)
-                        ax_histy.hist(values[1], bins=self.histogramBinsSpinBox.value(), orientation='horizontal', alpha=alpha)
-                    fig.tight_layout()
-                    ax_scatter.legend()
-
-                elif 'Scatter plot dI vs dt (log)' in plotType:
-                    axes_dict = self.create_joint_plot(self, fig, None, None, np.log(min_x), np.log(max_x), min_y, max_y, 'dI vs dt (log)', alpha)
-                    ax_scatter = axes_dict['ax_scatter']
-                    ax_histx = axes_dict['ax_histx']
-                    ax_histy = axes_dict['ax_histy']
-
-                    for filePath, values in plotData.items():
-                        alpha = self.alphaSpin.value()
-                        label = os.path.basename(filePath)
-
-                        ax_scatter.scatter(np.log(values[0]), values[1], s=int(self.markerSizeSpinBox.value()), alpha=alpha, label=label)
-                        ax_histx.hist(np.log(values[0]), bins=self.histogramBinsSpinBox.value(), alpha=alpha)
-                        ax_histy.hist(values[1], bins=self.histogramBinsSpinBox.value(), orientation='horizontal', alpha=alpha)
-                    fig.tight_layout()
-                    ax_scatter.legend()
-                    
-
-                elif 'Histogram of dt (log)' in plotType:
-                    ax = fig.add_subplot(111)
-
-                    for filePath, values in plotData.items():
-                        alpha = self.alphaSpin.value()
-                        label = os.path.basename(filePath)
-
-                        log_values = np.log(values[values > 0])
-                        ax.hist(log_values, bins=self.histogramBinsSpinBox.value(), range=(np.log(min_x), np.log(max_x)), alpha=alpha, label=label)
-                    fig.tight_layout()
-                    ax.legend()
-
-                elif 'Frequency plot' in plotType:
-                    ax = fig.add_subplot(111)
-
-                    for filePath, values in plotData.items():
-                        alpha = self.alphaSpin.value()
-                        label = os.path.basename(filePath)
-
-                        ax.plot(values[0], values[1], 'o', markersize=self.scatter_marker_size, alpha=alpha, label=label)
-
-                        if self.linearFitCheckBox.isChecked():
-                            if self.fitBetweenPointsCheckBox.isChecked():
-                                start_point = self.fitStartPointSpinBox.value()
-                                end_point = self.fitEndPointSpinBox.value()
-                                mask = (values[0] >= start_point) & (values[0] <= end_point)
-                                x_fit = values[0][mask]
-                                y_fit = values[1][mask]
-                                slope, intercept = np.polyfit(x_fit, y_fit, 1)
-                            else:
-                                slope, intercept = np.polyfit(values[0], values[1], 1)
-                                x_fit = np.array([min_x, max_x])
-                                y_fit = slope * x_fit + intercept
-
-                            ax.plot(x_fit, slope * x_fit + intercept, '--', alpha=alpha)
-
-                    ax.legend()
-
-                else:  # Regular histogram
-                    ax = fig.add_subplot(111)
-
-                    for filePath, values in plotData.items():
-                        alpha = self.alphaSpin.value()
-                        label = os.path.basename(filePath)
-
-                        ax.hist(values, bins=self.histogramBinsSpinBox.value(), range=(min_x, max_x), alpha=alpha, label=label)
-
-                    ax.legend()
-
-                fig.suptitle("Overlaid Plots", fontsize=12)
-                fig.tight_layout()
-                fig.tight_layout()
-                fig.tight_layout()
-                fig.tight_layout()
-                fig.tight_layout()
-                plotLayout.addWidget(canvas, 0, 0)
-                
-
-                
-            else:
-                row = col = 0
-                max_col = 1
-                
-                min_x, max_x, min_y, max_y = self.calculateGlobalAxisLimits(plotData, plotType)
-
-                for filePath, values in plotData.items():
-                    fig = Figure(figsize=(5, 5))
-                    canvas = FigureCanvas(fig)
-
-                    if 'Scatter plot dI vs dt' in plotType and 'log' not in plotType:
-                        axes_dict = self.create_joint_plot(self, fig, values[0], values[1], min_x, max_x, min_y, max_y, 'dI vs dt', alpha=1.0)
-                        canvas.axes_dict = axes_dict
-                        canvas.plotType = 'Scatter plot dI vs dt'
-                        title = f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
-
-                    elif 'Scatter plot area vs dt' in plotType:
-                        axes_dict = self.create_joint_plot(self, fig, values[0], values[1], min_x, max_x, min_y, max_y, 'area vs dt', alpha=1.0)
-                        canvas.axes_dict = axes_dict
-                        canvas.plotType = 'Scatter plot area vs dt'
-                        title = f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
-
-                    elif 'Scatter plot dI vs dt (log)' in plotType:
-                        axes_dict = self.create_joint_plot(self, fig, np.log(values[0]), values[1], np.log(min_x), np.log(max_x), min_y, max_y, 'dI vs dt (log)', alpha=1.0)
-                        canvas.axes_dict = axes_dict
-                        canvas.plotType = 'Scatter plot dI vs dt (log)'
-                        title = f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
-
-                    elif 'Histogram of dt (log)' in plotType:
-                        log_values = np.log(values[values > 0])
-                        axes_dict = self.create_histogram(fig, log_values, np.log(min_x), np.log(max_x), 'dt (log)', alpha)
-                        canvas.axes_dict = axes_dict
-                        canvas.plotType = 'Histogram of dt (log)'
-                        title = f"{os.path.basename(filePath)}\nEvents: {len(log_values)}"
-
-                    elif 'Frequency plot' in plotType:
-                        self.create_frequency_plot(fig, values[0], values[1], min_x, max_x, min_y, max_y, alpha=1.0)
-                        canvas.plotType = 'Frequency plot'
-                        title = f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
-                        if self.linearFitCheckBox.isChecked():
-                            if self.fitBetweenPointsCheckBox.isChecked():
-                                start_point = self.fitStartPointSpinBox.value()
-                                end_point = self.fitEndPointSpinBox.value()
-                                mask = (values[0] >= start_point) & (values[0] <= end_point)
-                                x_fit = values[0][mask]
-                                y_fit = values[1][mask]
-                                slope, intercept = np.polyfit(x_fit, y_fit, 1)
-                            else:
-                                slope, intercept = np.polyfit(values[0], values[1], 1)
-                                x_fit = np.array([min_x, max_x])
-                                y_fit = slope * x_fit + intercept
-
-                            ax = fig.axes[0]
-                            ax.plot(x_fit, slope * x_fit + intercept, 'r--', label=f'Fit: {slope:.2f} Events/s, Intercept: {intercept:.2f}')
-                            ax.legend()
-                            title += f"\nFit: {slope:.2f} Events/s, Intercept: {intercept:.2f}"
-
-                    else:
-                        # Regular histogram
-                        axes_dict = self.create_histogram(fig, values, min_x, max_x, plotType, alpha=1.0)
-                        canvas.axes_dict = axes_dict
-                        canvas.plotType = plotType
-                        title = f"{os.path.basename(filePath)}\nEvents: {len(values)}"
-
-                    fig.suptitle(title, fontsize=8)
-                    
-                    plotLayout.addWidget(canvas, row, col)
-                    tabCanvases.append(canvas)
-
-                    col += 1
-                    if col > max_col:
-                        col = 0
-                        row += 1
-                    
-                    # Adjust layout
-                    fig.tight_layout()
-
-            layout.addLayout(plotLayout)
-
-            if tabCanvases:
-                toolbar = NavigationToolbar(tabCanvases[0], self)
-                layout.addWidget(toolbar)
-
-            fig.tight_layout()
-
-            resetButton = QPushButton("Reset Zoom")
-            resetButton.clicked.connect(self.resetZoom)
-            layout.addWidget(resetButton)
-
-            self.rightPanel.addTab(tab, plotType)
-            tab.setProperty("canvases", tabCanvases)
-
-
-    def create_frequency_plot(self, fig, times, event_numbers, min_x, max_x, min_y, max_y, alpha):
-        ax = fig.add_subplot(111)
-        ax.plot(times, event_numbers, 'o', markersize=self.scatter_marker_size, alpha = alpha)
-        ax.set_xlim(min_x, max_x)
-        #ax.set_ylim(min_y, max_y)
-        ax.set_xlabel('Time (s)')
-        ax.set_ylabel('Event Number')
-        ax.ticklabel_format(style='sci', axis='both', scilimits=(0,0))
-        fig.tight_layout()
-    
-
-    def syncZoomAcrossPlots(self):
-        currentTab = self.rightPanel.currentWidget()
-        if hasattr(currentTab, "property"):
-            tabCanvases = currentTab.property("canvases")
-            if tabCanvases and len(tabCanvases) > 0:
-                # Assuming the first canvas' figure's first axes as the reference
-                referenceAxes = tabCanvases[0].figure.axes[0]
-                xlim = referenceAxes.get_xlim()
-                ylim = referenceAxes.get_ylim()
-                
-                for canvas in tabCanvases:
-                    plotType = getattr(canvas, 'plotType', '')
-                    if 'Scatter plot' in plotType:
-                        if hasattr(canvas, 'axes_dict'):
-                            canvas.axes_dict['ax_scatter'].set_xlim(xlim)
-                            canvas.axes_dict['ax_scatter'].set_ylim(ylim)
-                            canvas.axes_dict['ax_histx'].set_xlim(xlim)
-                            canvas.axes_dict['ax_histy'].set_ylim(ylim)  # Reverse y-limits for horizontal histogram
-                    elif 'Histogram' in plotType or 'Frequency plot' in plotType:
-                        # For histograms and frequency plots, synchronize only the X-axis
-                        ax = canvas.figure.axes[0]
-                        ax.set_xlim(xlim)
-                    else:
-                        # For other plots, synchronize both axes
-                        for ax in canvas.figure.axes:
-                            ax.set_xlim(xlim)
-                            ax.set_ylim(ylim)
-
-                    canvas.draw_idle()
-
-  
-
-    def create_histogram(self, fig, values, min_x, max_x, plotType, alpha):
-        ax = fig.add_subplot(111)
-        ax.hist(values, bins=self.histogramBinsSpinBox.value(), range=(min_x, max_x),  alpha = alpha)
-        ax.xaxis.set_major_formatter(ScalarFormatter(useMathText=True))
-        if 'dI' in plotType:
-            ax.set_xlabel('ΔI (nA)')
-        elif 'dt' in plotType and 'log' not in plotType:
-            ax.set_xlabel('Δt (s)')
-        elif 'dt (log)' in plotType:
-            ax.set_xlabel('log(Δt (ms))')
-        ax.set_ylabel('Count')
-        ax.ticklabel_format(style='sci', axis='both', scilimits=(0,0))
-        fig.tight_layout()
-
-        # Return the axis dictionary
-        return {'ax_hist': ax}
-
-
-    def resetZoom(self):
-        currentTab = self.rightPanel.currentWidget()
-        if currentTab is None:
-            return
-
-        plotType = self.rightPanel.tabText(self.rightPanel.indexOf(currentTab))
-
-        if plotType in self.global_limits:
-            min_x, max_x, min_y, max_y = self.global_limits[plotType]
-
-            tabCanvases = currentTab.property("canvases")
-            if tabCanvases:
-                for canvas in tabCanvases:
-                    if plotType == 'Scatter plot dI vs dt' or plotType == 'Scatter plot area vs dt' or plotType == 'Scatter plot dI vs dt (log)':
-                        if hasattr(canvas, 'axes_dict'):
-                            canvas.axes_dict['ax_scatter'].set_xlim(min_x, max_x)
-                            canvas.axes_dict['ax_scatter'].set_ylim(min_y, max_y)
-                            canvas.axes_dict['ax_histx'].set_xlim(min_x, max_x)
-                            canvas.axes_dict['ax_histy'].set_ylim(min_y, max_y)
-                    elif plotType == 'Frequency plot':
-                        ax = canvas.figure.axes[0]
-                        ax.set_xlim(min_x, max_x)
-                        #ax.set_ylim(min_y, max_y)
-                    elif plotType in ['Histogram of dI', 'Histogram of dt', 'Histogram of Area', 'Histogram of dt (log)']:
-                        ax = canvas.figure.axes[0]
-                        ax.set_xlim(min_x, max_x)
-                    else:
-                        print(f"Unsupported plot type: {plotType}")
-
-                    canvas.draw_idle()
-
-    
-    def prepareData(self, selectedFiles, plotOptions):
-        data = {}
-        for filePath in selectedFiles:
-            fileData = np.load(filePath)
-            X = fileData['X']
-            
-            for option in plotOptions:
-                if option not in data:
-                    data[option] = {}
-                
-                if 'Histogram' in option:
-                    index = 0 if 'dI' in option else 3 if 'Area' in option else 4  # Assuming the order dI, dt, Area
-                    values = X[:, index].astype(float)
-                    # Remove NaN values
-                    values = values[~np.isnan(values)]
-                    data[option][filePath] = values
-                    #print(f"Data type for {option}: {type(values)}")
-                elif 'Histogram of dt (log)' in option:
-                    # Assuming dt values are in the second column (index 1)
-                    dt_values = fileData['X'][:, 4]
-                    # Filter out non-positive values to avoid log(0) and log(negative)
-                    positive_dt_values = dt_values[dt_values > 0]
-                    # Apply logarithmic transformation
-                    log_dt_values = np.log(positive_dt_values*1e3)
-                    # Remove NaN values
-                    log_dt_values = log_dt_values[~np.isnan(log_dt_values)]
-                    data['Histogram of dt (log)'][filePath] = log_dt_values.astype(float)
-                    #print(f"Data type for Histogram of dt (log): {type(log_dt_values)}")
-                elif 'Frequency plot' in option:
-                    event_numbers = np.arange(1, len(fileData['X']) + 1).astype(float)
-                    times = fileData['X'][:, -1].astype(float)
-                    # Remove NaN values
-                    valid_indices = ~np.isnan(times)
-                    event_numbers = event_numbers[valid_indices]
-                    times = times[valid_indices]
-                    data[option][filePath] = (times, event_numbers)
-                    #print(f"Data type for Frequency plot: {type(times)}, {type(event_numbers)}")
-                else:  # Scatter plots
-                    x_index, y_index = (4, 0) if 'dI vs dt' in option else (4, 3)  # Assuming dI vs dt, Area vs dt
-                    x_values = X[:, x_index]*1e3
-                    y_values = X[:, y_index]
-                    # Remove NaN values
-                    valid_indices = ~np.isnan(x_values) & ~np.isnan(y_values)
-                    x_values = x_values[valid_indices]
-                    y_values = y_values[valid_indices]
-                    data[option][filePath] = (x_values, y_values)
-                    #print(f"Data type for {option}: {type(x_values)}, {type(y_values)}")
-                    
-        return data
-    
-    def calculateGlobalAxisLimits(self, plotData, plotType):
-        min_x = min_y = np.inf
-        max_x = max_y = -np.inf
-        for values in plotData.values():
-            if isinstance(values, dict):
-                # If values is a dictionary, iterate over its values
-                for subvalues in values.values():
-                    if 'Histogram' in plotType:
-                        curr_min_x = np.min(subvalues)
-                        curr_max_x = np.max(subvalues)
-                        #print(f"curr_min_x: {curr_min_x}, curr_max_x: {curr_max_x}")
-                        if not np.isfinite(curr_min_x) or not np.isfinite(curr_max_x):
-                            continue  # Skip this file if min_x or max_x is inf or -inf
-                        if curr_min_x < curr_max_x:
-                            min_x = min(min_x, curr_min_x)
-                            max_x = max(max_x, curr_max_x)
-                        else:
-                            min_x = min(min_x, curr_min_x)
-                            max_x = max(max_x, curr_min_x + 1e-6)  # Adjust max_x to be slightly larger than min_x
-                    elif 'Frequency plot' in plotType:
-                        x, y = subvalues
-                        min_x = min(min_x, np.min(x))
-                        max_x = max(max_x, np.max(x))
-                        curr_min_y = np.min(y)
-                        curr_max_y = np.max(y)
-                        if not np.isfinite(curr_min_y) or not np.isfinite(curr_max_y):
-                            continue  # Skip this file if min_y or max_y is inf or -inf
-                        min_y = min(min_y, curr_min_y)
-                        max_y = max(max_y, curr_max_y)
-                    else:  # Scatter plots
-                        x, y = subvalues
-                        min_x = min(min_x, np.min(x))
-                        max_x = max(max_x, np.max(x))
-                        curr_min_y = np.min(y)
-                        curr_max_y = np.max(y)
-                        if not np.isfinite(curr_min_y) or not np.isfinite(curr_max_y):
-                            continue  # Skip this file if min_y or max_y is inf or -inf
-                        min_y = min(min_y, curr_min_y)
-                        max_y = max(max_y, curr_max_y)
-            else:
-                if 'Histogram' in plotType:
-                    curr_min_x = np.min(values)
-                    curr_max_x = np.max(values)
-                    #print(f"curr_min_x: {curr_min_x}, curr_max_x: {curr_max_x}")
-                    if not np.isfinite(curr_min_x) or not np.isfinite(curr_max_x):
-                        continue  # Skip this file if min_x or max_x is inf or -inf
-                    if curr_min_x < curr_max_x:
-                        min_x = min(min_x, curr_min_x)
-                        max_x = max(max_x, curr_max_x)
-                    else:
-                        min_x = min(min_x, curr_min_x)
-                        max_x = max(max_x, curr_min_x + 1e-6)  # Adjust max_x to be slightly larger than min_x
-                elif 'Frequency plot' in plotType:
-                    x, y = values
-                    min_x = min(min_x, np.min(x))
-                    max_x = max(max_x, np.max(x))
-                    curr_min_y = np.min(y)
-                    curr_max_y = np.max(y)
-                    if not np.isfinite(curr_min_y) or not np.isfinite(curr_max_y):
-                        continue  # Skip this file if min_y or max_y is inf or -inf
-                    min_y = min(min_y, curr_min_y)
-                    max_y = max(max_y, curr_max_y)
-                else:  # Scatter plots
-                    x, y = values
-                    min_x = min(min_x, np.min(x))
-                    max_x = max(max_x, np.max(x))
-                    curr_min_y = np.min(y)
-                    curr_max_y = np.max(y)
-                    if not np.isfinite(curr_min_y) or not np.isfinite(curr_max_y):
-                        continue  # Skip this file if min_y or max_y is inf or -inf
-                    min_y = min(min_y, curr_min_y)
-                    max_y = max(max_y, curr_max_y)
-
-        if not np.isfinite(min_x) or not np.isfinite(max_x):
-            min_x, max_x = 0, 1  # Set default values if min_x or max_x is inf or -inf
-        if not np.isfinite(min_y) or not np.isfinite(max_y):
-            min_y, max_y = 0, 1  # Set default values if min_y or max_y is inf or -inf
-
-        # Store the global limits in the dictionary
-        self.global_limits[plotType] = (min_x, max_x, min_y, max_y)
-
-        return min_x, max_x, min_y, max_y
-    
-
-if __name__ == "__main__":
-
-    app = QApplication(sys.argv)
-    app.setStyle(QStyleFactory.create('Fusion'))  # Use Fusion or other available styles
-
-    # Customize the palette for a darker, more modern look
-    palette = QPalette()
-    palette.setColor(QPalette.ColorRole.Window, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.WindowText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Base, QColor(25, 25, 25))
-    palette.setColor(QPalette.ColorRole.AlternateBase, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.ToolTipBase, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.ToolTipText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Text, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.Button, QColor(53, 53, 53))
-    palette.setColor(QPalette.ColorRole.ButtonText, Qt.GlobalColor.white)
-    palette.setColor(QPalette.ColorRole.BrightText, Qt.GlobalColor.red)
-    palette.setColor(QPalette.ColorRole.Link, QColor(42, 130, 218))
-    palette.setColor(QPalette.ColorRole.Highlight, QColor(42, 130, 218))
-    palette.setColor(QPalette.ColorRole.HighlightedText, Qt.GlobalColor.black)
-    app.setPalette(palette)
-    
-    mainWindow = PlottingApplication()
-    mainWindow.showMaximized()
-    sys.exit(app.exec())
+        data =self .prepareData (self .selectedFilesOrder ,plotOptions )
+
+        for plotType ,plotData in data .items ():
+            tab =QWidget ()
+            layout =QVBoxLayout (tab )
+            plotLayout =QGridLayout ()
+            alpha =self .alphaSpin .value ()
+            tabCanvases =[]
+
+            if self .overlayPlotsCheckBox .isChecked ():
+
+                fig =Figure (figsize =(10 ,5 ))
+                canvas =FigureCanvas (fig )
+                tabCanvases .append (canvas )
+
+                min_x ,max_x ,min_y ,max_y =self .calculateGlobalAxisLimits (plotData ,plotType )
+
+                if 'Scatter plot dI vs dt'in plotType and 'log'not in plotType :
+                    axes_dict =self .create_joint_plot (self ,fig ,None ,None ,min_x ,max_x ,min_y ,max_y ,'dI vs dt',alpha )
+                    ax_scatter =axes_dict ['ax_scatter']
+                    ax_histx =axes_dict ['ax_histx']
+                    ax_histy =axes_dict ['ax_histy']
+
+                    for filePath ,values in plotData .items ():
+                        alpha =self .alphaSpin .value ()
+                        label =os .path .basename (filePath )
+
+                        ax_scatter .scatter (values [0 ],values [1 ],s =int (self .markerSizeSpinBox .value ()),alpha =alpha ,label =label )
+                        ax_histx .hist (values [0 ],bins =self .histogramBinsSpinBox .value (),alpha =alpha )
+                        ax_histy .hist (values [1 ],bins =self .histogramBinsSpinBox .value (),orientation ='horizontal',alpha =alpha )
+                    fig .tight_layout ()
+                    ax_scatter .legend ()
+
+                elif 'Scatter plot area vs dt'in plotType :
+                    axes_dict =self .create_joint_plot (self ,fig ,None ,None ,min_x ,max_x ,min_y ,max_y ,'area vs dt',alpha )
+                    ax_scatter =axes_dict ['ax_scatter']
+                    ax_histx =axes_dict ['ax_histx']
+                    ax_histy =axes_dict ['ax_histy']
+
+                    for filePath ,values in plotData .items ():
+                        alpha =self .alphaSpin .value ()
+                        label =os .path .basename (filePath )
+
+                        ax_scatter .scatter (values [0 ],values [1 ],s =int (self .markerSizeSpinBox .value ()),alpha =alpha ,label =label )
+                        ax_histx .hist (values [0 ],bins =self .histogramBinsSpinBox .value (),alpha =alpha )
+                        ax_histy .hist (values [1 ],bins =self .histogramBinsSpinBox .value (),orientation ='horizontal',alpha =alpha )
+                    fig .tight_layout ()
+                    ax_scatter .legend ()
+
+                elif 'Scatter plot dI vs dt (log)'in plotType :
+                    axes_dict =self .create_joint_plot (self ,fig ,None ,None ,np .log (min_x ),np .log (max_x ),min_y ,max_y ,'dI vs dt (log)',alpha )
+                    ax_scatter =axes_dict ['ax_scatter']
+                    ax_histx =axes_dict ['ax_histx']
+                    ax_histy =axes_dict ['ax_histy']
+
+                    for filePath ,values in plotData .items ():
+                        alpha =self .alphaSpin .value ()
+                        label =os .path .basename (filePath )
+
+                        ax_scatter .scatter (np .log (values [0 ]),values [1 ],s =int (self .markerSizeSpinBox .value ()),alpha =alpha ,label =label )
+                        ax_histx .hist (np .log (values [0 ]),bins =self .histogramBinsSpinBox .value (),alpha =alpha )
+                        ax_histy .hist (values [1 ],bins =self .histogramBinsSpinBox .value (),orientation ='horizontal',alpha =alpha )
+                    fig .tight_layout ()
+                    ax_scatter .legend ()
+
+
+                elif 'Histogram of dt (log)'in plotType :
+                    ax =fig .add_subplot (111 )
+
+                    for filePath ,values in plotData .items ():
+                        alpha =self .alphaSpin .value ()
+                        label =os .path .basename (filePath )
+
+                        log_values =np .log (values [values >0 ])
+                        ax .hist (log_values ,bins =self .histogramBinsSpinBox .value (),range =(np .log (min_x ),np .log (max_x )),alpha =alpha ,label =label )
+                    fig .tight_layout ()
+                    ax .legend ()
+
+                elif 'Frequency plot'in plotType :
+                    ax =fig .add_subplot (111 )
+
+                    for filePath ,values in plotData .items ():
+                        alpha =self .alphaSpin .value ()
+                        label =os .path .basename (filePath )
+
+                        ax .plot (values [0 ],values [1 ],'o',markersize =self .scatter_marker_size ,alpha =alpha ,label =label )
+
+                        if self .linearFitCheckBox .isChecked ():
+                            if self .fitBetweenPointsCheckBox .isChecked ():
+                                start_point =self .fitStartPointSpinBox .value ()
+                                end_point =self .fitEndPointSpinBox .value ()
+                                mask =(values [0 ]>=start_point )&(values [0 ]<=end_point )
+                                x_fit =values [0 ][mask ]
+                                y_fit =values [1 ][mask ]
+                                slope ,intercept =np .polyfit (x_fit ,y_fit ,1 )
+                            else :
+                                slope ,intercept =np .polyfit (values [0 ],values [1 ],1 )
+                                x_fit =np .array ([min_x ,max_x ])
+                                y_fit =slope *x_fit +intercept 
+
+                            ax .plot (x_fit ,slope *x_fit +intercept ,'--',alpha =alpha )
+
+                    ax .legend ()
+
+                else :
+                    ax =fig .add_subplot (111 )
+
+                    for filePath ,values in plotData .items ():
+                        alpha =self .alphaSpin .value ()
+                        label =os .path .basename (filePath )
+
+                        ax .hist (values ,bins =self .histogramBinsSpinBox .value (),range =(min_x ,max_x ),alpha =alpha ,label =label )
+
+                    ax .legend ()
+
+                fig .suptitle ("Overlaid Plots",fontsize =12 )
+                fig .tight_layout ()
+                fig .tight_layout ()
+                fig .tight_layout ()
+                fig .tight_layout ()
+                fig .tight_layout ()
+                plotLayout .addWidget (canvas ,0 ,0 )
+
+
+
+            else :
+                row =col =0 
+                max_col =1 
+
+                min_x ,max_x ,min_y ,max_y =self .calculateGlobalAxisLimits (plotData ,plotType )
+
+                for filePath ,values in plotData .items ():
+                    fig =Figure (figsize =(5 ,5 ))
+                    canvas =FigureCanvas (fig )
+
+                    if 'Scatter plot dI vs dt'in plotType and 'log'not in plotType :
+                        axes_dict =self .create_joint_plot (self ,fig ,values [0 ],values [1 ],min_x ,max_x ,min_y ,max_y ,'dI vs dt',alpha =1.0 )
+                        canvas .axes_dict =axes_dict 
+                        canvas .plotType ='Scatter plot dI vs dt'
+                        title =f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
+
+                    elif 'Scatter plot area vs dt'in plotType :
+                        axes_dict =self .create_joint_plot (self ,fig ,values [0 ],values [1 ],min_x ,max_x ,min_y ,max_y ,'area vs dt',alpha =1.0 )
+                        canvas .axes_dict =axes_dict 
+                        canvas .plotType ='Scatter plot area vs dt'
+                        title =f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
+
+                    elif 'Scatter plot dI vs dt (log)'in plotType :
+                        axes_dict =self .create_joint_plot (self ,fig ,np .log (values [0 ]),values [1 ],np .log (min_x ),np .log (max_x ),min_y ,max_y ,'dI vs dt (log)',alpha =1.0 )
+                        canvas .axes_dict =axes_dict 
+                        canvas .plotType ='Scatter plot dI vs dt (log)'
+                        title =f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
+
+                    elif 'Histogram of dt (log)'in plotType :
+                        log_values =np .log (values [values >0 ])
+                        axes_dict =self .create_histogram (fig ,log_values ,np .log (min_x ),np .log (max_x ),'dt (log)',alpha )
+                        canvas .axes_dict =axes_dict 
+                        canvas .plotType ='Histogram of dt (log)'
+                        title =f"{os.path.basename(filePath)}\nEvents: {len(log_values)}"
+
+                    elif 'Frequency plot'in plotType :
+                        self .create_frequency_plot (fig ,values [0 ],values [1 ],min_x ,max_x ,min_y ,max_y ,alpha =1.0 )
+                        canvas .plotType ='Frequency plot'
+                        title =f"{os.path.basename(filePath)}\nEvents: {len(values[0])}"
+                        if self .linearFitCheckBox .isChecked ():
+                            if self .fitBetweenPointsCheckBox .isChecked ():
+                                start_point =self .fitStartPointSpinBox .value ()
+                                end_point =self .fitEndPointSpinBox .value ()
+                                mask =(values [0 ]>=start_point )&(values [0 ]<=end_point )
+                                x_fit =values [0 ][mask ]
+                                y_fit =values [1 ][mask ]
+                                slope ,intercept =np .polyfit (x_fit ,y_fit ,1 )
+                            else :
+                                slope ,intercept =np .polyfit (values [0 ],values [1 ],1 )
+                                x_fit =np .array ([min_x ,max_x ])
+                                y_fit =slope *x_fit +intercept 
+
+                            ax =fig .axes [0 ]
+                            ax .plot (x_fit ,slope *x_fit +intercept ,'r--',label =f'Fit: {slope:.2f} Events/s, Intercept: {intercept:.2f}')
+                            ax .legend ()
+                            title +=f"\nFit: {slope:.2f} Events/s, Intercept: {intercept:.2f}"
+
+                    else :
+
+                        axes_dict =self .create_histogram (fig ,values ,min_x ,max_x ,plotType ,alpha =1.0 )
+                        canvas .axes_dict =axes_dict 
+                        canvas .plotType =plotType 
+                        title =f"{os.path.basename(filePath)}\nEvents: {len(values)}"
+
+                    fig .suptitle (title ,fontsize =8 )
+
+                    plotLayout .addWidget (canvas ,row ,col )
+                    tabCanvases .append (canvas )
+
+                    col +=1 
+                    if col >max_col :
+                        col =0 
+                        row +=1 
+
+
+                    fig .tight_layout ()
+
+            layout .addLayout (plotLayout )
+
+            if tabCanvases :
+                toolbar =NavigationToolbar (tabCanvases [0 ],self )
+                layout .addWidget (toolbar )
+
+            fig .tight_layout ()
+
+            resetButton =QPushButton ("Reset Zoom")
+            resetButton .clicked .connect (self .resetZoom )
+            layout .addWidget (resetButton )
+
+            self .rightPanel .addTab (tab ,plotType )
+            tab .setProperty ("canvases",tabCanvases )
+
+
+    def create_frequency_plot (self ,fig ,times ,event_numbers ,min_x ,max_x ,min_y ,max_y ,alpha ):
+        ax =fig .add_subplot (111 )
+        ax .plot (times ,event_numbers ,'o',markersize =self .scatter_marker_size ,alpha =alpha )
+        ax .set_xlim (min_x ,max_x )
+
+        ax .set_xlabel ('Time (s)')
+        ax .set_ylabel ('Event Number')
+        ax .ticklabel_format (style ='sci',axis ='both',scilimits =(0 ,0 ))
+        fig .tight_layout ()
+
+
+    def syncZoomAcrossPlots (self ):
+        currentTab =self .rightPanel .currentWidget ()
+        if hasattr (currentTab ,"property"):
+            tabCanvases =currentTab .property ("canvases")
+            if tabCanvases and len (tabCanvases )>0 :
+
+                referenceAxes =tabCanvases [0 ].figure .axes [0 ]
+                xlim =referenceAxes .get_xlim ()
+                ylim =referenceAxes .get_ylim ()
+
+                for canvas in tabCanvases :
+                    plotType =getattr (canvas ,'plotType','')
+                    if 'Scatter plot'in plotType :
+                        if hasattr (canvas ,'axes_dict'):
+                            canvas .axes_dict ['ax_scatter'].set_xlim (xlim )
+                            canvas .axes_dict ['ax_scatter'].set_ylim (ylim )
+                            canvas .axes_dict ['ax_histx'].set_xlim (xlim )
+                            canvas .axes_dict ['ax_histy'].set_ylim (ylim )
+                    elif 'Histogram'in plotType or 'Frequency plot'in plotType :
+
+                        ax =canvas .figure .axes [0 ]
+                        ax .set_xlim (xlim )
+                    else :
+
+                        for ax in canvas .figure .axes :
+                            ax .set_xlim (xlim )
+                            ax .set_ylim (ylim )
+
+                    canvas .draw_idle ()
+
+
+
+    def create_histogram (self ,fig ,values ,min_x ,max_x ,plotType ,alpha ):
+        ax =fig .add_subplot (111 )
+        ax .hist (values ,bins =self .histogramBinsSpinBox .value (),range =(min_x ,max_x ),alpha =alpha )
+        ax .xaxis .set_major_formatter (ScalarFormatter (useMathText =True ))
+        if 'dI'in plotType :
+            ax .set_xlabel ('ΔI (nA)')
+        elif 'dt'in plotType and 'log'not in plotType :
+            ax .set_xlabel ('Δt (s)')
+        elif 'dt (log)'in plotType :
+            ax .set_xlabel ('log(Δt (ms))')
+        ax .set_ylabel ('Count')
+        ax .ticklabel_format (style ='sci',axis ='both',scilimits =(0 ,0 ))
+        fig .tight_layout ()
+
+
+        return {'ax_hist':ax }
+
+
+    def resetZoom (self ):
+        currentTab =self .rightPanel .currentWidget ()
+        if currentTab is None :
+            return 
+
+        plotType =self .rightPanel .tabText (self .rightPanel .indexOf (currentTab ))
+
+        if plotType in self .global_limits :
+            min_x ,max_x ,min_y ,max_y =self .global_limits [plotType ]
+
+            tabCanvases =currentTab .property ("canvases")
+            if tabCanvases :
+                for canvas in tabCanvases :
+                    if plotType =='Scatter plot dI vs dt'or plotType =='Scatter plot area vs dt'or plotType =='Scatter plot dI vs dt (log)':
+                        if hasattr (canvas ,'axes_dict'):
+                            canvas .axes_dict ['ax_scatter'].set_xlim (min_x ,max_x )
+                            canvas .axes_dict ['ax_scatter'].set_ylim (min_y ,max_y )
+                            canvas .axes_dict ['ax_histx'].set_xlim (min_x ,max_x )
+                            canvas .axes_dict ['ax_histy'].set_ylim (min_y ,max_y )
+                    elif plotType =='Frequency plot':
+                        ax =canvas .figure .axes [0 ]
+                        ax .set_xlim (min_x ,max_x )
+
+                    elif plotType in ['Histogram of dI','Histogram of dt','Histogram of Area','Histogram of dt (log)']:
+                        ax =canvas .figure .axes [0 ]
+                        ax .set_xlim (min_x ,max_x )
+                    else :
+                        print (f"Unsupported plot type: {plotType}")
+
+                    canvas .draw_idle ()
+
+
+    def prepareData (self ,selectedFiles ,plotOptions ):
+        data ={}
+        for filePath in selectedFiles :
+            fileData =np .load (filePath )
+            X =fileData ['X']
+
+            for option in plotOptions :
+                if option not in data :
+                    data [option ]={}
+
+                if 'Histogram'in option :
+                    index =0 if 'dI'in option else 3 if 'Area'in option else 4 
+                    values =X [:,index ].astype (float )
+
+                    values =values [~np .isnan (values )]
+                    data [option ][filePath ]=values 
+
+                elif 'Histogram of dt (log)'in option :
+
+                    dt_values =fileData ['X'][:,4 ]
+
+                    positive_dt_values =dt_values [dt_values >0 ]
+
+                    log_dt_values =np .log (positive_dt_values *1e3 )
+
+                    log_dt_values =log_dt_values [~np .isnan (log_dt_values )]
+                    data ['Histogram of dt (log)'][filePath ]=log_dt_values .astype (float )
+
+                elif 'Frequency plot'in option :
+                    event_numbers =np .arange (1 ,len (fileData ['X'])+1 ).astype (float )
+                    times =fileData ['X'][:,-1 ].astype (float )
+
+                    valid_indices =~np .isnan (times )
+                    event_numbers =event_numbers [valid_indices ]
+                    times =times [valid_indices ]
+                    data [option ][filePath ]=(times ,event_numbers )
+
+                else :
+                    x_index ,y_index =(4 ,0 )if 'dI vs dt'in option else (4 ,3 )
+                    x_values =X [:,x_index ]*1e3 
+                    y_values =X [:,y_index ]
+
+                    valid_indices =~np .isnan (x_values )&~np .isnan (y_values )
+                    x_values =x_values [valid_indices ]
+                    y_values =y_values [valid_indices ]
+                    data [option ][filePath ]=(x_values ,y_values )
+
+
+        return data 
+
+    def calculateGlobalAxisLimits (self ,plotData ,plotType ):
+        min_x =min_y =np .inf 
+        max_x =max_y =-np .inf 
+        for values in plotData .values ():
+            if isinstance (values ,dict ):
+
+                for subvalues in values .values ():
+                    if 'Histogram'in plotType :
+                        curr_min_x =np .min (subvalues )
+                        curr_max_x =np .max (subvalues )
+
+                        if not np .isfinite (curr_min_x )or not np .isfinite (curr_max_x ):
+                            continue 
+                        if curr_min_x <curr_max_x :
+                            min_x =min (min_x ,curr_min_x )
+                            max_x =max (max_x ,curr_max_x )
+                        else :
+                            min_x =min (min_x ,curr_min_x )
+                            max_x =max (max_x ,curr_min_x +1e-6 )
+                    elif 'Frequency plot'in plotType :
+                        x ,y =subvalues 
+                        min_x =min (min_x ,np .min (x ))
+                        max_x =max (max_x ,np .max (x ))
+                        curr_min_y =np .min (y )
+                        curr_max_y =np .max (y )
+                        if not np .isfinite (curr_min_y )or not np .isfinite (curr_max_y ):
+                            continue 
+                        min_y =min (min_y ,curr_min_y )
+                        max_y =max (max_y ,curr_max_y )
+                    else :
+                        x ,y =subvalues 
+                        min_x =min (min_x ,np .min (x ))
+                        max_x =max (max_x ,np .max (x ))
+                        curr_min_y =np .min (y )
+                        curr_max_y =np .max (y )
+                        if not np .isfinite (curr_min_y )or not np .isfinite (curr_max_y ):
+                            continue 
+                        min_y =min (min_y ,curr_min_y )
+                        max_y =max (max_y ,curr_max_y )
+            else :
+                if 'Histogram'in plotType :
+                    curr_min_x =np .min (values )
+                    curr_max_x =np .max (values )
+
+                    if not np .isfinite (curr_min_x )or not np .isfinite (curr_max_x ):
+                        continue 
+                    if curr_min_x <curr_max_x :
+                        min_x =min (min_x ,curr_min_x )
+                        max_x =max (max_x ,curr_max_x )
+                    else :
+                        min_x =min (min_x ,curr_min_x )
+                        max_x =max (max_x ,curr_min_x +1e-6 )
+                elif 'Frequency plot'in plotType :
+                    x ,y =values 
+                    min_x =min (min_x ,np .min (x ))
+                    max_x =max (max_x ,np .max (x ))
+                    curr_min_y =np .min (y )
+                    curr_max_y =np .max (y )
+                    if not np .isfinite (curr_min_y )or not np .isfinite (curr_max_y ):
+                        continue 
+                    min_y =min (min_y ,curr_min_y )
+                    max_y =max (max_y ,curr_max_y )
+                else :
+                    x ,y =values 
+                    min_x =min (min_x ,np .min (x ))
+                    max_x =max (max_x ,np .max (x ))
+                    curr_min_y =np .min (y )
+                    curr_max_y =np .max (y )
+                    if not np .isfinite (curr_min_y )or not np .isfinite (curr_max_y ):
+                        continue 
+                    min_y =min (min_y ,curr_min_y )
+                    max_y =max (max_y ,curr_max_y )
+
+        if not np .isfinite (min_x )or not np .isfinite (max_x ):
+            min_x ,max_x =0 ,1 
+        if not np .isfinite (min_y )or not np .isfinite (max_y ):
+            min_y ,max_y =0 ,1 
+
+
+        self .global_limits [plotType ]=(min_x ,max_x ,min_y ,max_y )
+
+        return min_x ,max_x ,min_y ,max_y 
+
+
+if __name__ =="__main__":
+
+    app =QApplication (sys .argv )
+    app .setStyle (QStyleFactory .create ('Fusion'))
+
+
+    palette =QPalette ()
+    palette .setColor (QPalette .ColorRole .Window ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .WindowText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Base ,QColor (25 ,25 ,25 ))
+    palette .setColor (QPalette .ColorRole .AlternateBase ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .ToolTipBase ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .ToolTipText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Text ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .Button ,QColor (53 ,53 ,53 ))
+    palette .setColor (QPalette .ColorRole .ButtonText ,Qt .GlobalColor .white )
+    palette .setColor (QPalette .ColorRole .BrightText ,Qt .GlobalColor .red )
+    palette .setColor (QPalette .ColorRole .Link ,QColor (42 ,130 ,218 ))
+    palette .setColor (QPalette .ColorRole .Highlight ,QColor (42 ,130 ,218 ))
+    palette .setColor (QPalette .ColorRole .HighlightedText ,Qt .GlobalColor .black )
+    app .setPalette (palette )
+
+    mainWindow =PlottingApplication ()
+    mainWindow .showMaximized ()
+    sys .exit (app .exec ())
```

### Comparing `nanosense-0.3.1/nanosense/icons.icns` & `nanosense-0.3.2/nanosense/icons.icns`

 * *Files identical despite different names*

### Comparing `nanosense-0.3.1/nanosense/image_1.jpg` & `nanosense-0.3.2/nanosense/image_1.jpg`

 * *Files identical despite different names*

### Comparing `nanosense-0.3.1/nanosense.egg-info/PKG-INFO` & `nanosense-0.3.2/nanosense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosense
-Version: 0.3.1
+Version: 0.3.2
 Summary: A comprehensive package for nanosense data analysis and visualization.
 Home-page: https://github.com/shankardutt/nanosense
 Author: Shankar Dutt
 Author-email: shankar.dutt@anu.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanosense-0.3.1/nanosense.egg-info/SOURCES.txt` & `nanosense-0.3.2/nanosense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanosense-0.3.1/setup.py` & `nanosense-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nanosense',
-    version='0.3.1',
+    version='0.3.2',
     description='A comprehensive package for nanosense data analysis and visualization.',
     author='Shankar Dutt',
     author_email='shankar.dutt@anu.edu.au',
     url='https://github.com/shankardutt/nanosense',
     packages=find_packages(include=['nanosense', 'nanosense.*']),
     include_package_data=True,
     package_data={
```

