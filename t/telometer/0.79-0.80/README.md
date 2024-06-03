# Comparing `tmp/telometer-0.79.tar.gz` & `tmp/telometer-0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telometer-0.79.tar", last modified: Sun Jun  2 07:29:08 2024, max compression
+gzip compressed data, was "telometer-0.80.tar", last modified: Mon Jun  3 01:42:53 2024, max compression
```

## Comparing `telometer-0.79.tar` & `telometer-0.80.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-02 07:29:08.198202 telometer-0.79/
--rw-r--r--   0 santiago   (501) staff       (20)     1074 2024-05-22 15:01:09.000000 telometer-0.79/LICENSE.txt
--rw-r--r--   0 santiago   (501) staff       (20)      613 2024-06-02 07:29:08.197727 telometer-0.79/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)      148 2024-05-22 15:03:15.000000 telometer-0.79/README.md
--rw-r--r--   0 santiago   (501) staff       (20)       38 2024-06-02 07:29:08.198257 telometer-0.79/setup.cfg
--rw-r--r--   0 santiago   (501) staff       (20)      826 2024-06-02 07:29:02.000000 telometer-0.79/setup.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-02 07:29:08.187487 telometer-0.79/telometer/
--rw-r--r--   0 santiago   (501) staff       (20)       91 2023-12-02 23:50:44.000000 telometer-0.79/telometer/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)     7893 2024-06-02 07:28:41.000000 telometer-0.79/telometer/telometer.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-02 07:29:08.197343 telometer-0.79/telometer.egg-info/
--rw-r--r--   0 santiago   (501) staff       (20)      613 2024-06-02 07:29:08.000000 telometer-0.79/telometer.egg-info/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)      243 2024-06-02 07:29:08.000000 telometer-0.79/telometer.egg-info/SOURCES.txt
--rw-r--r--   0 santiago   (501) staff       (20)        1 2024-06-02 07:29:08.000000 telometer-0.79/telometer.egg-info/dependency_links.txt
--rw-r--r--   0 santiago   (501) staff       (20)       66 2024-06-02 07:29:08.000000 telometer-0.79/telometer.egg-info/entry_points.txt
--rw-r--r--   0 santiago   (501) staff       (20)       10 2024-06-02 07:29:08.000000 telometer-0.79/telometer.egg-info/top_level.txt
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-03 01:42:53.730991 telometer-0.80/
+-rw-r--r--   0 santiago   (501) staff       (20)     1074 2024-05-22 15:01:09.000000 telometer-0.80/LICENSE.txt
+-rw-r--r--   0 santiago   (501) staff       (20)      613 2024-06-03 01:42:53.730341 telometer-0.80/PKG-INFO
+-rw-r--r--   0 santiago   (501) staff       (20)      148 2024-05-22 15:03:15.000000 telometer-0.80/README.md
+-rw-r--r--   0 santiago   (501) staff       (20)       38 2024-06-03 01:42:53.731065 telometer-0.80/setup.cfg
+-rw-r--r--   0 santiago   (501) staff       (20)      826 2024-06-03 01:24:11.000000 telometer-0.80/setup.py
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-03 01:42:53.710184 telometer-0.80/telometer/
+-rw-r--r--   0 santiago   (501) staff       (20)       91 2023-12-02 23:50:44.000000 telometer-0.80/telometer/__init__.py
+-rw-r--r--   0 santiago   (501) staff       (20)     7938 2024-06-03 01:35:50.000000 telometer-0.80/telometer/telometer.py
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-06-03 01:42:53.729676 telometer-0.80/telometer.egg-info/
+-rw-r--r--   0 santiago   (501) staff       (20)      613 2024-06-03 01:42:53.000000 telometer-0.80/telometer.egg-info/PKG-INFO
+-rw-r--r--   0 santiago   (501) staff       (20)      243 2024-06-03 01:42:53.000000 telometer-0.80/telometer.egg-info/SOURCES.txt
+-rw-r--r--   0 santiago   (501) staff       (20)        1 2024-06-03 01:42:53.000000 telometer-0.80/telometer.egg-info/dependency_links.txt
+-rw-r--r--   0 santiago   (501) staff       (20)       66 2024-06-03 01:42:53.000000 telometer-0.80/telometer.egg-info/entry_points.txt
+-rw-r--r--   0 santiago   (501) staff       (20)       10 2024-06-03 01:42:53.000000 telometer-0.80/telometer.egg-info/top_level.txt
```

### Comparing `telometer-0.79/LICENSE.txt` & `telometer-0.80/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telometer-0.79/PKG-INFO` & `telometer-0.80/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telometer
-Version: 0.79
+Version: 0.80
 Summary: a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data
 Author: Santiago E Sanchez
 Author-email: ses94@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telometer-0.79/setup.py` & `telometer-0.80/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="telometer",
