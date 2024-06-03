# Comparing `tmp/funky_modifiers-0.3.6.tar.gz` & `tmp/funky_modifiers-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.3.6.tar", last modified: Sun Jun  2 19:34:10 2024, max compression
+gzip compressed data, was "funky_modifiers-0.3.7.tar", last modified: Mon Jun  3 08:58:42 2024, max compression
```

## Comparing `funky_modifiers-0.3.6.tar` & `funky_modifiers-0.3.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.974610 funky_modifiers-0.3.6/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.6/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0      483 2024-06-02 19:34:10.973619 funky_modifiers-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.6/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 19:34:10.974610 funky_modifiers-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-06-02 19:19:45.000000 funky_modifiers-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.929971 funky_modifiers-0.3.6/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.942372 funky_modifiers-0.3.6/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.6/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.946341 funky_modifiers-0.3.6/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.6/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-06-01 12:40:27.000000 funky_modifiers-0.3.6/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.6/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.951298 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0    27243 2024-06-02 19:08:53.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/cache_modifiers.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     1566 2024-06-02 18:51:49.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/method_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.6/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.6/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.954800 funky_modifiers-0.3.6/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.6/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.6/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    58908 2024-05-28 21:40:01.000000 funky_modifiers-0.3.6/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.6/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.959235 funky_modifiers-0.3.6/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.973122 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      483 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1423 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.972131 funky_modifiers-0.3.6/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.6/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.6/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.6/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.6/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.6/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    17001 2024-05-26 21:41:35.000000 funky_modifiers-0.3.6/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.6/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.6/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.6/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.6/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.6/test/test_pick.py
--rw-rw-rw-   0        0        0    23919 2024-06-02 19:16:52.000000 funky_modifiers-0.3.6/test/test_special_modifiers.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.490034 funky_modifiers-0.3.7/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-06-03 08:58:42.489538 funky_modifiers-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.7/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:58:42.490034 funky_modifiers-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-06-03 08:58:21.000000 funky_modifiers-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.457793 funky_modifiers-0.3.7/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.462258 funky_modifiers-0.3.7/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.7/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.465749 funky_modifiers-0.3.7/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.7/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-06-01 12:40:27.000000 funky_modifiers-0.3.7/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.7/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.469698 funky_modifiers-0.3.7/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.7/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0    27247 2024-06-03 08:54:30.000000 funky_modifiers-0.3.7/src/funk_py/modularity/decoration/cache_modifiers.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.7/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.7/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     1566 2024-06-02 18:51:49.000000 funky_modifiers-0.3.7/src/funk_py/modularity/decoration/method_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.7/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.7/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.7/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.472673 funky_modifiers-0.3.7/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.7/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.7/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    58908 2024-05-28 21:40:01.000000 funky_modifiers-0.3.7/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.7/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.475675 funky_modifiers-0.3.7/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.7/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.7/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.7/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.7/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.489042 funky_modifiers-0.3.7/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-06-03 08:58:42.000000 funky_modifiers-0.3.7/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2024-06-03 08:58:42.000000 funky_modifiers-0.3.7/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:58:42.000000 funky_modifiers-0.3.7/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 08:58:42.000000 funky_modifiers-0.3.7/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-03 08:58:42.000000 funky_modifiers-0.3.7/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 08:58:42.488050 funky_modifiers-0.3.7/test/
+-rw-rw-rw-   0        0        0    24631 2024-06-03 08:58:21.000000 funky_modifiers-0.3.7/test/test_cache_modifiers.py
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.7/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.7/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.7/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.7/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.7/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    17001 2024-05-26 21:41:35.000000 funky_modifiers-0.3.7/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.7/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.7/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.7/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.7/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.7/test/test_pick.py
```

### Comparing `funky_modifiers-0.3.6/LICENSE` & `funky_modifiers-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/setup.py` & `funky_modifiers-0.3.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.3.6',
+    version='0.3.7',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/cache_modifiers.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/decoration/cache_modifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
         ans = ';date;' + value.strftime('%Y-%m-%d')
         main_logger.debug(f'Result is {ans}')
         return ans
 
     @staticmethod
     def _time_str(value: time) -> str:
         main_logger.debug('Making a date into a string...')
