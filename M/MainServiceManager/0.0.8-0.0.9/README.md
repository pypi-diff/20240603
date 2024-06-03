# Comparing `tmp/mainservicemanager-0.0.8.tar.gz` & `tmp/mainservicemanager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainservicemanager-0.0.8.tar", max compression
+gzip compressed data, was "mainservicemanager-0.0.9.tar", max compression
```

## Comparing `mainservicemanager-0.0.8.tar` & `mainservicemanager-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.8/README.md
--rwxr-xr-x   0        0        0      736 2024-06-02 10:59:59.000000 mainservicemanager-0.0.8/pyproject.toml
--rwxr-xr-x   0        0        0      391 2024-06-02 10:59:50.000000 mainservicemanager-0.0.8/src/MainServiceManager/__init__.py
--rwxr-xr-x   0        0        0     4387 2024-06-02 10:51:09.000000 mainservicemanager-0.0.8/src/MainServiceManager/__main__.py
--rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.8/src/MainServiceManager/api.py
--rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.8/src/MainServiceManager/server.py
--rwxr-xr-x   0        0        0     7419 2024-06-02 09:54:48.000000 mainservicemanager-0.0.8/src/MainServiceManager/server_utils.py
--rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.9/README.md
+-rwxr-xr-x   0        0        0      736 2024-06-02 11:17:33.000000 mainservicemanager-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0      391 2024-06-02 11:17:28.000000 mainservicemanager-0.0.9/src/MainServiceManager/__init__.py
+-rwxr-xr-x   0        0        0     4387 2024-06-02 10:51:08.000000 mainservicemanager-0.0.9/src/MainServiceManager/__main__.py
+-rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.9/src/MainServiceManager/api.py
+-rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.9/src/MainServiceManager/server.py
+-rwxr-xr-x   0        0        0     7439 2024-06-02 11:15:48.000000 mainservicemanager-0.0.9/src/MainServiceManager/server_utils.py
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.9/PKG-INFO
```

### Comparing `mainservicemanager-0.0.8/README.md` & `mainservicemanager-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.8/pyproject.toml` & `mainservicemanager-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MainServiceManager"
-version = "0.0.8"
+version = "0.0.9"
 description = "Пользовательская программа для управления сервисами, аналогично systemd"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainServiceManager.py"
 packages = [
 { include = "MainServiceManager", from = "src" },
 ]
```

### Comparing `mainservicemanager-0.0.8/src/MainServiceManager/__main__.py` & `mainservicemanager-0.0.9/src/MainServiceManager/__main__.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.8/src/MainServiceManager/api.py` & `mainservicemanager-0.0.9/src/MainServiceManager/api.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.8/src/MainServiceManager/server.py` & `mainservicemanager-0.0.9/src/MainServiceManager/server.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.8/src/MainServiceManager/server_utils.py` & `mainservicemanager-0.0.9/src/MainServiceManager/server_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     self.closed=False
     self.enabled=False
     self.pid=None
     self.process=None
     if path=="admin":
       self.path=None
       self.name="admin"
+      self.data={}
     else:
       self.path=os.path.abspath(path)
       self.name=os.path.basename(self.path)
       if password==None:
         self.password=randbytes(16).hex()
       else:
         self.password=password
```

### Comparing `mainservicemanager-0.0.8/PKG-INFO` & `mainservicemanager-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainServiceManager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Пользовательская программа для управления сервисами, аналогично systemd
 Home-page: https://github.com/MainPlay-TG/MainServiceManager.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

