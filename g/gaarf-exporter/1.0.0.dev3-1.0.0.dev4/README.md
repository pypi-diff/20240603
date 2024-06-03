# Comparing `tmp/gaarf-exporter-1.0.0.dev3.tar.gz` & `tmp/gaarf-exporter-1.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaarf-exporter-1.0.0.dev3.tar", last modified: Wed May 15 07:02:24 2024, max compression
+gzip compressed data, was "gaarf-exporter-1.0.0.dev4.tar", last modified: Mon Jun  3 13:28:29 2024, max compression
```

## Comparing `gaarf-exporter-1.0.0.dev3.tar` & `gaarf-exporter-1.0.0.dev4.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6443 2024-03-26 12:03:46.000000 gaarf-exporter-1.0.0.dev3/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/gaarf_exporter/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1296 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/alert.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/alert_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2395 2024-05-02 16:45:02.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/bootstrap.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    19312 2024-05-15 06:57:25.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3424 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/disapprovals.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2410 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/mapping.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3290 2024-05-15 06:43:53.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/misc.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4622 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/performance.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     8242 2024-05-15 06:58:02.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/main.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6953 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/registry.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter/util.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-15 07:02:24.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      988 2024-05-15 07:02:24.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-05-15 07:02:24.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-05-15 07:02:24.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-05-15 07:02:24.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-05-15 07:02:24.000000 gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1848 2024-05-15 07:02:19.000000 gaarf-exporter-1.0.0.dev3/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:38:01.000000 gaarf-exporter-1.0.0.dev3/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/tests/end-to-end/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev3/tests/end-to-end/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3304 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/tests/end-to-end/test_gaarf_exporter.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 07:02:24.115006 gaarf-exporter-1.0.0.dev3/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev3/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev3/tests/unit/test_alerts.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    20199 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/tests/unit/test_collector.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev3/tests/unit/test_exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6501 2024-05-15 06:16:05.000000 gaarf-exporter-1.0.0.dev3/tests/unit/test_registry.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev3/tests/unit/test_util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6443 2024-03-26 12:03:46.000000 gaarf-exporter-1.0.0.dev4/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.206091 gaarf-exporter-1.0.0.dev4/gaarf_exporter/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2348 2024-05-28 14:49:58.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/_tmp.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1176 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/alert.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/alert_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2395 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/bootstrap.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    20404 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-15 12:59:56.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3455 2024-05-17 10:07:47.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/disapprovals.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2411 2024-05-17 10:16:42.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/mapping.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3290 2024-05-15 12:56:10.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/misc.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4622 2024-05-15 12:56:10.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/performance.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6844 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/main.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10229 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/registry.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-05-28 14:58:07.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter/util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-06-03 13:28:29.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1065 2024-06-03 13:28:29.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-06-03 13:28:29.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-06-03 13:28:29.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       61 2024-06-03 13:28:29.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-06-03 13:28:29.000000 gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1853 2024-06-03 13:27:52.000000 gaarf-exporter-1.0.0.dev4/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:38:01.000000 gaarf-exporter-1.0.0.dev4/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/tests/end-to-end/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev4/tests/end-to-end/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3935 2024-05-17 13:22:42.000000 gaarf-exporter-1.0.0.dev4/tests/end-to-end/test_gaarf_exporter.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev4/tests/unit/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-06-03 13:28:29.210091 gaarf-exporter-1.0.0.dev4/tests/unit/collector_definitions/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      410 2024-05-15 13:10:34.000000 gaarf-exporter-1.0.0.dev4/tests/unit/collector_definitions/test_collectors.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev4/tests/unit/test_alerts.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    22990 2024-05-15 19:13:48.000000 gaarf-exporter-1.0.0.dev4/tests/unit/test_collector.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev4/tests/unit/test_exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6659 2024-05-24 15:30:18.000000 gaarf-exporter-1.0.0.dev4/tests/unit/test_registry.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev4/tests/unit/test_util.py
```

### Comparing `gaarf-exporter-1.0.0.dev3/PKG-INFO` & `gaarf-exporter-1.0.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 1.0.0.dev3
+Version: 1.0.0.dev4
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gaarf-exporter-1.0.0.dev3/README.md` & `gaarf-exporter-1.0.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/alert.py` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/alert.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,28 +13,25 @@
 # limitations under the License.
 '''Module for building Prometheus alert.'''
 from __future__ import annotations
 
 import yaml
 
 from gaarf_exporter.alert_elements import AlertRule
-from gaarf_exporter.collector import Collector
 
 
 class Alert:
 
   def __init__(self,
                name: str,
                alert_rule: AlertRule,
                labels: str | None = None,
-               duration: str = '1h',
-               target: Collector | None = None) -> None:
+               duration: str = '1h') -> None:
     self.name = name
     self.alert_rule = str(alert_rule)
     self.labels = labels
     self.duration = duration
-    self.target = target
 
   @property
   def text(self) -> dict[str, str]:
     d = {'alert': self.name, 'expr': self.alert_rule, 'for': self.duration}
     return yaml.safe_dump(d)
```

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/alert_elements.py` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/alert_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/bootstrap.py` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector.py` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,97 +14,120 @@
 """Defines Collector class and corresponding helper methods.
 
 Collector serves an important roles of building Google Ads queries from set of
 diverse elements: metrics, dimensions, filters, resource names, etc.
 
 Collector can be:
   * similar (sharing the same metrics, dimensions and filters) which allows
-    to perform similar target deduplication with the lowest common level.
-  * equal (sharing the same attributes) - useful for checking target presence
+    to perform similar collector deduplication with the lowest common level.
+  * equal (sharing the same attributes) - useful for checking collector presence
     in the sets.
 
 Metrics, dimensions and filters of a Collector can be dynamically changed thus
 allowing Collector customization at the runtime.
 """
 from __future__ import annotations
 
+import copy
 import dataclasses
 import enum
+import itertools
 from collections.abc import Mapping
 from collections.abc import MutableSequence
 from collections.abc import Sequence
 from datetime import datetime
+from typing import TypedDict
 
 from gaarf.cli import utils as gaarf_utils
 
 from gaarf_exporter import util
 
 
+class QueryField(TypedDict):
+  field: str
+
+
+class QuerySpec(TypedDict):
+  level: str | None
+  metrics: list[str] | list[QueryField] | None
+  dimensions: list[QueryField] | None
+  resource_name: str | None
+  customizable: list[str] | None
+  filters: list[str] | None
+
+
+class CollectorDefinition(TypedDict):
+  name: str
+  type: str | dict[str, str] | None
+  query_spec: QuerySpec | None
+  query: str | None
+  has_conversion_split: str | None
+  registries: list[str]
+
+
+class CollectorCustomization(TypedDict):
+  start_date: str
+  end_date: str
+  level: str
+  metrics: list[str] | list[QueryField]
+  dimensions: list[str] | list[QueryField]
+  filters: list[str]
+
+
 class Field:
+  """Helper class for defining Google Ads API field.
+
+  Field can be a metric, dimension or segment.
+
+  Attributes:
+      name: Name of the field, i.e. metric.clicks.
+      alias: Optional alias for the field, i.e. clicks.
+  """
 
   def __init__(self, name: str, alias: str | None = None) -> None:
+    """Initializes Field.
+
+    Args:
+      name: Name of the field, i.e. metric.clicks.
+      alias: Optional alias for the field, i.e. clicks.
+    """
     self.name = name
     self.alias = alias or name.replace('.', '_')
 
   def to_query_field(self) -> str:
-    name = self.name
-
-    return f'{name} AS {self.alias}' if self.alias else name
+    """Converts Field to format 'name AS alias'."""
+    return f'{self.name} AS {self.alias}' if self.alias else self.name
 
   def __str__(self) -> str:
     return self.to_query_field()
 
   def __repr__(self) -> str:
     return f'Field(name={self.name}, alias={self.alias})'
 
-  def __eq__(self, other) -> bool:
+  def __eq__(self, other: Field) -> bool:
     if not other or not isinstance(other, Field):
       return False
     return util.remove_spaces(str(self)) == util.remove_spaces(str(other))
 
-  def __lt__(self, other) -> bool:
+  def __lt__(self, other: Field) -> bool:
     return util.remove_spaces(str(self)) < util.remove_spaces(str(other))
 
-  def __gt__(self, other) -> bool:
+  def __gt__(self, other: Field) -> bool:
     return util.remove_spaces(str(self)) > util.remove_spaces(str(other))
 
   def __hash__(self):
     return hash((util.remove_spaces(self.name),
                  util.remove_spaces(self.alias if self.alias else '')))
 
 
-_DEFAULT_METRICS = [
-    Field('clicks'),
-    Field('impressions'),
-    Field('conversions'),
-    Field('cost_micros / 1e6', 'cost')
-]
-
-_DEFAULT_CONVERSION_SPLIT_METRICS = [
-    Field('all_conversions'),
-    Field('all_conversions_value'),
-]
-
-_DEFAULT_CONVERSION_SPLIT_DIMENSIONS = [
-    Field('segments.conversion_action_category', 'conversion_category'),
-    Field('segments.conversion_action_name', 'conversion_name'),
-    Field('segments.conversion_action~0', 'conversion_id')
-]
-
-_DEFAULT_CONVERSION_SPLIT_FILTERS = [
-    'metrics.all_conversions > 0',
-    'segments.date DURING TODAY',
-]
-
-
 class CollectorLevel(enum.IntEnum):
   """Represents minimal level of entity.
 
   CollectorLevel regulates which entity id (ad_id, ad_group_id, campaign_id, etc.)
-  is associated with metrics and dimensions for a given target.
+  is associated with metrics and dimensions for a given collector.
   Collector levels are ordered hierarchically to support comparison operations.
   """
   UNKNOWN = 0
   AD_GROUP_AD_ASSET = 1
   AD_GROUP_AD = 2
   AD_GROUP = 3
   CAMPAIGN = 4
@@ -143,15 +166,15 @@
     return f'{self.id} AS {self.id_alias}'
 
   def to_field(self) -> Field:
     """Builds Field from level meta information."""
     return Field(name=self.id, alias=self.id_alias)
 
 
-LEVELS = {
+_LEVELS = {
     CollectorLevel.AD_GROUP_AD_ASSET:
         LevelInfo('ad_group_ad_asset_view', 'asset.id', 'asset_id',
                   'asset.name', 'asset',
                   'ad_group_ad_asset_view.enabled = TRUE'),
     CollectorLevel.AD_GROUP_AD:
         LevelInfo('ad_group_ad', 'ad_group_ad.ad.id', 'ad_id',
                   'ad_group_ad.ad.name', 'ad_name',
@@ -173,58 +196,70 @@
 }
 
 
 class Collector:
   """Represents collection of query elements needed to build a Google Ads query.
 
   Attributes:
-    name: Unique identifier of a target.
-    level: Minimal entity level in the target (ad_group, campaign, customer).
-    metrics: All metrics (started with `metrics.`) associated with the target.
-    dimensions: All segments and resources associated with the target.
+    name: Unique identifier of a collector.
+    level: Minimal entity level in the collector (ad_group, campaign, customer).
+    metrics: All metrics (started with `metrics.`) associated with the collector.
+    dimensions: All segments and resources associated with the collector.
     filters: Text conditions for limiting the query.
     resource_name: Name of resource to get data from (used in FROM statement).
     query: Full text of the query to be sent to Google Ads API.
-    suffix: Optional custom identifier to the target.
+    suffix: Optional custom identifier to the collector.
   """
 
   def __init__(self,
                name: str | None = None,
-               metrics: str | Sequence[Field] | None = None,
+               metrics: str | list[Field] | None = None,
                level: CollectorLevel | None = CollectorLevel.AD_GROUP,
                resource_name: str | None = None,
-               dimensions: str | Sequence[Field] | None = None,
-               filters: str | Sequence[str] | None = None,
+               dimensions: str | list[Field] | None = None,
+               filters: str | None = None,
                suffix: str | None = None,
                query: str | None = None) -> None:
     """Initializes Collector.
 
     Args:
-      name: Unique identifier of a target.
-      metrics: All metrics (started with `metrics.`) associated with the target.
-      level: Minimal entity level in the target (ad_group, campaign, customer).
+      name: Unique identifier of a collector.
+      metrics: All metrics (started with `metrics.`) associated with the collector.
+      level: Minimal entity level in the collector (ad_group, campaign, customer).
       resource_name: Name of resource to get data from (used in FROM statement).
-      dimensions: All segments and resources associated with the target.
+      dimensions: All segments and resources associated with the collector.
       filters: Text conditions for limiting the query.
-      suffix: Optional custom identifier to the target.
+      suffix: Optional custom identifier to the collector.
       query: Full query_text.
     """
     self.name = name
     self._level = level
     self._resource_name = resource_name
     self._filters = filters or set()
     self._metrics = self._init_fields(metrics, 'metrics')
     self._dimensions = self._init_fields(dimensions)
     self.suffix = suffix if suffix else name
     self._query = query
 
   @classmethod
-  def from_definition(cls, definition: dict) -> Collector:
+  def from_definition(cls, definition: CollectorDefinition) -> Collector:
+    """Creates Collector from a dictionary.
+
+    Args:
+      definition: Necessary data to create Collector.
+
+    Returns:
+      Initialized Collector.
+    """
+    if query := definition.get('query'):
+      return cls(
+          name=definition.get('name'),
+          query=query,
+          suffix=definition.get('suffix'))
     query_spec = definition.get('query_spec', {})
-    # query = definition.get('query')
     if definition.get('type') == 'service':
       metrics = [Field(name='1', alias='info')]
     elif service_alias := definition.get('type', {}).get('service'):
       metrics = [Field(name='1', alias=service_alias.get('alias'))]
     else:
       metrics = query_spec.get('metrics')
 
@@ -237,72 +272,85 @@
         suffix=definition.get('suffix'),
         metrics=metrics,
         dimensions=query_spec.get('dimensions'),
         filters=query_spec.get('filters'),
         resource_name=query_spec.get('resource_name'),
         level=level)
 
-  def create_conv_collector(self) -> Collector:
+  def create_conversion_split_collector(self) -> Collector:
+    """Builds new Collector with conversions metric and dimensions.
+
+    Returns:
+        New Collector on the same level as the seed one.
+    """
     return Collector(
         name=f'{self.name}_conversion_split',
         suffix=self.suffix,
         level=self.level,
-        metrics=_DEFAULT_CONVERSION_SPLIT_METRICS,
-        dimensions=_DEFAULT_CONVERSION_SPLIT_DIMENSIONS,
+        metrics='all_conversions,all_conversions_value',
+        dimensions=[
+            Field('segments.conversion_action_category', 'conversion_category'),
+            Field('segments.conversion_action_name', 'conversion_name'),
+            Field('segments.conversion_action~0', 'conversion_id')
+        ],
         resource_name=self.resource_name,
-        filters=_DEFAULT_CONVERSION_SPLIT_FILTERS)
+        filters='metrics.all_conversions > 0')
 
   @property
   def level(self) -> CollectorLevel | None:
-    """Represents entity level of a target."""
+    """Represents entity level of a collector."""
     return self._level
 
   @level.setter
   def level(self, value: CollectorLevel) -> None:
-    """Changes saved level of a target."""
+    """Changes saved level of a collector."""
     self._level = value
 
   @property
   def metrics(self) -> set[Field]:
     """Returns unique metrics."""
     return set(self._metrics)
 
   @metrics.setter
   def metrics(self, values: Sequence[Field]) -> None:
-    """Changes saved metrics of a target."""
+    """Changes saved metrics of a collector."""
     self._metrics = set(values)
 
   @property
   def dimensions(self) -> set[Field]:
     """Returns unique metrics."""
     return set(self._dimensions)
 
   @dimensions.setter
   def dimensions(self, values: Sequence[Field]) -> None:
-    """Changes saved dimensions of a target."""
+    """Changes saved dimensions of a collector."""
     self._dimensions = values
 
   @property
-  def filters(self) -> set[str]:
-    """Returns filters or default placeholder."""
+  def filters(self) -> str:
+    """Returns filters or default placeholder.
+
+    If collector has any metric inject a placeholder filter to fetch data
+    only for today.
+    """
     if isinstance(self._filters, str):
       self._filters = set(self._filters.split(' AND '))
     else:
       self._filters = set(self._filters)
     if isinstance(self, ServiceCollector) or not self._metrics:
       return self._filters
     if not self._filters:
       self._filters.add('segments.date DURING TODAY')
     elif not any('segments.date' in _filter for _filter in self._filters):
       self._filters.add('segments.date DURING TODAY')
     return self._filters
 
   @filters.setter
   def filters(self, values: str) -> None:
-    """Changes saved dimensions of a target."""
+    """Changes saved dimensions of a collector."""
     self._filters = values
 
   def _init_fields(self,
                    fields: str | list[Field],
                    prefix: str = '') -> list[Field]:
     """Transforms fields to proper Field format based on optional prefix.
 
@@ -354,92 +402,103 @@
 
       field.name = ' '.join(processed_tokens)
 
     return field_list
 
   @property
   def level_info(self) -> LevelInfo | None:
-    """Returns meta information related to a target level."""
-    return LEVELS.get(self.level)
+    """Returns meta information related to a collector level."""
+    return _LEVELS.get(self.level)
 
   @property
-  def _formatted_level(self) -> str:
+  def formatted_level(self) -> str:
     """Returns formatted level as field name with alias."""
     if level_info := self.level_info:
       return f'{level_info.to_query_field()},\n'
     return ''
 
   @property
-  def _formatted_metrics(self) -> str:
+  def formatted_metrics(self) -> str:
     """Returns formatted metrics as field names with aliases."""
     if not self.metrics:
       return '\n'
     metrics_info = ',\n'.join(
         [field.to_query_field() for field in sorted(self.metrics)])
     return f'{metrics_info},\n'
 
   @property
-  def _formatted_dimensions(self) -> str:
+  def formatted_dimensions(self) -> str:
     """Returns formatted metrics as field names with aliases."""
     if not (dimensions := self.dimensions):
       return '\n'
     if level_info := self.level_info:
       dimensions = set(dimensions).difference(set([level_info.to_field()]))
     if not dimensions:
       return '\n'
     dimensions_info = ',\n'.join(
         [field.to_query_field() for field in sorted(dimensions)])
     return f'{dimensions_info},\n'
 
   @property
-  def _formatted_filters(self) -> str:
+  def formatted_filters(self) -> str:
+    """Returns formatted filters with WHERE statement."""
     if not self.filters:
       return ''
     filters = ' AND '.join(self.filters)
     return f'WHERE {filters}'
 
   @property
   def resource_name(self) -> str:
-    """Gets resource_name or infers it from target level."""
+    """Gets resource_name or infers it from collector level."""
     if self._resource_name:
       return self._resource_name
     if level_info := self.level_info:
       return level_info.resource_name.lower()
     return self.level.name
 
   @property
   def query(self) -> str:
     """Formats query based on elements."""
     if self._query:
       return self._query
-    return (f'SELECT {self._formatted_level}{self._formatted_metrics}'
-            f'{self._formatted_dimensions}'
+    return (f'SELECT {self.formatted_level}{self.formatted_metrics}'
+            f'{self.formatted_dimensions}'
             f'FROM {self.resource_name}\n'
-            f'{self._formatted_filters}')
+            f'{self.formatted_filters}')
+
+  def customize(self, collector_customization: CollectorCustomization) -> None:
+    """Customizes collector elements based on provided customization mapping.
+
+    Based on provided collector_customization mapping this method changes
+    elements of Customizer instance (metrics, level, dimensions, filters).
 
-  def customize(self, kwargs: dict[str, str]) -> None:
-    if level := kwargs.get('level'):
+    Args:
+      collector_customization:
+        Provides mapping between names of customized parameter and its updated
+        values.
+    """
+    if level := collector_customization.get('level'):
       self.level = CollectorLevel[level.upper()]
-    if (start_date := kwargs.get('start_date')) and (end_date :=
-                                                     kwargs.get('end_date')):
+    if (start_date := collector_customization.get('start_date')) and (
+        end_date := collector_customization.get('end_date')):
       start_date = gaarf_utils.convert_date(start_date)
       end_date = gaarf_utils.convert_date(end_date)
       if not self.filters or 'segments.date DURING TODAY' in self.filters:
         self.filters.remove('segments.date DURING TODAY')
         self.filters.add(
             f"segments.date BETWEEN '{start_date}' AND '{end_date}'")
       n_days = (datetime.strptime(end_date, '%Y-%m-%d') -
                 datetime.strptime(start_date, '%Y-%m-%d')).days + 1
       self.dimensions.add(Field(str(n_days), 'n_days'))
 
   def is_similar(self, other: Collector) -> bool:
     """Compares similarity between two collectors.
 
     Similarity first checks whether two collectors are coming from different
-    non CollectorLevel specific resource_names, if they are different then
+    non CollectorLevel specific resouce_names, if they are different then
     collectors are not similar.
     Then is compares all  metrics, dimensions and filters between two collectors.
 
     Returns:
       Whether two collectors are similar.
     """
     if not other or not isinstance(other, Collector):
@@ -449,119 +508,102 @@
         not (CollectorLevel.contains(self.resource_name, other.resource_name))):
       return False
     if (self.metrics, self.dimensions,
         self.filters) == (other.metrics, other.dimensions, other.filters):
       return True
     return False
 
-  def generate_service_collector(self) -> ServiceCollector | None:
-    """Generates correct ServiceCollector based on provided level.
-
-     Based on level (AD_GROUP, CAMPAIGN, ACCOUNT, etc.) corresponding
-     ServiceCollector is created that contains all necessary mapping information
-     downstream. I.e. if 'level=AD_GROUP' then information on ad_group, campaign
-     and customer will be included in to the mapping.
-
-     Returns:
-      ServiceCollector called 'mapping' for an appropriate level.
-
-    """
-    if isinstance(self, ServiceCollector):
-      return None
-    if self.level == CollectorLevel.MCC:
-      level = CollectorLevel.CUSTOMER
-    else:
-      level = self.level
-    dimensions = []
-    filters = ''
-
-    for target_level in CollectorLevel:
-      if (target_level
-          not in (CollectorLevel.MCC, CollectorLevel.AD_GROUP_AD_ASSET) and
-          self.level <= target_level and
-          (level_info := LEVELS.get(target_level))):
-        dimensions.extend([
-            Field(name=level_info.id, alias=level_info.id_alias),
-            Field(name=level_info.name, alias=level_info.name_alias),
-        ])
-        if filters:
-          filters = filters + ' AND ' + level_info.active_entities_filter
-        else:
-          filters = level_info.active_entities_filter
-
-    return ServiceCollector(
-        name='mapping', dimensions=dimensions, level=level, filters=filters)
-
   def __eq__(self, other: Collector) -> bool:
-    """Compares two targets based on similarity, resource_name and level."""
+    """Compares two collectors based on similarity, resource_name and level."""
     if not self.is_similar(other):
       return False
     if self.level != other.level:
       return False
     return True
 
   def __lt__(self, other: Collector) -> bool:
-    """Compares targets by level values."""
+    """Compares collectors by level values."""
     if self.level.value < other.level.value:
       return True
     return False
 
   def __gt__(self, other: Collector) -> bool:
-    """Compares targets by level values."""
+    """Compares collectors by level values."""
     if self.level.value > other.level.value:
       return True
     return False
 
   def __hash__(self):
     return hash(self.query)
 
-  def __repr__(self) -> str:
-    return f'Collector(name="{self.name}")'
-
 
 class ServiceCollector(Collector):
-  """Helper class for targets without metrics."""
+  """Helper class for collectors without metrics."""
 
   @property
   def metrics(self) -> set[Field]:
     """Returns default info metric."""
     return set(self._metrics) or {
         Field(name='1', alias='info'),
     }
 
   @metrics.setter
   def metrics(self, value: Field) -> None:
     """Ensures that metrics cannot be overwritten."""
     raise ValueError('Cannot change value of "metrics"!')
 
 
-def create_default_service_collector(
-    level: CollectorLevel) -> ServiceCollector | None:
+def create_default_service_collector(level: CollectorLevel) -> ServiceCollector:
   """Generates correct ServiceCollector based on provided level.
 
    Based on level (AD_GROUP, CAMPAIGN, ACCOUNT, etc.) corresponding
    ServiceCollector is created that contains all necessary mapping information
    downstream. I.e. if 'level=AD_GROUP' then information on ad_group, campaign
    and customer will be included in to the mapping.
 
    Returns:
     ServiceCollector called 'mapping' for an appropriate level.
 
   """
   if level == CollectorLevel.MCC:
     level = CollectorLevel.CUSTOMER
-  dimensions = set()
-  filters = set()
+  dimensions = []
+  filters = ''
 
   for collector_level in CollectorLevel:
     if (collector_level
         not in (CollectorLevel.MCC, CollectorLevel.AD_GROUP_AD_ASSET) and
         level <= collector_level and
-        (level_info := LEVELS.get(collector_level))):
-      dimensions.update([
+        (level_info := _LEVELS.get(collector_level))):
+      dimensions.extend([
           Field(name=level_info.id, alias=level_info.id_alias),
-          Field(name=level_info.name, alias=level_info.name_alias)
+          Field(name=level_info.name, alias=level_info.name_alias),
       ])
-      filters.add(level_info.active_entities_filter)
+      if filters:
+        filters = filters + ' AND ' + level_info.active_entities_filter
+      else:
+        filters = level_info.active_entities_filter
 
   return ServiceCollector(
       name='mapping', dimensions=dimensions, level=level, filters=filters)
+
+
+def collectors_similarity_check(collectors: list[Collector]) -> list[Collector]:
+  """Dedupicates collectors.
+
+  If there are similar collector in the list return only those with the lowest
+  level.
+
+  Args:
+    collectors: Possible collector values.
+
+  Returns:
+    Deduplicated collectors.
+  """
+  cloned_collectors = copy.deepcopy(collectors)
+  combinations = itertools.combinations(collectors, 2)
+  for collector1, collector2 in combinations:
+    if collector1.is_similar(collector2):
+      max_collector = max(collector1, collector2)
+      if max_collector in cloned_collectors:
+        cloned_collectors.remove(max_collector)
+  return cloned_collectors
```

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/disapprovals.yaml` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/disapprovals.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     - disapprovals
 
 - name: sitelink_disapprovals
   query_spec:
     customizable:
       - filters
       - level
-    level: unknown
+    level: customer
     resource_name: asset
     dimensions:
       - asset_id:
           field: asset.id
       - sitelink_title:
           field: asset.sitelink_asset.link_text
       - sitelink_description1:
@@ -91,21 +91,23 @@
   query_spec:
     customizable:
       - dimensions
     level: unknown
     resource_name: asset_group_asset
     dimensions:
       - asset_group_id:
-          field: asset_group_asset.asset_group~0
+          field: asset_group.id
       - asset_id:
-          field: asset_group_asset.asset~0
+          field: asset.id
+      - asset_type:
+          field: asset_group_asset.field_type
       - approval_status:
           field: asset_group_asset.policy_summary.approval_status
       - review_status:
-          field: asset_group_asset.policy_summary.approval_status
+          field: asset_group_asset.policy_summary.review_status
       - topic_type:
           field: asset_group_asset.policy_summary.policy_topic_entries:type
       - topic:
           field: asset_group_asset.policy_summary.policy_topic_entries:topic
       - asset_count:
           field: '1'
     filters:
```

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/mapping.yaml` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/mapping.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
       - 'campaign.advertising_channel_type = MULTI_CHANNEL'
   registries:
     - app
 
 - name: app_asset_mapping
   type: service
   query_spec:
-    level: unknown
+    level: customer
     resource_name: asset
     dimensions:
       - asset_id:
           field: asset.id
       - asset_type:
           field: asset.type
       - asset_source:
```

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/misc.yaml` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/misc.yaml`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/collector_definitions/performance.yaml` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/collector_definitions/performance.yaml`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/exporter.py` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/main.py` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,32 +21,27 @@
 import argparse
 import logging
 from concurrent import futures
 from time import sleep
 from time import time
 
 import prometheus_client
