# Comparing `tmp/youqu3-0.1.0.tar.gz` & `tmp/youqu3-0.1.1.tar.gz`

## Comparing `youqu3-0.1.0.tar` & `youqu3-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu3-0.1.0/.env
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 youqu3-0.1.0/Pipfile
--rw-r--r--   0        0        0    16583 2020-02-02 00:00:00.000000 youqu3-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 youqu3-0.1.0/publish.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu3-0.1.0/docs/YouQu3架构设计.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 youqu3-0.1.0/tests/test.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/__version__.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/custom_exception.py
--rw-r--r--   0        0        0    27426 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/mousekey.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/setting/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/setting/_dynamic.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/setting/setting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.0/youqu3/vendor/__init__.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 youqu3-0.1.0/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 youqu3-0.1.0/LICENSE
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 youqu3-0.1.0/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 youqu3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 youqu3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu3-0.1.1/.env
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 youqu3-0.1.1/Pipfile
+-rw-r--r--   0        0        0     9527 2020-02-02 00:00:00.000000 youqu3-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 youqu3-0.1.1/publish.sh
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 youqu3-0.1.1/docs/YouQu3架构设计.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 youqu3-0.1.1/tests/test.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/__version__.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/custom_exception.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/_setting/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/_setting/_dynamic.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/_setting/_setting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/driver/__init__.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/driver/cli.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/driver/run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu3-0.1.1/youqu3/vendor/__init__.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 youqu3-0.1.1/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 youqu3-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 youqu3-0.1.1/README.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 youqu3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 youqu3-0.1.1/PKG-INFO
```

### Comparing `youqu3-0.1.0/youqu3/custom_exception.py` & `youqu3-0.1.1/youqu3/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.0/youqu3/setting/_dynamic.py` & `youqu3-0.1.1/youqu3/_setting/_dynamic.py`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.0/.gitignore` & `youqu3-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `youqu3-0.1.0/LICENSE` & `youqu3-0.1.1/LICENSE`

 * *Files identical despite different names*

