# Comparing `tmp/permutiveapi-3.5.2.tar.gz` & `tmp/permutiveapi-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permutiveapi-3.5.2.tar", last modified: Thu May 30 15:16:14 2024, max compression
+gzip compressed data, was "permutiveapi-3.5.3.tar", last modified: Mon Jun  3 09:50:41 2024, max compression
```

## Comparing `permutiveapi-3.5.2.tar` & `permutiveapi-3.5.3.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:16:14.527315 permutiveapi-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 15:16:14.527315 permutiveapi-3.5.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:16:14.527315 permutiveapi-3.5.2/PermutiveAPI/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10389 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/APIRequestHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/Cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/Import.py
--rw-r--r--   0 runner    (1001) docker     (127)    38864 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/Segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/User.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/Workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/PermutiveAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:16:14.527315 permutiveapi-3.5.2/PermutiveAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 15:16:14.000000 permutiveapi-3.5.2/PermutiveAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-30 15:16:14.000000 permutiveapi-3.5.2/PermutiveAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:16:14.000000 permutiveapi-3.5.2/PermutiveAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:16:14.000000 permutiveapi-3.5.2/PermutiveAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 15:16:10.000000 permutiveapi-3.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:16:14.527315 permutiveapi-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:50:41.642832 permutiveapi-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-03 09:50:41.642832 permutiveapi-3.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:50:41.642832 permutiveapi-3.5.3/PermutiveAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/PermutiveAPI/Cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/PermutiveAPI/Import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38859 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/PermutiveAPI/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/PermutiveAPI/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/PermutiveAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:50:41.642832 permutiveapi-3.5.3/PermutiveAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-03 09:50:41.000000 permutiveapi-3.5.3/PermutiveAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-03 09:50:41.000000 permutiveapi-3.5.3/PermutiveAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:50:41.000000 permutiveapi-3.5.3/PermutiveAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:50:41.000000 permutiveapi-3.5.3/PermutiveAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-03 09:50:37.000000 permutiveapi-3.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:50:41.642832 permutiveapi-3.5.3/setup.cfg
```

### Comparing `permutiveapi-3.5.2/LICENSE` & `permutiveapi-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `permutiveapi-3.5.2/PermutiveAPI/Cohort.py` & `permutiveapi-3.5.3/PermutiveAPI/Cohort.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Dict, List, Optional
 from dataclasses import dataclass, field
 import json
 import logging
 from typing import Dict, List, Optional, Union
 from dataclasses import dataclass
 from datetime import datetime
-from .APIRequestHandler import APIRequestHandler
-from .Utils import FileHelper
+from .. import RequestHelper, FileHelper
 from collections import defaultdict
 
 _API_VERSION = "v2"
 _API_ENDPOINT = f'https://api.permutive.app/cohorts-api/{_API_VERSION}/cohorts/'
 _API_PAYLOAD = ["id", "name", "query", "description", "tags"]
 
 
@@ -77,79 +76,81 @@
                privateKey: Optional[str] = None):
         """
         Creates a new cohort.
 
         :param cohort: Cohort to be created.
         :return: Created cohort object.
         """
-        logging.debug(f"CohortAPI::create::{self.name}")
+        logging.log
+        logging.debug(f"{datetime.now()}::CohortAPI::create::{self.name}")
+        logging.debug(f"{datetime.now()}::CohortAPI::create::{self.name}")
         if not privateKey:
             raise ValueError("privateKey must be specified")
         if not self.query:
             raise ValueError('query must be specified')
         if self.id:
             logging.warning("id is specified")
         url = f"{_API_ENDPOINT}"
-        response = APIRequestHandler.postRequest_static(privateKey=privateKey,
+        response = RequestHelper.postRequest_static(privateKey=privateKey,
                                                         url=url,
-                                                        data=APIRequestHandler.to_payload_static(self, _API_PAYLOAD))
+                                                        data=RequestHelper.to_payload_static(self, _API_PAYLOAD))
         created = Cohort(**response.json())
         self.id = created.id
         self.code = created.code
 
     def update(self,
                privateKey: Optional[str] = None):
         """
         Updates an existing cohort.
 
         :param cohort_id: ID of the cohort to be updated.
         :param updated_cohort: Updated cohort data.
         :return: Updated cohort object.
         """
-        logging.debug(f"CohortAPI::update::{self.name}")
+        logging.debug(f"{datetime.now()}::CohortAPI::update::{self.name}")
         if not privateKey:
             raise ValueError("privateKey must be specified")
         if not self.id:
             logging.warning("id must be specified")
         url = f"{_API_ENDPOINT}{self.id}"
 
-        response = APIRequestHandler.patchRequest_static(privateKey=privateKey,
+        response = RequestHelper.patchRequest_static(privateKey=privateKey,
                                                          url=url,
-                                                         data=APIRequestHandler.to_payload_static(self, _API_PAYLOAD))
+                                                         data=RequestHelper.to_payload_static(self, _API_PAYLOAD))
 
         return Cohort(**response.json())
 
     def delete(self,
                privateKey: Optional[str] = None) -> None:
         """
         Deletes a specific cohort.
         :param cohort_id: ID of the cohort to be deleted.
         :return: None
         """
-        logging.debug(f"CohortAPI::update::{self.name}")
+        logging.debug(f"{datetime.now()}::CohortAPI::update::{self.name}")
         if not privateKey:
             raise ValueError("privateKey must be specified")
         if not self.id:
             logging.warning("id must be specified")
         url = f"{_API_ENDPOINT}{self.id}"
-        APIRequestHandler.deleteRequest_static(privateKey=privateKey,
+        RequestHelper.deleteRequest_static(privateKey=privateKey,
                                                url=url)
 
     @staticmethod
     def get_by_id(id: str,
                   privateKey: str) -> 'Cohort':
         """
         Fetches a specific cohort from the API using its ID.
 
         :param cohort_id: ID of the cohort.
         :return: Cohort object or None if not found.
         """
-        logging.debug(f"CohortAPI::get::{id}")
+        logging.debug(f"{datetime.now()}::CohortAPI::get::{id}")
         url = f"{_API_ENDPOINT}{id}"
-        response = APIRequestHandler.getRequest_static(privateKey=privateKey,
+        response = RequestHelper.getRequest_static(privateKey=privateKey,
                                                        url=url)
 
         return Cohort(**response.json())
 
     @staticmethod
     def get_by_name(
         name: str,
@@ -157,15 +158,15 @@
     ) -> Optional['Cohort']:
         '''
             Object Oriented Permutive Cohort seqrch
             :rtype: Cohort object
             :param cohort_name: str Cohort Name. Required
             :return: Cohort object
         '''
-        logging.debug(f"CohortAPI::get_by_name::{name}")
+        logging.debug(f"{datetime.now()}::CohortAPI::get_by_name::{name}")
 
         for cohort in Cohort.list(include_child_workspaces=True,
                                   privateKey=privateKey):
             if name == cohort.name and cohort.id:
                 return Cohort.get_by_id(id=cohort.id,
                                         privateKey=privateKey)
 
@@ -177,15 +178,15 @@
         Object Oriented Permutive Cohort seqrch
         :rtype: Cohort object
         :param cohort_code: Union[int, str] Cohort Code. Required
         :return: Cohort object
         '''
         if type(code) == str:
             code = int(code)
-        logging.debug(f"CohortAPI::get_by_code::{code}")
+        logging.debug(f"{datetime.now()}::CohortAPI::get_by_code::{code}")
         for cohort in Cohort.list(include_child_workspaces=True,
                                   privateKey=privateKey):
             if code == cohort.code and cohort.id:
                 return Cohort.get_by_id(id=cohort.id,
                                         privateKey=privateKey)
 
     @staticmethod
@@ -197,20 +198,21 @@
             :return: List of all cohorts.
         """
         logging.debug(f"CohortAPI::list")
 
         if not privateKey:
             raise ValueError("No Private Key")
 
-        url = APIRequestHandler.gen_url_with_key(_API_ENDPOINT, privateKey)
+        url = RequestHelper.gen_url_with_key(_API_ENDPOINT, privateKey)
         if include_child_workspaces:
             url = f"{url}&include-child-workspaces=true"
 
-        response = APIRequestHandler.getRequest_static(privateKey, url)
-        cohort_list =CohortList([Cohort(**cohort) for cohort in response.json()])
+        response = RequestHelper.getRequest_static(privateKey, url)
+        cohort_list = CohortList([Cohort(**cohort)
+                                 for cohort in response.json()])
         return cohort_list
 
     def to_json(self, filepath: str):
         FileHelper.check_filepath(filepath)
         with open(file=filepath, mode='w', encoding='utf-8') as f:
             json.dump(self, f,
                       ensure_ascii=False, indent=4, default=FileHelper.json_default)
@@ -236,15 +238,14 @@
         default_factory=dict, init=False)
 
     def __init__(self, cohorts: Optional[List[Cohort]] = None):
         """Initializes the CohortList with an optional list of Cohort objects."""
         super().__init__(cohorts if cohorts is not None else [])
         self.rebuild_cache()
 
-
     def rebuild_cache(self):
         """Rebuilds all caches based on the current state of the list."""
         self._id_dictionary_cache = {
             cohort.id: cohort for cohort in self if cohort.id}
         self._name_dictionary_cache = {
             cohort.name: cohort for cohort in self if cohort.name}
         self._tag_dictionary_cache = defaultdict(CohortList)
@@ -253,15 +254,14 @@
             if cohort.tags:
                 for tag in cohort.tags:
                     self._tag_dictionary_cache[tag].append(cohort)
             if cohort.workspace_id:
                 self._workspace_dictionary_cache[cohort.workspace_id].append(
                     cohort)
 
-
     @property
     def id_dictionary(self) -> Dict[str, Cohort]:
         """Returns a dictionary of cohorts indexed by their IDs."""
         if not self._id_dictionary_cache:
             self.rebuild_cache()
         return self._id_dictionary_cache
```