-import smart_open
-import yaml
 from gaarf.cli import utils as gaarf_utils
 
 from gaarf_exporter import bootstrap
 from gaarf_exporter import exporter
 from gaarf_exporter import registry
-from gaarf_exporter import util
 
 
 def main() -> None:
   parser = argparse.ArgumentParser()
   parser.add_argument('--account', dest='account', default=None)
   parser.add_argument('-c', dest='config', default=None)
   parser.add_argument('--ads-config', dest='ads_config', default=None)
   parser.add_argument('--api-version', dest='api_version', default=None)
-  parser.add_argument('--queries.exclude', dest='exclude_queries', default=None)
-  parser.add_argument('--queries.include', dest='include_queries', default=None)
   parser.add_argument('--log', '--loglevel', dest='loglevel', default='info')
   parser.add_argument(
       '--http_server.address', dest='address', default='0.0.0.0')
   parser.add_argument('--http_server.port', dest='port', type=int, default=8000)
   parser.add_argument(
       '--pushgateway.address', dest='pushgateway_address', default=None)
   parser.add_argument(
@@ -60,51 +55,41 @@
       type=int)
   parser.add_argument('--delay-minutes', dest='delay', type=int, default=15)
   parser.add_argument(
       '--expose-metrics-with-zero-values',
       dest='zero_value_metrics',
       action='store_true')
   parser.add_argument('--namespace', dest='namespace', default='googleads')
