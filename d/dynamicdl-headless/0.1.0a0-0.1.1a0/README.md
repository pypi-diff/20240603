# Comparing `tmp/dynamicdl_headless-0.1.0a0.tar.gz` & `tmp/dynamicdl_headless-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicdl_headless-0.1.0a0.tar", last modified: Mon May 13 23:57:57 2024, max compression
+gzip compressed data, was "dynamicdl_headless-0.1.1a0.tar", last modified: Mon Jun  3 08:45:43 2024, max compression
```

## Comparing `dynamicdl_headless-0.1.0a0.tar` & `dynamicdl_headless-0.1.1a0.tar`

### file list

```diff
@@ -1,20 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:57:57.120464 dynamicdl_headless-0.1.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-13 23:57:57.120464 dynamicdl_headless-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:57:57.120464 dynamicdl_headless-0.1.0a0/dynamicdl/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/dynamicdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/dynamicdl/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25689 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/dynamicdl/data_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    60822 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/dynamicdl/dynamicdl.py
--rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/dynamicdl/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/dynamicdl/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:57:57.120464 dynamicdl_headless-0.1.0a0/dynamicdl_headless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-13 23:57:57.000000 dynamicdl_headless-0.1.0a0/dynamicdl_headless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-13 23:57:57.000000 dynamicdl_headless-0.1.0a0/dynamicdl_headless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 23:57:57.000000 dynamicdl_headless-0.1.0a0/dynamicdl_headless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 23:57:57.000000 dynamicdl_headless-0.1.0a0/dynamicdl_headless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 23:57:57.000000 dynamicdl_headless-0.1.0a0/dynamicdl_headless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 23:57:57.120464 dynamicdl_headless-0.1.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-13 23:57:49.000000 dynamicdl_headless-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:45:43.876883 dynamicdl_headless-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-06-03 08:45:43.876883 dynamicdl_headless-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:45:43.872883 dynamicdl_headless-0.1.1a0/dynamicdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:45:43.872883 dynamicdl_headless-0.1.1a0/dynamicdl/_main/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/_main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/_main/_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/_main/_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/_main/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/_main/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:45:43.872883 dynamicdl_headless-0.1.1a0/dynamicdl/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/data/dataentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/data/dataitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/data/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/data/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/data/partialtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/data/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49774 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/dynamicdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/dynamicds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:45:43.876883 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/ambiguouslist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/genericlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/impliedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/segmentationobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/parsing/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:45:43.876883 dynamicdl_headless-0.1.1a0/dynamicdl/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/jsonfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/txtfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/xmlfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/dynamicdl/processing/yamlfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:45:43.876883 dynamicdl_headless-0.1.1a0/dynamicdl_headless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-06-03 08:45:43.000000 dynamicdl_headless-0.1.1a0/dynamicdl_headless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-06-03 08:45:43.000000 dynamicdl_headless-0.1.1a0/dynamicdl_headless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:45:43.000000 dynamicdl_headless-0.1.1a0/dynamicdl_headless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-03 08:45:43.000000 dynamicdl_headless-0.1.1a0/dynamicdl_headless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 08:45:43.000000 dynamicdl_headless-0.1.1a0/dynamicdl_headless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:45:43.876883 dynamicdl_headless-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-06-03 08:45:35.000000 dynamicdl_headless-0.1.1a0/setup.py
```

### Comparing `dynamicdl_headless-0.1.0a0/LICENSE` & `dynamicdl_headless-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicdl_headless-0.1.0a0/PKG-INFO` & `dynamicdl_headless-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicdl-headless
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: A PyTorch-based dynamic dataloading library
 Home-page: https://github.com/ESB-AI-Lab/DynamicDL-Headless
 Author: Anthony Tong
 Author-email: atong28.usa@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dynamicdl_headless-0.1.0a0/README.md` & `dynamicdl_headless-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `dynamicdl_headless-0.1.0a0/dynamicdl/_utils.py` & `dynamicdl_headless-0.1.1a0/dynamicdl/_warnings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,8 @@
-'''
-Private utility functions for DynamicData.
-'''
-import json
-from typing import Union, NoReturn
-from itertools import repeat
-
-def union(item: Union[list[object], object]) -> list[object]:
-    '''
-    Returns the item in a list format if not already in a list format.
-    '''
-    if not isinstance(item, list):
-        item = [ item ]
-    return item
-
-def next_avail_id(idx_to_name: dict[int, str]) -> int:
-    '''Get next available id and fills in gaps'''
-    for i, idx in enumerate(idx_to_name):
-        if i != idx:
-            return i
-    return len(idx_to_name)
-
-def _get_str(data):
-    if isinstance(data, dict):
-        return {str(key): _get_str(val) for key, val in data.items()}
-    if isinstance(data, list):
-        return [_get_str(val) for val in data]
-    return str(data)
-
-def get_str(data):
-    '''Return pretty print string.'''
-    return json.dumps(_get_str(data), indent=4).replace('"', '')
-
-def check_map(it, num):
-    '''Check an iterator for num occurrences'''
-    return all(map(any, repeat(iter(it), num)))
+from typing import NoReturn
 
 class MergeError(Exception):
     '''
     Exceptions raised while merging.
     '''
 
 class LengthMismatchError(Exception):
@@ -92,30 +57,58 @@
     nan_exists = ('Found NaN values that will cause errors in row: \n{row}. You can automatically '
                   'purge NaN values with remove_invalid=True.', ValueError)
     new_exists = ('New set {type} {imgset_name} already exists!', KeyError)
     split_invalid = ('Split fraction invalid, cannot be {desc} 1', ValueError)
     file_exists = ('File already exists: {filename}. Set overwrite=True to overwrite the file.',
                    OSError)
     is_none = ('{desc} cannot be None!', TypeError)
-    fail_generic_match = ('Failed to match: {dataset} to {root}', MergeError)
-    static_missing = ('Static value {value} not found in dataset', ValueError)
     inappropriate_type = ('Inappropriate type found for value {value}', TypeError)
     nonredundant_add = ('Cannot add to item which is not redundant', ValueError)
     data_invalid = ('Value {value} is invalid for given delimiter type {delimiter}', ValueError)
     generics_missing = ('Must have at least 1 generic in alias instance.', ValueError)
     generic_list_length = ('List length ({length1}) must be a multiple of length of provided form '
                            '({length2})', LengthMismatchError)
     invalid_dataset = ('This may not be a valid CVDataset, or the dataset is too old.', ValueError)
     pairings_missing = ('Must have at least 2 pairing datatypes.', ValueError)
     invalid_pairing = ('Pairings are not of the same type, either must all be redundant or none'
                        'redundant. Given: {paired}', MergeError)
     invalid_shape = ('{mode} requires equal input image dimensions, try using the `resize` '
                      'parameter when getting dataloader, or specify your own collate function.',
                      RuntimeError)
     empty_bbox = ('Bounding box is empty for image at {file}.', RuntimeError)
+    no_images = ('Dataset has no image files. DynamicDL does not currently support non-image '
+                 'datasets.', RuntimeError)
+    illegal_capturing_group = ('Illegal presence of a regex capturing group in the pattern. For '
+                               'reference, (.+) and (.*) are not allowed.', ValueError)
+    invalid_csv_cols = ('CSV column length detected to be {n}, which is not equal to expected form '
+                        'which has length {exp}', RuntimeError)
+    invalid_csv_value = ('Invalid data {item} encountered, failed to fit into generic {form}',
+                         ValueError)
+    incorrect_type = ('Expected list at path {path}, got {got} instead', RuntimeError)
+    merged_all = ('The merging process returned one DataEntry, expected many', RuntimeError)
+
+    # data items
+    partial_overwrite = ('Partial datatype field {desc} was overwritten, which is not allowed',
+                         MergeError)
+    type_exists = ('Attempted to initialize a DataType object which already exists: {desc}',
+                   RuntimeError)
+
+    # pairing errors
+    empty_pairing = ('Attempted to apply Pairing object at path {path}, but had no pairings stored',
+                     RuntimeError)
+
+    # engine processes
+    static_missing = (
+        'Expected static value {value} but was not found at path {path}',
+        ValueError
+    )
+    fail_generic_match = (
+        'Parsing {value} with generic {generic} failed; pattern does not match at path {path}',
+        MergeError
+    )
 
     @staticmethod
     def warn(name: str, **kwargs: str) -> None:
         '''
         Warn from one of the warning presets.
         '''
         print(getattr(Warnings, name).format(**kwargs))
```

