# Comparing `tmp/python_motionmount-1.0.1.tar.gz` & `tmp/python_motionmount-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_motionmount-1.0.1.tar", last modified: Tue Apr 30 11:50:17 2024, max compression
+gzip compressed data, was "python_motionmount-2.0.0.tar", last modified: Mon Jun  3 12:47:34 2024, max compression
```

## Comparing `python_motionmount-1.0.1.tar` & `python_motionmount-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:17.002947 python_motionmount-1.0.1/
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     1073 2023-10-27 08:23:06.000000 python_motionmount-1.0.1/LICENSE.txt
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     3204 2024-04-30 11:50:17.002781 python_motionmount-1.0.1/PKG-INFO
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     1521 2024-04-30 11:48:02.000000 python_motionmount-1.0.1/README.md
--rw-r--r--   0 remcopoelstra   (501) staff       (20)       85 2023-10-27 08:23:06.000000 python_motionmount-1.0.1/pyproject.toml
--rw-r--r--   0 remcopoelstra   (501) staff       (20)      852 2024-04-30 11:50:17.003750 python_motionmount-1.0.1/setup.cfg
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:16.997402 python_motionmount-1.0.1/src/
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:17.000400 python_motionmount-1.0.1/src/motionmount/
--rw-r--r--   0 remcopoelstra   (501) staff       (20)      203 2023-10-27 08:23:06.000000 python_motionmount-1.0.1/src/motionmount/__init__.py
--rw-r--r--   0 remcopoelstra   (501) staff       (20)    16803 2024-04-30 11:48:02.000000 python_motionmount-1.0.1/src/motionmount/motionmount.py
--rw-r--r--   0 remcopoelstra   (501) staff       (20)        0 2023-11-06 15:45:57.000000 python_motionmount-1.0.1/src/motionmount/py.typed
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:17.002240 python_motionmount-1.0.1/src/python_MotionMount.egg-info/
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     3204 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/PKG-INFO
--rw-r--r--   0 remcopoelstra   (501) staff       (20)      314 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/SOURCES.txt
--rw-r--r--   0 remcopoelstra   (501) staff       (20)        1 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/dependency_links.txt
--rw-r--r--   0 remcopoelstra   (501) staff       (20)       12 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/top_level.txt
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-06-03 12:47:34.019720 python_motionmount-2.0.0/
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     1073 2023-10-27 08:23:06.000000 python_motionmount-2.0.0/LICENSE.txt
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     3246 2024-06-03 12:47:34.019549 python_motionmount-2.0.0/PKG-INFO
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     1564 2024-06-03 12:44:24.000000 python_motionmount-2.0.0/README.md
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)       85 2023-10-27 08:23:06.000000 python_motionmount-2.0.0/pyproject.toml
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)      852 2024-06-03 12:47:34.020506 python_motionmount-2.0.0/setup.cfg
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-06-03 12:47:34.013674 python_motionmount-2.0.0/src/
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-06-03 12:47:34.017091 python_motionmount-2.0.0/src/motionmount/
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)      203 2023-10-27 08:23:06.000000 python_motionmount-2.0.0/src/motionmount/__init__.py
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)    17387 2024-06-03 12:44:24.000000 python_motionmount-2.0.0/src/motionmount/motionmount.py
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)        0 2023-11-06 15:45:57.000000 python_motionmount-2.0.0/src/motionmount/py.typed
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-06-03 12:47:34.019005 python_motionmount-2.0.0/src/python_MotionMount.egg-info/
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     3246 2024-06-03 12:47:34.000000 python_motionmount-2.0.0/src/python_MotionMount.egg-info/PKG-INFO
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)      314 2024-06-03 12:47:34.000000 python_motionmount-2.0.0/src/python_MotionMount.egg-info/SOURCES.txt
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)        1 2024-06-03 12:47:34.000000 python_motionmount-2.0.0/src/python_MotionMount.egg-info/dependency_links.txt
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)       12 2024-06-03 12:47:34.000000 python_motionmount-2.0.0/src/python_MotionMount.egg-info/top_level.txt
```

### Comparing `python_motionmount-1.0.1/LICENSE.txt` & `python_motionmount-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_motionmount-1.0.1/PKG-INFO` & `python_motionmount-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-MotionMount
-Version: 1.0.1
+Version: 2.0.0
 Summary: Control your MotionMount Signature TVM7675 Pro using Python
 Home-page: https://github.com/vogelsproducts/python-MotionMount
 Author: Remco Poelstra
 Author-email: r.poelstra@vogels.com
 Project-URL: Bug Tracker, https://github.com/vogelsproducts/python-MotionMount/issues
 Project-URL: repository, https://github.com/vogelsproducts/python-MotionMount
 Classifier: Programming Language :: Python :: 3