+  parser.add_argument('--max-parallel', dest='parallel', default=None)
   parser.add_argument('--collectors', dest='collectors', default='default')
+  parser.add_argument(
+      '--no-deduplicate-collectors', dest='deduplicate', action='store_false')
+  parser.add_argument(
+      '--no-service-collectors',
+      dest='service_collectors',
+      action='store_false')
+  parser.set_defaults(deduplicate=True)
+  parser.set_defaults(service_collectors=True)
   args_bag = parser.parse_known_args()
   args = args_bag[0]
 
   logger = gaarf_utils.init_logging(
       loglevel=args.loglevel.upper(), logger_type=args.logger)
 
   params = gaarf_utils.ParamsParser([
       'macro',
       'sql',
       'template',
   ]).parse(args_bag[1])
-  collectors_registry = registry.Registry.from_collector_definitions()
-  macros = params.get('macro', {})
-  if config_file := args.config:
-    with smart_open.open(config_file, encoding='utf-8') as f:
-      config = yaml.safe_load(f)
-      queries = config.get('queries')
-  else:
-    if not (active_collectors := collectors_registry.find_collectors(
-        args.collectors)):
-      logger.warning('Failed to get "%s" collectors, using default ones',
-                     args.collectors)
-      active_collectors = collectors_registry.default_collectors
-    if macros:
-      active_collectors.customize(macros)
-  for collector in active_collectors:
-    if relative_metrics := util.find_relative_metrics(collector.query):
-      logger.warning(
-          'In query %s, relative metrics: [%s] are found, which might '
-          'not be useful.', collector.name, ', '.join(relative_metrics))
-  runtime_options = {
-      'exclude_queries':
-          args.exclude_queries.split(',') if args.exclude_queries else None,
-      'include_queries':
-          args.include_queries.split(',') if args.include_queries else None,
-  }
+
+  active_collectors = registry.initialize_collectors(
+      config_file=args.config,
+      collector_names=args.collectors,
+      create_service_collectors=args.service_collectors,
+      deduplicate_collectors=args.deduplicate)
 
   dependencies = bootstrap.inject_dependencies(
       ads_config_path=args.ads_config,
       api_version=args.api_version,
       account=args.account)
   report_fetcher, accounts = dependencies.get(
       'report_fetcher'), dependencies.get('accounts')
