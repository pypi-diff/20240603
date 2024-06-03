# Comparing `tmp/quantumdiceware-0.1.9.tar.gz` & `tmp/quantumdiceware-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quantumdiceware-0.1.9.tar", last modified: Sat Jan  6 22:30:31 2018, max compression
+gzip compressed data, was "quantumdiceware-0.3.0.tar", last modified: Mon Apr 11 02:57:24 2022, max compression
```

## Comparing `quantumdiceware-0.1.9.tar` & `quantumdiceware-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2018-01-06 22:30:31.000000 quantumdiceware-0.1.9/
--rw-r--r--   0 justin     (501) staff       (20)     2262 2018-01-06 22:30:31.000000 quantumdiceware-0.1.9/PKG-INFO
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2018-01-06 22:30:31.000000 quantumdiceware-0.1.9/quantumdiceware/
--rw-r--r--   0 justin     (501) staff       (20)        0 2018-01-05 17:48:21.000000 quantumdiceware-0.1.9/quantumdiceware/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)       60 2018-01-05 18:13:47.000000 quantumdiceware-0.1.9/quantumdiceware/__main__.py
--rw-r--r--   0 justin     (501) staff       (20)    87392 2018-01-05 13:54:29.000000 quantumdiceware-0.1.9/quantumdiceware/diceware_word_list.txt
--rw-r--r--   0 justin     (501) staff       (20)     3235 2018-01-06 21:15:25.000000 quantumdiceware-0.1.9/quantumdiceware/quantumdiceware.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2018-01-06 22:30:31.000000 quantumdiceware-0.1.9/quantumdiceware.egg-info/
--rw-r--r--   0 justin     (501) staff       (20)        1 2018-01-06 22:30:27.000000 quantumdiceware-0.1.9/quantumdiceware.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (501) staff       (20)       62 2018-01-06 22:30:27.000000 quantumdiceware-0.1.9/quantumdiceware.egg-info/entry_points.txt
--rw-r--r--   0 justin     (501) staff       (20)     2262 2018-01-06 22:30:27.000000 quantumdiceware-0.1.9/quantumdiceware.egg-info/PKG-INFO
--rw-r--r--   0 justin     (501) staff       (20)       29 2018-01-06 22:30:27.000000 quantumdiceware-0.1.9/quantumdiceware.egg-info/requires.txt
--rw-r--r--   0 justin     (501) staff       (20)      385 2018-01-06 22:30:27.000000 quantumdiceware-0.1.9/quantumdiceware.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (501) staff       (20)       16 2018-01-06 22:30:27.000000 quantumdiceware-0.1.9/quantumdiceware.egg-info/top_level.txt
--rw-r--r--   0 justin     (501) staff       (20)     1407 2018-01-06 21:28:54.000000 quantumdiceware-0.1.9/README.rst
--rw-r--r--   0 justin     (501) staff       (20)       59 2018-01-06 22:30:31.000000 quantumdiceware-0.1.9/setup.cfg
--rw-r--r--   0 justin     (501) staff       (20)     1002 2018-01-06 19:44:04.000000 quantumdiceware-0.1.9/setup.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2022-04-11 02:57:24.806223 quantumdiceware-0.3.0/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2247 2022-04-11 02:57:24.806223 quantumdiceware-0.3.0/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1384 2022-04-11 02:15:00.000000 quantumdiceware-0.3.0/README.rst
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2022-04-11 02:57:24.806223 quantumdiceware-0.3.0/quantumdiceware/
+-rw-rw-r--   0 justin    (1000) justin    (1000)        0 2022-04-11 02:15:00.000000 quantumdiceware-0.3.0/quantumdiceware/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)       60 2022-04-11 02:15:00.000000 quantumdiceware-0.3.0/quantumdiceware/__main__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    87392 2022-04-11 02:15:00.000000 quantumdiceware-0.3.0/quantumdiceware/diceware_word_list.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4451 2022-04-11 02:57:19.000000 quantumdiceware-0.3.0/quantumdiceware/quantumdiceware.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2022-04-11 02:57:24.806223 quantumdiceware-0.3.0/quantumdiceware.egg-info/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2247 2022-04-11 02:57:24.000000 quantumdiceware-0.3.0/quantumdiceware.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)      385 2022-04-11 02:57:24.000000 quantumdiceware-0.3.0/quantumdiceware.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2022-04-11 02:57:24.000000 quantumdiceware-0.3.0/quantumdiceware.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       62 2022-04-11 02:57:24.000000 quantumdiceware-0.3.0/quantumdiceware.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       29 2022-04-11 02:57:24.000000 quantumdiceware-0.3.0/quantumdiceware.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       16 2022-04-11 02:57:24.000000 quantumdiceware-0.3.0/quantumdiceware.egg-info/top_level.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       38 2022-04-11 02:57:24.806223 quantumdiceware-0.3.0/setup.cfg
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1002 2022-04-11 02:15:00.000000 quantumdiceware-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `quantumdiceware-0.1.9/PKG-INFO` & `quantumdiceware-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 1.2
 Name: quantumdiceware
-Version: 0.1.9
+Version: 0.3.0
 Summary: Generates Diceware passphrases from quantum random data.
 Home-page: http://github.com/justinsloan/qdg
 Author: Justin M. Sloan
 Author-email: justin@justinsloan.com
 License: UNKNOWN
 Description: ===
         QDG
         ===
-        Diceware passphrases from quantum random data
+        Generate truly random diceware passphrases.
         
         |build-status| |docs|
         
         .. image:: password_strength.png
         
         
         Features
         --------
         - Simulates dice rolls by gathering quantum data.
         - Includes the complete standard Diceware wordlist.
         - Generate passphrases from custom wordlists.
         
-        Python 3.6 is required.
+        *Python 3.6 is required.*
         
         
         Usage
         -----
         
         Install
         
-            $ pip3 install quantumdiceware
+            $ pip install quantumdiceware
         
         Generate a Passphrase
         
             $ qdg
         
         Generate five Passphrases and save them to output.txt
         
@@ -56,15 +56,15 @@
         
         See `The Diceware Passphrase Home Page <http://world.std.com/~reinhold/diceware.html>`_ to learn more about Diceware.
         
         
         Meta
         ----
         
