# Comparing `tmp/mainshortcuts-1.6.95.tar.gz` & `tmp/mainshortcuts-1.6.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.95.tar", max compression
+gzip compressed data, was "mainshortcuts-1.6.96.tar", max compression
```

## Comparing `mainshortcuts-1.6.95.tar` & `mainshortcuts-1.6.96.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.95/README.md
--rwxr-xr-x   0        0        0      696 2024-05-20 12:11:57.000000 mainshortcuts-1.6.95/pyproject.toml
--rwxr-xr-x   0        0        0     5954 2024-05-08 16:40:54.000000 mainshortcuts-1.6.95/src/MainShortcuts/MainCore.py
--rwxr-xr-x   0        0        0     1025 2024-05-20 12:11:52.000000 mainshortcuts-1.6.95/src/MainShortcuts/__init__.py
--rwxr-xr-x   0        0        0      495 2024-05-08 16:41:02.000000 mainshortcuts-1.6.95/src/MainShortcuts/addon.py
--rwxr-xr-x   0        0        0     4975 2024-05-20 12:11:29.000000 mainshortcuts-1.6.95/src/MainShortcuts/cfg.py
--rwxr-xr-x   0        0        0     1057 2024-05-08 16:41:00.000000 mainshortcuts-1.6.95/src/MainShortcuts/dict.py
--rwxr-xr-x   0        0        0     1538 2024-05-08 16:41:02.000000 mainshortcuts-1.6.95/src/MainShortcuts/dictplus.py
--rwxr-xr-x   0        0        0     4189 2024-05-16 08:59:32.000000 mainshortcuts-1.6.95/src/MainShortcuts/dir.py
--rwxr-xr-x   0        0        0     3043 2024-05-08 16:40:46.000000 mainshortcuts-1.6.95/src/MainShortcuts/file.py
--rwxr-xr-x   0        0        0     6183 2024-05-08 16:41:04.000000 mainshortcuts-1.6.95/src/MainShortcuts/fileobj.py
--rwxr-xr-x   0        0        0     3659 2024-05-20 12:12:01.000000 mainshortcuts-1.6.95/src/MainShortcuts/imports.py
--rwxr-xr-x   0        0        0     3948 2024-05-09 14:07:38.000000 mainshortcuts-1.6.95/src/MainShortcuts/json.py
--rwxr-xr-x   0        0        0     2292 2024-05-08 16:41:06.000000 mainshortcuts-1.6.95/src/MainShortcuts/list.py
--rwxr-xr-x   0        0        0     1073 2024-05-08 16:40:46.000000 mainshortcuts-1.6.95/src/MainShortcuts/main.py
--rwxr-xr-x   0        0        0       93 2024-05-08 16:40:46.000000 mainshortcuts-1.6.95/src/MainShortcuts/os.py
--rwxr-xr-x   0        0        0     6585 2024-05-08 16:40:58.000000 mainshortcuts-1.6.95/src/MainShortcuts/path.py
--rwxr-xr-x   0        0        0      857 2024-05-08 16:41:06.000000 mainshortcuts-1.6.95/src/MainShortcuts/proc.py
--rwxr-xr-x   0        0        0     1507 2024-05-08 16:40:50.000000 mainshortcuts-1.6.95/src/MainShortcuts/script.py
--rwxr-xr-x   0        0        0     1047 2024-05-08 16:41:08.000000 mainshortcuts-1.6.95/src/MainShortcuts/str.py
--rwxr-xr-x   0        0        0    15238 2024-05-08 16:40:50.000000 mainshortcuts-1.6.95/src/MainShortcuts/values.py
--rwxr-xr-x   0        0        0     1327 2024-05-08 16:41:00.000000 mainshortcuts-1.6.95/src/MainShortcuts/win.py
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.95/PKG-INFO
+-rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.96/README.md
+-rwxr-xr-x   0        0        0      696 2024-06-03 13:21:01.000000 mainshortcuts-1.6.96/pyproject.toml
+-rwxr-xr-x   0        0        0     5954 2024-05-08 16:40:54.000000 mainshortcuts-1.6.96/src/MainShortcuts/MainCore.py
+-rwxr-xr-x   0        0        0     1020 2024-06-03 13:20:57.000000 mainshortcuts-1.6.96/src/MainShortcuts/__init__.py
+-rwxr-xr-x   0        0        0      495 2024-05-08 16:41:02.000000 mainshortcuts-1.6.96/src/MainShortcuts/addon.py
+-rwxr-xr-x   0        0        0     4975 2024-05-20 12:11:28.000000 mainshortcuts-1.6.96/src/MainShortcuts/cfg.py
+-rwxr-xr-x   0        0        0     1057 2024-05-08 16:41:00.000000 mainshortcuts-1.6.96/src/MainShortcuts/dict.py
+-rwxr-xr-x   0        0        0     1538 2024-05-08 16:41:02.000000 mainshortcuts-1.6.96/src/MainShortcuts/dictplus.py
+-rwxr-xr-x   0        0        0     4189 2024-05-16 08:59:32.000000 mainshortcuts-1.6.96/src/MainShortcuts/dir.py
+-rwxr-xr-x   0        0        0     3043 2024-05-08 16:40:46.000000 mainshortcuts-1.6.96/src/MainShortcuts/file.py
+-rwxr-xr-x   0        0        0     6183 2024-05-08 16:41:04.000000 mainshortcuts-1.6.96/src/MainShortcuts/fileobj.py
+-rwxr-xr-x   0        0        0     3768 2024-06-03 13:21:01.000000 mainshortcuts-1.6.96/src/MainShortcuts/imports.py
+-rwxr-xr-x   0        0        0     3948 2024-05-09 14:07:38.000000 mainshortcuts-1.6.96/src/MainShortcuts/json.py
+-rwxr-xr-x   0        0        0     2292 2024-05-08 16:41:06.000000 mainshortcuts-1.6.96/src/MainShortcuts/list.py
+-rwxr-xr-x   0        0        0     1279 2024-06-03 13:18:56.000000 mainshortcuts-1.6.96/src/MainShortcuts/main.py
+-rwxr-xr-x   0        0        0       93 2024-05-08 16:40:46.000000 mainshortcuts-1.6.96/src/MainShortcuts/os.py
+-rwxr-xr-x   0        0        0     6585 2024-05-08 16:40:58.000000 mainshortcuts-1.6.96/src/MainShortcuts/path.py
+-rwxr-xr-x   0        0        0      857 2024-05-08 16:41:06.000000 mainshortcuts-1.6.96/src/MainShortcuts/proc.py
+-rwxr-xr-x   0        0        0     1507 2024-05-08 16:40:50.000000 mainshortcuts-1.6.96/src/MainShortcuts/script.py
+-rwxr-xr-x   0        0        0     1047 2024-05-08 16:41:08.000000 mainshortcuts-1.6.96/src/MainShortcuts/str.py
+-rwxr-xr-x   0        0        0    15238 2024-05-08 16:40:50.000000 mainshortcuts-1.6.96/src/MainShortcuts/values.py
+-rwxr-xr-x   0        0        0     1327 2024-05-08 16:41:00.000000 mainshortcuts-1.6.96/src/MainShortcuts/win.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.96/PKG-INFO
```

### Comparing `mainshortcuts-1.6.95/README.md` & `mainshortcuts-1.6.96/README.md`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/pyproject.toml` & `mainshortcuts-1.6.96/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "1.6.95"
+version = "1.6.96"
 name = "MainShortcuts"
 description = "Simplifying Python Built-in Commands"
 authors = [ "MainPlay TG <xbox.roman6666666666@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainShortcuts.py"
 packages = [
     { include = "MainShortcuts", from = "src" },
```

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/MainCore.py` & `mainshortcuts-1.6.96/src/MainShortcuts/MainCore.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/__init__.py` & `mainshortcuts-1.6.96/src/MainShortcuts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """MainShortcuts - \u043D\u0435\u0431\u043E\u043B\u044C\u0448\u0430\u044F \u0431\u0438\u0431\u043B\u0438\u043E\u0442\u0435\u043A\u0430 \u0434\u043B\u044F \u0443\u043F\u0440\u043E\u0449\u0435\u043D\u0438\u044F \u043D\u0430\u043F\u0438\u0441\u0430\u043D\u0438\u044F \u043A\u043E\u0434\u0430
 \u0420\u0430\u0437\u0440\u0430\u0431\u043E\u0442\u0447\u0438\u043A: MainPlay TG
-https://t.me/MainPlay_InfoCh"""
+https://t.me/MainPlayCh"""
 