@@ -132,46 +117,33 @@
   while True:
     if iterations_left := args.iterations_left:
       iterations_left -= 1
     if accounts and iterations_left == 0:
       accounts = report_fetcher.expand_mcc(args.account)
       iterations_left = args.iterations_left
     start_export_time = time()
-    if not args.config:
-      if macros:
-        active_collectors.customize(macros)
+    if not args.config and params:
+      active_collectors.customize(params)
     for collector in active_collectors:
       if not (query_text := collector.query):
         raise ValueError(f'Missing query text for query "{collector.name}"')
-      if include_queries := runtime_options.get('include_queries'):
-        if collector.name not in include_queries:
-          continue
-      if exclude_queries := runtime_options.get('exclude_queries'):
-        if collector.name in exclude_queries:
-          continue
       logger.info('Beginning export')
       if not accounts:
-        logging.info('Starting fake export for query "[%s]"', collector.name)
         report = report_fetcher.fetch(query_text, accounts)
-        logging.info('Ending export for query "[%s]"', collector.name)
       else:
-        with futures.ThreadPoolExecutor() as executor:
+        with futures.ThreadPoolExecutor(max_workers=args.parallel) as executor:
           future_to_account = {
               executor.submit(report_fetcher.fetch, collector.query, account):
                   account for account in accounts
           }
           for future in futures.as_completed(future_to_account):
             account = future_to_account[future]
