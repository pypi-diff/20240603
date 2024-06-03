# Comparing `tmp/pulse_linter-0.0.5.tar.gz` & `tmp/pulse_linter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulse_linter-0.0.5.tar", last modified: Mon Jun  3 09:07:41 2024, max compression
+gzip compressed data, was "pulse_linter-0.0.6.tar", last modified: Mon Jun  3 10:58:09 2024, max compression
```

## Comparing `pulse_linter-0.0.5.tar` & `pulse_linter-0.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.222201 pulse_linter-0.0.5/
--rw-rw-rw-   0        0        0     1689 2024-06-03 09:07:41.222201 pulse_linter-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.185261 pulse_linter-0.0.5/pulse_linter/
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.192270 pulse_linter-0.0.5/pulse_linter/Blacklist/
--rw-rw-rw-   0        0        0        0 2024-05-22 09:13:00.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.197185 pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/
--rw-rw-rw-   0        0        0        0 2024-05-22 11:25:38.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/__init__.py
--rw-rw-rw-   0        0        0      249 2024-05-22 09:20:12.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/base_dictionary.py
--rw-rw-rw-   0        0        0    71670 2024-06-03 07:33:05.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/blacklist.py
--rw-rw-rw-   0        0        0    54782 2024-05-22 17:52:41.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/constants.py
--rw-rw-rw-   0        0        0     2426 2024-05-22 09:21:15.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/cwe.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.200764 pulse_linter-0.0.5/pulse_linter/Blacklist/imports/
--rw-rw-rw-   0        0        0        0 2024-05-22 11:26:16.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/imports/__init__.py
--rw-rw-rw-   0        0        0      249 2024-05-22 09:20:12.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/imports/base_dictionary.py
--rw-rw-rw-   0        0        0    12758 2024-06-03 07:33:05.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/imports/blacklist.py
--rw-rw-rw-   0        0        0     1692 2024-05-22 11:34:21.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/imports/cwe.py
--rw-rw-rw-   0        0        0     1153 2024-05-28 16:27:06.000000 pulse_linter-0.0.5/pulse_linter/Blacklist/link_generator.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.201790 pulse_linter-0.0.5/pulse_linter/Extensions/
--rw-rw-rw-   0        0        0        0 2024-05-22 09:08:26.000000 pulse_linter-0.0.5/pulse_linter/Extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.206066 pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/
--rw-rw-rw-   0        0        0        0 2024-05-22 09:43:45.000000 pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/__init__.py
--rw-rw-rw-   0        0        0     2418 2024-06-03 07:33:05.000000 pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/attributes.py
--rw-rw-rw-   0        0        0     1519 2024-06-03 07:33:05.000000 pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/constants.py
--rw-rw-rw-   0        0        0     2177 2024-06-03 07:33:05.000000 pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/p1.py
--rw-rw-rw-   0        0        0      150 2024-05-27 08:52:13.000000 pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/p2.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.208109 pulse_linter-0.0.5/pulse_linter/Extensions/flake8_function_snake_case_checker/
--rw-rw-rw-   0        0        0        0 2024-05-22 06:58:12.000000 pulse_linter-0.0.5/pulse_linter/Extensions/flake8_function_snake_case_checker/__init__.py
--rw-rw-rw-   0        0        0      641 2024-05-22 07:34:36.000000 pulse_linter-0.0.5/pulse_linter/Extensions/flake8_function_snake_case_checker/checker.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.211112 pulse_linter-0.0.5/pulse_linter/Extensions/package_scanner/
--rw-rw-rw-   0        0        0        0 2024-05-22 11:39:23.000000 pulse_linter-0.0.5/pulse_linter/Extensions/package_scanner/__init__.py
--rw-rw-rw-   0        0        0     1234 2024-06-03 07:33:05.000000 pulse_linter-0.0.5/pulse_linter/Extensions/package_scanner/bad_import.py
--rw-rw-rw-   0        0        0     1197 2024-06-03 07:33:05.000000 pulse_linter-0.0.5/pulse_linter/Extensions/package_scanner/bad_importfrom.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.213109 pulse_linter-0.0.5/pulse_linter/Extensions/use_of_eval/
--rw-rw-rw-   0        0        0        0 2024-05-22 08:38:41.000000 pulse_linter-0.0.5/pulse_linter/Extensions/use_of_eval/__init__.py
--rw-rw-rw-   0        0        0      711 2024-05-27 05:28:24.000000 pulse_linter-0.0.5/pulse_linter/Extensions/use_of_eval/checker.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.214620 pulse_linter-0.0.5/pulse_linter/Report/
--rw-rw-rw-   0        0        0        0 2024-05-28 16:27:06.000000 pulse_linter-0.0.5/pulse_linter/Report/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-28 16:27:06.000000 pulse_linter-0.0.5/pulse_linter/Report/report_format.py
--rw-rw-rw-   0        0        0       43 2024-06-03 08:00:39.000000 pulse_linter-0.0.5/pulse_linter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.216854 pulse_linter-0.0.5/pulse_linter/add_ons/
--rw-rw-rw-   0        0        0        0 2024-05-29 14:43:39.000000 pulse_linter-0.0.5/pulse_linter/add_ons/__init__.py
--rw-rw-rw-   0        0        0     1335 2024-05-31 05:20:41.000000 pulse_linter-0.0.5/pulse_linter/add_ons/eval.py
--rw-rw-rw-   0        0        0      786 2024-05-30 05:29:36.000000 pulse_linter-0.0.5/pulse_linter/add_ons/exec.py
--rw-rw-rw-   0        0        0       88 2024-05-29 09:51:50.000000 pulse_linter-0.0.5/pulse_linter/dumper.py
--rw-rw-rw-   0        0        0      817 2024-06-03 07:57:20.000000 pulse_linter-0.0.5/pulse_linter/pulse_linter.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.219193 pulse_linter-0.0.5/pulse_linter/severity/
--rw-rw-rw-   0        0        0        0 2024-05-30 06:27:29.000000 pulse_linter-0.0.5/pulse_linter/severity/__init__.py
--rw-rw-rw-   0        0        0      190 2024-05-30 06:36:28.000000 pulse_linter-0.0.5/pulse_linter/severity/calculator.py
--rw-rw-rw-   0        0        0     5752 2024-05-30 11:06:05.000000 pulse_linter-0.0.5/pulse_linter/severity/code_duplications_finder.py
--rw-rw-rw-   0        0        0       57 2024-05-31 06:19:53.000000 pulse_linter-0.0.5/pulse_linter/test.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:41.220199 pulse_linter-0.0.5/pulse_linter.egg-info/
--rw-rw-rw-   0        0        0     1689 2024-06-03 09:07:40.000000 pulse_linter-0.0.5/pulse_linter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1761 2024-06-03 09:07:40.000000 pulse_linter-0.0.5/pulse_linter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 09:07:40.000000 pulse_linter-0.0.5/pulse_linter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      399 2024-06-03 09:07:40.000000 pulse_linter-0.0.5/pulse_linter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-06-03 09:07:40.000000 pulse_linter-0.0.5/pulse_linter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-03 09:07:40.000000 pulse_linter-0.0.5/pulse_linter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 09:07:41.223469 pulse_linter-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1519 2024-06-03 09:07:36.000000 pulse_linter-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.380195 pulse_linter-0.0.6/
+-rw-rw-rw-   0        0        0     1734 2024-06-03 10:58:09.379181 pulse_linter-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.330340 pulse_linter-0.0.6/pulse_linter/
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.339022 pulse_linter-0.0.6/pulse_linter/Blacklist/
+-rw-rw-rw-   0        0        0        0 2024-05-22 09:13:00.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.344045 pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/
+-rw-rw-rw-   0        0        0        0 2024-05-22 11:25:38.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/__init__.py
+-rw-rw-rw-   0        0        0      249 2024-05-22 09:20:12.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/base_dictionary.py
+-rw-rw-rw-   0        0        0    71670 2024-06-03 07:33:05.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/blacklist.py
+-rw-rw-rw-   0        0        0    54782 2024-05-22 17:52:41.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/constants.py
+-rw-rw-rw-   0        0        0     2426 2024-05-22 09:21:15.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/cwe.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.348569 pulse_linter-0.0.6/pulse_linter/Blacklist/imports/
+-rw-rw-rw-   0        0        0        0 2024-05-22 11:26:16.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/imports/__init__.py
+-rw-rw-rw-   0        0        0      249 2024-05-22 09:20:12.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/imports/base_dictionary.py
+-rw-rw-rw-   0        0        0    12758 2024-06-03 07:33:05.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/imports/blacklist.py
+-rw-rw-rw-   0        0        0     1692 2024-05-22 11:34:21.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/imports/cwe.py
+-rw-rw-rw-   0        0        0     1153 2024-05-28 16:27:06.000000 pulse_linter-0.0.6/pulse_linter/Blacklist/link_generator.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.349567 pulse_linter-0.0.6/pulse_linter/Extensions/
+-rw-rw-rw-   0        0        0        0 2024-05-22 09:08:26.000000 pulse_linter-0.0.6/pulse_linter/Extensions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.355607 pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/
+-rw-rw-rw-   0        0        0        0 2024-05-22 09:43:45.000000 pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/__init__.py
+-rw-rw-rw-   0        0        0     2418 2024-06-03 07:33:05.000000 pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/attributes.py
+-rw-rw-rw-   0        0        0     1519 2024-06-03 07:33:05.000000 pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/constants.py
+-rw-rw-rw-   0        0        0     2177 2024-06-03 07:33:05.000000 pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/p1.py
+-rw-rw-rw-   0        0        0      150 2024-05-27 08:52:13.000000 pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/p2.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.357604 pulse_linter-0.0.6/pulse_linter/Extensions/flake8_function_snake_case_checker/
+-rw-rw-rw-   0        0        0        0 2024-05-22 06:58:12.000000 pulse_linter-0.0.6/pulse_linter/Extensions/flake8_function_snake_case_checker/__init__.py
+-rw-rw-rw-   0        0        0      641 2024-05-22 07:34:36.000000 pulse_linter-0.0.6/pulse_linter/Extensions/flake8_function_snake_case_checker/checker.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.363155 pulse_linter-0.0.6/pulse_linter/Extensions/package_scanner/
+-rw-rw-rw-   0        0        0        0 2024-05-22 11:39:23.000000 pulse_linter-0.0.6/pulse_linter/Extensions/package_scanner/__init__.py
+-rw-rw-rw-   0        0        0     1234 2024-06-03 07:33:05.000000 pulse_linter-0.0.6/pulse_linter/Extensions/package_scanner/bad_import.py
+-rw-rw-rw-   0        0        0     1197 2024-06-03 07:33:05.000000 pulse_linter-0.0.6/pulse_linter/Extensions/package_scanner/bad_importfrom.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.365171 pulse_linter-0.0.6/pulse_linter/Extensions/use_of_eval/
+-rw-rw-rw-   0        0        0        0 2024-05-22 08:38:41.000000 pulse_linter-0.0.6/pulse_linter/Extensions/use_of_eval/__init__.py
+-rw-rw-rw-   0        0        0      711 2024-05-27 05:28:24.000000 pulse_linter-0.0.6/pulse_linter/Extensions/use_of_eval/checker.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.367334 pulse_linter-0.0.6/pulse_linter/Report/
+-rw-rw-rw-   0        0        0        0 2024-05-28 16:27:06.000000 pulse_linter-0.0.6/pulse_linter/Report/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 16:27:06.000000 pulse_linter-0.0.6/pulse_linter/Report/report_format.py
+-rw-rw-rw-   0        0        0       43 2024-06-03 08:00:39.000000 pulse_linter-0.0.6/pulse_linter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.371375 pulse_linter-0.0.6/pulse_linter/add_ons/
+-rw-rw-rw-   0        0        0        0 2024-05-29 14:43:39.000000 pulse_linter-0.0.6/pulse_linter/add_ons/__init__.py
+-rw-rw-rw-   0        0        0     1335 2024-05-31 05:20:41.000000 pulse_linter-0.0.6/pulse_linter/add_ons/eval.py
+-rw-rw-rw-   0        0        0      786 2024-05-30 05:29:36.000000 pulse_linter-0.0.6/pulse_linter/add_ons/exec.py
+-rw-rw-rw-   0        0        0       88 2024-05-29 09:51:50.000000 pulse_linter-0.0.6/pulse_linter/dumper.py
+-rw-rw-rw-   0        0        0     1568 2024-06-03 10:45:24.000000 pulse_linter-0.0.6/pulse_linter/pulse_linter.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.374773 pulse_linter-0.0.6/pulse_linter/severity/
+-rw-rw-rw-   0        0        0        0 2024-05-30 06:27:29.000000 pulse_linter-0.0.6/pulse_linter/severity/__init__.py
+-rw-rw-rw-   0        0        0      190 2024-05-30 06:36:28.000000 pulse_linter-0.0.6/pulse_linter/severity/calculator.py
+-rw-rw-rw-   0        0        0     5752 2024-05-30 11:06:05.000000 pulse_linter-0.0.6/pulse_linter/severity/code_duplications_finder.py
+-rw-rw-rw-   0        0        0       57 2024-05-31 06:19:53.000000 pulse_linter-0.0.6/pulse_linter/test.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:58:09.376771 pulse_linter-0.0.6/pulse_linter.egg-info/
+-rw-rw-rw-   0        0        0     1734 2024-06-03 10:58:09.000000 pulse_linter-0.0.6/pulse_linter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1761 2024-06-03 10:58:09.000000 pulse_linter-0.0.6/pulse_linter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:58:09.000000 pulse_linter-0.0.6/pulse_linter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      399 2024-06-03 10:58:09.000000 pulse_linter-0.0.6/pulse_linter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-06-03 10:58:09.000000 pulse_linter-0.0.6/pulse_linter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 10:58:09.000000 pulse_linter-0.0.6/pulse_linter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:58:09.381191 pulse_linter-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2024-06-03 10:57:54.000000 pulse_linter-0.0.6/setup.py
```

### Comparing `pulse_linter-0.0.5/PKG-INFO` & `pulse_linter-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pulse_linter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Security Weakness Finder
 Author: sooraj
 Author-email: sooraj.cs22@duk.ac.in
