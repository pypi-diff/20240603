# Comparing `tmp/pr_pilot-1.4.1.tar.gz` & `tmp/pr_pilot-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot-1.4.1.tar", last modified: Thu May 30 01:13:55 2024, max compression
+gzip compressed data, was "pr_pilot-1.5.0.tar", last modified: Mon Jun  3 02:36:32 2024, max compression
```

## Comparing `pr_pilot-1.4.1.tar` & `pr_pilot-1.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:13:55.984592 pr_pilot-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-30 01:13:55.984592 pr_pilot-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:13:55.980592 pr_pilot-1.4.1/pr_pilot/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:13:55.980592 pr_pilot-1.4.1/pr_pilot/api/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/api/task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/api/task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26237 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15422 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:13:55.980592 pr_pilot-1.4.1/pr_pilot/models/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/models/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/models/not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/models/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:13:55.984592 pr_pilot-1.4.1/pr_pilot/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/test/test_bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/test/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/test/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/test/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/test/test_task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/test/test_task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/pr_pilot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:13:55.984592 pr_pilot-1.4.1/pr_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-30 01:13:55.000000 pr_pilot-1.4.1/pr_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 01:13:55.000000 pr_pilot-1.4.1/pr_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:13:55.000000 pr_pilot-1.4.1/pr_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 01:13:55.000000 pr_pilot-1.4.1/pr_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 01:13:55.000000 pr_pilot-1.4.1/pr_pilot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:13:55.984592 pr_pilot-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-30 01:13:49.000000 pr_pilot-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:36:32.778477 pr_pilot-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-06-03 02:36:32.778477 pr_pilot-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:36:32.774476 pr_pilot-1.5.0/pr_pilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:36:32.778477 pr_pilot-1.5.0/pr_pilot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/api/task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/api/task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26237 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15422 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:36:32.778477 pr_pilot-1.5.0/pr_pilot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/models/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/models/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/models/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:36:32.778477 pr_pilot-1.5.0/pr_pilot/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/test/test_bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/test/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/test/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/test/test_task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/test/test_task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/pr_pilot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:36:32.778477 pr_pilot-1.5.0/pr_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-06-03 02:36:32.000000 pr_pilot-1.5.0/pr_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-06-03 02:36:32.000000 pr_pilot-1.5.0/pr_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 02:36:32.000000 pr_pilot-1.5.0/pr_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-03 02:36:32.000000 pr_pilot-1.5.0/pr_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 02:36:32.000000 pr_pilot-1.5.0/pr_pilot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 02:36:32.778477 pr_pilot-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-06-03 02:36:26.000000 pr_pilot-1.5.0/setup.py
```

### Comparing `pr_pilot-1.4.1/LICENSE` & `pr_pilot-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/PKG-INFO` & `pr_pilot-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.4.1 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.5.0 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.4.1/README.md` & `pr_pilot-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/__init__.py` & `pr_pilot-1.5.0/pr_pilot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
```

### Comparing `pr_pilot-1.4.1/pr_pilot/api/task_creation_api.py` & `pr_pilot-1.5.0/pr_pilot/api/task_creation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
```

### Comparing `pr_pilot-1.4.1/pr_pilot/api/task_retrieval_api.py` & `pr_pilot-1.5.0/pr_pilot/api/task_retrieval_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
```

### Comparing `pr_pilot-1.4.1/pr_pilot/api_client.py` & `pr_pilot-1.5.0/pr_pilot/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import datetime
```

### Comparing `pr_pilot-1.4.1/pr_pilot/api_response.py` & `pr_pilot-1.5.0/pr_pilot/api_response.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/configuration.py` & `pr_pilot-1.5.0/pr_pilot/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -394,15 +394,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.15\n"\
+               "Version of the API: 1.3.24\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `pr_pilot-1.4.1/pr_pilot/exceptions.py` & `pr_pilot-1.5.0/pr_pilot/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
 from typing_extensions import Self
```