-            logging.info('Started fetching for query "[%s]" for account "[%s]"',
-                         collector.name, account)
             start = time()
             report = future.result()
             end = time()
-            logging.info('Ended fetching for query "[%s]" for account "[%s]"',
-                         collector.name, account)
             gaarf_exporter.report_fetcher_gauge.labels(
                 collector=collector.name, account=account).set(end - start)
             if dependencies.get('convert_fake_report'):
               report.is_fake = False
             logging.info('Started export for query "[%s]" for account "[%s]"',
                          collector.name, account)
             gaarf_exporter.export(
```

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter/util.py` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter/util.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/PKG-INFO` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 1.0.0.dev3
+Version: 1.0.0.dev4
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gaarf-exporter-1.0.0.dev3/gaarf_exporter.egg-info/SOURCES.txt` & `gaarf-exporter-1.0.0.dev4/gaarf_exporter.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 gaarf_exporter/__init__.py
+gaarf_exporter/_tmp.py
 gaarf_exporter/alert.py
 gaarf_exporter/alert_elements.py
 gaarf_exporter/bootstrap.py
 gaarf_exporter/collector.py
 gaarf_exporter/exporter.py
 gaarf_exporter/main.py
 gaarf_exporter/registry.py
@@ -24,8 +25,9 @@
 tests/end-to-end/__init__.py
 tests/end-to-end/test_gaarf_exporter.py
 tests/unit/__init__.py
 tests/unit/test_alerts.py
 tests/unit/test_collector.py
 tests/unit/test_exporter.py
 tests/unit/test_registry.py
-tests/unit/test_util.py
+tests/unit/test_util.py
+tests/unit/collector_definitions/test_collectors.yaml
```

### Comparing `gaarf-exporter-1.0.0.dev3/setup.py` & `gaarf-exporter-1.0.0.dev4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / 'README.md').read_text()
 
 setup(
   name='gaarf-exporter',
-  version='1.0.0.dev3',
+  version='1.0.0.dev4',
   long_description=README,
   long_description_content_type='text/markdown',
   author='Google Inc. (gTech gPS CSE team)',
   author_email='no-reply@google.com',
   license='Apache 2.0',
   classifiers=[
     'Programming Language :: Python :: 3 :: Only',
@@ -40,14 +40,14 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: Apache Software License'
   ],
   packages=find_packages(),
   package_data={'': ['collector_definitions/*.yaml']},
   install_requires=[
-    'prometheus-client', 'google-ads-api-report-fetcher==1.13.4'
+    'prometheus-client', 'google-ads-api-report-fetcher==1.14.0.dev6'
   ],
   setup_requires=['pytest-runner'],
   tests_requires=['pytest'],
   entry_points={
     'console_scripts': ['gaarf-exporter=gaarf_exporter.main:main',]
   })
```

### Comparing `gaarf-exporter-1.0.0.dev3/tests/end-to-end/test_gaarf_exporter.py` & `gaarf-exporter-1.0.0.dev4/tests/end-to-end/test_gaarf_exporter.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
+import pathlib
 import random
 import subprocess
 
 import pytest
 
 from gaarf_exporter import registry
 
+_SCRIPT_DIR = pathlib.Path(__file__).parent
 _START_PORT = 30000
 _END_PORT = 60000
 collectors_registry = registry.Registry.from_collector_definitions()
 
 
 def _generate_collector_port_pairs(property_name: str,
                                    start_port: int = _START_PORT
@@ -94,10 +96,29 @@
       '--delay=0',
       '--api-version=16',
   ],
                           capture_output=True,
                           text=True)
   out = result.stdout
   assert not result.stderr
