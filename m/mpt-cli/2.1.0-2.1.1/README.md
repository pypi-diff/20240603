# Comparing `tmp/mpt_cli-2.1.0.tar.gz` & `tmp/mpt_cli-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpt_cli-2.1.0.tar", max compression
+gzip compressed data, was "mpt_cli-2.1.1.tar", max compression
```

## Comparing `mpt_cli-2.1.0.tar` & `mpt_cli-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2024-05-28 16:13:46.326083 mpt_cli-2.1.0/LICENSE
--rw-r--r--   0        0        0      861 2024-05-28 16:13:46.326083 mpt_cli-2.1.0/README.md
--rw-r--r--   0        0        0     2873 2024-05-28 16:14:00.762285 mpt_cli-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/__init__.py
--rw-r--r--   0        0        0       29 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/accounts/__init__.py
--rw-r--r--   0        0        0     7402 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/accounts/app.py
--rw-r--r--   0        0        0     3093 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/accounts/flows.py
--rw-r--r--   0        0        0      181 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/accounts/models.py
--rw-r--r--   0        0        0      854 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/alias_group.py
--rw-r--r--   0        0        0     1791 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/console.py
--rw-r--r--   0        0        0     2024 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/errors.py
--rw-r--r--   0        0        0      301 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/icons/fake-icon.png
--rw-r--r--   0        0        0        0 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/mpt/__init__.py
--rw-r--r--   0        0        0     1481 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/mpt/client.py
--rw-r--r--   0        0        0     6574 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/mpt/flows.py
--rw-r--r--   0        0        0      965 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/mpt/models.py
--rw-r--r--   0        0        0      486 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/plugins.py
--rw-r--r--   0        0        0       29 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/pricelists/__init__.py
--rw-r--r--   0        0        0     3930 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/pricelists/app.py
--rw-r--r--   0        0        0     2192 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/pricelists/constants.py
--rw-r--r--   0        0        0     6663 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/pricelists/flows.py
--rw-r--r--   0        0        0       29 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/products/__init__.py
--rw-r--r--   0        0        0     7001 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/products/app.py
--rw-r--r--   0        0        0     8438 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/products/constants.py
--rw-r--r--   0        0        0    27565 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/products/flows.py
--rw-r--r--   0        0        0     3665 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/stats.py
--rw-r--r--   0        0        0     4747 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/core/utils.py
--rw-r--r--   0        0        0        0 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/plugins/__init__.py
--rw-r--r--   0        0        0     1215 2024-05-28 16:13:46.330083 mpt_cli-2.1.0/swo/mpt/cli/swocli.py
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 mpt_cli-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/LICENSE
+-rw-r--r--   0        0        0      861 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/README.md
+-rw-r--r--   0        0        0     2873 2024-06-03 15:10:05.308308 mpt_cli-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/__init__.py
+-rw-r--r--   0        0        0       29 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/accounts/__init__.py
+-rw-r--r--   0        0        0     7402 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/accounts/app.py
+-rw-r--r--   0        0        0     3093 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/accounts/flows.py
+-rw-r--r--   0        0        0      181 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/accounts/models.py
+-rw-r--r--   0        0        0      854 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/alias_group.py
+-rw-r--r--   0        0        0     1791 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/console.py
+-rw-r--r--   0        0        0     2024 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/errors.py
+-rw-r--r--   0        0        0      301 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/icons/fake-icon.png
+-rw-r--r--   0        0        0        0 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/mpt/__init__.py
+-rw-r--r--   0        0        0     1481 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/mpt/client.py
+-rw-r--r--   0        0        0     6752 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/mpt/flows.py
+-rw-r--r--   0        0        0      965 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/mpt/models.py
+-rw-r--r--   0        0        0      486 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/plugins.py
+-rw-r--r--   0        0        0       29 2024-06-03 15:09:51.928326 mpt_cli-2.1.1/swo/mpt/cli/core/pricelists/__init__.py
+-rw-r--r--   0        0        0     3930 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/pricelists/app.py
+-rw-r--r--   0        0        0     2192 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/pricelists/constants.py
+-rw-r--r--   0        0        0     6663 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/pricelists/flows.py
+-rw-r--r--   0        0        0       29 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/products/__init__.py
+-rw-r--r--   0        0        0     7001 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/products/app.py
+-rw-r--r--   0        0        0     8438 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/products/constants.py
+-rw-r--r--   0        0        0    27759 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/products/flows.py
+-rw-r--r--   0        0        0     3665 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/stats.py
+-rw-r--r--   0        0        0     4747 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/core/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/plugins/__init__.py
+-rw-r--r--   0        0        0     1215 2024-06-03 15:09:51.932326 mpt_cli-2.1.1/swo/mpt/cli/swocli.py
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 mpt_cli-2.1.1/PKG-INFO
```

### Comparing `mpt_cli-2.1.0/LICENSE` & `mpt_cli-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/README.md` & `mpt_cli-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/pyproject.toml` & `mpt_cli-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpt-cli"
-version = "2.1.0"
+version = "2.1.1"
 description = "Command line utility for SoftwareOne Marketplace Platform"
 authors = ["SoftwareOne AG"]
 license = "Apache-2.0 license"
 packages = [
     { include = "swo" }
 ]
 readme = "README.md"
