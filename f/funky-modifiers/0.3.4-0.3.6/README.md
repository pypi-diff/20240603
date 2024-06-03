# Comparing `tmp/funky_modifiers-0.3.4.tar.gz` & `tmp/funky_modifiers-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.3.4.tar", last modified: Sun May 26 21:56:39 2024, max compression
+gzip compressed data, was "funky_modifiers-0.3.6.tar", last modified: Sun Jun  2 19:34:10 2024, max compression
```

## Comparing `funky_modifiers-0.3.4.tar` & `funky_modifiers-0.3.6.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.822154 funky_modifiers-0.3.4/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.4/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      483 2024-05-26 21:56:39.821657 funky_modifiers-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.4/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 21:56:39.822154 funky_modifiers-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-05-26 21:55:59.000000 funky_modifiers-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.792391 funky_modifiers-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.796856 funky_modifiers-0.3.4/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.4/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.800328 funky_modifiers-0.3.4/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.4/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.3.4/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.4/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.803304 funky_modifiers-0.3.4/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.4/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.4/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.4/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.4/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.4/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.4/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.805786 funky_modifiers-0.3.4/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.4/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.4/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    58346 2024-05-26 21:55:59.000000 funky_modifiers-0.3.4/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.4/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.808266 funky_modifiers-0.3.4/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.4/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.4/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.4/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.4/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.821162 funky_modifiers-0.3.4/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      483 2024-05-26 21:56:39.000000 funky_modifiers-0.3.4/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2024-05-26 21:56:39.000000 funky_modifiers-0.3.4/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 21:56:39.000000 funky_modifiers-0.3.4/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-26 21:56:39.000000 funky_modifiers-0.3.4/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 21:56:39.000000 funky_modifiers-0.3.4/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 21:56:39.820171 funky_modifiers-0.3.4/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.4/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.4/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.4/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.4/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.4/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    17001 2024-05-26 21:41:35.000000 funky_modifiers-0.3.4/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.4/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.4/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.4/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.4/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.4/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.974610 funky_modifiers-0.3.6/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-06-02 19:34:10.973619 funky_modifiers-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.6/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:34:10.974610 funky_modifiers-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-06-02 19:19:45.000000 funky_modifiers-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.929971 funky_modifiers-0.3.6/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.942372 funky_modifiers-0.3.6/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.6/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.946341 funky_modifiers-0.3.6/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.6/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-06-01 12:40:27.000000 funky_modifiers-0.3.6/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.6/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.951298 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0    27243 2024-06-02 19:08:53.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/cache_modifiers.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     1566 2024-06-02 18:51:49.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/method_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.6/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.6/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.6/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.954800 funky_modifiers-0.3.6/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.6/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.6/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    58908 2024-05-28 21:40:01.000000 funky_modifiers-0.3.6/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.6/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.959235 funky_modifiers-0.3.6/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.6/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.973122 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1423 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 19:34:10.000000 funky_modifiers-0.3.6/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 19:34:10.972131 funky_modifiers-0.3.6/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.6/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.6/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.6/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.6/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.6/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    17001 2024-05-26 21:41:35.000000 funky_modifiers-0.3.6/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.6/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.6/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.6/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.6/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.6/test/test_pick.py
+-rw-rw-rw-   0        0        0    23919 2024-06-02 19:16:52.000000 funky_modifiers-0.3.6/test/test_special_modifiers.py
```

### Comparing `funky_modifiers-0.3.4/LICENSE` & `funky_modifiers-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/setup.py` & `funky_modifiers-0.3.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.3.4',
+    version='0.3.6',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.3.4/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.3.6/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.3.6/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.3.6/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/modularity/logging.py` & `funky_modifiers-0.3.6/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.3.6/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/sorting/converters.py` & `funky_modifiers-0.3.6/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.3.6/src/funk_py/sorting/dict_manip.py`

 * *Files 2% similar despite different names*

```diff
@@ -535,14 +535,22 @@
 class DictBuilder:
     """
     A builder for dictionaries that has a few helpful methods for merging in data from other
     dictionaries.
     """
 
     class _Instruction:
+        # This class and _Cur implement the following patterns.
+        # Chain of Responsibility
+        # Command Pattern
+        # Builder Pattern
+        # Fluent Interface
+        # Interpreter Pattern (loosely)
+        # Proxy Pattern
+        # Decorator Pattern
         def __init__(inner_self, method: str, *args, **kwargs):
             # Construct the base of a chain.
             inner_self._chain = [{_METHOD: method, _ARGS: args, _KWARGS: kwargs}]
 
         def __call__(inner_self, *args, **kwargs) -> 'DictBuilder._Instruction':
             # Update the last instruction in chain with the received args and kwargs. The user
             # intends to call a function and did not just want a value.
@@ -589,14 +597,22 @@
                                    if v in (DictBuilder._Cur, DictBuilder._Instruction)
                                    else v
                                    for k, v in instruction[_KWARGS].items()})
 
             return attr
 
     class _Cur:
+        # This class and _Instruction implement the following patterns.
+        # Chain of Responsibility
+        # Command Pattern
+        # Builder Pattern
+        # Fluent Interface
+        # Interpreter Pattern (loosely)
+        # Proxy Pattern
+        # Decorator Pattern
         def __getitem__(self, key):
             return DictBuilder._Instruction('__getitem__', key)
 
         @staticmethod
         def get(key: Any, default: Any = None):
             return DictBuilder._Instruction('get', key, default)
```

### Comparing `funky_modifiers-0.3.4/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.3.6/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.3.6/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.3.6/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.3.6/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.3.6/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.3.6/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 src/funk_py/__init__.py
 src/funk_py/modularity/__init__.py
 src/funk_py/modularity/basic_structures.py
 src/funk_py/modularity/bespoke_properties.py
 src/funk_py/modularity/logging.py
 src/funk_py/modularity/type_matching.py
 src/funk_py/modularity/decoration/__init__.py
+src/funk_py/modularity/decoration/cache_modifiers.py
 src/funk_py/modularity/decoration/enum_modifiers.py
 src/funk_py/modularity/decoration/init_modifiers.py
+src/funk_py/modularity/decoration/method_modifiers.py
 src/funk_py/modularity/decoration/transforming_list.py
 src/funk_py/sorting/__init__.py
 src/funk_py/sorting/converters.py
 src/funk_py/sorting/dict_manip.py
 src/funk_py/sorting/pieces.py
 src/funk_py/super_dicts/__init__.py
 src/funk_py/super_dicts/drop_none_dict.py
@@ -32,8 +34,9 @@
 test/test_converters.py
 test/test_converts_enums.py
 test/test_dict_builder.py
 test/test_drop_none_dict.py
 test/test_function_hash_and_equality.py
 test/test_logs_vars.py
 test/test_obj.py
-test/test_pick.py
+test/test_pick.py
+test/test_special_modifiers.py
```

### Comparing `funky_modifiers-0.3.4/test/test_check_dict_equality.py` & `funky_modifiers-0.3.6/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_check_list_equality.py` & `funky_modifiers-0.3.6/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.3.6/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_converters.py` & `funky_modifiers-0.3.6/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_converts_enums.py` & `funky_modifiers-0.3.6/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_dict_builder.py` & `funky_modifiers-0.3.6/test/test_dict_builder.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_drop_none_dict.py` & `funky_modifiers-0.3.6/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_function_hash_and_equality.py` & `funky_modifiers-0.3.6/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_logs_vars.py` & `funky_modifiers-0.3.6/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_obj.py` & `funky_modifiers-0.3.6/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.4/test/test_pick.py` & `funky_modifiers-0.3.6/test/test_pick.py`

 * *Files identical despite different names*