### Comparing `dynamicdl_headless-0.1.0a0/dynamicdl/dynamicdl.py` & `dynamicdl_headless-0.1.1a0/dynamicdl/dynamicdl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,183 +1,73 @@
-'''
-Main module for processing datasets. Collects all parsed objects into the DynamicData object, and
-maintains the DynamicDL class for PyTorch Dataset and DataLoader functionalities.
-
-Collate functions (pseudo-private)
-
-DynamicData main class public functions:
- - parse()
- - get_transforms()
- - get_dataset()
- - get_dataloader()
- - get_image_set()
- - split_image_set()
- - clear_image_sets()
- - delete_image_set()
- - save()
- - load()
- - sample_image()
- - inference()
-
-DynamicDS class (VisionDataset extension)
-'''
 import os
 import time
 import json
 from hashlib import md5
 from functools import partial
 import random
-from typing import Union, Optional, Callable, Iterable, Tuple, Any
+from typing import Union, Optional, Callable, Iterable, Tuple
 
 import cv2
 from tqdm import tqdm
 import numpy as np
 import jsonpickle
 from pandas import DataFrame
 from pandas import isna
 from pandas.core.series import Series
 from torch.utils.data import DataLoader
-from torch import Tensor, LongTensor, FloatTensor
+from torch import FloatTensor
 import torch
-from torchvision.datasets.vision import VisionDataset
 from torchvision.utils import draw_bounding_boxes
 import torchvision.transforms.functional as F
 from torchvision import transforms as T
 from PIL.Image import open as open_image
 import matplotlib.pyplot as plt
 from typing_extensions import Self
 
-from ._utils import next_avail_id, union, Warnings
-from .processing import populate_data
-from .transforms import Transforms
-
-def _collate_classification(batch):
-    images, labels = zip(*batch)
-    try:
-        return torch.stack(images), torch.IntTensor(list(labels))
-    except RuntimeError as e:
-        if 'stack expects each tensor to be equal size, but got' in str(e):
-            Warnings.error('invalid_shape', mode='classification')
-        raise
-
-def _collate_classification_dim(batch):
-    images, labels = zip(*batch)
-    labels = {'label': torch.IntTensor([label['label'] for label in labels]),
-              'dim': [label['dim'] for label in labels]}
-    try:
-        return torch.stack(images), labels
-    except RuntimeError as e:
-        if 'stack expects each tensor to be equal size, but got' in str(e):
-            Warnings.error('invalid_shape', mode='classification')
-        raise
-
-def _collate_detection(batch):
-    return list(zip(*batch))
-
-def _collate_detection_dim(batch):
-    images, labels = zip(*batch)
-    labels = {'label': torch.IntTensor([label['label'] for label in labels]),
-              'dim': [label['dim'] for label in labels]}
-    return tuple(images), tuple(labels)
-
-def _collate_segmentation(batch):
-    images, labels = zip(*batch)
-    try:
-        return torch.stack(images), torch.stack(labels)
-    except RuntimeError as e:
-        if 'stack expects each tensor to be equal size, but got' in str(e):
-            Warnings.error('invalid_shape', mode='segmentation')
-        raise
-
-def _collate_segmentation_dim(batch):
-    images, labels = zip(*batch)
-    labels = {'label': torch.stack([label['label'] for label in labels]),
-              'dim': [label['dim'] for label in labels]}
-    try:
-        return torch.stack(images), labels
-    except RuntimeError as e:
-        if 'stack expects each tensor to be equal size, but got' in str(e):
-            Warnings.error('invalid_shape', mode='segmentation')
-        raise
-
-def _collate_default(batch):
-    return list(zip(*batch))
-
-def _collate(mode: str, store_dim: bool) -> Callable:
-    '''
-    Getters for all preset collate functions.
-    '''
-    if mode == 'classification':
-        return _collate_classification_dim if store_dim else _collate_classification
-    if mode == 'segmentation':
-        return _collate_segmentation_dim if store_dim else _collate_segmentation
-    if mode == 'detection':
-        return _collate_detection_dim if store_dim else _collate_detection
-    return _collate_default
+from ._utils import next_avail_id, union, config
+from ._warnings import Warnings
+from ._main._engine import populate_data
+from ._main._transforms import Transforms
+from ._main._collate import _collate
+from .dynamicds import DynamicDS
 
 class DynamicData:
     '''
     Main dataset class. Accepts root directory path and dictionary form of the structure.
+    DynamicDL expands a generic dataset form and interprets it through a series of recursive
+    hierarchical inheritances, to flatten the dataset into a list of entries fit for image
+    processing.
     
-    Args:
-     - `root` (`str`): the root directory to access the dataset.
-     - `form` (`dict`): the form of the dataset. See documentation for further details on valid
-        forms.
-     - `bbox_scale_option` (`str`): choose from either 'auto', 'zeroone', or 'full' scale options to
-        define, or leave empty for automatic. Default: 'auto'
-     - `seg_scale_option` (`str`): choose from either 'auto', 'zeroone', or 'full' scale options to
-        define, or leave empty for automatic. Default: 'auto'
-     - `get_md5_hashes` (`bool`): when set to True, create a new column which finds md5 hashes for
-        each image available, and makes sure there are no duplicates. Default: False
-     - `purge_duplicates` (`Optional[bool]`): when set to True, remove all duplicate image entries.
-        Duplicate images are defined by having the same md5 hash, so this has no effect when
-        get_md5_hashes is False. When set to False, do not purge duplicates. Default: None
+    :param root: The root directory to access the dataset.
+    :type root: str
+    :param form: The form of the dataset. See documentation for further details on valid forms.
+    :type form: dict
+    :param bbox_scale_option: Choose from either `auto`, `zeroone`, or `full` scale options to
+        define, or leave empty for automatic. `zeroone` assumes detection coordinates to be
+        interpreted on a 0-1 scale as ratios dependent on image size. `full` leaves coordinates
+        as is. `auto` for auto-detection. Default: `auto`
+    :type bbox_scale_option: str
+    :param seg_scale_option: Choose from either `auto`, `zeroone`, or `full` scale options to
+        define, or leave empty for automatic. `zeroone` assumes segmentation coordinates to be
+        interpreted on a 0-1 scale as ratios dependent on image size. `full` leaves coordinates
+        as is. `auto` for auto-detection. Default: `auto`
+    :type seg_scale_option: str
+    :param get_md5_hashes: When set to True, create a new column which finds md5 hashes for each
+        image available, and makes sure there are no duplicates. Default: `False`
+    :type get_md5_hashes: bool
+    :param purge_duplicates: When set to True, remove all duplicate image entries. Duplicate images
+        are defined by having the same md5 hash, so this has no effect when `get_md5_hashes` is 
+        `False`. When set to `False`, do not purge duplicates. Default: `None`
+    :type purge_duplicates: Optional[bool]
     '''
 