### Comparing `pr_pilot-1.4.1/pr_pilot/models/bad_request.py` & `pr_pilot-1.5.0/pr_pilot/models/bad_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `pr_pilot-1.4.1/pr_pilot/models/not_found.py` & `pr_pilot-1.5.0/pr_pilot/models/not_found.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `pr_pilot-1.4.1/pr_pilot/models/prompt.py` & `pr_pilot-1.5.0/pr_pilot/models/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -27,15 +27,16 @@
     Prompt
     """ # noqa: E501
     prompt: StrictStr = Field(description="The prompt for the task")
     github_repo: StrictStr = Field(description="The full name of the Github repository, e.g. 'owner/repo'")
     issue_number: Optional[StrictInt] = Field(default=None, description="Number of the issue if task is triggered in the context of an issue")
     pr_number: Optional[StrictInt] = Field(default=None, description="Number of the PR if task is triggered in the context of a PR")
     gpt_model: Optional[StrictStr] = Field(default='gpt-4-turbo', description="The GPT model to use for the task")
-    __properties: ClassVar[List[str]] = ["prompt", "github_repo", "issue_number", "pr_number", "gpt_model"]
+    image: Optional[StrictStr] = Field(default=None, description="An image to be used in the task")
+    __properties: ClassVar[List[str]] = ["prompt", "github_repo", "issue_number", "pr_number", "gpt_model", "image"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -84,12 +85,13 @@
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "prompt": obj.get("prompt"),
             "github_repo": obj.get("github_repo"),
             "issue_number": obj.get("issue_number"),
             "pr_number": obj.get("pr_number"),
-            "gpt_model": obj.get("gpt_model") if obj.get("gpt_model") is not None else 'gpt-4-turbo'
+            "gpt_model": obj.get("gpt_model") if obj.get("gpt_model") is not None else 'gpt-4-turbo',
+            "image": obj.get("image")
         })
         return _obj
```

### Comparing `pr_pilot-1.4.1/pr_pilot/models/task.py` & `pr_pilot-1.5.0/pr_pilot/models/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `pr_pilot-1.4.1/pr_pilot/rest.py` & `pr_pilot-1.5.0/pr_pilot/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.3.15
+    The version of the OpenAPI document: 1.3.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `pr_pilot-1.4.1/pr_pilot/test/test_bad_request.py` & `pr_pilot-1.5.0/pr_pilot/test/test_bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/test/test_not_found.py` & `pr_pilot-1.5.0/pr_pilot/test/test_not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/test/test_prompt.py` & `pr_pilot-1.5.0/pr_pilot/test/test_prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/test/test_task.py` & `pr_pilot-1.5.0/pr_pilot/test/test_task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/test/test_task_creation_api.py` & `pr_pilot-1.5.0/pr_pilot/test/test_task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/test/test_task_retrieval_api.py` & `pr_pilot-1.5.0/pr_pilot/test/test_task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/pr_pilot/util.py` & `pr_pilot-1.5.0/pr_pilot/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import base64
 import logging
 import os
 import time
+from pathlib import Path
+from typing import Optional
 
 import pr_pilot
 from pr_pilot import Task, Prompt
 
 # Set log level to INFO
 logging.basicConfig(level=logging.INFO)
 
@@ -57,24 +60,26 @@
     if output_file is not None:
         with open(output_file, "a") as file:
             file.write(f"{summary}\n")
     else:
         logger.debug("GITHUB_STEP_SUMMARY environment variable is not set.")
 
 
-def create_task(repo: str, prompt: str, log=True, pr_number=None, issue_number=None, gpt_model=None) -> Task:
+def create_task(repo: str, prompt: str, log=True, pr_number=None, issue_number=None, gpt_model=None, image: Optional[Path]=None) -> Task:
     """Create a task for the specified repository with the given prompt."""
     with pr_pilot.ApiClient(_get_config_from_env()) as api_client:
         api_instance = pr_pilot.TaskCreationApi(api_client)
         if pr_number is not None:
             pr_number = int(pr_number)
         if issue_number is not None:
             issue_number = int(issue_number)
+
+        image_base64 = base64.encode(image.read_bytes()).decode("utf-8") if image else None
         task = api_instance.tasks_create(Prompt(prompt=prompt, github_repo=repo, issue_number=issue_number,
-                                                pr_number=pr_number, gpt_model=gpt_model))
+                                                pr_number=pr_number, gpt_model=gpt_model, image=image_base64))
         dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{str(task.id)}/"
         set_github_action_output("task-id", str(task.id))
         set_github_action_output("task-url", dashboard_url)
         if log:
             logger.info(f"PR Pilot task created: {dashboard_url}")
         return task
```

### Comparing `pr_pilot-1.4.1/pr_pilot.egg-info/PKG-INFO` & `pr_pilot-1.5.0/pr_pilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.4.1 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.5.0 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.4.1/pr_pilot.egg-info/SOURCES.txt` & `pr_pilot-1.5.0/pr_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.4.1/setup.py` & `pr_pilot-1.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 requirements_path = path.join(this_dir, 'requirements.txt')
 with open(requirements_path) as f:
     required = f.read().splitlines()
 
 setup(
     name='pr_pilot',
-    version='1.4.1',
+    version='1.5.0',
     packages=find_packages(),
     install_requires=required,
     python_requires='>=3.6',
     author='Marco Lamina',
     author_email='marco@pr-pilot.ai',
     description='Python SDK for PR Pilot, a text-to-task automation platform for Github.',
     long_description=open('README.md').read(),
```