+  assert 'Started http_server at http://0.0.0.0:8000' in out
+  assert 'Beginning export' in out
+  assert 'Export completed' in out
+
+
+@pytest.mark.e2e
+def test_gaarf_exporter_run_selected_collectors_from_config_file():
+  result = subprocess.run([
+      'gaarf-exporter',
+      '--expose-metrics-with-zero-values',
+      '--iterations=1',
+      f'-c={_SCRIPT_DIR}/test_gaarf_exporter.yaml',
+      '--delay=0',
+      '--api-version=16',
+  ],
+                          capture_output=True,
+                          text=True)
+  out = result.stdout
+  assert not result.stderr
   assert 'Started http_server at http://0.0.0.0:8000' in out
   assert 'Beginning export' in out
   assert 'Export completed' in out
```

### Comparing `gaarf-exporter-1.0.0.dev3/tests/unit/test_alerts.py` & `gaarf-exporter-1.0.0.dev4/tests/unit/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/tests/unit/test_collector.py` & `gaarf-exporter-1.0.0.dev4/tests/unit/test_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,61 @@
     print(sorted_expected_sql_tokens)
 
   assert sorted_actual_sql_tokens == sorted_expected_sql_tokens
 
 
 class TestCollector:
 
+  def test_from_definition_with_query_spec_creates_correct_collector(self):
+    collector_definition = {
+        'name': 'test',
+        'query_spec': {
+            'level': 'ad_group',
+            'metrics': ['clicks']
+        }
+    }
+    collector = query_collector.Collector.from_definition(collector_definition)
+    expected_collector = query_collector.Collector(
+        name='test',
+        metrics='clicks',
+        level=query_collector.CollectorLevel.AD_GROUP)
+    assert collector == expected_collector
+
+  def test_from_definition_with_query_creates_correct_collector(self):
+    collector_definition = {
+        'name': 'test',
+        'query': 'SELECT campaign.id FROM campaign',
+    }
+    collector = query_collector.Collector.from_definition(collector_definition)
+    expected_collector = query_collector.Collector(
+        name='test', query='SELECT campaign.id FROM campaign')
+    assert collector.query == expected_collector.query
+
+  def test_create_conversion_split_collector_returns_correct_collector(self):
+    test_collector = query_collector.Collector(
+        name='test',
+        metrics='clicks',
+        level=query_collector.CollectorLevel.AD_GROUP)
+    conv_split_collector = test_collector.create_conversion_split_collector()
+    expected_collector = query_collector.Collector(
+        name='test_conversion_split',
+        metrics='all_conversions,all_conversions_value',
+        level=test_collector.level,
+        dimensions=[
+            query_collector.Field('segments.conversion_action_category',
+                                  'conversion_category'),
+            query_collector.Field('segments.conversion_action_name',
+                                  'conversion_name'),
+            query_collector.Field('segments.conversion_action~0',
+                                  'conversion_id')
+        ],
+        resource_name=test_collector.resource_name,
+        filters='metrics.all_conversions > 0')
+    assert conv_split_collector == expected_collector
+
   class TestCollectorQuery:
 
     def test_simple_collector_creates_correct_query(self):
       collector = query_collector.Collector(
           name='simple',
           metrics='impressions',
           level=query_collector.CollectorLevel.AD_GROUP)