-    _inference_cols = {'ABSOLUTE_FILE', 'IMAGE_ID', 'IMAGE_DIM'}
-    _diffusion_cols = {'ABSOLUTE_FILE', 'IMAGE_ID', 'IMAGE_DIM'}
-    _classification_cols = {'ABSOLUTE_FILE', 'IMAGE_ID', 'CLASS_ID', 'IMAGE_DIM'}
-    _detection_cols = {'ABSOLUTE_FILE', 'IMAGE_ID', 'BBOX_CLASS_ID', 'BOX', 'IMAGE_DIM'}
-    _segmentation_img_cols = {'ABSOLUTE_FILE', 'IMAGE_ID', 'ABSOLUTE_FILE_SEG', 'IMAGE_DIM'}
-    _segmentation_poly_cols = {'ABSOLUTE_FILE', 'IMAGE_ID', 'POLYGON', 'SEG_CLASS_ID', 'IMAGE_DIM'}
-
-    _BBOX_MODES = [
-        (
-            {'X1', 'X2', 'Y1', 'Y2'},
-            ('X1', 'Y1', 'X2', 'Y2'),
-            (lambda x: round(min(x[0], x[1]), 6), lambda y: round(min(y[0], y[1]), 6),
-             lambda x: round(max(x[0], x[1]), 6), lambda y: round(max(y[0], y[1]), 6))
-        ),
-        (
-            {'XMIN', 'YMIN', 'XMAX', 'YMAX'},
-            ('XMIN', 'YMIN', 'XMAX', 'YMAX'),
-            (lambda x: round(x[0], 6), lambda y: round(y[0], 6),
-             lambda x: round(x[1], 6), lambda y: round(y[1], 6))
-        ),
-        (
-            {'XMIN', 'YMIN', 'WIDTH', 'HEIGHT'},
-            ('XMIN', 'YMIN', 'WIDTH', 'HEIGHT'),
-            (lambda x: round(x[0], 6), lambda y: round(y[0], 6),
-             lambda x: round(x[0]+x[1], 6), lambda y: round(y[0]+y[1], 6))
-        ),
-        (
-            {'XMID', 'YMID', 'WIDTH', 'HEIGHT'},
-            ('XMID', 'YMID', 'WIDTH', 'HEIGHT'),
-            (lambda x: round(x[0]-x[1]/2, 6), lambda y: round(y[0]-y[1]/2, 6),
-             lambda x: round(x[0]+x[1]/2, 6), lambda y: round(y[0]+y[1]/2, 6))
-        ),
-        (
-            {'XMAX', 'YMAX', 'WIDTH', 'HEIGHT'},
-            ('XMAX', 'YMAX', 'WIDTH', 'HEIGHT'),
-            (lambda x: round(x[0]-x[1], 6), lambda y: round(y[0]-y[1], 6),
-             lambda x: round(x[0], 6), lambda y: round(y[0], 6))
-        )
-    ]
-    _BBOX_COLS = {'X1', 'X2', 'Y1', 'Y2', 'XMIN', 'XMAX', 'YMIN', 'YMAX', 'XMID', 'YMID', 'WIDTH',
-                  'HEIGHT', 'BBOX_CLASS_ID', 'BBOX_CLASS_NAME'}
+    _modes: dict[str, set[str]] = config['MODES']
+
+    _BBOX_MODES = config['BBOX_MODES']
+    _BBOX_COLS = config['BBOX_COLS']
 
     _scale_options = ('zeroone', 'full')
 
     def __init__(
         self,
         root: str,
         form: dict,
@@ -199,126 +89,111 @@
         self.available_modes = []
         self.cleaned = False
         self.get_md5_hashes = get_md5_hashes
         self.purge_duplicates = purge_duplicates
         self.bbox_scale_option = bbox_scale_option
         self.seg_scale_option = seg_scale_option
 
-    def parse(self, override: bool = False) -> None:
+    def parse(self, override: bool = False, verbose: bool = False) -> None:
         '''
         Must be called to instantiate the data in the dataset instance. Performs the recursive
         populate_data algorithm and creates the dataframe, and then cleans up the data.
         
-        Args:
-         - `override` (`bool`): whether to overwrite existing data if it has already been parsed and
-            cleaned. Default: False
+        :param override: Whether to overwrite existing data if it has already been parsed and
+            cleaned. Default: `False`
+        :type override: bool
+        :param verbose: Whether to show more details about the merging process. May have an impact
+            on runtime. Default: `False`
+        :type verbose: bool
         '''
         print('[DynamicData] Parsing data...')
         start = time.time()
         if self.cleaned and not override:
             Warnings.error('already_parsed')
-        data = populate_data(self.root, self.form)
+        data = populate_data(self.root, self.form, verbose=verbose)
         entries = [{key: val.value for key, val in item.data.items()} for item in data]
         self.dataframe = DataFrame(entries)
         end = time.time()
         print(f'[DynamicData] Parsed! ({(end - start):.3f}s)')
         start = time.time()
-        self._cleanup()
+        self._cleanup(verbose=verbose)
         end = time.time()
         print(f'[DynamicData] Cleaned! ({(end - start):.3f}s)')
         print(self._get_statistics())
 
-    def _cleanup(self) -> None:
+    def _cleanup(self, verbose: bool = False) -> None:
         '''
         Run cleanup and sanity checks on all data. Assigns IDs to name-only values.
         '''
         print('[DynamicData] Cleaning up data...')
 
+        if 'ABSOLUTE_FILE' not in self.dataframe:
+            Warnings.error('no_images')
+
         # sort by image id first to prevent randomness
         if 'IMAGE_ID' in self.dataframe:
             self.dataframe.sort_values('IMAGE_ID', ignore_index=True, inplace=True)
         else:
             self.dataframe.sort_values('IMAGE_NAME', ignore_index=True, inplace=True)
             self.dataframe['IMAGE_ID'] = self.dataframe.index
 
         # get image sizes
         self._get_img_sizes()
 
         # get md5 hashes
         if self.get_md5_hashes:
             self._get_md5_hashes()
 
-        # drop generic as it is useless data
-        self.dataframe.drop(columns='GENERIC', inplace=True, errors='ignore')
-
         # convert bounding boxes into proper format and store under 'BOX'
         self._convert_bbox()
 
         if 'BOX' in self.dataframe:
             self._get_box_scale()
             self._convert_box_scale()
 
         if 'POLYGON' in self.dataframe:
             self._get_seg_scale()
             self._convert_seg_scale()
 
         # assign ids
         self._cleanup_id()
-        self._process_ids('CLASS', redundant=False)
-        self._process_ids('SEG_CLASS', redundant=True)
-        self._process_ids('BBOX_CLASS', redundant=True)
+        self._process_ids('CLASS', redundant=False, verbose=verbose)
+        self._process_ids('SEG_CLASS', redundant=True, verbose=verbose)
+        self._process_ids('BBOX_CLASS', redundant=True, verbose=verbose)
 
         # check available columns to determine mode availability
         self.available_modes = DynamicData._get_modes(self.dataframe)
 
         # cleanup image sets
         self._cleanup_image_sets()
         self.cleaned = True
 
     @staticmethod
     def _get_modes(df: DataFrame) -> list:
-        modes = []
-        if DynamicData._inference_cols.issubset(df.columns):
-            modes.append('inference')
-        if DynamicData._diffusion_cols.issubset(df.columns):
-            modes.append('diffusion')
-        if DynamicData._classification_cols.issubset(df.columns):
-            modes.append('classification')
-        if DynamicData._detection_cols.issubset(df.columns):
-            modes.append('detection')
-        if DynamicData._segmentation_img_cols.issubset(df.columns) or \
-            DynamicData._segmentation_poly_cols.issubset(df.columns):
-            modes.append('segmentation')
+        modes = [mode for mode, subset in DynamicData._modes.items() if subset.issubset(df.columns)]
         return modes
 
     def _get_statistics(self):
         data = '[DynamicData] Dataset statistics:\n'
         data += f'       | Available modes: {", ".join(self.available_modes)}\n'
         data += f'       | Images: {len(self.dataframe)}\n'
         for mode in self.available_modes:
-            if mode != 'segmentation':
-                opt = ''
-            elif 'POLYGON' in self.dataframe.columns:
-                opt = 'poly_'
-            else:
-                opt = 'img_'
-            colset = f"_{mode}_{opt}cols"
-
             count = len(self.dataframe) - len(self.dataframe[
-                self.dataframe[list(getattr(self, colset))].isna().any(axis=1)
+                self.dataframe[list(DynamicData._modes[mode])].isna().any(axis=1)
             ])
             data += f'       | Complete entries for {mode}: {count}\n'
 
         if 'detection' in self.available_modes:
             data += f'       | Bounding box scaling option: {self.bbox_scale_option}\n'
-        if 'segmentation' in self.available_modes:
+        if ('segmentation_poly' in self.available_modes or 
+            'segmentation_mask' in self.available_modes):
             data += f'       | Segmentation object scaling option: {self.seg_scale_option}\n'
         return data.strip()
 
-    def _process_ids(self, name: str, redundant: bool = False) -> None:
+    def _process_ids(self, name: str, redundant: bool = False, verbose: bool = False) -> None:
         if f'{name}_NAME' in self.dataframe:
             if f'{name}_ID' not in self.dataframe:
                 call = partial(self._assign_ids, redundant=redundant)
             else: call = partial(self._validate_ids, redundant=redundant)
             result = call(f'{name}')
             setattr(self, f'{name.lower()}_to_idx', result[0])
             setattr(self, f'idx_to_{name.lower()}', result[1])
@@ -334,15 +209,16 @@
             self.dataframe[f'{name}_NAME'] = names
         else:
             return
         self._patch_ids(
             name,
             getattr(self, f'{name.lower()}_to_idx'),
             getattr(self, f'idx_to_{name.lower()}'),
-            redundant=redundant
+            redundant=redundant,
+            verbose=verbose
         )
 
     def _get_img_sizes(self) -> None:
         self.dataframe['IMAGE_DIM'] = [open_image(filename).size if isinstance(filename, str)
                                        else np.nan for filename in self.dataframe['ABSOLUTE_FILE']]
 
     def _get_md5_hashes(self) -> None:
@@ -372,29 +248,31 @@
                 if any(coord > 1 for box in boxes for coord in box):
                     self.bbox_scale_option = 'full'
                 if any(coord < 0 for box in boxes for coord in box):
                     Warnings.error('invalid_scale_data_bbox', id=i)
             if self.bbox_scale_option == 'full':
                 print('[DynamicData] Detected full size bounding box scale option')
                 return
-            print('[DynamicData] Detected [0, 1] bounding box scale option to be converted to full size')
+            print('[DynamicData] Detected [0, 1] bounding box scale option to be converted to full '
+                  'size')
             self.bbox_scale_option = 'zeroone'
         if self.bbox_scale_option not in DynamicData._scale_options:
             Warnings.error('invalid_scale', scale=self.bbox_scale_option)
 
     def _get_seg_scale(self) -> None:
         if self.seg_scale_option == 'auto':
             for i, shapes in enumerate(self.dataframe['POLYGON']):
                 if any(val > 1 for shape in shapes for coord in shape for val in coord):
                     self.seg_scale_option = 'full'
                     print('[DynamicData] Detected full size segmentation scale option')
                     return
                 if any(coord < 0 for shape in shapes for coord in shape):
                     Warnings.error('invalid_scale_data', id=i)
-            print('[DynamicData] Detected [0, 1] segmentation scale option to be converted to full size')
+            print('[DynamicData] Detected [0, 1] segmentation scale option to be converted to full '
+                  'size')
             self.seg_scale_option = 'zeroone'
         if self.seg_scale_option not in DynamicData._scale_options:
             Warnings.error('invalid_scale', scale=self.seg_scale_option)
 
     def _convert_box_scale(self) -> None:
         if self.bbox_scale_option == 'zeroone':
             boxes_list = []
@@ -590,45 +468,52 @@
         for col in cols:
             if col not in self.dataframe:
                 continue
             self.dataframe[col] = self.dataframe[col].astype('Int64')
 
     def get_transforms(
         self,
-        mode: str,
+        mode: str = 'inference',
         calculate_stats: bool = True,
         mean: Tuple[float, ...] = (0.485, 0.456, 0.406),
         std: Tuple[float, ...] = (0.229, 0.224, 0.225),
         normalize: bool = True,
         remove_invalid: bool = True,
-        resize: Optional[tuple[int, int]] = None
+        resize: Optional[Tuple[int, ...]] = None
     ) -> Tuple[Optional[Callable], ...]:
         '''
         Retrieve the default standard image/label transforms for specified mode.
         
-        Args:
-         - `mode` (`str`): choose a mode out of available modes for the transforms. Each mode has
+        :param mode: Choose a mode out of available modes for the transforms. Each mode has
             slightly altered standard transforms.
-         - `calculate_stats` (`bool`): when set to True, calculate the statistics for the entire
+        :type mode: str
+        :param calculate_stats: When set to True, calculate the statistics for the entire
             dataset, overriding default mean/std kwarg (defaults from ImageNet). Use this feature
             when dataset mean/std is unknown and differs significantly from ImageNet. Default: True.
-         - `mean` (`Tuple[float, ...]`): default mean statistics for the dataset. Has no effect when
+        :type calculate_stats: bool
+        :param mean: Default mean statistics for the dataset. Has no effect when
             `calculate_stats = True`. Default: ImageNet values.
-         - `std` (`Tuple[float, ...]`): default mean statistics for the dataset. Has no effect when
+        :type mean: Tuple[float, ...]
+        :param std: Default mean statistics for the dataset. Has no effect when
             `calculate_stats = True`. Default: ImageNet values.
-         - `normalize` (`bool`): when set to True, normalize the dataset according to some
+        :type std: Tuple[float, ...]
+        :param normalize: When set to True, normalize the dataset according to some
             mean/std values, either from calculated stats or ImageNet default. This statement is
             overriden when `calculate_stats` is set to True. Default: True.
-         - `remove_invalid` (`bool`): remove invalid entries when calculating the statistics,
-            assuming `calculate_stats` is set to True. If `calculate_stats` is False, this value
-            has no effect. Default: True.
-         - `resize` (`Optional[tuple[int, int]]`): resize to specific tuple dimensions before
-            calculating statistics, only when `calculate_stats` is set to True, just like
-            `remove_invalid`. Default: None.
-        
+        :type normalize: bool
+        :param remove_invalid: Remove invalid entries when calculating the statistics, assuming
+            `calculate_stats` is set to `True`. If `calculate_stats` is `False`, this value has no
+            effect. Default: `True`.
+        :type remove_invalid: bool
+        :param resize: Resize to specific tuple dimensions before calculating statistics, only when
+            `calculate_stats` is set to True, just like `remove_invalid`. Default: `None`.
+        :type resize: Optional[Tuple[int, ...]]
+        :return: A tuple of two callable transforms, the first being the standard image transform
+            and the latter being the standard target transform.
+        :rtype: Tuple[Optional[Callable], ...]
         '''
         if not calculate_stats:
             return Transforms.get(mode, resize=resize, normalize=normalize, mean=mean, std=std)
         if mode not in self.available_modes or mode in ('inference', 'diffusion'):
             return (None, None)
         loader = self.get_dataloader(
             mode,
@@ -660,15 +545,15 @@
         std /= len(loader.dataset)
 
         print(f"[DynamicData] Got mean {mean} and std {std}")
         return Transforms.get(mode, resize=resize, mean=mean, std=std, normalize=True)
 
     def get_dataset(
         self,
-        mode: str,
+        mode: str = 'inference',
         remove_invalid: bool = True,
         store_dim: bool = False,
         preset_transform: bool = True,
         calculate_stats: bool = True,
         mean: Tuple[float, ...] = (0.485, 0.456, 0.406),
         std: Tuple[float, ...] = (0.229, 0.224, 0.225),
         normalize: bool = True,
@@ -676,48 +561,58 @@
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         transforms: Optional[tuple[Callable]] = None,
         resize: Optional[tuple[int, int]] = None,
         normalize_to: Optional[str] = None
     ) -> 'DynamicDS':
         '''
-        Retrieve the PyTorch dataset (torch.utils.data.Dataset) of a specific mode and image set.
+        Retrieve the PyTorch dataset (`torch.utils.data.Dataset`) of a specific mode and image set.
         
-        Args:
-         - `mode` (`str`): the mode of training to select. See available modes with
-            `available_modes`.
-         - `remove_invalid` (`bool`): if set to True, deletes any NaN/corrupt items in the image set
+        :param mode: The mode of training to select. See available modes with `available_modes`.
+        :type mode: str
+        :param remove_invalid: If set to True, deletes any NaN/corrupt items in the image set
             pertaining to the relevant mode. In the False case, either NaN values are substituted
             with empty values or an error is thrown, depending on the mode selected.
-         - `store_dim` (`bool`): if set to True, the labels in the dataset will return a dict with
-            two keys. 'label' contains the standard PyTorch labels and 'dim' contains the image's
+        :type remove_invalid: bool
+        :param store_dim: If set to True, the labels in the dataset will return a dict with two
+            keys. `label` contains the standard PyTorch labels and `dim` contains the image's
             former dimensions.
-         - `preset_transform` (`bool`): whether to use default preset transforms. Consists of
-            normalization with either calculated mean of the dataset about to be used or standard
-            ImageNet statistics depending on `calculate_stats`. Default: True
-         - `calculate_stats` (`bool`): whether to calculate mean and std for this dataset to be used
-            in normalization transforms. If False, uses ImageNet default weights. Only has effect
-            when `preset_transform` is set to True. Default: True
-         - `mean` (`Tuple[float, ...]`): default mean statistics for the dataset. Has no effect when
+        :type store_dim: bool
+        :param preset_transform: Whether to use default preset transforms. Consists of normalization
+            with either calculated mean of the dataset about to be used or standard ImageNet
+            statistics depending on `calculate_stats`. Default: `True`
+        :type preset_transform: bool
+        :param calculate_stats: Whether to calculate mean and std for this dataset to be used in
+            normalization transforms. If False, uses ImageNet default weights. Only has effect
+            when `preset_transform` is set to `True`. Default: `True`
+        :type calculate_stats: bool
+        :param mean: Default mean statistics for the dataset. Has no effect when
             `calculate_stats = True`. Default: ImageNet values.
-         - `std` (`Tuple[float, ...]`): default mean statistics for the dataset. Has no effect when
+        :type mean: Tuple[float, ...]
+        :param std: Default mean statistics for the dataset. Has no effect when
             `calculate_stats = True`. Default: ImageNet values.
-         - `normalize` (`bool`): when set to True, normalize the dataset according to some
-            mean/std values, either from calculated stats or ImageNet default. This statement is
-            overriden when `calculate_stats` is set to True. Default: True.
-         - `image_set` (`Optional[str]`): the image set to pull from. Default: all images.
-         - `transform` (`Optional[Callable]`): the transform operation to apply to the images.
-         - `target_transform` (`Optional[Callable]`): the transform operation on the labels.
-         - `transforms` (`Optional[tuple[Optional[Callable], ...]]`): tuple in the format
-            `(transform, target_transform)`. Default PyTorch transforms are available in the
-            CVTransforms class.
-         - `resize` (`Optional[tuple[int, int]]`): if provided, resize all images to exact
-            configuration.
-         - `normalize_to` (`Optional[str]`): if provided, normalize bounding box/segmentation
-            coordinates to a specific configuration. Options: 'zeroone', 'full'
+        :type std: Tuple[float, ...]
+        :param normalize: When set to `True`, normalize the dataset according to some mean/std
+            values, either from calculated stats or ImageNet default. This statement is overriden
+            when `calculate_stats` is set to `True`. Default: `True`.
+        :type normalize: bool
+        :param image_set: The image set to pull from. Default: all images.
+        :type image_set: Optional[str]
+        :param transform: The transform operation to apply to the images.
+        :type transform: Optional[Callable]
+        :param target_transform: The transform operation to apply to the labels.
+        :type target_transform: Optional[Callable]
+        :param transforms: Tuple in the format `(transform, target_transform)`. Obtain default
+            transforms from `DynamicData.get_transforms()`, or supply your own.
+        :type transforms: Optional[Tuple[Optional[Callable], ...]]
+        :param resize: If provided, resize all images to exact `(width, height)` configuration.
+        :type resize: Optional[Tuple[int, ...]]
+        :param normalize_to: If provided, normalize bounding box/segmentation coordinates to a
+            specific configuration. Options: 'zeroone', 'full'
+        :type normalize_to: Optional[str]
         '''
         if not self.cleaned:
             self.parse()
         if mode.lower().strip() not in self.available_modes:
             Warnings.error('mode_unavailable', mode=mode.lower().strip())
 
         if transforms:
@@ -737,65 +632,68 @@
         dataframe = self.dataframe[[image_set in item for item in
                                     self.dataframe[f'IMAGE_SET_{imgset_mode.upper()}']]]
         if image_set is None:
             dataframe = self.dataframe
         if len(dataframe) == 0:
             Warnings.error('image_set_missing', imgset_name=imgset_mode, image_set=image_set)
         normalization = None
+        dataframe = dataframe[list(DynamicData._modes[mode])]
         if mode == 'classification':
-            dataframe = dataframe[list(DynamicData._classification_cols)]
             id_mapping = {k: i for i, k in enumerate(self.idx_to_class)}
         elif mode == 'detection':
-            dataframe = dataframe[list(DynamicData._detection_cols)]
             normalization = self.bbox_scale_option
             id_mapping = {k: i for i, k in enumerate(self.idx_to_bbox_class)}
-        elif mode == 'segmentation':
-            dataframe = dataframe[list(DynamicData._segmentation_poly_cols if 'POLYGON' in
-                                       dataframe else DynamicData._segmentation_img_cols)]
+        elif mode == 'segmentation_mask' or mode == 'segmentation_poly':
             normalization = self.seg_scale_option
             id_mapping = {k: i for i, k in enumerate(self.idx_to_seg_class)}
-        elif mode == 'inference':
-            dataframe = dataframe[list(DynamicData._inference_cols)]
-            id_mapping = None
-        elif mode == 'diffusion':
-            dataframe = dataframe[list(DynamicData._diffusion_cols)]
+        elif mode == 'inference' or mode == 'diffusion':
             id_mapping = None
         if remove_invalid:
             dataframe = dataframe.dropna()
             if mode == 'detection':
                 start = len(dataframe)
                 dataframe = dataframe[dataframe['BOX'].apply(lambda x: len(x) != 0)]
                 end = len(dataframe)
                 print(f'[DynamicData] Removed {start - end} empty entries from data.')
         else:
             replace_nan = (lambda x: ([] if isinstance(x, float) and isna(x) else x))
+            cols = []
             if mode == 'detection':
                 cols = ['BBOX_CLASS_ID'] # BOX already accounted for in bbox creation
-            elif mode == 'segmentation':
-                cols = ['POLYGON', 'SEG_CLASS_ID'] if 'POLYGON' in dataframe else []
+            elif mode == 'segmentation_poly':
+                cols = ['POLYGON', 'SEG_CLASS_ID']
             for col in cols:
                 dataframe[col] = dataframe[col].apply(replace_nan)
             for i, row in dataframe.iterrows():
                 for val in row.values:
                     if isinstance(val, float) and isna(val):
                         row = str(dataframe.iloc[i])
                         Warnings.error('nan_exists', row=row)
 
         if len(dataframe) == 0:
             Warnings.error('image_set_empty', image_set=image_set)
-        return DynamicDS(dataframe, self.root, mode, id_mapping=id_mapping, transform=transform,
-                        target_transform=target_transform, resize=resize, store_dim=store_dim,
-                        normalize_to=normalize_to, normalization=normalization)
+        return DynamicDS(
+            dataframe,
+            self.root,
+            mode,
+            id_mapping=id_mapping,
+            transform=transform,
+            target_transform=target_transform,
+            resize=resize,
+            store_dim=store_dim,
+            normalize_to=normalize_to,
+            normalization=normalization
+        )
 
     def get_dataloader(
         self,
-        mode: str,
-        batch_size: int = 4,
+        mode: str = 'inference',
+        batch_size: int = 16,
         shuffle: bool = True,
-        num_workers: int = 1,
+        num_workers: int = 0,
         remove_invalid: bool = True,
         store_dim: bool = False,
         preset_transform: bool = True,
         calculate_stats: bool = True,
         mean: Tuple[float, ...] = (0.485, 0.456, 0.406),
         std: Tuple[float, ...] = (0.229, 0.224, 0.225),
         normalize: bool = True,
@@ -804,50 +702,63 @@
         target_transform: Optional[Callable] = None,
         transforms: Optional[tuple[Callable]] = None,
         resize: Optional[tuple[int, int]] = None,
         normalize_to: Optional[str] = None
     ) -> DataLoader:
         '''
         Retrieve the PyTorch dataloader (torch.utils.data.DataLoader) for this dataset.
-        
-        Args:
-         - `mode` (`str`): the mode of training to select. See available modes with
-            `available_modes`.
-         - `batch_size` (`int`): the batch size of the image. Default: 4.
-         - `shuffle` (`bool`): whether to shuffle the data before loading. Default: True.
-         - `num_workers` (`int`): number of workers for the dataloader. Default: 1.
-         - `remove_invalid` (`bool`): if set to True, deletes any NaN/corrupt items in the image set
+            
+        :param mode: The mode of training to select. See available modes with `available_modes`.
+        :type mode: str
+        :param batch_size: The batch size of the image. Default: 16.
+        :type batch_size: int
+        :param shuffle: Whether to shuffle the data before loading. Default: `True`.
+        :type shuffle: bool
+        :param num_workers: Number of workers for the dataloader. Default: 0.
+        :type num_workers: int
+        :param remove_invalid: If set to True, deletes any NaN/corrupt items in the image set
             pertaining to the relevant mode. In the False case, either NaN values are substituted
             with empty values or an error is thrown, depending on the mode selected.
-         - `store_dim` (`bool`): if set to True, the labels in the dataset will return a dict with
-            two keys. 'label' contains the standard PyTorch labels and 'dim' contains the image's
+        :type remove_invalid: bool
+        :param store_dim: If set to True, the labels in the dataset will return a dict with two
+            keys. `label` contains the standard PyTorch labels and `dim` contains the image's
             former dimensions.
-         - `preset_transform` (`bool`): whether to use default preset transforms. Consists of
-            normalization with either calculated mean of the dataset about to be used or standard
-            ImageNet statistics depending on `calculate_stats`. Default: True
-         - `calculate_stats` (`bool`): whether to calculate mean and std for this dataset to be used
-            in normalization transforms. If False, uses ImageNet default weights. Only has effect
-            when `preset_transform` is set to True. Default: True
-         - `mean` (`Tuple[float, ...]`): default mean statistics for the dataset. Has no effect when
+        :type store_dim: bool
+        :param preset_transform: Whether to use default preset transforms. Consists of normalization
+            with either calculated mean of the dataset about to be used or standard ImageNet
+            statistics depending on `calculate_stats`. Default: `True`
+        :type preset_transform: bool
+        :param calculate_stats: Whether to calculate mean and std for this dataset to be used in
+            normalization transforms. If False, uses ImageNet default weights. Only has effect
+            when `preset_transform` is set to `True`. Default: `True`
+        :type calculate_stats: bool
+        :param mean: Default mean statistics for the dataset. Has no effect when
             `calculate_stats = True`. Default: ImageNet values.
-         - `std` (`Tuple[float, ...]`): default mean statistics for the dataset. Has no effect when
+        :type mean: Tuple[float, ...]
+        :param std: Default mean statistics for the dataset. Has no effect when
             `calculate_stats = True`. Default: ImageNet values.
-         - `normalize` (`bool`): when set to True, normalize the dataset according to some
-            mean/std values, either from calculated stats or ImageNet default. This statement is
-            overriden when `calculate_stats` is set to True. Default: True.
-         - `image_set` (`Optional[str]`): the image set to pull from. Default: all images.
-         - `transform` (`Optional[Callable]`): the transform operation to apply to the images.
-         - `target_transform` (`Optional[Callable]`): the transform operation on the labels.
-         - `transforms` (`Optional[tuple[Optional[Callable], ...]]`): tuple in the format
-            `(transform, target_transform)`. Default PyTorch transforms are available in the
-            CVTransforms class.
-         - `resize` (`Optional[tuple[int, int]]`): if provided, resize all images to exact
-            configuration.
-         - `normalize_to` (`Optional[str]`): if provided, normalize bounding box/segmentation
-            coordinates to a specific configuration. Options: 'zeroone', 'full'
+        :type std: Tuple[float, ...]
+        :param normalize: When set to True, normalize the dataset according to some mean/std values,
+            either from calculated stats or ImageNet default. This statement is overriden when
+            `calculate_stats` is set to T`rue. Default: `True`.
+        :type normalize: bool
+        :param image_set: The image set to pull from. Default: all images.
+        :type image_set: Optional[str]
+        :param transform: The transform operation to apply to the images.
+        :type transform: Optional[Callable]
+        :param target_transform: The transform operation to apply to the labels.
+        :type target_transform: Optional[Callable]
+        :param transforms: Tuple in the format `(transform, target_transform)`. Obtain default
+            transforms from `DynamicData.get_transforms()`, or supply your own.
+        :type transforms: Optional[Tuple[Optional[Callable], ...]]
+        :param resize: If provided, resize all images to exact `(width, height)` configuration.
+        :type resize: Optional[Tuple[int, ...]]
+        :param normalize_to: If provided, normalize bounding box/segmentation coordinates to a
+            specific configuration. Options: 'zeroone', 'full'
+        :type normalize_to: Optional[str]
         '''
         return DataLoader(
             self.get_dataset(
                 mode,
                 remove_invalid=remove_invalid,
                 store_dim=store_dim,
                 image_set=image_set,
@@ -875,24 +786,27 @@
         seed: Optional[int] = None
     ) -> None:
         '''
         Split the existing image set into new image sets. If inplace is True, the existing image
         set will receive the percentage that is missing from the rest of the sets, or deleted if
         the other sets add up to 1.
         
-        Args:
-         - `image_set` (`str | int`): the old image set name to split. Accepts both name and ID.
-         - `new_sets` (`tuple[str, float]`): each entry of new_sets has a name for the set
-            accompanied with a float to represent the percentage to split data into.
-         - `inplace` (`bool`): whether to perform the operation inplace on the existing image set.
-            If False, then the new sets are required to add up to exactly 100% of the compositions.
-            If True, any remaining percentages less than 100% will be filled back into the old image
-            set. Default: False.
-         - `seed` (`Optional[int]`): the seed to use for the operation, in case consistent dataset
-            manipulation in memory is required. Default: None
+        :param image_set: The old image set name to split. Accepts both name and ID.
+        :type image_set: str | int
+        :param new_sets: Each entry of `new_sets` has a name for the set accompanied with a float to
+            represent the percentage to split data into.
+        :type new_sets: Tuple[str, float]
+        :param inplace: Whether to perform the operation inplace on the existing image set. If
+            `False`, then the new sets are required to add up to exactly 100% of the compositions.
+            If `True`, any remaining percentages less than 100% will be filled back into the old
+            image set. Default: `False`.
+        :type inplace: bool
+        :param seed: The seed to use for the operation, in case consistent dataset manipulation
+            in memory is required. Default: `None`
+        :type seed: Optional[int]
         '''
         # checks before splitting
         mode = 'name' if isinstance(image_set, str) else 'id'
         check_set = self.image_set_to_idx if mode == 'name' else self.idx_to_image_set
         if image_set not in check_set:
             Warnings.error('image_set_missing', imgset_name=mode, image_set=image_set)
         for new_set in new_sets:
@@ -947,32 +861,32 @@
 
     def get_image_set(
         self,
         image_set: Union[str, int]
     ) -> DataFrame:
         '''
         Retrieve the sub-DataFrame which contains all images in a specific image set.
-        
-        Args:
-         - image_set (str, int): the image set. Accepts both string and int.
+
+        :param image_set: The image set. Accepts both string and int.
+        :type image_set: str | int
         '''
         if isinstance(image_set, str):
             return self.dataframe[self.dataframe['IMAGE_SET_NAME'].apply(lambda x: image_set in x)]
         return self.dataframe[self.dataframe['IMAGE_SET_ID'].apply(lambda x: image_set in x)]
 
     def clear_image_sets(
         self,
         sets: Optional[list[Union[str, int]]] = None
     ) -> None:
         '''
         Clear image sets from the dict if they contain no elements.
-        
-        Args:
-         - sets (list[str | int], Optional): If defined, only scan the provided list, otherwise
-            scan all sets. Default: None.
+
+        :param sets: If defined, only scan the provided list, otherwise scan all sets.
+            Default: `None`.
+        :type sets: list[str | int], Optional
         '''
         to_pop = []
         if sets is None:
             sets = self.image_set_to_idx
         for image_set in sets:
             if len(self.get_image_set(image_set)) == 0:
                 to_pop.append(image_set)
@@ -988,17 +902,17 @@
     def delete_image_set(
         self,
         image_set: Union[str, int]
     ) -> None:
         '''
         Delete image set from all entries. If an entry has only that image set, replace with the
         default dataset.
-        
-        Args:
-         - image_set (str, int): the image set to delete. Accepts both name and ID.
+
+        :param image_set: The image set to delete. Accepts both name and ID.
+        :type image_set: str | int
         '''
         using_id: bool = isinstance(image_set, int)
         if using_id:
             if image_set not in self.idx_to_image_set:
                 Warnings.error('image_set_missing', imgset_name='ID', image_set=image_set)
             idx = image_set
             name = self.idx_to_image_set[idx]
@@ -1023,26 +937,28 @@
         if default and 'default' not in self.image_set_to_idx:
             self.image_set_to_idx['default'] = default_idx
             self.idx_to_image_set[default_idx] = 'default'
         self.clear_image_sets()
 
     def save(
         self,
-        filename: str,
+        filename: str = '',
         overwrite: bool = False,
         safe: bool = True
     ) -> None:
         '''
         Save the dataset into DynamicData json format.
-        
-        Args:
-         - filename (str): the filename to save the dataset.
-         - overwrite (bool): whether to overwrite the file if it already exists. Default: False.
-         - safe (bool): if True, do not encode `form` with jsonpickle. Then dataset cannot be
+
+        :param filename: The filename to save the dataset.
+        :type filename: str
+        :param overwrite: Whether to overwrite the file if it already exists. Default: `False`.
+        :type overwrite: bool
+        :param safe: If `True`, do not encode `form` with jsonpickle. Then dataset cannot be
             re-parsed, but is no longer subject to arbitrary code injection upon load.
+        :type safe: bool
         '''
         if not safe:
             Warnings.warn('unsafe_save')
         this = {
             'root': self.root,
             'safe': safe,
             'form': None if safe else jsonpickle.encode(self.form, keys=True),
@@ -1063,22 +979,22 @@
         }
         if os.path.exists(filename) and not overwrite:
             Warnings.error('file_exists', filename=filename)
         with open(filename, 'w', encoding='utf-8') as f:
             f.write(json.dumps(this))
 
     @classmethod
-    def load(cls, filename: str) -> Self:
+    def load(cls, filename: str = '') -> Self:
         '''
-        Load a DynamicData object from file. Warning: do not load any json files that you did not create.
-        This method uses jsonpickle, an insecure loading system with potential for arbitrary Python
-        code execution.
-        
-        Args:
-         - filename (str): the filename to load the data from.
+        Load a DynamicData object from file. Warning: do not load any json files that you did not
+        create. This method uses jsonpickle, an insecure loading system with potential for arbitrary
+        Python code execution.
+
+        :param filename: The filename to load the data from.
+        :type filename: str
         '''
         try:
             print('[DynamicData] Loading dataset...')
             start = time.time()
             with open(filename, 'r', encoding='utf-8') as f:
                 data = json.load(f)
             if not data['safe']:
@@ -1115,20 +1031,22 @@
         self,
         dpi: float = 1200,
         mode: Optional[str | list[str]] = None,
         idx: Optional[int] = None
     ) -> None:
         '''
         Sample an image from the dataset.
-        
-        Args:
-         - `dpi` (`float`): the image display size, if not in segmentation mode.
-         - `mode` (`Optional[str | list[str]]`): pick from any of the available modes, or supply a
-            list of modes. Default: all modes.
-         - `idx` (`Optional[int]`): use a specific idx from the dataset. Default: a random image.
+
+        :param dpi: The image display size, if not in segmentation mode.
+        :type dpi: float
+        :param mode: Pick from any of the available modes, or supply a list of modes. Default:
+            all modes.
+        :type mode: Optional[str | list[str]]
+        :param idx: Use a specific idx from the dataset. Default: a random image.
+        :type idx: Optional[int]
         '''
         if not self.cleaned:
             self.parse()
         if mode is not None:
             mode = union(mode)
             for try_mode in mode:
                 if try_mode not in self.available_modes:
@@ -1149,205 +1067,27 @@
                     image,
                     torch.stack([FloatTensor(box) for box in item['BOX']]),
                     width=3,
                     labels=item['BBOX_CLASS_NAME'],
                     colors='red'
                 )
             else: print('[DynamicData] Warning: Image has no bounding boxes.')
-        if 'segmentation' in mode:
+        if 'segmentation_mask' in mode:
             _, axarr = plt.subplots(ncols=2)
             axarr[0].imshow(image.permute(1, 2, 0))
-            if 'ABSOLUTE_FILE_SEG' in item:
-                mask = F.to_tensor(open_image(item['ABSOLUTE_FILE_SEG']))
-                axarr[1].imshow(mask.permute(1, 2, 0))
-            else:
-                assert len(item['POLYGON']) == len(item['SEG_CLASS_ID']), \
-                    'SEG_CLASS_ID and POLYGON len mismatch'
-                mask = np.asarray(cv2.imread(item['ABSOLUTE_FILE'], cv2.IMREAD_GRAYSCALE))
-                mask = np.asarray(mask, dtype=np.int32)
-                mask = np.full_like(mask, next_avail_id(self.idx_to_seg_class))
-                for class_id, polygon in zip(item['SEG_CLASS_ID'], item['POLYGON']):
-                    mask = cv2.fillPoly(mask, pts=[np.asarray(polygon, dtype=np.int32)],
-                                    color=class_id)
-                mask = torch.from_numpy(np.asarray(mask))
-                axarr[1].imshow(mask)
-        else:
-            plt.imshow(image.permute(1, 2, 0))
-
-    def inference(
-        self,
-        image: torch.Tensor,
-        label: Any,
-        result: Any,
-        dpi: float = 1200,
-        mode: str = None
-    ) -> None:
-        '''
-        Plot an image output. Not implemented yet
-        '''
-        if not self.cleaned:
-            self.parse()
-        if mode is None:
-            Warnings.error('is_none', desc='Mode')
-        if mode not in self.available_modes:
-            Warnings.error('mode_unavailable', mode=mode)
-        plt.figure(dpi=dpi)
-        if mode == 'classification':
-            _, pred = torch.max(result, dim=1)
-            print(f'[DynamicData] Image Class ID/Name: {pred}/{self.idx_to_class[pred]}')
-        elif mode == 'detection':
-            boxes = result['boxes']
-            labels = result['labels']
-            if len(boxes) != 0:
-                image = draw_bounding_boxes(
-                    image,
-                    boxes,
-                    width=3,
-                    colors='red',
-                    labels=[self.idx_to_bbox_class[label] for label in labels]
-                )
-            else: print('[DynamicData] Warning: Image has no bounding boxes.')
-        if mode == 'segmentation':
+            mask = F.to_tensor(open_image(item['ABSOLUTE_FILE_SEG']))
+            axarr[1].imshow(mask.permute(1, 2, 0))
+        if 'segmentation_poly' in mode:
             _, axarr = plt.subplots(ncols=2)
             axarr[0].imshow(image.permute(1, 2, 0))
-            mask = result['out'] if isinstance(result, dict) and 'out' in result else result
-            if not isinstance(mask, torch.Tensor):
-                raise ValueError('Cannot infer output mask tensor.')
-            mask = torch.argmax(mask, dim=1)
-            axarr[1].imshow(mask.permute(1, 2, 0))
+            assert len(item['POLYGON']) == len(item['SEG_CLASS_ID']), \
+                'SEG_CLASS_ID and POLYGON len mismatch'
+            mask = np.asarray(cv2.imread(item['ABSOLUTE_FILE'], cv2.IMREAD_GRAYSCALE))
+            mask = np.asarray(mask, dtype=np.int32)
+            mask = np.full_like(mask, next_avail_id(self.idx_to_seg_class))
+            for class_id, polygon in zip(item['SEG_CLASS_ID'], item['POLYGON']):
+                mask = cv2.fillPoly(mask, pts=[np.asarray(polygon, dtype=np.int32)],
+                                color=class_id)
+            mask = torch.from_numpy(np.asarray(mask))
+            axarr[1].imshow(mask)
         else:
             plt.imshow(image.permute(1, 2, 0))
-
-class DynamicDS(VisionDataset):
-    '''
-    Dataset implementation for the DynamicData environment.
-    
-    Args:
-    - `df` (`DataFrame`): the dataframe from DynamicData.
-    - `root` (`str`): the root of the dataset folder.
-    - `mode` (`str`): the mode of the data to retrieve, i.e. classification, segmentation, etc.
-    - `id_mapping` (`dict[int, int]`): the id mapping from the dataframe to retrieve class names.
-    This is used primarily as a safety feature in order to make sure that used IDs are provided
-    in order starting from 0 without holes so that training works properly.
-    - `image_type` (`str`): the type of the image to export, to convert PIL images to.
-    Default: 'RGB'. Also accepts 'L' and 'CMYK'.
-    - `normalization` (`str`): the type of normalization that the dataset currently is formatted in,
-    for box and polygon items. Accepts 'full' or 'zeroone'.
-    - `normalize_to` (`str`): the type of normalization that the dataset is to be resized to, for
-    box and polygon items. Accepts 'full' or 'zeroone'.
-    - `transform` (`Optional[Callable]`): the transform operation to apply to the images.
-    - `target_transform` (`Optional[Callable]`): the transform operation on the labels.
-    '''
-    def __init__(
-        self,
-        df: DataFrame,
-        root: str,
-        mode: str,
-        id_mapping: Optional[dict[int, int]],
-        image_type: str = 'RGB',
-        normalization: str = 'full',
-        store_dim: bool = False,
-        resize: Optional[tuple[int, int]] = None,
-        normalize_to: Optional[str] = None,
-        transform: Optional[Callable] = None,
-        target_transform: Optional[Callable] = None
-    ):
-        self.dataframe = df
-        self.data = self.dataframe.to_dict('records')
-        self.mode = mode
-        self.image_type = image_type
-        self.id_mapping = id_mapping
-        self.store_dim = store_dim
-        self.resize = resize
-        self.normalize_to = normalize_to
-        self.normalization = normalization
-        if self.mode == 'segmentation':
-            self.default = len(self.id_mapping)
-        super().__init__(
-            root,
-            transforms=None,
-            transform=transform,
-            target_transform=target_transform
-        )
-
-    def __len__(self):
-        return len(self.dataframe)
-
-    def _get_class_labels(self, item: Series) -> Tensor:
-        return self.id_mapping[int(item['CLASS_ID'])]
-
-    def _get_bbox_labels(self, item: Series) -> dict[str, Tensor]:
-        # execute checks
-        assert len(item['BOX']) == len(item['BBOX_CLASS_ID']), \
-            'BOX and BBOX_CLASS_ID len mismatch'
-        class_ids = list(map(lambda x: self.id_mapping[x], item['BBOX_CLASS_ID']))
-        boxes = item['BOX']
-        if self.resize:
-            factor_resize = self.resize
-        else:
-            factor_resize = (1, 1)
-        if self.normalization == 'full':
-            factor_norm = item['IMAGE_DIM']
-        else:
-            factor_norm = (1, 1)
-        apply_resize = lambda p: (p[0] * factor_resize[0] / factor_norm[0],
-                                  p[1] * factor_resize[1] / factor_norm[1],
-                                  p[2] * factor_resize[0] / factor_norm[0],
-                                  p[3] * factor_resize[1] / factor_norm[1])
-        bbox_tensors = [FloatTensor(apply_resize(box)) for box in boxes]
-        if not bbox_tensors:
-            Warnings.error('empty_bbox', file=item['ABSOLUTE_FILE'])
-        if self.store_dim:
-            return {
-                'label': {'boxes': torch.stack(bbox_tensors), 'labels': LongTensor(class_ids)},
-                'dim': item['IMAGE_DIM']
-            }
-        return {'boxes': torch.stack(bbox_tensors), 'labels': LongTensor(class_ids)}
-
-    def _get_seg_labels(self, item: Series) -> Tensor:
-        if 'ABSOLUTE_FILE_SEG' in item:
-            mask = F.to_tensor(open_image(item['ABSOLUTE_FILE_SEG']))
-            if self.resize:
-                return F.resize(mask, [self.resize[1], self.resize[0]])
-            return mask
-        assert len(item['POLYGON']) == len(item['SEG_CLASS_ID']), \
-            'SEG_CLASS_ID and POLYGON len mismatch'
-        if self.resize is not None:
-            mask = np.full(self.resize, self.default, dtype=np.int32)
-            factor_resize = self.resize
-        else:
-            mask = np.full(item['IMAGE_DIM'], self.default, dtype=np.int32)
-            factor_resize = (1, 1)
-        if self.normalization == 'full':
-            factor_norm = item['IMAGE_DIM']
-        else: factor_norm = (1, 1)
-        apply_resize = lambda p: (p[0] * factor_resize[0] / factor_norm[0],
-                                  p[1] * factor_resize[1] / factor_norm[1])
-        for class_id, polygon in zip(item['SEG_CLASS_ID'], item['POLYGON']):
-            if self.resize is not None:
-                polygon = list(map(apply_resize, polygon))
-            mask = cv2.fillPoly(mask, pts=[np.asarray(polygon, dtype=np.int32)],
-                            color=self.id_mapping[class_id])
-        mask = torch.from_numpy(np.asarray(mask)).unsqueeze(-1).permute(2, 0, 1)
-        return mask
-
-    def __getitem__(self, idx):
-        item: dict = self.data[idx]
-        image: Tensor = F.to_tensor(open_image(item.get('ABSOLUTE_FILE')).convert(self.image_type))
-        if self.resize:
-            image = F.resize(image, [self.resize[1], self.resize[0]])
-        label: dict[str, Tensor]
-        if self.mode in {'inference', 'diffusion'}:
-            if self.transform:
-                image = self.transform(image)
-            return image, {'dim': item['IMAGE_DIM']}
-        if self.mode == 'classification':
-            label = self._get_class_labels(item)
-        elif self.mode == 'detection':
-            label = self._get_bbox_labels(item)
-        elif self.mode == 'segmentation':
-            label = self._get_seg_labels(item)
-        if self.transforms:
-            image, label = self.transforms(image, label)
-        if self.store_dim:
-            return image, {'label': label, 'dim': item['IMAGE_DIM']}
-        return image, label
```

### Comparing `dynamicdl_headless-0.1.0a0/dynamicdl/transforms.py` & `dynamicdl_headless-0.1.1a0/dynamicdl/_main/_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,17 +143,17 @@
 
 class Transforms:
     '''
     Standard transforms presets for computer vision. Adapted from torchvision 0.17.2
     '''
     CLASSIFICATION = (ImageClassification(crop_size=224), None)
     DETECTION = (ObjectDetection(), None)
-    SEGMENTATION = (SemanticSegmentation(resize_size=520, normalize=True), 
+    SEGMENTATION = (SemanticSegmentation(resize_size=520, normalize=True),
                     SemanticSegmentation(resize_size=520, normalize=False))
-    SEGMENTATION_NORESIZE = (SemanticSegmentation(resize_size=None, normalize=True), 
+    SEGMENTATION_NORESIZE = (SemanticSegmentation(resize_size=None, normalize=True),
                              SemanticSegmentation(resize_size=None, normalize=False))
 
     @staticmethod
     def get(
         mode: str,
         resize: bool = False,
         normalize: bool = True,
```

### Comparing `dynamicdl_headless-0.1.0a0/dynamicdl_headless.egg-info/PKG-INFO` & `dynamicdl_headless-0.1.1a0/dynamicdl_headless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicdl-headless
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: A PyTorch-based dynamic dataloading library
 Home-page: https://github.com/ESB-AI-Lab/DynamicDL-Headless
 Author: Anthony Tong
 Author-email: atong28.usa@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dynamicdl_headless-0.1.0a0/pyproject.toml` & `dynamicdl_headless-0.1.1a0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "dynamicdl-headless"
-version = "0.1.0-alpha"
+version = "0.1.1-alpha"
 description = "A PyTorch-based dynamic dataloading library"
 authors = ["Anthony Tong <atong28.usa@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://esb-ai-lab.github.io/DynamicDL"
 repository = "https://github.com/ESB-AI-Lab/DynamicDL"
+include = [{ path = "dynamicdl/config.json", format = ["sdist", "wheel"] }]
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.9"
 opencv-python-headless = { version = ">=4.6.0,<=4.9.0.80" }
 Pillow = { version = ">=8.0.0,<=10.3.0" }
 PyYAML = { version = ">=5.4.0,<=6.0.1" }
 tqdm = { version = ">=4.1.0,<=4.66.2" }
 numpy = { version = ">=1.18.0,<2.0.0" }
 pandas = { version = ">=1.0.0,<=2.2.2" }
 torch = { version = ">=2.0.0,<=2.3.0" }
```

### Comparing `dynamicdl_headless-0.1.0a0/setup.py` & `dynamicdl_headless-0.1.1a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dynamicdl-headless',
-    version='0.1.0-alpha',
+    version='0.1.1-alpha',
     packages=find_packages(),
     license='Apache License 2.0',
     author='Anthony Tong',
     author_email='atong28.usa@gmail.com',
     description='A PyTorch-based dynamic dataloading library',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
@@ -21,8 +21,9 @@
         "torch>=2.0.0,<=2.3.0",
         "torchvision>=0.15.1,<=0.18.0",
         "typing-extensions>=4.0.0,<=4.11.0",
         "xmltodict>=0.12.0,<=0.13.0",
         "jsonpickle>=3.0.0,<=3.1.0",
         "matplotlib>=3.6.0,<=3.8.4"
     ],
+    include_package_data=True
 )
```

