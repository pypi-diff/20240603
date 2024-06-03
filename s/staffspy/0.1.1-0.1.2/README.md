# Comparing `tmp/staffspy-0.1.1.tar.gz` & `tmp/staffspy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staffspy-0.1.1.tar", max compression
+gzip compressed data, was "staffspy-0.1.2.tar", max compression
```

## Comparing `staffspy-0.1.1.tar` & `staffspy-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-06-03 05:22:43.493751 staffspy-0.1.1/LICENSE
--rw-r--r--   0        0        0     2898 2024-06-03 05:22:43.493751 staffspy-0.1.1/README.md
--rw-r--r--   0        0        0      457 2024-06-03 05:22:43.493751 staffspy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1044 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/__init__.py
--rw-r--r--   0        0        0      121 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/exceptions.py
--rw-r--r--   0        0        0    19294 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/linkedin/__init__.py
--rw-r--r--   0        0        0     3696 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/models.py
--rw-r--r--   0        0        0     3656 2024-06-03 05:22:43.493751 staffspy-0.1.1/staffspy/utils.py
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 staffspy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-03 05:29:58.841686 staffspy-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2915 2024-06-03 05:29:58.841686 staffspy-0.1.2/README.md
+-rw-r--r--   0        0        0      457 2024-06-03 05:29:58.841686 staffspy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1061 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/__init__.py
+-rw-r--r--   0        0        0      121 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/exceptions.py
+-rw-r--r--   0        0        0    19294 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/linkedin/__init__.py
+-rw-r--r--   0        0        0     3696 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/models.py
+-rw-r--r--   0        0        0     3656 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/utils.py
+-rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 staffspy-0.1.2/PKG-INFO
```

### Comparing `staffspy-0.1.1/LICENSE` & `staffspy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.1/README.md` & `staffspy-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,37 +57,43 @@
 ├── session_file (str): 
 |    file path to save session cookies, so only one manual login is needed.
 |    can use mult profiles this way
 │
 ├── log_level (int): 
 |    Controls the verbosity of the runtime printouts 
 |    (0 prints only errors, 1 is info, 2 is all logs. Default is 0.)
-│
+```
 
 ### Staff Schema
-
 ```plaintext
 Staff
+Staff
 ├── search_term
 ├── id
 ├── name
+|
 ├── position
 ├── profile_id
 ├── profile_link
 ├── first_name
 ├── last_name
+|
 ├── followers
 ├── connections
+|
 ├── location
 ├── company
 ├── school
+|
 ├── influencer
 ├── creator
 ├── premium
+|
 ├── profile_photo
+|
 ├── skills
 │   ├── name
 │   └── endorsements
 ├── experiences
 │   ├── from_date
 │   ├── to_date
 │   ├── duration
```

### Comparing `staffspy-0.1.1/staffspy/__init__.py` & `staffspy-0.1.2/staffspy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 
-from linkedin import LinkedInScraper
+from staffspy.linkedin import LinkedInScraper
 
-from .utils import set_logger_level, logger
+from staffspy.utils import set_logger_level, logger
 
 
 def scrape_staff(
     *,
     company_name: str,
     session_file: str = None,
     search_term: str = None,
```

### Comparing `staffspy-0.1.1/staffspy/linkedin/__init__.py` & `staffspy-0.1.2/staffspy/linkedin/__init__.py`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.1/staffspy/models.py` & `staffspy-0.1.2/staffspy/models.py`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.1/staffspy/utils.py` & `staffspy-0.1.2/staffspy/utils.py`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.1/PKG-INFO` & `staffspy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staffspy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Staff scraper library for LinkedIn
 Author: Cullen Watson
 Author-email: cullen@bunsly.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -73,37 +73,43 @@
 ├── session_file (str): 
 |    file path to save session cookies, so only one manual login is needed.
 |    can use mult profiles this way
 │
 ├── log_level (int): 
 |    Controls the verbosity of the runtime printouts 
 |    (0 prints only errors, 1 is info, 2 is all logs. Default is 0.)
-│
+```
 
 ### Staff Schema
-
 ```plaintext
 Staff
+Staff
 ├── search_term
 ├── id
 ├── name
+|
 ├── position
 ├── profile_id
 ├── profile_link
 ├── first_name
 ├── last_name
+|
 ├── followers
 ├── connections
+|
 ├── location
 ├── company
 ├── school
+|
 ├── influencer
 ├── creator
 ├── premium
+|
 ├── profile_photo
+|
 ├── skills
 │   ├── name
 │   └── endorsements
 ├── experiences
 │   ├── from_date
 │   ├── to_date
 │   ├── duration
```

