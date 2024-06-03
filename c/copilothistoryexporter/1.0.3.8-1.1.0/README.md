# Comparing `tmp/copilothistoryexporter-1.0.3.8.tar.gz` & `tmp/copilothistoryexporter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.3.8.tar", last modified: Sun Jun  2 22:59:51 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.1.0.tar", last modified: Mon Jun  3 07:11:15 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.3.8.tar` & `copilothistoryexporter-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.653771 copilothistoryexporter-1.0.3.8/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.8/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)      420 2024-06-02 22:59:51.653550 copilothistoryexporter-1.0.3.8/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.8/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.651127 copilothistoryexporter-1.0.3.8/copilothistoryexporter/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:51:23.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/__init__.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.652032 copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:24:19.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1514 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/binding.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.652772 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/
--rw-r--r--   0 mustafakilic   (501) staff       (20)       68 2024-06-02 22:24:05.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      517 2024-06-02 22:25:29.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/cache.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      651 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/chain.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      205 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/interceptor.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      362 2024-06-02 22:26:15.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/markdown.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      606 2024-06-02 22:26:15.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/vote.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1105 2024-06-02 22:30:47.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/main.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.653139 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      107 2024-06-02 22:24:05.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/conversation.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      251 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/request.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/sample.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2383 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/utils.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.653297 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      420 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      895 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       25 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       23 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 22:59:51.654043 copilothistoryexporter-1.0.3.8/setup.cfg
--rw-r--r--   0 mustafakilic   (501) staff       (20)      911 2024-06-02 22:59:32.000000 copilothistoryexporter-1.0.3.8/setup.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.213134 copilothistoryexporter-1.1.0/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.1.0/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2761 2024-06-03 07:11:15.212929 copilothistoryexporter-1.1.0/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.1.0/README.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      657 2024-06-03 07:00:53.000000 copilothistoryexporter-1.1.0/pyproject.toml
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-03 07:11:15.213172 copilothistoryexporter-1.1.0/setup.cfg
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.210313 copilothistoryexporter-1.1.0/src/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.0/src/__init__.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.210761 copilothistoryexporter-1.1.0/src/copilothistoryexporter/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/__init__.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.211655 copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 05:45:17.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1516 2024-06-03 07:04:53.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/binding.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.212344 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-03 06:01:46.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      517 2024-06-03 07:05:36.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/cache.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      652 2024-06-03 07:05:46.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/chain.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      205 2024-06-03 07:05:50.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/interceptor.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      362 2024-06-03 07:05:56.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/markdown.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      606 2024-06-03 07:06:02.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/vote.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1158 2024-06-03 07:06:39.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/main.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.212583 copilothistoryexporter-1.1.0/src/copilothistoryexporter/model/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/model/conversation.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      251 2024-06-03 07:06:09.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/model/request.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/sample.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2383 2024-06-03 07:06:54.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-03 07:11:15.212738 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2761 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      956 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       25 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       32 2024-06-03 07:11:15.000000 copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/top_level.txt
```

### Comparing `copilothistoryexporter-1.0.3.8/LICENCE` & `copilothistoryexporter-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.8/README.md` & `copilothistoryexporter-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/binding.py` & `copilothistoryexporter-1.1.0/src/copilothistoryexporter/addons/binding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import re
 
 from mitmproxy import http
 
+
 from copilothistoryexporter.intercp.chain import InterceptorChain
 from copilothistoryexporter.model.conversation import Conversation
 from copilothistoryexporter.model.request import Request
 
+
 LISTEN_URL = "https://api.githubcopilot.com/chat/completions"
 LISTEN_URL_RATING = "https://copilot-telemetry.githubusercontent.com/telemetry"
 
 chain = InterceptorChain()
 
 
 def get_message_from_response(data) -> list[Conversation]:
```

### Comparing `copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/cache.py` & `copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/cache.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/chain.py` & `copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from copilothistoryexporter.intercp.cache import CacheInterceptor
 from copilothistoryexporter.intercp.markdown import MarkdownInterceptor
 from copilothistoryexporter.intercp.vote import VoteInterceptor
 from copilothistoryexporter.model.request import Request
 
