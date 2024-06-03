# Comparing `tmp/youqu3-0.1.1.tar.gz` & `tmp/youqu3-0.1.2.tar.gz`

## Comparing `youqu3-0.1.1.tar` & `youqu3-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu3-0.1.1/.env
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 youqu3-0.1.1/Pipfile
--rw-r--r--   0        0        0     9527 2020-02-02 00:00:00.000000 youqu3-0.1.1/Pipfile.lock
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 youqu3-0.1.1/publish.sh
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 youqu3-0.1.1/docs/YouQu3架构设计.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 youqu3-0.1.1/tests/test.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/__version__.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/custom_exception.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/_setting/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/_setting/_dynamic.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/_setting/_setting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/driver/__init__.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/driver/cli.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/driver/run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/vendor/__init__.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 youqu3-0.1.1/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 youqu3-0.1.1/LICENSE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 youqu3-0.1.1/README.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 youqu3-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 youqu3-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu3-0.1.2/.env
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 youqu3-0.1.2/Pipfile
+-rw-r--r--   0        0        0     9527 2020-02-02 00:00:00.000000 youqu3-0.1.2/Pipfile.lock
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 youqu3-0.1.2/publish.sh
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 youqu3-0.1.2/docs/YouQu3架构设计.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 youqu3-0.1.2/tests/test.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/__version__.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/custom_exception.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/_setting/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/_setting/_dynamic.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/_setting/_setting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/driver/__init__.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/driver/cli.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/driver/run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.2/youqu3/vendor/__init__.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 youqu3-0.1.2/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 youqu3-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 youqu3-0.1.2/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 youqu3-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 youqu3-0.1.2/PKG-INFO
```

### Comparing `youqu3-0.1.1/Pipfile.lock` & `youqu3-0.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/docs/YouQu3架构设计.md` & `youqu3-0.1.2/docs/YouQu3架构设计.md`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/youqu3/__init__.py` & `youqu3-0.1.2/youqu3/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/youqu3/custom_exception.py` & `youqu3-0.1.2/youqu3/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/youqu3/_setting/_dynamic.py` & `youqu3-0.1.2/youqu3/_setting/_dynamic.py`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/youqu3/driver/cli.py` & `youqu3-0.1.2/youqu3/driver/cli.py`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/youqu3/driver/run.py` & `youqu3-0.1.2/youqu3/driver/run.py`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/.gitignore` & `youqu3-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/LICENSE` & `youqu3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/README.md` & `youqu3-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.1/pyproject.toml` & `youqu3-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 ]
 dependencies = [
     "pytest",
     "pytest-timeout",
     "pytest-rerunfailures",
     "allure-pytest",
     "funnylog",
+    "click",
+    "rich",
 ]
 dynamic = [
     "version",
 ]
 
 requires-python = ">=3.7"
 readme = "README.md"
```

### Comparing `youqu3-0.1.1/PKG-INFO` & `youqu3-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: youqu3
-Version: 0.1.1
+Version: 0.1.2
 Summary: YouQu-Next
 Author-email: mikigo <huangmingqiang@uniontech.com>
 License: GPL2.0
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: allure-pytest
+Requires-Dist: click
 Requires-Dist: funnylog
 Requires-Dist: pytest
 Requires-Dist: pytest-rerunfailures
 Requires-Dist: pytest-timeout
+Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # [YouQu3]() 🐉
 
 YouQu3 是下一代 Linux 自动化测试框架，整体架构重新设计，全新的插件化及模块化功能，带来全新的使用效果。
 
 [YouQu3架构设计](docs/YouQu3架构设计.md)
```