-        ans = ';time;' + value.strftime('%H-%M-%S')
+        ans = ';time;' + value.strftime('%H-%M-%S--%Z')
         main_logger.debug(f'Result is {ans}')
         return ans
 
     @staticmethod
     def _list_to_str(value: list) -> str:
         main_logger.debug('Converting a list to a string...')
         builder = []
```

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/method_modifiers.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/decoration/method_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/logging.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.3.7/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/sorting/converters.py` & `funky_modifiers-0.3.7/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.3.7/src/funk_py/sorting/dict_manip.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.3.7/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.3.7/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.3.7/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.3.7/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.3.7/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.3.7/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 src/funk_py/super_dicts/list_dict.py
 src/funk_py/super_dicts/windowed_list.py
 src/funky_modifiers.egg-info/PKG-INFO
 src/funky_modifiers.egg-info/SOURCES.txt
 src/funky_modifiers.egg-info/dependency_links.txt
 src/funky_modifiers.egg-info/requires.txt
 src/funky_modifiers.egg-info/top_level.txt
+test/test_cache_modifiers.py
 test/test_check_dict_equality.py
 test/test_check_list_equality.py
 test/test_convert_tuplish_dict.py
 test/test_converters.py
 test/test_converts_enums.py
 test/test_dict_builder.py
 test/test_drop_none_dict.py
 test/test_function_hash_and_equality.py
 test/test_logs_vars.py
 test/test_obj.py
-test/test_pick.py
-test/test_special_modifiers.py
+test/test_pick.py
```

### Comparing `funky_modifiers-0.3.6/test/test_check_dict_equality.py` & `funky_modifiers-0.3.7/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_check_list_equality.py` & `funky_modifiers-0.3.7/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.3.7/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_converters.py` & `funky_modifiers-0.3.7/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_converts_enums.py` & `funky_modifiers-0.3.7/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_dict_builder.py` & `funky_modifiers-0.3.7/test/test_dict_builder.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_drop_none_dict.py` & `funky_modifiers-0.3.7/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_function_hash_and_equality.py` & `funky_modifiers-0.3.7/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_logs_vars.py` & `funky_modifiers-0.3.7/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_obj.py` & `funky_modifiers-0.3.7/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_pick.py` & `funky_modifiers-0.3.7/test/test_pick.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.6/test/test_special_modifiers.py` & `funky_modifiers-0.3.7/test/test_cache_modifiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
-import pickle
 from collections import namedtuple
-from typing import Tuple, Any, Union, List
-from pathlib import Path
+from datetime import datetime, time, date, timedelta, timezone
 
 import pytest
 
 from t_support import cov, cov_counter
 # Importing an internal class here in order to test it.
 from funk_py.modularity.decoration.cache_modifiers import (_DiskCacheNameConverters, disk_cache,
                                                            DISK_CACHE_INDEX_NAME, DiskCacheMethod)