@@ -55,21 +102,19 @@
         FROM ad_group
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(collector.query, expected_sql)
 
     def test_complex_collector_creates_correct_query(self):
       collector = query_collector.Collector(
-          name='complex',
           metrics='impressions,clicks',
           level=query_collector.CollectorLevel.AD_GROUP,
           dimensions=[
               query_collector.Field(
-                  name='segments.conversion_action~0',
-                  alias='conversion_id'),
+                  name='segments.conversion_action~0', alias='conversion_id'),
               query_collector.Field(
                   name='search_terms_view.search_term', alias='search_term')
           ])
       expected_sql = """
         SELECT
             ad_group.id AS ad_group_id,
             metrics.impressions AS impressions,
@@ -79,28 +124,26 @@
         FROM ad_group
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(collector.query, expected_sql)
 
     def test_complex_collector_with_virtual_column_creates_correct_query(self):
       collector = query_collector.Collector(
-          name='complex',
           metrics=[
               query_collector.Field(name='impressions'),
               query_collector.Field(name='clicks'),
               query_collector.Field(name='cost_micros * 1e6', alias='cost'),
               query_collector.Field(name='clicks / impressions', alias='ctr'),
               query_collector.Field(
                   name='var1-var2/(1.05e3+var3)*100.5', alias='vc')
           ],
           level=query_collector.CollectorLevel.AD_GROUP,
           dimensions=[
               query_collector.Field(
-                  name='segments.conversion_action~0',
-                  alias='conversion_id'),
+                  name='segments.conversion_action~0', alias='conversion_id'),
               query_collector.Field(
                   name='search_terms_view.search_term', alias='search_term')
           ])
       expected_sql = """
         SELECT
             ad_group.id AS ad_group_id,
             metrics.impressions AS impressions,
@@ -117,17 +160,19 @@
       assert_sql_functionally_equivalent(collector.query, expected_sql)
 
     def test_service_collector_creates_correct_query(self):
       collector = query_collector.ServiceCollector(
           name='mapping',
           dimensions=[
               query_collector.Field(name='ad_group.id', alias='ad_group_id'),
-              query_collector.Field(name='ad_group.name', alias='ad_group_name'),
+              query_collector.Field(
+                  name='ad_group.name', alias='ad_group_name'),
               query_collector.Field(name='campaign.id', alias='campaign_id'),
-              query_collector.Field(name='campaign.name', alias='campaign_name'),
+              query_collector.Field(
+                  name='campaign.name', alias='campaign_name'),
               query_collector.Field(name='customer.id', alias='customer_id'),
               query_collector.Field(
                   name='customer.descriptive_name', alias='account_name'),
           ],
           filters=('ad_group.status = ENABLED'
                    ' AND campaign.status = ENABLED'
                    ' AND customer.status = ENABLED'))
@@ -216,15 +261,15 @@
     def test_collector_with_nested_fieds_names_creates_correct_query(self):
       collector = query_collector.Collector(
           name='bid_budget',
           metrics=[
               query_collector.Field('impressions'),
               query_collector.Field('campaign_budget.amount_micros', 'budget'),
               query_collector.Field('campaign.target_cpa.target_cpa_micros',
-                                   'target_cpa'),
+                                    'target_cpa'),
           ],
           level=query_collector.CollectorLevel.CAMPAIGN)
       expected_sql = """
         SELECT
             campaign.id AS campaign_id,
             metrics.impressions AS impressions,
             campaign_budget.amount_micros AS budget,
@@ -236,18 +281,19 @@
 
     def test_collector_with_empty_metrics_creates_correct_query(self):
       collector = query_collector.Collector(
           name='disapproval',
           level=query_collector.CollectorLevel.AD_GROUP_AD,
           dimensions=[
               query_collector.Field('campaign.id', 'campaign_id'),
-              query_collector.Field('ad_group_ad.policy_summary.approval_status',
-                                   'approval_status'),
+              query_collector.Field(
+                  'ad_group_ad.policy_summary.approval_status',
+                  'approval_status'),
               query_collector.Field('ad_group_ad.policy_summary.review_status',
-                                   'review_status')
+                                    'review_status')
           ],
           filters=(
               'campaign.status = ENABLED'
               ' AND ad_group.status = ENABLED'
               ' AND ad_group_ad.status = ENABLED'
               ' AND ad_group_ad.policy_summary.approval_status != APPROVED'))
       expected_sql = """
