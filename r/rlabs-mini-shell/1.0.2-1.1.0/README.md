# Comparing `tmp/rlabs_mini_shell-1.0.2.tar.gz` & `tmp/rlabs_mini_shell-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlabs_mini_shell-1.0.2.tar", max compression
+gzip compressed data, was "rlabs_mini_shell-1.1.0.tar", max compression
```

## Comparing `rlabs_mini_shell-1.0.2.tar` & `rlabs_mini_shell-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       96 2024-06-03 08:07:48.669731 rlabs_mini_shell-1.0.2/README.md
--rw-r--r--   0        0        0      571 2024-06-03 08:03:31.000000 rlabs_mini_shell-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      810 2024-06-03 08:03:31.000000 rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/__init__.py
--rw-r--r--   0        0        0     4857 2024-06-03 08:07:48.670731 rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/cmd.py
--rw-r--r--   0        0        0     1411 2024-06-03 08:07:48.670731 rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/config.py
--rw-r--r--   0        0        0     1536 2024-06-03 08:07:48.670731 rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/error.py
--rw-r--r--   0        0        0     2013 2024-06-03 08:07:48.670731 rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/logger.py
--rw-r--r--   0        0        0     1333 2024-06-03 08:07:48.670731 rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/manual_test_run.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 rlabs_mini_shell-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      204 2024-06-03 08:25:51.408922 rlabs_mini_shell-1.1.0/README.md
+-rw-r--r--   0        0        0      571 2024-06-03 08:21:43.000000 rlabs_mini_shell-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      810 2024-06-03 08:21:43.000000 rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/__init__.py
+-rw-r--r--   0        0        0     4857 2024-06-03 08:25:51.409922 rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/cmd.py
+-rw-r--r--   0        0        0     1411 2024-06-03 08:25:51.409922 rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/config.py
+-rw-r--r--   0        0        0     1536 2024-06-03 08:25:51.409922 rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/error.py
+-rw-r--r--   0        0        0     2013 2024-06-03 08:25:51.409922 rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/logger.py
+-rw-r--r--   0        0        0     1333 2024-06-03 08:25:51.409922 rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/manual_test_run.py
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 rlabs_mini_shell-1.1.0/PKG-INFO
```

### Comparing `rlabs_mini_shell-1.0.2/pyproject.toml` & `rlabs_mini_shell-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rlabs-mini-shell"
-version = "1.0.2"
+version = "1.1.0"
 description = ""
 authors = ["RomanLabs <rromanotero@romanlabs.com>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 packages = [{include = "rlabs_mini_shell", from = "src"}]
 
 [tool.poetry.scripts]
```

### Comparing `rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/__init__.py` & `rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with API Pipe. If not, see <http://www.gnu.org/licenses/>.
 #
 '''
     Module Name
 '''
-__version__ = '1.0.2'
+__version__ = '1.1.0'
 __author__ = 'RomanLabs'
```

### Comparing `rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/cmd.py` & `rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/cmd.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/config.py` & `rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/config.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/error.py` & `rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/error.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/logger.py` & `rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/logger.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_shell-1.0.2/src/rlabs_mini_shell/manual_test_run.py` & `rlabs_mini_shell-1.1.0/src/rlabs_mini_shell/manual_test_run.py`

 * *Files identical despite different names*

### Comparing `rlabs_mini_shell-1.0.2/PKG-INFO` & `rlabs_mini_shell-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: rlabs-mini-shell
-Version: 1.0.2
+Version: 1.1.0
 Summary: 
 License: LGPL-3.0-or-later
 Author: RomanLabs
 Author-email: rromanotero@romanlabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mypy (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Description-Content-Type: text/markdown
 
-## rlabs_mini_shell
+# Rlabs Mini Shell
 
-[Project in Gitlab](https://gitlab.com/romanlabs/public/rlabs_mini_shell)
+RLabs Mini Shell is a simple Python library for executing shell commands. Intended for quick prototyping.  
+
+[Project in Gitlab](https://gitlab.com/romanlabs/public/rlabs-mini-shell)
```

