# Comparing `tmp/kumparanian-1.2.0rc2.tar.gz` & `tmp/kumparanian-1.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumparanian-1.2.0rc2.tar", max compression
+gzip compressed data, was "kumparanian-1.2.0rc3.tar", max compression
```

## Comparing `kumparanian-1.2.0rc2.tar` & `kumparanian-1.2.0rc3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1486 2024-05-15 07:02:16.132381 kumparanian-1.2.0rc2/LICENSE
--rw-r--r--   0        0        0     2863 2024-05-30 04:46:04.796932 kumparanian-1.2.0rc2/README.md
--rw-r--r--   0        0        0        0 2024-05-15 07:02:16.133186 kumparanian-1.2.0rc2/kumparanian/__init__.py
--rw-r--r--   0        0        0       30 2024-05-15 07:02:16.133323 kumparanian-1.2.0rc2/kumparanian/__main__.py
--rw-r--r--   0        0        0     1687 2024-05-28 11:10:59.573760 kumparanian-1.2.0rc2/kumparanian/cli.py
--rw-r--r--   0        0        0      392 2024-05-27 06:29:00.637103 kumparanian-1.2.0rc2/kumparanian/ds/__init__.py
--rw-r--r--   0        0        0      893 2024-05-22 18:00:54.982713 kumparanian-1.2.0rc2/kumparanian/ds/help_text.py
--rw-r--r--   0        0        0     9470 2024-05-29 08:10:23.998982 kumparanian-1.2.0rc2/kumparanian/ds/model.py
--rw-r--r--   0        0        0     1016 2024-05-30 11:08:52.423947 kumparanian-1.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 kumparanian-1.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1486 2024-05-15 07:02:16.132381 kumparanian-1.2.0rc3/LICENSE
+-rw-r--r--   0        0        0     2830 2024-06-02 08:53:23.061455 kumparanian-1.2.0rc3/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 07:02:16.133186 kumparanian-1.2.0rc3/kumparanian/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-15 07:02:16.133323 kumparanian-1.2.0rc3/kumparanian/__main__.py
+-rw-r--r--   0        0        0     1687 2024-05-28 11:10:59.573760 kumparanian-1.2.0rc3/kumparanian/cli.py
+-rw-r--r--   0        0        0      392 2024-05-27 06:29:00.637103 kumparanian-1.2.0rc3/kumparanian/ds/__init__.py
+-rw-r--r--   0        0        0      881 2024-06-03 01:46:24.740578 kumparanian-1.2.0rc3/kumparanian/ds/help_text.py
+-rw-r--r--   0        0        0     9470 2024-05-29 08:10:23.998982 kumparanian-1.2.0rc3/kumparanian/ds/model.py
+-rw-r--r--   0        0        0     1016 2024-06-02 08:48:02.277590 kumparanian-1.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 kumparanian-1.2.0rc3/PKG-INFO
```

### Comparing `kumparanian-1.2.0rc2/LICENSE` & `kumparanian-1.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `kumparanian-1.2.0rc2/README.md` & `kumparanian-1.2.0rc3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Kumparanian [![Build Status](https://travis-ci.org/kumparan/kumparanian.svg?branch=master)](https://travis-ci.org/kumparan/kumparanian) [![PyPI version](https://badge.fury.io/py/kumparanian.svg)](https://badge.fury.io/py/kumparanian)
-Kumparanian is a set of workflows that optimize Kumparan's data engineering 
-and data scientist hiring process. It cuts down 1-2 working day(s) submission 
-review process to just less than an hour.
+Kumparanian is a set of workflows that optimize Kumparan's data scientist 
+hiring process. It cuts down 1-2 working day(s) submission review process 
+to just less than an hour.
 
-If you are our candidate, you need to install `kumparanian` using following command (we highly recommend to install inside virtual env, like venv):
+If you are our candidate, you need to install `kumparanian` using following command 
+(we highly recommend to install inside virtual env, like venv):
 
     python -m venv <your_env_name>
 
     source <your_env_name>/bin/activate
 
     pip install kumparanian 
 
@@ -20,16 +21,16 @@
 
       Before you submit your trained model, you can verify your trained model
       using the following command:
 
       $ kumparanian ds verify YOURMODEL.pickle YOURFILE.pickle
     
       YOURMODEL.pickle should contain your trained model, and YOURFILE.pickle
-      should contain the necessary preprocessing components such as the vectorizer, 
-      label encoder, and model type.
+      should contain the necessary preprocessing components such as the vectorizer 
+      and label encoder.
 
       Use the following command to evaluate your trained model against your test
       dataset:
 
       $ kumparanian ds evaluate YOURMODEL.pickle YOURFILE.pickle test_file.csv
 
     Options:
```

