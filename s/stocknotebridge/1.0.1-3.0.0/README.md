# Comparing `tmp/stocknotebridge-1.0.1.tar.gz` & `tmp/stocknotebridge-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\stocknotebridge-1.0.1.tar", last modified: Mon Jul 20 03:58:20 2020, max compression
+gzip compressed data, was "stocknotebridge-3.0.0.tar", last modified: Mon Jun  3 11:49:07 2024, max compression
```

## Comparing `stocknotebridge-1.0.1.tar` & `stocknotebridge-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2020-07-20 03:58:20.123235 stocknotebridge-1.0.1/
--rw-rw-rw-   0        0        0     1082 2020-06-26 11:01:57.000000 stocknotebridge-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       25 2020-07-01 05:58:56.000000 stocknotebridge-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      822 2020-07-20 03:58:20.123235 stocknotebridge-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    43188 2020-07-02 05:33:04.000000 stocknotebridge-1.0.1/README.md
--rw-rw-rw-   0        0        0      118 2020-07-20 03:58:20.125290 stocknotebridge-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      909 2020-07-20 03:56:37.000000 stocknotebridge-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2020-07-20 03:58:20.064676 stocknotebridge-1.0.1/snapi_py_client/
--rw-rw-rw-   0        0        0        0 2020-06-11 11:15:32.000000 stocknotebridge-1.0.1/snapi_py_client/__init__.py
--rw-rw-rw-   0        0        0    26717 2020-06-16 08:50:03.000000 stocknotebridge-1.0.1/snapi_py_client/api_client.py
--rw-rw-rw-   0        0        0     9289 2020-07-20 03:40:53.000000 stocknotebridge-1.0.1/snapi_py_client/configuration.py
--rw-rw-rw-   0        0        0    14674 2020-06-11 11:15:32.000000 stocknotebridge-1.0.1/snapi_py_client/rest.py
--rw-rw-rw-   0        0        0   155280 2020-07-16 13:26:42.000000 stocknotebridge-1.0.1/snapi_py_client/snapi_bridge.py
-drwxrwxrwx   0        0        0        0 2020-07-20 03:58:20.115216 stocknotebridge-1.0.1/stocknotebridge.egg-info/
--rw-rw-rw-   0        0        0      822 2020-07-20 03:58:19.000000 stocknotebridge-1.0.1/stocknotebridge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2020-07-20 03:58:19.000000 stocknotebridge-1.0.1/stocknotebridge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-20 03:58:19.000000 stocknotebridge-1.0.1/stocknotebridge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2020-07-20 03:58:19.000000 stocknotebridge-1.0.1/stocknotebridge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2020-07-20 03:58:19.000000 stocknotebridge-1.0.1/stocknotebridge.egg-info/top_level.txt
+drwxr-xr-x   0 mohammad.arsh   (502) wheel        (0)        0 2024-06-03 11:49:07.695222 stocknotebridge-3.0.0/
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)     1082 2024-05-27 13:30:50.000000 stocknotebridge-3.0.0/LICENSE
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)       25 2024-05-27 13:30:50.000000 stocknotebridge-3.0.0/MANIFEST.in
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)      814 2024-06-03 11:49:07.695289 stocknotebridge-3.0.0/PKG-INFO
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)    43188 2024-05-27 13:30:50.000000 stocknotebridge-3.0.0/README.md
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)      108 2024-06-03 11:49:07.695521 stocknotebridge-3.0.0/setup.cfg
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)      912 2024-06-03 11:17:56.000000 stocknotebridge-3.0.0/setup.py
+drwxr-xr-x   0 mohammad.arsh   (502) wheel        (0)        0 2024-06-03 11:49:07.693267 stocknotebridge-3.0.0/snapi_py_client/
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)        0 2024-05-27 13:30:50.000000 stocknotebridge-3.0.0/snapi_py_client/__init__.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)    26717 2024-05-27 13:30:50.000000 stocknotebridge-3.0.0/snapi_py_client/api_client.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)     9289 2024-06-03 11:18:22.000000 stocknotebridge-3.0.0/snapi_py_client/configuration.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)    14674 2024-05-27 13:30:50.000000 stocknotebridge-3.0.0/snapi_py_client/rest.py
+-rwxrwxrwx   0 mohammad.arsh   (502) wheel        (0)   237011 2024-05-29 12:27:12.000000 stocknotebridge-3.0.0/snapi_py_client/snapi_bridge.py
+drwxr-xr-x   0 mohammad.arsh   (502) wheel        (0)        0 2024-06-03 11:49:07.695117 stocknotebridge-3.0.0/stocknotebridge.egg-info/
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)      814 2024-06-03 11:49:07.000000 stocknotebridge-3.0.0/stocknotebridge.egg-info/PKG-INFO
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)      389 2024-06-03 11:49:07.000000 stocknotebridge-3.0.0/stocknotebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)        1 2024-06-03 11:49:07.000000 stocknotebridge-3.0.0/stocknotebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)       44 2024-06-03 11:49:07.000000 stocknotebridge-3.0.0/stocknotebridge.egg-info/requires.txt
+-rw-r--r--   0 mohammad.arsh   (502) wheel        (0)       16 2024-06-03 11:49:07.000000 stocknotebridge-3.0.0/stocknotebridge.egg-info/top_level.txt
```

### Comparing `stocknotebridge-1.0.1/LICENSE` & `stocknotebridge-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stocknotebridge-1.0.1/README.md` & `stocknotebridge-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `stocknotebridge-1.0.1/setup.py` & `stocknotebridge-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(name='stocknotebridge',
-version='1.0.1',
+version='3.0.0',
 description='official python library for Stocknote APIs',
 url='https://github.com/samco-sdk/Python-SDK',
-install_requires=['future', 'requests','websocket','websocket-client'],
+install_requires=['future', 'requests','websocket-client','six','pandas'],
 author='Samco Securities Limited',
 author_email='apisupport@samco.in',
 license='MIT License',
 packages=['snapi_py_client'],
 keywords = ['stocknote api', 'stocknote python sdk','samco api trading','samco algo trading', 'stock markets samco'],
 classifiers=[
     'Intended Audience :: Developers',
```

### Comparing `stocknotebridge-1.0.1/snapi_py_client/api_client.py` & `stocknotebridge-3.0.0/snapi_py_client/api_client.py`

 * *Files identical despite different names*

### Comparing `stocknotebridge-1.0.1/snapi_py_client/configuration.py` & `stocknotebridge-3.0.0/snapi_py_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         """Constructor"""
         if self._default:
             for key in self._default.__dict__.keys():
                 self.__dict__[key] = copy.copy(self._default.__dict__[key])
             return
 
         # Default Base url
-        self.host = "https://api.stocknote.com"
+        self.host = "https://tradeapi.samco.in"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
```

### Comparing `stocknotebridge-1.0.1/snapi_py_client/rest.py` & `stocknotebridge-3.0.0/snapi_py_client/rest.py`

 * *Files identical despite different names*