-    version="0.79",
+    version="0.80",
     author="Santiago E Sanchez",
     author_email="ses94@stanford.edu",
     description="a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data",
     packages=setuptools.find_packages(),
     license='MIT',
     long_description=open('README.md').read(),
     classifiers=[
```

### Comparing `telometer-0.79/telometer/telometer.py` & `telometer-0.80/telometer/telometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Telometer v0.78
+# Telometer v0.79
 # Created by: Santiago E Sanche8
 # Artandi Lab, Stanford University, 2024
 # Measures telomeres from ONT or PacBio long reads aligned to a T2T genome assembly
 # Simple Usage: telometer -b sorted_t2t.bam -o output.ts8
 import pysam
 import re
 import regex as re
@@ -84,36 +84,33 @@
 
         telomere_region = seq_to_check[telomere_start:telomere_end]
         telomere_repeat = [m.group() for m in re.finditer(g_rich_telomere_pattern, telomere_region)]
         if not telomere_repeat:
             telomere_repeat = [m.group() for m in re.finditer(c_rich_telomere_pattern, telomere_region)]
 
         telomere_length = len(''.join(telomere_repeat))
-
+        if telomere_length > 0:
         # Find the region immediately adjacent to the telomere region
-        boundary_mm1_region = seq_to_check[telomere_end:]
-        boundary_mm1_length = find_initial_boundary_region(boundary_mm1_region, g_rich_telomere_pattern.split('|') + c_rich_telomere_pattern.split('|'), max_mismatches=2)
-    else:
-        telomere_start = None
-        telomere_end = None
-        telomere_length = 0
-        boundary_mm1_length = 0
-
-    result = {
-        'read_id': read_data['read_id'],
-        'telomere_start': telomere_start,
-        'telomere_end': telomere_end,
-        'telomere_length': telomere_length,
-        'subtel_boundary_length': boundary_mm1_length,
-        'chromosome': read_data['reference_name'],
-        'mapping_quality': read_data['mapping_quality'],
-        'direction': direction,
-        'arm': arm
-    }
-    return result
+            boundary_mm1_region = seq_to_check[telomere_end:]
+            boundary_mm1_length = find_initial_boundary_region(boundary_mm1_region, g_rich_telomere_pattern.split('|') + c_rich_telomere_pattern.split('|'), max_mismatches=2)
+            result = {
+                'chromosome': read_data['reference_name'],
+                'arm': arm,
+                'telomere_start': telomere_start,
+                'telomere_end': telomere_end,
+                'telomere_length': telomere_length,
+                'subtel_boundary_length': boundary_mm1_length,
+                'read_id': read_data['read_id'],
+                'mapping_quality': read_data['mapping_quality'],
+                'direction': direction
+            }
+            return result
+        else:
+            return None
+
 
 def calculate_telomere_length():
     parser = argparse.ArgumentParser(description='Calculate telomere length from a BAM file.')
     parser.add_argument('-b', '--bam', help='The path to the sorted BAM file.', required=True)
     parser.add_argument('-o', '--output', help='The path to the output file.', required=True)
     parser.add_argument('-c', '--chemistry', default="r10", help="Sequencing chemistry (r9 or r10, default=r10). Optional", required=False)
     parser.add_argument('-m', '--minreadlen', default=1000, type=int, help='Minimum read length to consider (Default: 1000 for telomere capture, use 4000 for WGS). Optional', required=False)
```

### Comparing `telometer-0.79/telometer.egg-info/PKG-INFO` & `telometer-0.80/telometer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telometer
-Version: 0.79
+Version: 0.80
 Summary: a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data
 Author: Santiago E Sanchez
 Author-email: ses94@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