@@ -322,15 +368,16 @@
                     customer.descriptive_name AS account_name,
                 FROM customer
                 WHERE customer.status = ENABLED
             """),
     ])
     def test_create_default_service_collector_returns_correct_service_collector_query_for_level(  # pylint: disable=line-too-long
         self, test_level, expected_sql):
-      actual_collector = query_collector.create_default_service_collector(test_level)
+      actual_collector = query_collector.create_default_service_collector(
+          test_level)
       assert_sql_functionally_equivalent(actual_collector.query, expected_sql)
 
   class TestCollectorProperties:
 
     def test_metrics_returns_correct_fields(self):
       collector = query_collector.Collector(metrics='clicks')
       assert collector.metrics == {
@@ -340,34 +387,31 @@
     def test_dimensions_returns_correct_fields(self):
       collector = query_collector.Collector(dimensions='segments.date')
       assert collector.dimensions == {
           query_collector.Field(name='segments.date', alias=None),
       }
 
     @pytest.mark.parametrize('filters,expected_filter', [
-        ('segments.date DURING YESTERDAY', {
-            'segments.date DURING YESTERDAY',
-        }),
-        (None, {
-            'segments.date DURING TODAY',
-        }),
+        ('segments.date DURING YESTERDAY',
+         'WHERE segments.date DURING YESTERDAY'),
+        (None, 'WHERE segments.date DURING TODAY'),
     ])
     def test_filters_returns_correct_expression(self, filters, expected_filter):
-      collector = query_collector.Collector(
-          name='test', metrics='clicks', filters=filters)
+      collector = query_collector.Collector(metrics='clicks', filters=filters)
 
-      assert collector.filters == expected_filter
+      assert collector.formatted_filters == expected_filter
 
     def test_resource_name_returns_correct_expression_for_explicit_resource_name(
         self):
       resource_name = 'search_term_view'
       level = query_collector.CollectorLevel.AD_GROUP
       expected_resource_name = 'search_term_view'
 
-      collector = query_collector.Collector(level=level, resource_name=resource_name)
+      collector = query_collector.Collector(
+          level=level, resource_name=resource_name)
 
       assert collector.resource_name == expected_resource_name
 
     def test_resource_name_returns_correct_expression_for_missing_resource_name(
         self):
       level = query_collector.CollectorLevel.CAMPAIGN
       expected_resource_name = 'campaign'
@@ -390,49 +434,43 @@
       collector1 = query_collector.Collector(
           name='collector1', metrics='clicks,conversions')
       collector2 = query_collector.Collector(
           name='collector2', metrics='clicks,conversions')
 
       assert collector1 == collector2
 
-    def test_collectors_with_different_metrics_and_dimensions_are_not_equal(self):
+    def test_collectors_with_different_metrics_and_dimensions_are_not_equal(
+        self):
       collector1 = query_collector.Collector(
           name='collector1', metrics='clicks,conversions')
       collector2 = query_collector.Collector(
           name='collector2', dimensions='clicks,conversions')
 
       assert collector1 != collector2
 
     def test_collectors_with_same_metrics_but_different_instantiations_are_equal(
         self):
-      collector1 = query_collector.Collector(
-          name='test', metrics='clicks,conversions')
-      collector2 = query_collector.Collector(
-          name='test',
-          metrics=[
-              query_collector.Field(name='clicks'),
-              query_collector.Field(name='conversions'),
-          ])
+      collector1 = query_collector.Collector(metrics='clicks,conversions')
+      collector2 = query_collector.Collector(metrics=[
+          query_collector.Field(name='clicks'),
+          query_collector.Field(name='conversions'),
+      ])
 
       assert collector1 == collector2
 
     def test_collectors_with_different_order_of_metrics_are_equal(self):
-      collector1 = query_collector.Collector(
-          name='test',
-          metrics=[
-              query_collector.Field(name='conversions'),
-              query_collector.Field(name='impressions', alias='imp'),
-          ])
+      collector1 = query_collector.Collector(metrics=[
+          query_collector.Field(name='conversions'),
+          query_collector.Field(name='impressions', alias='imp'),
+      ])
       collector2 = query_collector.Collector(
-          name='test',
           metrics=[
               query_collector.Field(name='impressions', alias='imp'),
               query_collector.Field(name='conversions')
-          ],
-      )
+          ],)
 
       assert collector1 == collector2
 
   class TestCollectorSimilarity:
 
     def test_collectors_with_same_metrics_and_dimensions_are_similar(self):
       collector1 = query_collector.Collector(
@@ -504,7 +542,33 @@
           name='collector2',
           metrics='clicks,conversions',
           dimensions='segments.date',
           resource_name='gender_view',
           filters='segments.date DURING TODAY',
           level=query_collector.CollectorLevel.AD_GROUP_AD)
       assert not collector1.is_similar(collector2)
+
+
+@pytest.mark.parametrize('collectors,expected', [
+    ([
+        query_collector.Collector(
+            name='collector1',
+            metrics='clicks,conversions',
+            level=query_collector.CollectorLevel.CUSTOMER),
+        query_collector.Collector(
+            name='collector2',
+            metrics='clicks,conversions',
+            level=query_collector.CollectorLevel.AD_GROUP),
+        query_collector.Collector(
+            name='collector3',
+            metrics='clicks,conversions',
+            level=query_collector.CollectorLevel.AD_GROUP_AD),
+        query_collector.Collector(
+            name='collector4',
+            metrics='clicks,conversions,impressions',
+            level=query_collector.CollectorLevel.MCC)
+    ], ['collector3', 'collector4']),
+])
+def test_collectors_similarity_check_returns_deduplicated_collectors(
+    collectors, expected):
+  actual = query_collector.collectors_similarity_check(collectors)
+  assert set([t.name for t in actual]) == set(expected)
```

### Comparing `gaarf-exporter-1.0.0.dev3/tests/unit/test_exporter.py` & `gaarf-exporter-1.0.0.dev4/tests/unit/test_exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev3/tests/unit/test_registry.py` & `gaarf-exporter-1.0.0.dev4/tests/unit/test_registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import pytest
+import yaml
 
 from gaarf_exporter import collector as query_collector
 from gaarf_exporter import registry as collector_registry
 
 
 class TestRegistry:
 
@@ -122,16 +123,16 @@
   def test_collector_set_performs_deduplication(
       self, simple_target, simple_target_at_customer_level):
     collector_set = collector_registry.CollectorSet(
         {simple_target, simple_target_at_customer_level})
     assert simple_target_at_customer_level not in collector_set
     assert simple_target in collector_set
 
-  def test_collector_set_generatees_service_target(self, simple_target,
-                                                   no_metric_target):
+  def test_collector_set_generates_service_target(self, simple_target,
+                                                  no_metric_target):
     collector_set = collector_registry.CollectorSet({
         simple_target,
     })
     assert no_metric_target in collector_set
 
   def test_customize_returns_modified_target_start_end_date(
       self, collector_set):
@@ -162,30 +163,35 @@
         'level': 'unknown-level',
     }
 
     with pytest.raises(KeyError):
       collector_set.customize(customize_dict)
 
 
-class TestNewRegistry:
-
-  @pytest.fixture(scope='class')
-  def registry(self):
-    return collector_registry.Registry.from_collector_definitions()
-
-  def test_load_collectors_gets_collector_by_name(self, registry):
-    perf = registry.collectors.get('performance')
-    assert perf.name == 'performance'
-    assert perf.query
-
-  def test_load_collectors_gets_collector_by_subregistry_name(self, registry):
-    default_registry = registry.collectors.get('default')
-    assert len(default_registry) == 3
-    assert default_registry.get('performance').name == 'performance'
-
-  def test_load_collectors_gets_conversion_split_collector(self, registry):
-    perf = registry.collectors.get('performance_conversion_split')
-    assert perf.query
-
-  def test_load_collectors_gets_correct_collector_query(self, registry):
-    collector = registry.find_collectors('performance')
-    assert collector
+def test_initialize_collectors_from_config_file_loads_data_from_file(tmp_path):
+  config_file = tmp_path / 'config.yaml'
+  config = [{
+      'name': 'performance',
+      'query': 'SELECT customer.id FROM customer'
+  }]
+  with open(config_file, mode='w', encoding='utf-8') as f:
+    yaml.dump(config, f)
+  collectors = collector_registry.initialize_collectors(config_file=config_file)
+  assert {
+      'performance',
+  } == {c.name for c in collectors}
+
+
+def test_initialize_collectors_from_collector_names_returns_correct_collectors(
+    tmp_path):
+  collectors = collector_registry.initialize_collectors(
+      collector_names='performance', create_service_collectors=False)
+  assert {
+      'performance',
+  } == {c.name for c in collectors}
+
+
+def test_initialize_collectors_from_collector_names_returns_correct_collectors(
+    tmp_path):
+  collectors = collector_registry.initialize_collectors(
+      collector_names='performance', create_service_collectors=True)
+  assert {'performance', 'mapping'} == {c.name for c in collectors}
```

### Comparing `gaarf-exporter-1.0.0.dev3/tests/unit/test_util.py` & `gaarf-exporter-1.0.0.dev4/tests/unit/test_util.py`

 * *Files identical despite different names*

