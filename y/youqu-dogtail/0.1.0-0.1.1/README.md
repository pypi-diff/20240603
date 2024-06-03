# Comparing `tmp/youqu_dogtail-0.1.0.tar.gz` & `tmp/youqu_dogtail-0.1.1.tar.gz`

## Comparing `youqu_dogtail-0.1.0.tar` & `youqu_dogtail-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/.env
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/Pipfile
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/publish.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/tests/test.py
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/__version__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/conf.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/install_depends.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/__init__.py
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/config.py
--rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/distro.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/dump.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/errors.py
--rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/i18n.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/logging.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/path.py
--rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/predicate.py
--rw-r--r--   0        0        0    13198 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/procedural.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/rawinput.py
--rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/sessions.py
--rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/tc.py
--rw-r--r--   0        0        0    47649 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/tree.py
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/utils.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/youqu_dogtail/dogtail/wrapped.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/LICENSE
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/README.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/.env
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/Pipfile
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/publish.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/tests/test.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/__version__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/conf.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/install_depends.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/__init__.py
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/config.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/distro.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/dump.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/errors.py
+-rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/i18n.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/logging.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/path.py
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/predicate.py
+-rw-r--r--   0        0        0    13198 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/procedural.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/rawinput.py
+-rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/sessions.py
+-rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/tc.py
+-rw-r--r--   0        0        0    47649 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/tree.py
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/utils.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/version.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/youqu_dogtail/dogtail/wrapped.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/LICENSE
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/README.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 youqu_dogtail-0.1.1/PKG-INFO
```

### Comparing `youqu_dogtail-0.1.0/Pipfile.lock` & `youqu_dogtail-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/__init__.py` & `youqu_dogtail-0.1.1/youqu_dogtail/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             else:
                 self.obj = root
             if number > 0:
                 self.obj = self.obj.findChildren(predicate.GenericPredicate(**key))[number]
 
         except SearchError:
             if check_start:
-                search_app = easyprocess.EasyProcessError(f"ps -ef | grep {self.name}")
+                search_app = easyprocess.EasyProcess(f"ps -ef | grep {self.name}").call().stdout
                 logger.error(search_app)
                 raise ApplicationStartError(self.name) from SearchError
 
     def app_element(self, *args, **kwargs) -> Node:
         """
          获取app元素的对象
         :return: 元素的对象
```

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/install_depends.py` & `youqu_dogtail-0.1.1/youqu_dogtail/install_depends.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 import os
 import sys
+import easyprocess
 
+from conf import conf
 
 def install_depends():
+    os.environ['QT_ACCESSIBILITY'] = '1'
+    os.environ['QT_LINUX_ACCESSIBILITY_ALWAYS_ON'] = '1'
+
+    for pkg in [
+        "gir1.2-atspi-2.0",
+        "libatk-adaptor",
+        "at-spi2-core",
+    ]:
+        check_installed: bool = easyprocess.EasyProcess(f"apt show {pkg}").call().stdout.startswith("Package:")
+        if not check_installed:
+            # TODO
+            # 调研是否能不带权限安装
+            easyprocess.EasyProcess(f"echo '{conf.PASSWORD}' | sudo -S apt install gir1.2-atspi-2.0").call()
+
     python_path = sys.executable
     site_packages_path = os.path.join(
         os.path.dirname(os.path.dirname(python_path)),
         'lib',
         f'python{sys.version_info.major}.{sys.version_info.minor}',
         'site-packages'
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/__init__.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/config.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/config.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/distro.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/distro.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/dump.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/dump.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/errors.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/errors.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/i18n.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/i18n.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/logging.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/logging.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/path.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/path.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/predicate.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/predicate.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/procedural.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/procedural.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/rawinput.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/rawinput.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/sessions.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/sessions.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/tc.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/tc.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/tree.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/tree.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/utils.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/utils.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/version.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/version.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/youqu_dogtail/dogtail/wrapped.py` & `youqu_dogtail-0.1.1/youqu_dogtail/dogtail/wrapped.py`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/.gitignore` & `youqu_dogtail-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `youqu_dogtail-0.1.0/LICENSE` & `youqu_dogtail-0.1.1/LICENSE`

 * *Files identical despite different names*