-License: Nil
+License: MIT
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 Requires-Dist: flake8
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=5.0; extra == "dev"
 
@@ -28,14 +28,20 @@
 
 You can install Pulse Linter via pip:
 
 ```bash 
 pip install pulse_linter
 ```
 
+## Help
+
+```bash 
+pulse_linter -h
+```
+
 ## Example
 
 ```bash
 # example.py
 def execute_command(command):
     exec(command)
```

### Comparing `pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/blacklist.py` & `pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/blacklist.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/constants.py` & `pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/constants.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Blacklist/build_1/cwe.py` & `pulse_linter-0.0.6/pulse_linter/Blacklist/build_1/cwe.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Blacklist/imports/blacklist.py` & `pulse_linter-0.0.6/pulse_linter/Blacklist/imports/blacklist.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Blacklist/imports/cwe.py` & `pulse_linter-0.0.6/pulse_linter/Blacklist/imports/cwe.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Blacklist/link_generator.py` & `pulse_linter-0.0.6/pulse_linter/Blacklist/link_generator.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/attributes.py` & `pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/attributes.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/constants.py` & `pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/constants.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Extensions/common_patterns/p1.py` & `pulse_linter-0.0.6/pulse_linter/Extensions/common_patterns/p1.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Extensions/flake8_function_snake_case_checker/checker.py` & `pulse_linter-0.0.6/pulse_linter/Extensions/flake8_function_snake_case_checker/checker.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Extensions/package_scanner/bad_import.py` & `pulse_linter-0.0.6/pulse_linter/Extensions/package_scanner/bad_import.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Extensions/package_scanner/bad_importfrom.py` & `pulse_linter-0.0.6/pulse_linter/Extensions/package_scanner/bad_importfrom.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/Extensions/use_of_eval/checker.py` & `pulse_linter-0.0.6/pulse_linter/Extensions/use_of_eval/checker.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/add_ons/eval.py` & `pulse_linter-0.0.6/pulse_linter/add_ons/eval.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/add_ons/exec.py` & `pulse_linter-0.0.6/pulse_linter/add_ons/exec.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter/severity/code_duplications_finder.py` & `pulse_linter-0.0.6/pulse_linter/severity/code_duplications_finder.py`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/pulse_linter.egg-info/PKG-INFO` & `pulse_linter-0.0.6/pulse_linter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pulse_linter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Security Weakness Finder
 Author: sooraj
 Author-email: sooraj.cs22@duk.ac.in
-License: Nil
+License: MIT
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 Requires-Dist: flake8
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=5.0; extra == "dev"
 
@@ -28,14 +28,20 @@
 
 You can install Pulse Linter via pip:
 
 ```bash 
 pip install pulse_linter
 ```
 
+## Help
+
+```bash 
+pulse_linter -h
+```
+
 ## Example
 
 ```bash
 # example.py
 def execute_command(command):
     exec(command)
```

### Comparing `pulse_linter-0.0.5/pulse_linter.egg-info/SOURCES.txt` & `pulse_linter-0.0.6/pulse_linter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulse_linter-0.0.5/setup.py` & `pulse_linter-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('Readme.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='pulse_linter',
-    version='0.0.5',
+    version='0.0.6',
     description='Security Weakness Finder',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='sooraj',
     author_email='sooraj.cs22@duk.ac.in',
-    license='Nil',
+    license='MIT',
     packages=find_packages(),
     install_requires=[
         'flake8',
     ],
     extras_require={
         'dev': [
             'pytest>=7.0',
```

