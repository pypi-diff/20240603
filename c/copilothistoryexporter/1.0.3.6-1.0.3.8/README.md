# Comparing `tmp/copilothistoryexporter-1.0.3.6.tar.gz` & `tmp/copilothistoryexporter-1.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.3.6.tar", last modified: Sun Jun  2 20:57:46 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.3.8.tar", last modified: Sun Jun  2 22:59:51 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.3.6.tar` & `copilothistoryexporter-1.0.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966991 copilothistoryexporter-1.0.3.6/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.6/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:57:46.966819 copilothistoryexporter-1.0.3.6/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.6/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966653 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      610 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       53 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        4 2024-06-02 20:57:46.000000 copilothistoryexporter-1.0.3.6/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:57:46.967025 copilothistoryexporter-1.0.3.6/setup.cfg
--rw-r--r--   0 mustafakilic   (501) staff       (20)      732 2024-06-02 20:57:40.000000 copilothistoryexporter-1.0.3.6/setup.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.965382 copilothistoryexporter-1.0.3.6/src/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:51:23.000000 copilothistoryexporter-1.0.3.6/src/__init__.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.965582 copilothistoryexporter-1.0.3.6/src/addons/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:52:06.000000 copilothistoryexporter-1.0.3.6/src/addons/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1457 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/addons/binding.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966212 copilothistoryexporter-1.0.3.6/src/intercp/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:55:28.000000 copilothistoryexporter-1.0.3.6/src/intercp/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      460 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/cache.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      575 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/chain.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      186 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/interceptor.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      305 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/markdown.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      549 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/intercp/vote.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1136 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/main.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:57:46.966507 copilothistoryexporter-1.0.3.6/src/model/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/model/__init__.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.6/src/model/conversation.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)      232 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/model/request.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.6/src/sample.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2364 2024-06-02 20:55:47.000000 copilothistoryexporter-1.0.3.6/src/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.653771 copilothistoryexporter-1.0.3.8/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.8/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      420 2024-06-02 22:59:51.653550 copilothistoryexporter-1.0.3.8/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.8/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.651127 copilothistoryexporter-1.0.3.8/copilothistoryexporter/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:51:23.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/__init__.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.652032 copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:24:19.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1514 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/binding.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.652772 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       68 2024-06-02 22:24:05.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      517 2024-06-02 22:25:29.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/cache.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      651 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/chain.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      205 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/interceptor.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      362 2024-06-02 22:26:15.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/markdown.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      606 2024-06-02 22:26:15.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/vote.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1105 2024-06-02 22:30:47.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/main.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.653139 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      107 2024-06-02 22:24:05.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/__init__.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      395 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/conversation.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      251 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/model/request.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/sample.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2383 2024-06-02 21:17:18.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 22:59:51.653297 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      420 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      895 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       25 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       23 2024-06-02 22:59:51.000000 copilothistoryexporter-1.0.3.8/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 22:59:51.654043 copilothistoryexporter-1.0.3.8/setup.cfg
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      911 2024-06-02 22:59:32.000000 copilothistoryexporter-1.0.3.8/setup.py
```

### Comparing `copilothistoryexporter-1.0.3.6/LICENCE` & `copilothistoryexporter-1.0.3.8/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.6/README.md` & `copilothistoryexporter-1.0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.6/setup.py` & `copilothistoryexporter-1.0.3.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import os
 
 from setuptools import setup, find_packages
 
+
+def read_file(filename):
+    full_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), filename)
+    with open(full_path, "rt", encoding="utf-8") as f:
+        lines = f.readlines()
+    return lines
+
+
 setup(
     name="copilothistoryexporter",
-    version='1.0.3.6',
+    version='1.0.3.8',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kilic',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
     packages=find_packages(),
     package_data={'': ['*.md']},
     install_requires=[
         "requests",
         "click",
         "mitmproxy",
-        "wheel",
-        "setuptools",
     ],
-    entry_points={
-        'console_scripts': [
-            'copilothistoryexporter = main:main'
-        ]
-    },
+    entry_points='''
+     [console_scripts]
+     copilothistoryexporter=copilothistoryexporter.main:sys_main
+     '''
 )
```

### Comparing `copilothistoryexporter-1.0.3.6/src/addons/binding.py` & `copilothistoryexporter-1.0.3.8/copilothistoryexporter/addons/binding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
 from mitmproxy import http
 
-from src.intercp.chain import InterceptorChain
-from src.model.conversation import Conversation
-from src.model.request import Request
+from copilothistoryexporter.intercp.chain import InterceptorChain
+from copilothistoryexporter.model.conversation import Conversation
+from copilothistoryexporter.model.request import Request
 
 LISTEN_URL = "https://api.githubcopilot.com/chat/completions"
 LISTEN_URL_RATING = "https://copilot-telemetry.githubusercontent.com/telemetry"
 
 chain = InterceptorChain()
```

### Comparing `copilothistoryexporter-1.0.3.6/src/intercp/vote.py` & `copilothistoryexporter-1.0.3.8/copilothistoryexporter/intercp/vote.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from src import utils
-from src.intercp.interceptor import Interceptor
-from src.model.request import Request
+from copilothistoryexporter import utils
+from copilothistoryexporter.intercp.interceptor import Interceptor
+from copilothistoryexporter.model.request import Request
 
 
 class VoteInterceptor(Interceptor):
     def process(self, request: Request):
         prompt = request.conversation.prompt
         if prompt == "vote:good" or prompt == "vote:bad":
             conversations = utils.get_json_files()
```

### Comparing `copilothistoryexporter-1.0.3.6/src/main.py` & `copilothistoryexporter-1.0.3.8/copilothistoryexporter/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import subprocess
 import traceback
 
 import click
 
-from utils import SharedValues
-
+from .utils import SharedValues
 
 
 @click.command()
 @click.option('--port', default=9696, help='Running port')
 @click.option('--debug', default=False, help='Debug mode')
 @click.argument('project', type=click.Path(exists=True, writable=True), required=False)
 def main(port, debug, project):
@@ -34,9 +33,8 @@
         main()
         return 0
     except Exception:
         print(traceback.format_exc())
         return 1
 
 
-if __name__ == '__main__':
-    sys_main()
+sys_main()
```

### Comparing `copilothistoryexporter-1.0.3.6/src/utils.py` & `copilothistoryexporter-1.0.3.8/copilothistoryexporter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 
 import subprocess
 
-from src.model.conversation import Conversation
+from copilothistoryexporter.model.conversation import Conversation
 
 
 class SharedValues:
     WORKSPACE = ""
 
     @staticmethod
     def change_workspace(src: str):
```