@@ -39,32 +37,42 @@
             yield ABC[i]
 
 
 @pytest.fixture(params=(
     TDef('lorem', ';str;lorem'),
     TDef(543, ';int;543'),
     TDef(97.5, ';float;97.5'),
-), ids=('str', 'int', 'float'))
+    TDef(datetime(2024, 9, 18, 14, 22, 33), ';datetime;2024-09-18--14-22-33--'),
+    TDef(date(2024, 9, 18), ';date;2024-09-18'),
+    TDef(time(14, 22, 33), ';time;14-22-33--'),
+), ids=('str', 'int', 'float', 'datetime', 'date', 'time'))
 def simple_vals(request):
     return request.param
 
 
 @pytest.fixture(params=(
     TDef('ipsum', ';str;ipsum'),
     TDef(987, ';int;987'),
     TDef(16.666, ';float;16.666'),
-), ids=('str', 'int', 'float'))
+    TDef(datetime(2025, 4, 13, 19, 12, 0, tzinfo=timezone(-timedelta(hours=6))),
+         ';datetime;2025-04-13--19-12-00--UTC-06:00'),
+    TDef(date(2025, 4, 13), ';date;2025-04-13'),
+    TDef(time(19, 12, 0, tzinfo=timezone(-timedelta(hours=6))), ';time;19-12-00--UTC-06:00'),
+), ids=('str', 'int', 'float', 'datetime', 'date', 'time'))
 def more_simple_vals(request):
     return request.param
 
 @pytest.fixture(params=(
     TDef('dolor', ';str;dolor'),
     TDef(5, ';int;5'),
     TDef(9.0, ';float;9.0'),
-), ids=('str', 'int', 'float'))
+    TDef(datetime(2023, 1, 1, 1, 0, 0, 19), ';datetime;2023-01-01--01-00-00--'),
+    TDef(date(2023, 1, 1), ';date;2023-01-01'),
+    TDef(time(1, 0, 0, 19), ';time;01-00-00--'),
+), ids=('str', 'int', 'float', 'datetime', 'date', 'time'))
 def even_more_simple_vals(request):
     return request.param
 
 @pytest.fixture(params=(
     TDef('sit', ';str;sit'),
     TDef(19, ';int;19'),
     TDef(float('inf'), ';float;inf'),
@@ -125,16 +133,15 @@
     out = (f';dict;{simple_vals.output}:{more_simple_vals.output},'
            f'{even_more_simple_vals.output}:{still_even_more_simple_vals.output};end-dict;')
     return TDef(_in, out)
 
 
 @pytest.fixture
 def unknown_val():
-    return TDef(Horse('Bob', 19),
-                ';<class \'test_special_modifiers.Horse\'>;Horse(name=Bob, age=19)')
+    return TDef(Horse('Bob', 19), ';<class \'test_cache_modifiers.Horse\'>;Horse(name=Bob, age=19)')
 
 
 def test_simple_vals_name(simple_vals):
     assert _DiskCacheNameConverters.to_str(simple_vals.input) == simple_vals.output
 
 
 def test_simple_subclass_vals_name(simple_subclass_vals):
@@ -580,15 +587,15 @@
         assert ans == horse02.output[1]
         index = t_func._DiskCache__index
         assert len(index) == MAX_SIZE, BAD_NUMBER
         for name in index:
             if name == horse01.output[0]:
                 assert index[name][1] == 3, BAD_USES
 
-            elif name == horse02.output[0]:
+            elif name in (horse02.output[0], horse11.output[0]):
                 assert index[name][1] == 1, BAD_USES
 
             else:
                 assert index[name][1] == 2, BAD_USES
 
             assert os.path.exists(os.path.join(TARGET_DIR, index[name][0])), EXPECTED_PATH
 
@@ -629,15 +636,15 @@
 
                 else:
                     assert index[name][1] == 1, BAD_USES
 
                 assert os.path.exists(os.path.join(TARGET_DIR, index[name][0])), EXPECTED_PATH
 
         def test_not_replace_higher(self, setup, t_func, horse01, horse02, horse11):
-            TestLruDiskCache.overwrite_tst(t_func, horse01, horse02, horse11)
+            TestWuncDiskCache.overwrite_tst(t_func, horse01, horse02, horse11)
 
     class TestMultipleInstances:
         # Scope of the below is not set The goal of this is to ensure a new object is instantiated
         # for every test. This ensures that files are actually saved correctly.
         @pytest.fixture
         def t_func(self):
             @disk_cache(TARGET_DIR, MAX_SIZE, cache_method=DiskCacheMethod.WUNC)
@@ -669,8 +676,8 @@
 
                 else:
                     assert index[name][1] == 1, BAD_USES
 
                 assert os.path.exists(os.path.join(TARGET_DIR, index[name][0])), EXPECTED_PATH
 
         def test_not_replace_higher(self, setup, t_func, horse01, horse02, horse11):
-            TestLruDiskCache.overwrite_tst(t_func, horse01, horse02, horse11)
+            TestWuncDiskCache.overwrite_tst(t_func, horse01, horse02, horse11)
```

