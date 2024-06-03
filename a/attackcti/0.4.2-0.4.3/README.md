# Comparing `tmp/attackcti-0.4.2.tar.gz` & `tmp/attackcti-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attackcti-0.4.2.tar", last modified: Tue Apr  9 06:17:16 2024, max compression
+gzip compressed data, was "attackcti-0.4.3.tar", last modified: Mon Jun  3 10:20:49 2024, max compression
```

## Comparing `attackcti-0.4.2.tar` & `attackcti-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-09 06:17:16.162282 attackcti-0.4.2/
--rw-r--r--   0 wardog     (501) staff       (20)     1517 2024-03-30 02:47:07.000000 attackcti-0.4.2/LICENSE
--rw-r--r--   0 wardog     (501) staff       (20)     4631 2024-04-09 06:17:16.162213 attackcti-0.4.2/PKG-INFO
--rw-r--r--   0 wardog     (501) staff       (20)     3457 2024-04-09 01:42:38.000000 attackcti-0.4.2/README.md
-drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-09 06:17:16.161115 attackcti-0.4.2/attackcti/
--rw-r--r--   0 wardog     (501) staff       (20)       60 2024-03-30 02:47:07.000000 attackcti-0.4.2/attackcti/__init__.py
--rw-r--r--   0 wardog     (501) staff       (20)   129039 2024-04-09 05:41:49.000000 attackcti-0.4.2/attackcti/attack_api.py
--rw-r--r--   0 wardog     (501) staff       (20)     8749 2024-04-09 06:05:40.000000 attackcti-0.4.2/attackcti/models.py
-drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-09 06:17:16.161926 attackcti-0.4.2/attackcti.egg-info/
--rw-r--r--   0 wardog     (501) staff       (20)     4631 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/PKG-INFO
--rw-r--r--   0 wardog     (501) staff       (20)      266 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/SOURCES.txt
--rw-r--r--   0 wardog     (501) staff       (20)        1 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/dependency_links.txt
--rw-r--r--   0 wardog     (501) staff       (20)       29 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/requires.txt
--rw-r--r--   0 wardog     (501) staff       (20)       10 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/top_level.txt
--rw-r--r--   0 wardog     (501) staff       (20)       79 2024-04-09 06:17:16.162480 attackcti-0.4.2/setup.cfg
--rw-r--r--   0 wardog     (501) staff       (20)     1650 2024-04-09 01:43:15.000000 attackcti-0.4.2/setup.py
+drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-06-03 10:20:49.244639 attackcti-0.4.3/
+-rw-r--r--   0 wardog     (501) staff       (20)     1517 2024-03-30 02:47:07.000000 attackcti-0.4.3/LICENSE
+-rw-r--r--   0 wardog     (501) staff       (20)     4631 2024-06-03 10:20:49.244570 attackcti-0.4.3/PKG-INFO
+-rw-r--r--   0 wardog     (501) staff       (20)     3457 2024-04-09 01:42:38.000000 attackcti-0.4.3/README.md
+drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-06-03 10:20:49.243143 attackcti-0.4.3/attackcti/
+-rw-r--r--   0 wardog     (501) staff       (20)       60 2024-03-30 02:47:07.000000 attackcti-0.4.3/attackcti/__init__.py
+-rw-r--r--   0 wardog     (501) staff       (20)   130047 2024-06-03 10:16:22.000000 attackcti-0.4.3/attackcti/attack_api.py
+-rw-r--r--   0 wardog     (501) staff       (20)     9119 2024-06-03 09:06:22.000000 attackcti-0.4.3/attackcti/models.py
+drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-06-03 10:20:49.244209 attackcti-0.4.3/attackcti.egg-info/
+-rw-r--r--   0 wardog     (501) staff       (20)     4631 2024-06-03 10:20:49.000000 attackcti-0.4.3/attackcti.egg-info/PKG-INFO
+-rw-r--r--   0 wardog     (501) staff       (20)      266 2024-06-03 10:20:49.000000 attackcti-0.4.3/attackcti.egg-info/SOURCES.txt
+-rw-r--r--   0 wardog     (501) staff       (20)        1 2024-06-03 10:20:49.000000 attackcti-0.4.3/attackcti.egg-info/dependency_links.txt
+-rw-r--r--   0 wardog     (501) staff       (20)       29 2024-06-03 10:20:49.000000 attackcti-0.4.3/attackcti.egg-info/requires.txt
+-rw-r--r--   0 wardog     (501) staff       (20)       10 2024-06-03 10:20:49.000000 attackcti-0.4.3/attackcti.egg-info/top_level.txt
+-rw-r--r--   0 wardog     (501) staff       (20)       79 2024-06-03 10:20:49.244837 attackcti-0.4.3/setup.cfg
+-rw-r--r--   0 wardog     (501) staff       (20)     1650 2024-06-03 10:18:34.000000 attackcti-0.4.3/setup.py
```

### Comparing `attackcti-0.4.2/LICENSE` & `attackcti-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `attackcti-0.4.2/PKG-INFO` & `attackcti-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.4.2
+Version: 0.4.3
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
```

