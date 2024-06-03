# Comparing `tmp/pynocaptcha-1.9.0.tar.gz` & `tmp/pynocaptcha-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynocaptcha-1.9.0.tar", last modified: Mon Apr 22 12:56:55 2024, max compression
+gzip compressed data, was "pynocaptcha-1.9.1.tar", last modified: Mon Jun  3 08:52:08 2024, max compression
```

## Comparing `pynocaptcha-1.9.0.tar` & `pynocaptcha-1.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-22 12:56:55.298423 pynocaptcha-1.9.0/
--rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.9.0/LICENSE
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-22 12:56:55.298238 pynocaptcha-1.9.0/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.9.0/README.md
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-22 12:56:55.295878 pynocaptcha-1.9.0/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)     1265 2024-04-22 12:56:31.000000 pynocaptcha-1.9.0/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-22 12:56:55.297703 pynocaptcha-1.9.0/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)      668 2024-04-04 15:59:57.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/aws.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5116 2024-04-08 01:16:56.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)      904 2024-04-22 12:56:10.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/datadome.py
--rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/discord.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1540 2024-04-19 13:27:00.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/kasada.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-04-19 13:25:15.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/perimeterx.py
--rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.9.0/pynocaptcha/crackers/tls.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-22 12:56:55.296406 pynocaptcha-1.9.0/pynocaptcha.egg-info/
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-22 12:56:55.000000 pynocaptcha-1.9.0/pynocaptcha.egg-info/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)      641 2024-04-22 12:56:55.000000 pynocaptcha-1.9.0/pynocaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-22 12:56:55.000000 pynocaptcha-1.9.0/pynocaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-22 12:56:55.000000 pynocaptcha-1.9.0/pynocaptcha.egg-info/not-zip-safe
--rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-04-22 12:56:55.000000 pynocaptcha-1.9.0/pynocaptcha.egg-info/requires.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-04-22 12:56:55.000000 pynocaptcha-1.9.0/pynocaptcha.egg-info/top_level.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-04-22 12:56:55.298461 pynocaptcha-1.9.0/setup.cfg
--rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-04-22 12:56:48.000000 pynocaptcha-1.9.0/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-06-03 08:52:08.698698 pynocaptcha-1.9.1/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.9.1/LICENSE
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-06-03 08:52:08.698518 pynocaptcha-1.9.1/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.9.1/README.md
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-06-03 08:52:08.695190 pynocaptcha-1.9.1/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1265 2024-04-22 12:56:31.000000 pynocaptcha-1.9.1/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-06-03 08:52:08.698315 pynocaptcha-1.9.1/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      668 2024-04-04 15:59:57.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/aws.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5116 2024-04-26 14:26:39.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      904 2024-04-22 12:56:10.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/datadome.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/discord.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1589 2024-06-03 08:51:46.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/kasada.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-04-19 13:25:15.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/perimeterx.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.9.1/pynocaptcha/crackers/tls.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-06-03 08:52:08.695828 pynocaptcha-1.9.1/pynocaptcha.egg-info/
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-06-03 08:52:08.000000 pynocaptcha-1.9.1/pynocaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)      641 2024-06-03 08:52:08.000000 pynocaptcha-1.9.1/pynocaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-06-03 08:52:08.000000 pynocaptcha-1.9.1/pynocaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-06-03 08:52:08.000000 pynocaptcha-1.9.1/pynocaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-06-03 08:52:08.000000 pynocaptcha-1.9.1/pynocaptcha.egg-info/requires.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-06-03 08:52:08.000000 pynocaptcha-1.9.1/pynocaptcha.egg-info/top_level.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-06-03 08:52:08.698737 pynocaptcha-1.9.1/setup.cfg
+-rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-06-03 08:51:59.000000 pynocaptcha-1.9.1/setup.py
```

### Comparing `pynocaptcha-1.9.0/LICENSE` & `pynocaptcha-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/PKG-INFO` & `pynocaptcha-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynocaptcha
-Version: 1.9.0
+Version: 1.9.1
 Summary: nocaptcha.io api
 License: MIT
 Keywords: nocaptcha
 Platform: all
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pynocaptcha-1.9.0/pynocaptcha/__init__.py` & `pynocaptcha-1.9.1/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/aws.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/aws.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/base.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/datadome.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/datadome.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/discord.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/discord.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/kasada.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/kasada.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,18 +21,20 @@
         proxy="user:pass@ip:port",
         debug=True,
     )
     ret = cracker.crack()
     """
 
     # 必传参数
-    must_check_params = ["href", "script_url", "proxy"]
+    must_check_params = ["href", "ips_url", "proxy"]
     # 默认可选参数
     option_params = {
         "branch": "Master",
+        "ips_script": None,
+        "submit": True,
         "user_agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
         "timeout": 30
     }
 
 
 class KasadaCdCracker(BaseCracker):
     cracker_name = "kasada"
```

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/perimeterx.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/perimeterx.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha/crackers/tls.py` & `pynocaptcha-1.9.1/pynocaptcha/crackers/tls.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/pynocaptcha.egg-info/PKG-INFO` & `pynocaptcha-1.9.1/pynocaptcha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynocaptcha
-Version: 1.9.0
+Version: 1.9.1
 Summary: nocaptcha.io api
 License: MIT
 Keywords: nocaptcha
 Platform: all
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pynocaptcha-1.9.0/pynocaptcha.egg-info/SOURCES.txt` & `pynocaptcha-1.9.1/pynocaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.9.0/setup.py` & `pynocaptcha-1.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 setup(
     name='pynocaptcha',
-    version='1.9.0',
+    version='1.9.1',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