### Comparing `permutiveapi-3.5.2/PermutiveAPI/Query.py` & `permutiveapi-3.5.3/PermutiveAPI/Query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
-
+import json
 from typing import Dict, List, Optional, Union, Any, Tuple
 from dataclasses import dataclass, field
 
 from collections import defaultdict
 from collections.abc import Iterable
 import urllib.parse
 
-from .Utils import FileHelper, ListHelper
-
+from .. import FileHelper, ListHelper
 from .Cohort import Cohort
-import json
+
 
 ITEMS = {'ä': 'a',  'â': 'a', 'á': 'a', 'à': 'a', 'ã': 'a', 'ç': 'c', 'è': 'e', 'é': 'e', 'ê': 'e', 'ë': 'e',
          'í': 'i',  'ï': 'i', 'ò': 'o', 'ó': 'o', 'õ': 'o', 'ô': 'o', 'ñ': 'n', 'ù': 'u', 'ú': 'u', 'ü': 'u'}
 
 
 @dataclass
 class Query():
```

### Comparing `permutiveapi-3.5.2/PermutiveAPI/Workspace.py` & `permutiveapi-3.5.3/PermutiveAPI/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from typing import Dict, List, Optional
-from collections.abc import Iterable
 from dataclasses import dataclass, field
+import os
 import json
 import logging
-from typing import List, Optional, Dict
-from dataclasses import dataclass
-import os
-
 
-from .Utils import FileHelper, ListHelper
+from .. import ListHelper, FileHelper
 from .Cohort import Cohort, CohortList
-from .Query import Query
-from .Import import Import
-from .Segment import Segment
+from .Import import Import, ImportList,Segment, SegmentList
+from .User import User
+from .Query import Query, QueryList
+
 
 TAGS = ['#automatic', '#imports']
 
 
 @dataclass
 class Workspace():
     """
@@ -182,7 +179,11 @@
             filepath = os.environ.get("PERMUTIVE_APPLICATION_CREDENTIALS")
         if not filepath:
             raise ValueError(
                 'Unable to get PERMUTIVE_APPLICATION_CREDENTIALS from .env')
 
         workspace_list = FileHelper.from_json(filepath)
         return WorkspaceList([Workspace(**workspace) for workspace in workspace_list])
+
+
+__all__ = ["Cohort", "CohortList", "Import", "ImportList", "Segment", "SegmentList",
+           "Workspace", "WorkspaceList", "Query", "QueryList", "User"]
```