+
 class InterceptorChain:
     def __init__(self):
         self.interceptors = [
             VoteInterceptor(),
             CacheInterceptor(),
             MarkdownInterceptor()
         ]
```

### Comparing `copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/vote.py` & `copilothistoryexporter-1.1.0/src/copilothistoryexporter/intercp/vote.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.8/copilothistoryexporter/main.py` & `copilothistoryexporter-1.1.0/src/copilothistoryexporter/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 import subprocess
 import traceback
 
 import click
 
-from .utils import SharedValues
+from copilothistoryexporter.utils import SharedValues
 
 
 @click.command()
 @click.option('--port', default=9696, help='Running port')
 @click.option('--debug', default=False, help='Debug mode')
 @click.argument('project', type=click.Path(exists=True, writable=True), required=False)
 def main(port, debug, project):
     project = os.path.abspath(project) if project else os.getcwd()
     SharedValues.change_workspace(project)
     script = os.path.join(os.path.dirname(__file__), "addons", "binding.py")
     launch = "mitmdump" if not debug else "mitmweb"
     shell = f"{launch} -s {script} -p {port}"
     print(f"running on --port {port} --debug {debug} {project}")
     print("running mitm with command: ", shell)
+
     subprocess.run(shell, shell=True)
 
 
 def sys_main():
     """
     Runs the main function using the system cli arguments, and
     returns a system error code.
@@ -33,8 +34,9 @@
         main()
         return 0
     except Exception:
         print(traceback.format_exc())
         return 1
 
 
-sys_main()
+if __name__ == '__main__':
+    sys_main()
```

### Comparing `copilothistoryexporter-1.0.3.8/copilothistoryexporter/utils.py` & `copilothistoryexporter-1.1.0/src/copilothistoryexporter/utils.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/SOURCES.txt` & `copilothistoryexporter-1.1.0/src/copilothistoryexporter.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENCE
 README.md
-setup.py
-copilothistoryexporter/__init__.py
-copilothistoryexporter/main.py
-copilothistoryexporter/sample.md
-copilothistoryexporter/utils.py
-copilothistoryexporter.egg-info/PKG-INFO
-copilothistoryexporter.egg-info/SOURCES.txt
-copilothistoryexporter.egg-info/dependency_links.txt
-copilothistoryexporter.egg-info/entry_points.txt
-copilothistoryexporter.egg-info/requires.txt
-copilothistoryexporter.egg-info/top_level.txt
-copilothistoryexporter/addons/__init__.py
-copilothistoryexporter/addons/binding.py
-copilothistoryexporter/intercp/__init__.py
-copilothistoryexporter/intercp/cache.py
-copilothistoryexporter/intercp/chain.py
-copilothistoryexporter/intercp/interceptor.py
-copilothistoryexporter/intercp/markdown.py
-copilothistoryexporter/intercp/vote.py
-copilothistoryexporter/model/__init__.py
-copilothistoryexporter/model/conversation.py
-copilothistoryexporter/model/request.py
+pyproject.toml
+src/__init__.py
+src/copilothistoryexporter/__init__.py
+src/copilothistoryexporter/main.py
+src/copilothistoryexporter/sample.md
+src/copilothistoryexporter/utils.py
+src/copilothistoryexporter.egg-info/PKG-INFO
+src/copilothistoryexporter.egg-info/SOURCES.txt
+src/copilothistoryexporter.egg-info/dependency_links.txt
+src/copilothistoryexporter.egg-info/entry_points.txt
+src/copilothistoryexporter.egg-info/requires.txt
+src/copilothistoryexporter.egg-info/top_level.txt
+src/copilothistoryexporter/addons/__init__.py
+src/copilothistoryexporter/addons/binding.py
+src/copilothistoryexporter/intercp/__init__.py
+src/copilothistoryexporter/intercp/cache.py
+src/copilothistoryexporter/intercp/chain.py
+src/copilothistoryexporter/intercp/interceptor.py
+src/copilothistoryexporter/intercp/markdown.py
+src/copilothistoryexporter/intercp/vote.py
+src/copilothistoryexporter/model/conversation.py
+src/copilothistoryexporter/model/request.py
```