```

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/accounts/app.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/accounts/app.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/accounts/flows.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/accounts/flows.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/alias_group.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/alias_group.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/console.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/console.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/errors.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/mpt/client.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/mpt/client.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/mpt/flows.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/mpt/flows.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,14 +145,20 @@
 @wrap_http_error
 def publish_item(mpt_client: MPTClient, item_id: str) -> None:
     response = mpt_client.post(f"/items/{item_id}/publish")
     response.raise_for_status()
 
 
 @wrap_http_error
+def unpublish_item(mpt_client: MPTClient, item_id: str) -> None:
+    response = mpt_client.post(f"/items/{item_id}/unpublish")
+    response.raise_for_status()
+
+
+@wrap_http_error
 def update_item(mpt_client, item_id: str, item_json: dict) -> None:
     response = mpt_client.put(f"/items/{item_id}", json=item_json)
     response.raise_for_status()
 
 
 @cache
 @wrap_http_error
```

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/mpt/models.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/mpt/models.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/pricelists/app.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/pricelists/app.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/pricelists/constants.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/pricelists/constants.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/pricelists/flows.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/pricelists/flows.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/products/app.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/products/app.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/products/constants.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/products/constants.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/products/flows.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/products/flows.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     create_parameter_group,
     create_product,
     create_template,
     get_products,
     publish_item,
     review_item,
     search_uom_by_name,
+    unpublish_item,
 )
 from swo.mpt.cli.core.mpt.flows import (
     update_item as mpt_update_item,
 )
 from swo.mpt.cli.core.mpt.models import (
     Item,
     ItemGroup,
@@ -63,14 +64,15 @@
 
 
 class ItemAction(enum.Enum):
     CREATE = "create"
     UPDATE = "update"
     REVIEW = "review"
     PUBLISH = "publish"
+    UNPUBLISH = "unpublish"
     SKIP = "-"
     SKIPPED = ""
 
 
 def get_definition_file(path: str) -> Path:
     """
     Returns product definition file path. If only product id is passed assumed
@@ -570,14 +572,17 @@
             match ItemAction(action):
                 case ItemAction.REVIEW:
                     review_item(mpt_client, item_id)
                     stats.add_synced(ws.title)
                 case ItemAction.PUBLISH:
                     publish_item(mpt_client, item_id)
                     stats.add_synced(ws.title)
+                case ItemAction.UNPUBLISH:
+                    unpublish_item(mpt_client, item_id)
+                    stats.add_synced(ws.title)
                 case ItemAction.UPDATE:
                     update_item(
                         mpt_client, active_account, item_id, product_id, sheet_value
                     )
                     stats.add_synced(ws.title)
                 case _:
                     stats.add_skipped(ws.title)
```

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/stats.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/stats.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/core/utils.py` & `mpt_cli-2.1.1/swo/mpt/cli/core/utils.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/swo/mpt/cli/swocli.py` & `mpt_cli-2.1.1/swo/mpt/cli/swocli.py`

 * *Files identical despite different names*

### Comparing `mpt_cli-2.1.0/PKG-INFO` & `mpt_cli-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpt-cli
-Version: 2.1.0
+Version: 2.1.1
 Summary: Command line utility for SoftwareOne Marketplace Platform
 License: Apache-2.0 license
 Keywords: fulfillment,command,line,interface,utility,cli,softwareone,marketplace
 Author: SoftwareOne AG
 Requires-Python: >=3.12,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