### Comparing `attackcti-0.4.2/README.md` & `attackcti-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `attackcti-0.4.2/attackcti/attack_api.py` & `attackcti-0.4.3/attackcti/attack_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # License: BSD 3-Clause
 # Reference:
 # https://www.mitre.org/capabilities/cybersecurity/overview/cybersecurity-blog/attck%E2%84%A2-content-available-in-stix%E2%84%A2-20-via
 # https://github.com/mitre/cti/blob/master/USAGE.md
 # https://github.com/oasis-open/cti-python-stix2/issues/183
 # https://stackoverflow.com/a/4406521
 
-from stix2 import TAXIICollectionSource, Filter, CompositeDataSource, FileSystemSource
+from stix2 import TAXIICollectionSource, Filter, CompositeDataSource
 from stix2.datastore.filters import apply_common_filters
 from stix2.utils import get_type_from_id
 from stix2.v20.sdo import (
     AttackPattern as AttackPattern_v20, # Technique
     Campaign as Campaign_v20, # Campaign
     Malware as Malware_v20, # Malware
     CourseOfAction as CourseOfAction_v20, # Mitigation
@@ -21,40 +21,30 @@
     Tool as Tool_v20 # Tool
 )
 from stix2.v20.sro import Relationship as Relationship_v20
 from taxii2client.v20 import Collection
 import json
 import os
 
-from .models import *
-from pydantic import TypeAdapter
+from pydantic import TypeAdapter, ValidationError
 from typing import List, Type, Dict, Any, Union
+from attackcti.models import *
+from attackcti.utils.storage import STIXStore
 
 # os.environ['http_proxy'] = "http://xxxxxxx"
 # os.environ['https_proxy'] = "https://xxxxxxx"
 
 ATTACK_STIX_COLLECTIONS = "https://cti-taxii.mitre.org/stix/collections/"
 ENTERPRISE_ATTACK = "95ecc380-afe9-11e4-9b6c-751b66dd541e"
-PRE_ATTACK = "062767bd-02d2-4b72-84ba-56caef0f8658"
 MOBILE_ATTACK = "2f669986-b40b-4423-b720-4396ca6a462b"
 ICS_ATTACK = "02c3ef24-9cd4-48f3-a99f-b74ce24f1d34"
 
-ENTERPRISE_ATTACK_LOCAL_DIR = "enterprise-attack"
-PRE_ATTACK_LOCAL_DIR = "pre-attack"
-MOBILE_ATTACK_LOCAL_DIR = "mobile-attack"
-ICS_ATTACK_LOCAL_DIR = "ics-attack"
-
-class attack_client(object):
-    """A Python Module for ATT&CK"""
-    TC_ENTERPRISE_SOURCE = None
-    TC_PRE_SOURCE = None
-    TC_MOBILE_SOURCE = None
-    TC_ICS_SOURCE = None
-    COMPOSITE_DS = None
-
+class attack_client:
+    """A Python Module for accessing ATT&CK data locally or remotely."""
+    
     pydantic_model_mapping = {
         "techniques": Technique,
         "data-component": DataComponent,
         "mitigations": Mitigation,
         "groups": Group,
         "malware": Software,
         "tools": Software,
@@ -70,45 +60,87 @@
         "attack-pattern": Technique,
         "course-of-action": Mitigation,
         "intrusion-set": Group,
         "x-mitre-data-source": DataSource,
         "x-mitre-data-component": DataComponent
     }
     
