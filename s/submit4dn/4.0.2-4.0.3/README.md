# Comparing `tmp/submit4dn-4.0.2.tar.gz` & `tmp/submit4dn-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "submit4dn-4.0.2.tar", max compression
+gzip compressed data, was "submit4dn-4.0.3.tar", max compression
```

## Comparing `submit4dn-4.0.2.tar` & `submit4dn-4.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2024-04-18 19:14:22.106597 submit4dn-4.0.2/LICENSE.txt
--rw-r--r--   0        0        0     7905 2024-04-18 19:14:22.106597 submit4dn-4.0.2/README.md
--rw-r--r--   0        0        0      935 2024-04-18 19:14:22.110597 submit4dn-4.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 19:14:22.114597 submit4dn-4.0.2/wranglertools/__init__.py
--rwxr-xr-x   0        0        0    22110 2024-04-18 19:14:22.118597 submit4dn-4.0.2/wranglertools/get_field_info.py
--rwxr-xr-x   0        0        0    71618 2024-04-18 19:14:22.118597 submit4dn-4.0.2/wranglertools/import_data.py
--rw-r--r--   0        0        0     8781 1970-01-01 00:00:00.000000 submit4dn-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-06-03 14:23:01.210482 submit4dn-4.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     7905 2024-06-03 14:23:01.210482 submit4dn-4.0.3/README.md
+-rw-r--r--   0        0        0      935 2024-06-03 14:23:01.214482 submit4dn-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 14:23:01.218482 submit4dn-4.0.3/wranglertools/__init__.py
+-rwxr-xr-x   0        0        0    22110 2024-06-03 14:23:01.218482 submit4dn-4.0.3/wranglertools/get_field_info.py
+-rwxr-xr-x   0        0        0    71675 2024-06-03 14:23:01.218482 submit4dn-4.0.3/wranglertools/import_data.py
+-rw-r--r--   0        0        0     8781 1970-01-01 00:00:00.000000 submit4dn-4.0.3/PKG-INFO
```

### Comparing `submit4dn-4.0.2/LICENSE.txt` & `submit4dn-4.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `submit4dn-4.0.2/README.md` & `submit4dn-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `submit4dn-4.0.2/pyproject.toml` & `submit4dn-4.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Submit4DN"
-version = "4.0.2"
+version = "4.0.3"
 description = "Utility package for submitting data to the 4DN Data Portal"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/4dn-dcic/Submit4DN"
 repository = "https://github.com/4dn-dcic/Submit4DN"
 packages = [
```

### Comparing `submit4dn-4.0.2/wranglertools/get_field_info.py` & `submit4dn-4.0.3/wranglertools/get_field_info.py`

 * *Files identical despite different names*

### Comparing `submit4dn-4.0.2/wranglertools/import_data.py` & `submit4dn-4.0.3/wranglertools/import_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -794,14 +794,15 @@
                 not_found = None
                 alias_bit = None
                 if utrl_txt in error_description:
                     alias_bit = error_description.replace(utrl_txt, '')
                 elif error_description.endswith(nf_txt):
                     alias_bit = error_description.replace(nf_txt, '').replace("'", '')
                 if alias_bit:
+                    alias_bit = alias_bit.split('/')[-1]
                     not_found = alias_bit.strip()
                 # ignore ones about existing aliases
                 if not_found and not_found in all_aliases:
                     continue
                 error_field = err['name']
                 report.append("{sheet:<30}{eid} Field '{er}': {des}"
                               .format(er=error_field, des=error_description, eid=error_id, sheet="ERROR " + sheet.lower()))
```

### Comparing `submit4dn-4.0.2/PKG-INFO` & `submit4dn-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: submit4dn
-Version: 4.0.2
+Version: 4.0.3
 Summary: Utility package for submitting data to the 4DN Data Portal
 Home-page: https://github.com/4dn-dcic/Submit4DN
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.0,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