### Comparing `kumparanian-1.2.0rc2/kumparanian/cli.py` & `kumparanian-1.2.0rc3/kumparanian/cli.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.2.0rc2/kumparanian/ds/help_text.py` & `kumparanian-1.2.0rc3/kumparanian/ds/help_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 Before you submit your trained model, you can verify your trained model using
 the following command:
 
 $ kumparanian ds verify YOURMODEL.pickle YOURFILE.pickle
 
 YOURMODEL.pickle should contain your trained model, and YOURFILE.pickle
-should contain the necessary preprocessing components such as the vectorizer, label encoder, and model type.
+should contain the necessary preprocessing components such as the vectorizer 
+and label encoder.
 
 Use the following command to evaluate your trained model against your test
 dataset:
 
 $ kumparanian ds evaluate YOURMODEL.pickle YOURFILE.pickle test_file.csv
 """
```

### Comparing `kumparanian-1.2.0rc2/kumparanian/ds/model.py` & `kumparanian-1.2.0rc3/kumparanian/ds/model.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.2.0rc2/pyproject.toml` & `kumparanian-1.2.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kumparanian"
-version = "1.2.0rc2"
+version = "1.2.0rc3"
 description = "Kumparanian CLI"
 authors = ["Zavli Juwantara <zavli.juwantara@kumparan.com>"]
 repository = "https://github.com/kumparan/kumparanian"
 maintainers = [
     "Bayu <bayualdiyansyah@gmail.com>",
     "Raden <radenmaharjo@gmail.com>",
     "Aslam <aslam.hadi@kumparan.com>",
```

### Comparing `kumparanian-1.2.0rc2/PKG-INFO` & `kumparanian-1.2.0rc3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kumparanian
-Version: 1.2.0rc2
+Version: 1.2.0rc3
 Summary: Kumparanian CLI
 Home-page: https://github.com/kumparan/kumparanian
 License: kumparan
 Author: Zavli Juwantara
 Author-email: zavli.juwantara@kumparan.com
 Maintainer: Bayu
 Maintainer-email: bayualdiyansyah@gmail.com
@@ -19,19 +19,20 @@
 Requires-Dist: numpy (==1.24.3)
 Requires-Dist: scikit-learn (==1.4.2)
 Requires-Dist: tensorflow (==2.13.0)
 Project-URL: Repository, https://github.com/kumparan/kumparanian
 Description-Content-Type: text/markdown
 
 # Kumparanian [![Build Status](https://travis-ci.org/kumparan/kumparanian.svg?branch=master)](https://travis-ci.org/kumparan/kumparanian) [![PyPI version](https://badge.fury.io/py/kumparanian.svg)](https://badge.fury.io/py/kumparanian)
-Kumparanian is a set of workflows that optimize Kumparan's data engineering 
-and data scientist hiring process. It cuts down 1-2 working day(s) submission 
-review process to just less than an hour.
+Kumparanian is a set of workflows that optimize Kumparan's data scientist 
+hiring process. It cuts down 1-2 working day(s) submission review process 
+to just less than an hour.
 
-If you are our candidate, you need to install `kumparanian` using following command (we highly recommend to install inside virtual env, like venv):
+If you are our candidate, you need to install `kumparanian` using following command 
+(we highly recommend to install inside virtual env, like venv):
 
     python -m venv <your_env_name>
 
     source <your_env_name>/bin/activate
 
     pip install kumparanian 
 
@@ -44,16 +45,16 @@
 
       Before you submit your trained model, you can verify your trained model
       using the following command:
 
       $ kumparanian ds verify YOURMODEL.pickle YOURFILE.pickle
     
       YOURMODEL.pickle should contain your trained model, and YOURFILE.pickle
-      should contain the necessary preprocessing components such as the vectorizer, 
-      label encoder, and model type.
+      should contain the necessary preprocessing components such as the vectorizer 
+      and label encoder.
 
       Use the following command to evaluate your trained model against your test
       dataset:
 
       $ kumparanian ds evaluate YOURMODEL.pickle YOURFILE.pickle test_file.csv
 
     Options:
```