-__version_tuple__ = (1, 6, 95)
+__version_tuple__ = (1, 6, 96)
 __depends__ = {
     "required": [
         "json",
         "os",
         "platform",
         "shutil",
         "subprocess",
```

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/cfg.py` & `mainshortcuts-1.6.96/src/MainShortcuts/cfg.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/dict.py` & `mainshortcuts-1.6.96/src/MainShortcuts/dict.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/dictplus.py` & `mainshortcuts-1.6.96/src/MainShortcuts/dictplus.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/dir.py` & `mainshortcuts-1.6.96/src/MainShortcuts/dir.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/file.py` & `mainshortcuts-1.6.96/src/MainShortcuts/file.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/fileobj.py` & `mainshortcuts-1.6.96/src/MainShortcuts/fileobj.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/imports.py` & `mainshortcuts-1.6.96/src/MainShortcuts/imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,133 +1,139 @@
 """Этот файл просто импортирует части модуля
 Он создаётся автоматически"""
 import os
 import MainShortcuts.main as main
-imports_all = []
-imports_import_errors = {}
-noimport = []
+imports_all=[]
+imports_import_errors={}
+noimport=[]
 if "MS_NOIMPORT" in os.environ:
   for i in os.environ["MS_NOIMPORT"].split(","):
     if i.strip():
       noimport.append(i.strip().lower())
 noimport.sort()
 if not 'cd' in noimport:
   try:
-    cd = main.cd
+    cd=main.cd
     imports_all.append('cd')
   except Exception as e:
-    imports_import_errors['cd'] = e
+    imports_import_errors['cd']=e
 if not 'clear_ANSI' in noimport:
   try:
-    clear_ANSI = main.clear_ANSI
+    clear_ANSI=main.clear_ANSI
     imports_all.append('clear_ANSI')
   except Exception as e:
-    imports_import_errors['clear_ANSI'] = e
-if not 'cls_ANSI' in noimport:
-  try:
-    cls_ANSI = main.cls_ANSI
-    imports_all.append('cls_ANSI')
-  except Exception as e:
-    imports_import_errors['cls_ANSI'] = e
+    imports_import_errors['clear_ANSI']=e
 if not 'clear' in noimport:
   try:
-    clear = main.clear
+    clear=main.clear
     imports_all.append('clear')
   except Exception as e:
-    imports_import_errors['clear'] = e
+    imports_import_errors['clear']=e
+if not 'cls_ANSI' in noimport:
+  try:
+    cls_ANSI=main.cls_ANSI
+    imports_all.append('cls_ANSI')
+  except Exception as e:
+    imports_import_errors['cls_ANSI']=e
 if not 'cls' in noimport:
   try:
-    cls = main.cls
+    cls=main.cls
     imports_all.append('cls')
   except Exception as e:
-    imports_import_errors['cls'] = e
+    imports_import_errors['cls']=e
 if not 'exit' in noimport:
   try:
-    exit = main.exit
+    exit=main.exit
     imports_all.append('exit')
   except Exception as e:
-    imports_import_errors['exit'] = e
+    imports_import_errors['exit']=e
 if not 'pwd' in noimport:
   try:
-    pwd = main.pwd
+    pwd=main.pwd
     imports_all.append('pwd')
   except Exception as e:
-    imports_import_errors['pwd'] = e
+    imports_import_errors['pwd']=e
+if not 'timedelta' in noimport:
+  try:
+    timedelta=main.timedelta
+    imports_all.append('timedelta')
+  except Exception as e:
+    imports_import_errors['timedelta']=e
 if not 'cfg' in noimport:
   try:
     from MainShortcuts.cfg import cfg
     imports_all.append('cfg')
   except Exception as e:
-    imports_import_errors['cfg'] = e
+    imports_import_errors['cfg']=e
 if not 'dictplus' in noimport:
   try:
     from MainShortcuts.dictplus import dictplus
     imports_all.append('dictplus')
   except Exception as e:
-    imports_import_errors['dictplus'] = e
+    imports_import_errors['dictplus']=e
 if not 'fileobj' in noimport:
   try:
     from MainShortcuts.fileobj import fileobj
     imports_all.append('fileobj')
   except Exception as e:
-    imports_import_errors['fileobj'] = e
+    imports_import_errors['fileobj']=e
 if not 'dict' in noimport:
   try:
     import MainShortcuts.dict as dict
     imports_all.append('dict')
   except Exception as e:
-    imports_import_errors['dict'] = e
+    imports_import_errors['dict']=e
 if not 'dir' in noimport:
   try:
     import MainShortcuts.dir as dir
     imports_all.append('dir')
   except Exception as e:
-    imports_import_errors['dir'] = e
+    imports_import_errors['dir']=e
 if not 'file' in noimport:
   try:
     import MainShortcuts.file as file
     imports_all.append('file')
   except Exception as e:
-    imports_import_errors['file'] = e
+    imports_import_errors['file']=e
 if not 'json' in noimport:
   try:
     import MainShortcuts.json as json
     imports_all.append('json')
   except Exception as e:
-    imports_import_errors['json'] = e
+    imports_import_errors['json']=e
 if not 'list' in noimport:
   try:
     import MainShortcuts.list as list
     imports_all.append('list')
   except Exception as e:
-    imports_import_errors['list'] = e
+    imports_import_errors['list']=e
 if not 'os' in noimport:
   try:
     import MainShortcuts.os as os
     imports_all.append('os')
   except Exception as e:
-    imports_import_errors['os'] = e
+    imports_import_errors['os']=e
 if not 'path' in noimport:
   try:
     import MainShortcuts.path as path
     imports_all.append('path')
   except Exception as e:
-    imports_import_errors['path'] = e
+    imports_import_errors['path']=e
 if not 'proc' in noimport:
   try:
     import MainShortcuts.proc as proc
     imports_all.append('proc')
   except Exception as e:
-    imports_import_errors['proc'] = e
+    imports_import_errors['proc']=e
 if not 'str' in noimport:
   try:
     import MainShortcuts.str as str
     imports_all.append('str')
   except Exception as e:
-    imports_import_errors['str'] = e
+    imports_import_errors['str']=e
 if not 'win' in noimport:
   try:
     import MainShortcuts.win as win
     imports_all.append('win')
   except Exception as e:
-    imports_import_errors['win'] = e
-imports_all.sort()
+    imports_import_errors['win']=e
+imports_all.sort()
```

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/json.py` & `mainshortcuts-1.6.96/src/MainShortcuts/json.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/list.py` & `mainshortcuts-1.6.96/src/MainShortcuts/list.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/main.py` & `mainshortcuts-1.6.96/src/MainShortcuts/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import datetime
 import MainShortcuts.os as m_os
 import os as _os
 import sys as _sys
+from typing import Union
 # Универсальные команды
 exit = _sys.exit
 cd = _os.chdir
 pwd = _os.getcwd
 
 
 def clear_ANSI():
   print("\u001b[2J")
-
+def timedelta(time:Union[int,float,dict])->datetime.timedelta:
+  if type(time)==dict:
+    return datetime.timedelta(**time)
+  return datetime.timedelta(seconds=time)
 
 cls_ANSI = clear_ANSI
 # Команды для разных ОС
 if m_os.platform == "Windows":  # Windows
   def clear():
     '''Очистить весь текст в терминале (использует "cls")'''
     _os.system("cls")
```

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/path.py` & `mainshortcuts-1.6.96/src/MainShortcuts/path.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/proc.py` & `mainshortcuts-1.6.96/src/MainShortcuts/proc.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/script.py` & `mainshortcuts-1.6.96/src/MainShortcuts/script.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/str.py` & `mainshortcuts-1.6.96/src/MainShortcuts/str.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/values.py` & `mainshortcuts-1.6.96/src/MainShortcuts/values.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/src/MainShortcuts/win.py` & `mainshortcuts-1.6.96/src/MainShortcuts/win.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.95/PKG-INFO` & `mainshortcuts-1.6.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainShortcuts
-Version: 1.6.95
+Version: 1.6.96
 Summary: Simplifying Python Built-in Commands
 Home-page: https://github.com/MainPlay-TG/MainShortcuts.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