-        Justin M. Sloan - `justinsloan.com <https://justinsloan.com>`_ - pydev@justinsloan.com
+        Justin M. Sloan - `justinsloan.com <https://justinsloan.com>`_ 
         
         Public Domain. See ``LICENSE.txt`` for more information.
         
         https://github.com/justinsloan/qdg
         
         
         .. |build-status| image:: https://travis-ci.org/justinsloan/QDG.svg?branch=master
@@ -72,9 +72,10 @@
             :scale: 100%
             :target: https://travis-ci.org/justinsloan/QDG.svg?branch=master
         
         .. |docs| image:: https://readthedocs.org/projects/docs/badge/?version=latest
             :alt: Documentation Status
             :scale: 100%
             :target: https://qdg.readthedocs.io/en/latest/?badge=latest
+        
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `quantumdiceware-0.1.9/quantumdiceware/diceware_word_list.txt` & `quantumdiceware-0.3.0/quantumdiceware/diceware_word_list.txt`

 * *Files identical despite different names*

### Comparing `quantumdiceware-0.1.9/quantumdiceware.egg-info/PKG-INFO` & `quantumdiceware-0.3.0/quantumdiceware.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 1.2
 Name: quantumdiceware
-Version: 0.1.9
+Version: 0.3.0
 Summary: Generates Diceware passphrases from quantum random data.
 Home-page: http://github.com/justinsloan/qdg
 Author: Justin M. Sloan
 Author-email: justin@justinsloan.com
 License: UNKNOWN
 Description: ===
         QDG
         ===
-        Diceware passphrases from quantum random data
+        Generate truly random diceware passphrases.
         
         |build-status| |docs|
         
         .. image:: password_strength.png
         
         
         Features
         --------
         - Simulates dice rolls by gathering quantum data.
         - Includes the complete standard Diceware wordlist.
         - Generate passphrases from custom wordlists.
         
-        Python 3.6 is required.
+        *Python 3.6 is required.*
         
         
         Usage
         -----
         
         Install
         
-            $ pip3 install quantumdiceware
+            $ pip install quantumdiceware
         
         Generate a Passphrase
         
             $ qdg
         
         Generate five Passphrases and save them to output.txt
         
@@ -56,15 +56,15 @@
         
         See `The Diceware Passphrase Home Page <http://world.std.com/~reinhold/diceware.html>`_ to learn more about Diceware.
         
         
         Meta
         ----
         
-        Justin M. Sloan - `justinsloan.com <https://justinsloan.com>`_ - pydev@justinsloan.com
+        Justin M. Sloan - `justinsloan.com <https://justinsloan.com>`_ 
         
         Public Domain. See ``LICENSE.txt`` for more information.
         
         https://github.com/justinsloan/qdg
         
         
         .. |build-status| image:: https://travis-ci.org/justinsloan/QDG.svg?branch=master
@@ -72,9 +72,10 @@
             :scale: 100%
             :target: https://travis-ci.org/justinsloan/QDG.svg?branch=master
         
         .. |docs| image:: https://readthedocs.org/projects/docs/badge/?version=latest
             :alt: Documentation Status
             :scale: 100%
             :target: https://qdg.readthedocs.io/en/latest/?badge=latest
+        
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `quantumdiceware-0.1.9/README.rst` & `quantumdiceware-0.3.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 ===
 QDG
 ===
-Diceware passphrases from quantum random data
+Generate truly random diceware passphrases.
 
 |build-status| |docs|
 
 .. image:: password_strength.png
 
 
 Features
 --------
 - Simulates dice rolls by gathering quantum data.
 - Includes the complete standard Diceware wordlist.
 - Generate passphrases from custom wordlists.
 
-Python 3.6 is required.
+*Python 3.6 is required.*
 
 
 Usage
 -----
 
 Install
 
-    $ pip3 install quantumdiceware
+    $ pip install quantumdiceware
 
 Generate a Passphrase
 
     $ qdg
 
 Generate five Passphrases and save them to output.txt
 
@@ -48,23 +48,23 @@
 
 See `The Diceware Passphrase Home Page <http://world.std.com/~reinhold/diceware.html>`_ to learn more about Diceware.
 
 
 Meta
 ----
 
-Justin M. Sloan - `justinsloan.com <https://justinsloan.com>`_ - pydev@justinsloan.com
+Justin M. Sloan - `justinsloan.com <https://justinsloan.com>`_ 
 
 Public Domain. See ``LICENSE.txt`` for more information.
 
 https://github.com/justinsloan/qdg
 
 
 .. |build-status| image:: https://travis-ci.org/justinsloan/QDG.svg?branch=master
     :alt: Build Status
     :scale: 100%
     :target: https://travis-ci.org/justinsloan/QDG.svg?branch=master
 
 .. |docs| image:: https://readthedocs.org/projects/docs/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
-    :target: https://qdg.readthedocs.io/en/latest/?badge=latest
+    :target: https://qdg.readthedocs.io/en/latest/?badge=latest
```

### Comparing `quantumdiceware-0.1.9/setup.py` & `quantumdiceware-0.3.0/setup.py`

 * *Files identical despite different names*

