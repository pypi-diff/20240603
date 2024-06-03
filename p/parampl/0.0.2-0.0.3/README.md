# Comparing `tmp/parampl-0.0.2.tar.gz` & `tmp/parampl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parampl-0.0.2.tar", max compression
+gzip compressed data, was "parampl-0.0.3.tar", max compression
```

## Comparing `parampl-0.0.2.tar` & `parampl-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35823 2024-05-31 20:51:31.876860 parampl-0.0.2/LICENSE
--rw-r--r--   0        0        0       25 2024-05-31 23:21:15.600757 parampl-0.0.2/parampl/__init__.py
--rw-r--r--   0        0        0    10292 2024-06-02 04:54:22.609419 parampl-0.0.2/parampl/core.py
--rw-r--r--   0        0        0     3985 2024-06-02 04:38:53.232069 parampl-0.0.2/parampl/statics.py
--rw-r--r--   0        0        0      584 2024-06-02 05:00:02.905705 parampl-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       53 2024-05-31 20:51:31.876860 parampl-0.0.2/README.md
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 parampl-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-05-31 20:51:31.876860 parampl-0.0.3/LICENSE
+-rw-r--r--   0        0        0       25 2024-05-31 23:21:15.600757 parampl-0.0.3/parampl/__init__.py
+-rw-r--r--   0        0        0    10221 2024-06-02 06:06:56.618674 parampl-0.0.3/parampl/core.py
+-rw-r--r--   0        0        0     5571 2024-06-02 06:06:56.625900 parampl-0.0.3/parampl/statics.py
+-rw-r--r--   0        0        0      584 2024-06-02 06:08:35.152783 parampl-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-05-31 20:51:31.876860 parampl-0.0.3/README.md
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 parampl-0.0.3/PKG-INFO
```

### Comparing `parampl-0.0.2/LICENSE` & `parampl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parampl-0.0.2/parampl/core.py` & `parampl-0.0.3/parampl/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from matplotlib import pyplot as plt
 
-from parampl.statics import split_into_paragraphs, parse_avoid
-
-vertical_lims = tuple[float, float]
-avoid_specification = tuple[float, vertical_lims]
+from parampl.statics import split_into_paragraphs, parse_avoid, avoid_specification
 
 
 class ParaMPL:
     def write(self,
               text,
               xy,
               collapse_whites=True,
@@ -237,14 +234,14 @@
     ax.axvline(test_xy[0])
     ax.axvline(test_xy[0] + test_width)
 
     para.write(test_text, test_xy,
                avoid_left_of=[(0.4, (0.2, 0.4)),
                               (0.2, (0, 0.7)),
                               ],
-               avoid_right_of=[(0.8, (0.6, 0.5)),
+               avoid_right_of=[(0.8, (0.7, 0.5)),
                                (0.7, (0, 0.2)),
                                ],
-               width=test_width, justify='center')
+               width=test_width, justify='full')
     # , justify='full')#, avoid_left_of=(0.2, (0.2, 0.4)))
 
     f.show()
```

### Comparing `parampl-0.0.2/pyproject.toml` & `parampl-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "parampl"
 description = "Formatting paragraphs for matplotlib text"
 authors = ["duckrojo <3063609+duckrojo@users.noreply.github.com>"]
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.3"
 #documentation = "https://parampl.readthedocs.io/en/latest/"
 repository = "https://github.com/duckrojo/parampl"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `parampl-0.0.2/PKG-INFO` & `parampl-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parampl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Formatting paragraphs for matplotlib text
 Home-page: https://github.com/duckrojo/parampl
 Author: duckrojo
 Author-email: 3063609+duckrojo@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

