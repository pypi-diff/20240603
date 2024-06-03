# Comparing `tmp/resc_vcs_scanner-3.3.1.tar.gz` & `tmp/resc_vcs_scanner-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-3.3.1.tar", last modified: Fri May 31 11:44:16 2024, max compression
+gzip compressed data, was "resc_vcs_scanner-3.3.2.tar", last modified: Mon Jun  3 09:44:02 2024, max compression
```

## Comparing `resc_vcs_scanner-3.3.1.tar` & `resc_vcs_scanner-3.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-31 11:44:16.377848 resc_vcs_scanner-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.365848 resc_vcs_scanner-3.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-31 11:44:16.000000 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-31 11:44:16.000000 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:44:16.000000 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 11:44:16.000000 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:44:16.000000 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-31 11:44:16.000000 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 11:44:16.000000 resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.369848 resc_vcs_scanner-3.3.1/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/finding_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/gitleaks_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/ignore_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/rule_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/rule_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/output_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/rws_api_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/stdout_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15909 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/secret_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:44:16.373848 resc_vcs_scanner-3.3.1/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-31 11:44:09.000000 resc_vcs_scanner-3.3.1/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.220172 resc_vcs_scanner-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-06-03 09:44:02.220172 resc_vcs_scanner-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-06-03 09:44:02.220172 resc_vcs_scanner-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.208171 resc_vcs_scanner-3.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.216172 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-06-03 09:44:02.000000 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-06-03 09:44:02.000000 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:44:02.000000 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-03 09:44:02.000000 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:44:02.000000 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-03 09:44:02.000000 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 09:44:02.000000 resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.212171 resc_vcs_scanner-3.3.2/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.216172 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/finding_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/gitleaks_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.216172 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/rule_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/rule_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.216172 resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/output_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/rws_api_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/stdout_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.216172 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16110 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/secret_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:44:02.216172 resc_vcs_scanner-3.3.2/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-03 09:43:57.000000 resc_vcs_scanner-3.3.2/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-3.3.1/LICENSE.md` & `resc_vcs_scanner-3.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/PKG-INFO` & `resc_vcs_scanner-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 3.3.1
+Version: 3.3.2
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-3.3.1/README.md` & `resc_vcs_scanner-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/setup.cfg` & `resc_vcs_scanner-3.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 3.3.1
+version = 3.3.2
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
```

### Comparing `resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/PKG-INFO` & `resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 3.3.1
+Version: 3.3.2
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-3.3.1/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-3.3.2/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/common.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/cli.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/env_default.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/finding_filter.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/finding_filter.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/gitleaks_types.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/gitleaks_types.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/ignore_list.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/ignore_list.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/rule_comment.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/rule_comment.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/rule_file.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/rule_file.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/helpers/providers/rule_tag.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/helpers/providers/rule_tag.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/input_parser.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/model.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/output_module.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/output_module.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/rws_api_writer.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/rws_api_writer.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/output_modules/stdout_writer.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/output_modules/stdout_writer.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/cli.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/cli.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/git_operation.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/git_operation.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,17 +350,23 @@
             return False
 
         self._findings = self._findings_from_repo + self._findings_from_dir
         self._findings = list(map(self._populate_if_empty, self._findings))
         return True
 
     def _populate_if_empty(self, finding: FindingBase) -> FindingBase:
-        finding.commit_id = finding.commit_id or self.head_commit.hexsha or "unknown"
-        finding.commit_message = finding.commit_message or self.head_commit.message
-        finding.commit_timestamp = finding.commit_timestamp or self.head_commit.committed_date
+        finding.commit_id = finding.commit_id or (
+            self.head_commit.hexsha if self.head_commit is not None else "unknown"
+        )
+        finding.commit_message = finding.commit_message or (
+            self.head_commit.message if self.head_commit is not None else ""
+        )
+        finding.commit_timestamp = finding.commit_timestamp or (
+            self.head_commit.committed_date if self.head_commit is not None else datetime.now(UTC)
+        )
         finding.author = finding.author or "vcs-scanner"
         return finding
 
     def _write_findings(self) -> True:
         logger.info(f"Scan completed: {len(self._findings)} findings were found.")
         self._output_module.write_findings(
             repository_id=getattr(self._created_repository, "id_", 0),
```

### Comparing `resc_vcs_scanner-3.3.1/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-3.3.2/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*