-    def __init__(self, local_path=None, include_pre_attack=False, proxies=None, verify=True):
+    def __init__(self, local_paths=None, proxies=None, verify=True):
+        """
+        Initializes the ATT&CK client, setting up local or remote data sources.
+
+        Args:
+            local_paths (dict, optional): Dictionary with paths to local directories or JSON files for each domain.
+                                          Keys should be 'enterprise', 'mobile', and 'ics'.
+            proxies (dict, optional): Dictionary mapping protocol or protocol and hostname to the URL of the proxy.
+            verify (bool, optional): Whether to verify SSL certificates. Defaults to True.
         """
+        self.COMPOSITE_DS = CompositeDataSource()
+
+        # Validate local_paths with Pydantic
+        if local_paths:
+            try:
+                self.local_paths = STIXLocalPaths(**local_paths)
+            except ValidationError as e:
+                raise ValueError(f"Invalid local_paths: {e}")
+
+        # Initialize data sources
+        self.init_data_sources(self.local_paths if local_paths else None, proxies, verify)
+
+    def init_data_sources(self, local_paths, proxies, verify):
+        """
+        Initializes data sources, either local or remote.
+
         Args:
-            proxies - See https://requests.readthedocs.io/en/latest/user/advanced/#proxies
-            verify - See https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+            local_paths (LocalPathsModel, optional): Validated dictionary with paths to local directories or JSON files for each domain.
+            proxies (dict, optional): Dictionary mapping protocol or protocol and hostname to the URL of the proxy.
+            verify (bool, optional): Whether to verify SSL certificates. Defaults to True.
         """
+        if local_paths:
+            self.TC_ENTERPRISE_SOURCE = self.load_stix_store(local_paths.enterprise)
+            self.TC_MOBILE_SOURCE = self.load_stix_store(local_paths.mobile)
+            self.TC_ICS_SOURCE = self.load_stix_store(local_paths.ics)
 
-        if local_path is not None and os.path.isdir(os.path.join(local_path, ENTERPRISE_ATTACK_LOCAL_DIR)) \
-                                  and os.path.isdir(os.path.join(local_path, PRE_ATTACK_LOCAL_DIR)) \
-                                  and os.path.isdir(os.path.join(local_path, MOBILE_ATTACK_LOCAL_DIR)) \
-                                  and os.path.isdir(os.path.join(local_path, ICS_ATTACK_LOCAL_DIR)):
-            self.TC_ENTERPRISE_SOURCE = FileSystemSource(os.path.join(local_path, ENTERPRISE_ATTACK_LOCAL_DIR))
-            self.TC_PRE_SOURCE = FileSystemSource(os.path.join(local_path, PRE_ATTACK_LOCAL_DIR))
-            self.TC_MOBILE_SOURCE = FileSystemSource(os.path.join(local_path, MOBILE_ATTACK_LOCAL_DIR))
-            self.TC_ICS_SOURCE = FileSystemSource(os.path.join(local_path, ICS_ATTACK_LOCAL_DIR))
+            if not (self.TC_ENTERPRISE_SOURCE and self.TC_MOBILE_SOURCE and self.TC_ICS_SOURCE):
+                self.initialize_taxii_sources(proxies, verify)
         else:
-            ENTERPRISE_COLLECTION = Collection(ATTACK_STIX_COLLECTIONS + ENTERPRISE_ATTACK + "/", verify=verify, proxies=proxies)
-            PRE_COLLECTION = Collection(ATTACK_STIX_COLLECTIONS + PRE_ATTACK + "/", verify=verify, proxies=proxies)
-            MOBILE_COLLECTION = Collection(ATTACK_STIX_COLLECTIONS + MOBILE_ATTACK + "/", verify=verify, proxies=proxies)
-            ICS_COLLECTION = Collection(ATTACK_STIX_COLLECTIONS + ICS_ATTACK + "/", verify=verify, proxies=proxies)
-
-            self.TC_ENTERPRISE_SOURCE = TAXIICollectionSource(ENTERPRISE_COLLECTION)
-            self.TC_PRE_SOURCE = TAXIICollectionSource(PRE_COLLECTION)
-            self.TC_MOBILE_SOURCE = TAXIICollectionSource(MOBILE_COLLECTION)
-            self.TC_ICS_SOURCE = TAXIICollectionSource(ICS_COLLECTION)
+            self.initialize_taxii_sources(proxies, verify)
 