@@ -55,14 +55,15 @@
 
 To get the IP address of the MotionMount you can use [pyzeroconf](https://github.com/paulsm/pyzeroconf) or you can use a manual tool like `dns-sd` in the macOS Terminal or a GUI tool like [Discovery](https://apps.apple.com/nl/app/discovery-dns-sd-browser/id1381004916?mt=12) (macOS) or [Bonjour Browser](https://hobbyistsoftware.com/bonjourbrowser) (Windows)
   
 A simple example using `pyzeroconf` is included in the `examples` folder.
     
 # Changelog
 1.0.1: - Fix bug in allowed preset indices
+2.0.0: - Include position data in presets
 
 MIT License
 
 Copyright (c) 2023 Vogel's Products
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `python_motionmount-1.0.1/README.md` & `python_motionmount-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,7 +39,8 @@
 
 To get the IP address of the MotionMount you can use [pyzeroconf](https://github.com/paulsm/pyzeroconf) or you can use a manual tool like `dns-sd` in the macOS Terminal or a GUI tool like [Discovery](https://apps.apple.com/nl/app/discovery-dns-sd-browser/id1381004916?mt=12) (macOS) or [Bonjour Browser](https://hobbyistsoftware.com/bonjourbrowser) (Windows)
   
 A simple example using `pyzeroconf` is included in the `examples` folder.
     
 # Changelog
 1.0.1: - Fix bug in allowed preset indices
+2.0.0: - Include position data in presets
```

### Comparing `python_motionmount-1.0.1/setup.cfg` & `python_motionmount-2.0.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-MotionMount
-version = 1.0.1
+version = 2.0.0
 author = Remco Poelstra
 author_email = r.poelstra@vogels.com
 description = Control your MotionMount Signature TVM7675 Pro using Python
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/vogelsproducts/python-MotionMount
 project_urls =
```

### Comparing `python_motionmount-1.0.1/src/motionmount/motionmount.py` & `python_motionmount-2.0.0/src/motionmount/motionmount.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,26 @@
     elif value_type == MotionMountValueType.Bool:
         return bool(int(value))
     elif value_type == MotionMountValueType.Void:
         return value
     else:
         raise ValueError("Unknown value type")
 
+class Preset:
+    """Class for storing preset related data"""
+    index: int
+    name: str
+    extension: int
+    turn: int
+
+    def __init__(self, index, name, extension, turn):
+        self.index = index
+        self.name = name
+        self.extension = extension
+        self.turn = turn
 
 class MotionMount:
     """
     Class to represent a MotionMount.
 
     You can create one with the IP address and port number which should be used to connect.
 
@@ -292,24 +304,30 @@
 
     async def update_error_status(self):
         """Fetch the error status from the MotionMount"""
         # We mark the value types as Void, as we've no further interest in the actual value
         # We just want to trigger the notification logic
         await self._request(Request("mount/errorStatus", MotionMountValueType.Void))
 
-    async def get_presets(self) -> dict[int, str]:
+    async def get_presets(self) -> [Preset]:
         """Gets the valid user presets from the device."""
-        presets = {}
-        
+        presets = []
+
         for i in range(1,8):
             valid = await self._request(Request(f"mount/preset/{i}/active", MotionMountValueType.Bool))
 
             if valid:
-                presets[i] = await self._request(Request(f"mount/preset/{i}/name", MotionMountValueType.String))
-            
+                name = await self._request(Request(f"mount/preset/{i}/name", MotionMountValueType.String))
+                extension = await self._request(Request(f"mount/preset/{i}/extension", MotionMountValueType.Integer))
+                turn = await self._request(Request(f"mount/preset/{i}/turn", MotionMountValueType.Integer))
+
+                preset = Preset(i, name, extension, turn)
+
+                presets.append(preset)
+
         return presets
         
     async def go_to_preset(self, position: int):
         """
         Go to a preset position.
         Preset 0 is the (fixed) Wall position.
```

### Comparing `python_motionmount-1.0.1/src/python_MotionMount.egg-info/PKG-INFO` & `python_motionmount-2.0.0/src/python_MotionMount.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-MotionMount
-Version: 1.0.1
+Version: 2.0.0
 Summary: Control your MotionMount Signature TVM7675 Pro using Python
 Home-page: https://github.com/vogelsproducts/python-MotionMount
 Author: Remco Poelstra
 Author-email: r.poelstra@vogels.com
 Project-URL: Bug Tracker, https://github.com/vogelsproducts/python-MotionMount/issues
 Project-URL: repository, https://github.com/vogelsproducts/python-MotionMount
 Classifier: Programming Language :: Python :: 3
@@ -55,14 +55,15 @@
 
 To get the IP address of the MotionMount you can use [pyzeroconf](https://github.com/paulsm/pyzeroconf) or you can use a manual tool like `dns-sd` in the macOS Terminal or a GUI tool like [Discovery](https://apps.apple.com/nl/app/discovery-dns-sd-browser/id1381004916?mt=12) (macOS) or [Bonjour Browser](https://hobbyistsoftware.com/bonjourbrowser) (Windows)
   
 A simple example using `pyzeroconf` is included in the `examples` folder.
     
 # Changelog
 1.0.1: - Fix bug in allowed preset indices
+2.0.0: - Include position data in presets
 
 MIT License
 
 Copyright (c) 2023 Vogel's Products
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

