# Comparing `tmp/rlabs_mini_cli-0.0.3.tar.gz` & `tmp/rlabs_mini_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlabs_mini_cli-0.0.3.tar", max compression
+gzip compressed data, was "rlabs_mini_cli-0.1.0.tar", max compression
```

## Comparing `rlabs_mini_cli-0.0.3.tar` & `rlabs_mini_cli-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       92 2024-06-03 08:02:09.293245 rlabs_mini_cli-0.0.3/README.md
--rw-r--r--   0        0        0      565 2024-06-03 08:03:33.000000 rlabs_mini_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      807 2024-06-03 08:03:33.000000 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/__init__.py
--rw-r--r--   0        0        0     1436 2024-06-03 08:02:09.294245 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/args.py
--rw-r--r--   0        0        0     4067 2024-06-03 08:02:09.294245 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/cli.py
--rw-r--r--   0        0        0     1571 2024-06-03 08:02:09.294245 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/directory.py
--rw-r--r--   0        0        0     2153 2024-06-03 08:02:09.294245 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/envvars.py
--rw-r--r--   0        0        0     1306 2024-06-03 08:02:09.294245 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/error.py
--rw-r--r--   0        0        0     2000 2024-06-03 08:02:09.294245 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/logger.py
--rw-r--r--   0        0        0     2257 2024-06-03 08:02:09.294245 rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/manual_test_run.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 rlabs_mini_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      210 2024-06-03 08:26:05.340563 rlabs_mini_cli-0.1.0/README.md
+-rw-r--r--   0        0        0      565 2024-06-03 08:21:37.000000 rlabs_mini_cli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      807 2024-06-03 08:21:37.000000 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/__init__.py
+-rw-r--r--   0        0        0     1436 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/args.py
+-rw-r--r--   0        0        0     4067 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/cli.py
+-rw-r--r--   0        0        0     1571 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/directory.py
+-rw-r--r--   0        0        0     2153 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/envvars.py
+-rw-r--r--   0        0        0     1306 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/error.py
+-rw-r--r--   0        0        0     2000 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/logger.py
+-rw-r--r--   0        0        0     2257 2024-06-03 08:26:05.341563 rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/manual_test_run.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 rlabs_mini_cli-0.1.0/PKG-INFO
```

### Comparing `rlabs_mini_cli-0.0.3/pyproject.toml` & `rlabs_mini_cli-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rlabs-mini-cli"
-version = "0.0.3"
+version = "0.1.0"
 description = ""
 authors = ["RomanLabs <rromanotero@romanlabs.com>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 packages = [{include = "rlabs_mini_cli", from = "src"}]
 
 [tool.poetry.scripts]
```

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/__init__.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with API Pipe. If not, see <http://www.gnu.org/licenses/>.
 #
 '''
     Module Name
 '''
-__version__ = '0.0.3'
+__version__ = '0.1.0'
 __author__ = 'RomanLabs'
```

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/args.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/args.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/cli.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/cli.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/directory.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/directory.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/envvars.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/envvars.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/error.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/error.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/logger.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/logger.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_cli-0.0.3/src/rlabs_mini_cli/manual_test_run.py` & `rlabs_mini_cli-0.1.0/src/rlabs_mini_cli/manual_test_run.py`

 * *Files identical despite different names*