-        self.COMPOSITE_DS = CompositeDataSource()
         self.COMPOSITE_DS.add_data_sources([self.TC_ENTERPRISE_SOURCE, self.TC_MOBILE_SOURCE, self.TC_ICS_SOURCE])
 
-        if include_pre_attack:
-            self.COMPOSITE_DS.add_data_sources([self.TC_PRE_SOURCE])
+    def load_stix_store(self, path):
+        """
+        Loads a STIXStore from the given path.
+
+        Args:
+            path (str): Path to the source directory or JSON file.
+
+        Returns:
+            The loaded STIXStore or None if the path is invalid.
+        """
+        if path and os.path.exists(path):
+            store = STIXStore(path)
+            return store.get_store()
+        return None
+
+    def initialize_taxii_sources(self, proxies, verify):
+        """
+        Initializes data sources from the ATT&CK TAXII server.
+
+        Args:
+            proxies (dict, optional): Dictionary mapping protocol or protocol and hostname to the URL of the proxy.
+            verify (bool, optional): Whether to verify SSL certificates. Defaults to True.
+        """
+        ENTERPRISE_COLLECTION = Collection(ATTACK_STIX_COLLECTIONS + ENTERPRISE_ATTACK + "/", verify=verify, proxies=proxies)
+        MOBILE_COLLECTION = Collection(ATTACK_STIX_COLLECTIONS + MOBILE_ATTACK + "/", verify=verify, proxies=proxies)
+        ICS_COLLECTION = Collection(ATTACK_STIX_COLLECTIONS + ICS_ATTACK + "/", verify=verify, proxies=proxies)
+
+        self.TC_ENTERPRISE_SOURCE = TAXIICollectionSource(ENTERPRISE_COLLECTION)
+        self.TC_MOBILE_SOURCE = TAXIICollectionSource(MOBILE_COLLECTION)
+        self.TC_ICS_SOURCE = TAXIICollectionSource(ICS_COLLECTION)
     
     def get_stix_objects(
         self, 
         source: TAXIICollectionSource, 
         filter_objects: Dict[str, Union[Filter, callable]], 
         stix_format: bool = True
     ) -> Dict[str, List]:
```

### Comparing `attackcti-0.4.2/attackcti/models.py` & `attackcti-0.4.3/attackcti/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,8 +187,13 @@
 
     @model_validator(mode='before')
     def extract_phase_name(cls, values: Dict[str, Any]):
         if 'tactic' in values:
             kill_chain_phases = values['tactic']
             phase_names = [phase['phase_name'] for phase in kill_chain_phases if 'phase_name' in phase]
             values['tactic'] = phase_names
-        return values
+        return values
+
+class STIXLocalPaths(BaseModel):
+    enterprise: Optional[str] = Field(None, description="Path to the local enterprise-attack directory or JSON file.")
+    mobile: Optional[str] = Field(None, description="Path to the local mobile-attack directory or JSON file.")
+    ics: Optional[str] = Field(None, description="Path to the local ics-attack directory or JSON file.")
```

### Comparing `attackcti-0.4.2/attackcti.egg-info/PKG-INFO` & `attackcti-0.4.3/attackcti.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.4.2
+Version: 0.4.3
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
```

### Comparing `attackcti-0.4.2/setup.py` & `attackcti-0.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md')as f:
     long_description = f.read()
 
 setup(
     name="attackcti",
-    version="0.4.2",
+    version="0.4.3",
     author="Roberto Rodriguez",
     description="MITRE ATTACK CTI Python Libary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OTRF/ATTACK-Python-Client",
     project_urls={
         "Documentation": "https://attackcti.com",
```

