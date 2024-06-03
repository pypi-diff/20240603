# Comparing `tmp/rlabs_mini_cli-0.1.0.tar.gz` & `tmp/rlabs_mini_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlabs_mini_cli-0.1.0.tar", max compression
+gzip compressed data, was "rlabs_mini_cli-1.0.0.tar", max compression
```

## Comparing `rlabs_mini_cli-0.1.0.tar` & `rlabs_mini_cli-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      210 2024-06-03 08:26:05.340563 rlabs_mini_cli-0.1.0/README.md
--rw-r--r--   0        0        0      565 2024-06-03 08:21:37.000000 rlabs_mini_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      807 2024-06-03 08:21:37.000000 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/__init__.py
--rw-r--r--   0        0        0     1436 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/args.py
--rw-r--r--   0        0        0     4067 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/cli.py
--rw-r--r--   0        0        0     1571 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/directory.py
--rw-r--r--   0        0        0     2153 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/envvars.py
--rw-r--r--   0        0        0     1306 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/error.py
--rw-r--r--   0        0        0     2000 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/logger.py
--rw-r--r--   0        0        0     2257 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/manual_test_run.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 rlabs_mini_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      210 2024-06-03 08:38:30.057642 rlabs_mini_cli-1.0.0/README.md
+-rw-r--r--   0        0        0      565 2024-06-03 08:34:22.000000 rlabs_mini_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      807 2024-06-03 08:34:22.000000 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/__init__.py
+-rw-r--r--   0        0        0     1436 2024-06-03 08:38:30.058642 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/args.py
+-rw-r--r--   0        0        0     4067 2024-06-03 08:38:30.058642 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/cli.py
+-rw-r--r--   0        0        0     1571 2024-06-03 08:38:30.058642 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/directory.py
+-rw-r--r--   0        0        0     2153 2024-06-03 08:38:30.058642 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/envvars.py
+-rw-r--r--   0        0        0     1306 2024-06-03 08:38:30.058642 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/error.py
+-rw-r--r--   0        0        0     1999 2024-06-03 08:38:30.058642 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/logger.py
+-rw-r--r--   0        0        0     2257 2024-06-03 08:38:30.058642 rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/manual_test_run.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 rlabs_mini_cli-1.0.0/PKG-INFO
```

### Comparing `rlabs_mini_cli-0.1.0/pyproject.toml` & `rlabs_mini_cli-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rlabs-mini-cli"
-version = "0.1.0"
+version = "1.0.0"
 description = ""
 authors = ["RomanLabs <rromanotero@romanlabs.com>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 packages = [{include = "rlabs_mini_cli", from = "src"}]
 
 [tool.poetry.scripts]
```

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/__init__.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with API Pipe. If not, see <http://www.gnu.org/licenses/>.
 #
 '''
     Module Name
 '''
-__version__ = '0.1.0'
+__version__ = '1.0.0'
 __author__ = 'RomanLabs'
```

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/args.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/args.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/cli.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/cli.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/directory.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/directory.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/envvars.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/envvars.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/error.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/error.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/logger.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from rich.logging import RichHandler
 from rich.traceback import install
 
 def enable_pretty_tracebacks() -> None:
     '''
         Enable Pretty Traceback
 
-        Uses rich to print pretty tracebacks.
+        Uses rich to print pretty tracebacks
     '''
     install()
 
 def stdout(
         name: str,
         log_level: int,
         format: str,
```

### Comparing `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/manual_test_run.py` & `rlabs_mini_cli-1.0.0/src/rlabs_mini_cli/manual_test_run.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.1.0/PKG-INFO` & `rlabs_mini_cli-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlabs-mini-cli
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
 License: LGPL-3.0-or-later
 Author: RomanLabs
 Author-email: rromanotero@romanlabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

