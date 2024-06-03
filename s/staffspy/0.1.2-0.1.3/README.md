# Comparing `tmp/staffspy-0.1.2.tar.gz` & `tmp/staffspy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staffspy-0.1.2.tar", max compression
+gzip compressed data, was "staffspy-0.1.3.tar", max compression
```

## Comparing `staffspy-0.1.2.tar` & `staffspy-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-06-03 05:29:58.841686 staffspy-0.1.2/LICENSE
--rw-r--r--   0        0        0     2915 2024-06-03 05:29:58.841686 staffspy-0.1.2/README.md
--rw-r--r--   0        0        0      457 2024-06-03 05:29:58.841686 staffspy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1061 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/__init__.py
--rw-r--r--   0        0        0      121 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/exceptions.py
--rw-r--r--   0        0        0    19294 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/linkedin/__init__.py
--rw-r--r--   0        0        0     3696 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/models.py
--rw-r--r--   0        0        0     3656 2024-06-03 05:29:58.841686 staffspy-0.1.2/staffspy/utils.py
--rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 staffspy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-03 05:33:20.246213 staffspy-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2915 2024-06-03 05:33:20.246213 staffspy-0.1.3/README.md
+-rw-r--r--   0        0        0      457 2024-06-03 05:33:20.246213 staffspy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1061 2024-06-03 05:33:20.246213 staffspy-0.1.3/staffspy/__init__.py
+-rw-r--r--   0        0        0      121 2024-06-03 05:33:20.246213 staffspy-0.1.3/staffspy/exceptions.py
+-rw-r--r--   0        0        0    19312 2024-06-03 05:33:20.246213 staffspy-0.1.3/staffspy/linkedin/__init__.py
+-rw-r--r--   0        0        0     3696 2024-06-03 05:33:20.246213 staffspy-0.1.3/staffspy/models.py
+-rw-r--r--   0        0        0     3656 2024-06-03 05:33:20.246213 staffspy-0.1.3/staffspy/utils.py
+-rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 staffspy-0.1.3/PKG-INFO
```

### Comparing `staffspy-0.1.2/LICENSE` & `staffspy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.2/README.md` & `staffspy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.2/staffspy/__init__.py` & `staffspy-0.1.3/staffspy/__init__.py`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.2/staffspy/linkedin/__init__.py` & `staffspy-0.1.3/staffspy/linkedin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import re
 import sys
 from urllib.parse import quote
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
-import utils
+import staffspy.utils as utils
 from staffspy.utils import logger
 from staffspy.exceptions import TooManyRequests
 from staffspy.models import Staff, Experience, Certification, Skill, School
 
 
 class LinkedInScraper:
     company_id_ep = "https://www.linkedin.com/voyager/api/organization/companies?q=universalName&universalName="
```

### Comparing `staffspy-0.1.2/staffspy/models.py` & `staffspy-0.1.3/staffspy/models.py`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.2/staffspy/utils.py` & `staffspy-0.1.3/staffspy/utils.py`

 * *Files identical despite different names*

### Comparing `staffspy-0.1.2/PKG-INFO` & `staffspy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staffspy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Staff scraper library for LinkedIn
 Author: Cullen Watson
 Author-email: cullen@bunsly.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

