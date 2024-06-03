# Comparing `tmp/rssbot-556.tar.gz` & `tmp/rssbot-557.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssbot-556.tar", last modified: Thu May 23 18:37:34 2024, max compression
+gzip compressed data, was "rssbot-557.tar", last modified: Mon Jun  3 12:27:03 2024, max compression
```

## Comparing `rssbot-556.tar` & `rssbot-557.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.073503 rssbot-556/
--rw-r--r--   0 bart      (1000) bart      (1001)     2378 2024-05-23 18:37:34.073503 rssbot-556/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1841 2024-05-23 18:37:14.000000 rssbot-556/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.069503 rssbot-556/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2537 2024-05-22 15:24:52.000000 rssbot-556/bin/rssbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1921 2024-05-22 15:24:52.000000 rssbot-556/bin/rssbotd
--rw-r--r--   0 bart      (1000) bart      (1001)      861 2024-05-22 15:24:52.000000 rssbot-556/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.069503 rssbot-556/rssbot/
--rw-r--r--   0 bart      (1000) bart      (1001)       72 2024-05-22 15:24:52.000000 rssbot-556/rssbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-22 15:24:52.000000 rssbot-556/rssbot/broker.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-22 15:24:52.000000 rssbot-556/rssbot/client.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-22 15:24:52.000000 rssbot-556/rssbot/disk.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2002 2024-05-23 01:28:27.000000 rssbot-556/rssbot/find.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-22 15:24:52.000000 rssbot-556/rssbot/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-22 15:24:52.000000 rssbot-556/rssbot/log.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.073503 rssbot-556/rssbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      294 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18778 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3112 2024-05-23 13:09:07.000000 rssbot-556/rssbot/modules/opm.py
--rw-r--r--   0 bart      (1000) bart      (1001)     8892 2024-05-23 13:13:33.000000 rssbot-556/rssbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-23 01:33:08.000000 rssbot-556/rssbot/object.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-22 15:24:52.000000 rssbot-556/rssbot/run.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-22 15:24:52.000000 rssbot-556/rssbot/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.069503 rssbot-556/rssbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     2378 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      521 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-23 18:37:34.073503 rssbot-556/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      185 2024-05-22 15:24:52.000000 rssbot-556/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-06-03 12:27:03.829855 rssbot-557/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2421 2024-06-03 12:27:03.825855 rssbot-557/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1884 2024-06-03 03:08:32.000000 rssbot-557/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-06-03 12:27:03.825855 rssbot-557/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2537 2024-05-25 12:36:48.000000 rssbot-557/bin/rssbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1935 2024-06-03 02:54:24.000000 rssbot-557/bin/rssbotd
+-rw-r--r--   0 bart      (1000) bart      (1001)      861 2024-05-25 12:36:41.000000 rssbot-557/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-06-03 12:27:03.825855 rssbot-557/rssbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)       72 2024-05-22 15:24:52.000000 rssbot-557/rssbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2144 2024-05-25 11:42:18.000000 rssbot-557/rssbot/attrs.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-22 15:24:52.000000 rssbot-557/rssbot/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-22 15:24:52.000000 rssbot-557/rssbot/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-22 15:24:52.000000 rssbot-557/rssbot/disk.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2002 2024-05-23 01:28:27.000000 rssbot-557/rssbot/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-22 15:24:52.000000 rssbot-557/rssbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-22 15:24:52.000000 rssbot-557/rssbot/log.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-06-03 12:27:03.825855 rssbot-557/rssbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      294 2024-05-22 15:24:52.000000 rssbot-557/rssbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-22 15:24:52.000000 rssbot-557/rssbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-22 15:24:52.000000 rssbot-557/rssbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18778 2024-05-22 15:24:52.000000 rssbot-557/rssbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-22 15:24:52.000000 rssbot-557/rssbot/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3203 2024-05-26 06:21:49.000000 rssbot-557/rssbot/modules/opm.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     8892 2024-05-23 13:13:33.000000 rssbot-557/rssbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-22 15:24:52.000000 rssbot-557/rssbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6265 2024-06-03 02:51:58.000000 rssbot-557/rssbot/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-22 15:24:52.000000 rssbot-557/rssbot/run.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-22 15:24:52.000000 rssbot-557/rssbot/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      561 2024-05-25 11:45:20.000000 rssbot-557/rssbot/utils.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-06-03 12:27:03.825855 rssbot-557/rssbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2421 2024-06-03 12:27:03.000000 rssbot-557/rssbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      553 2024-06-03 12:27:03.000000 rssbot-557/rssbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-06-03 12:27:03.000000 rssbot-557/rssbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-06-03 12:27:03.000000 rssbot-557/rssbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-06-03 12:27:03.829855 rssbot-557/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      185 2024-05-22 15:24:52.000000 rssbot-557/setup.py
```

### Comparing `rssbot-556/PKG-INFO` & `rssbot-557/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 556
+Version: 557
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
@@ -113,15 +113,16 @@
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.rssbot
     ExecStart=/home/<user>/.local/pipx/venvs/rssbot/bin/rssbotd
-    RemainAfterExit=yes
+    PIDFile=/home/<user>/.rssbot/rssbot.pid
+    RemainAfterExit=no
 
     [Install]
     WantedBy=default.target
 
 
 then run this
```

### Comparing `rssbot-556/README.rst` & `rssbot-557/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,16 @@
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.rssbot
     ExecStart=/home/<user>/.local/pipx/venvs/rssbot/bin/rssbotd
-    RemainAfterExit=yes
+    PIDFile=/home/<user>/.rssbot/rssbot.pid
+    RemainAfterExit=no
 
     [Install]
     WantedBy=default.target
 
 
 then run this
```

### Comparing `rssbot-556/bin/rssbot` & `rssbot-557/bin/rssbot`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 Cfg             = Default()
 Cfg.dis         = ""
 Cfg.mod         = "cmd,irc,mod,opm,rss"
 Cfg.opts        = ""
 Cfg.name        = __file__.rsplit(os.sep, maxsplit=1)[-1]
-Cfg.version     = "556"
+Cfg.version     = "557"
 Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
 
 
 Workdir.workdir = Cfg.wdr
```

### Comparing `rssbot-556/bin/rssbotd` & `rssbot-557/bin/rssbotd`

 * *Files 22% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 import pathlib
 import pwd
 import sys
 import time
 
 
 from rssbot.disk   import Workdir, skel
-from rssbot.object import Default
+from rssbot.object import Default, cdir
 from rssbot.run    import init, scan
 from rssbot.thread import errors
 
 
 from rssbot import modules
 
 
 Cfg             = Default()
 Cfg.dis         = ""
 Cfg.name        = "rssbot"
-Cfg.mod         = "cmd,irc,mod,rss"
-Cfg.version     = "556"
+Cfg.mod         = "irc,rss"
+Cfg.version     = "557"
 Cfg.opts        = ""
 Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
 
 
 Workdir.workdir = Cfg.wdr
 
 
-def daemon(pidfile, verbose=False):
+def daemon(verbose=False):
     "switch to background."
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
@@ -51,37 +51,42 @@
             os.dup2(sis.fileno(), sys.stdin.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as sos:
             os.dup2(sos.fileno(), sys.stdout.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as ses:
             os.dup2(ses.fileno(), sys.stderr.fileno())
     os.umask(0)
     os.chdir("/")
-    if os.path.exists(pidfile):
-        os.unlink(pidfile)
-    path = pathlib.Path(pidfile)
-    path.parent.mkdir(parents=True, exist_ok=True)
-    with open(pidfile, "w", encoding="utf-8") as fds:
+
+
+def pidfile(path):
+    if os.path.exists(path):
+        os.unlink(path)
+    cdir(path)
+    with open(path, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
 def privileges(username):
     "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
 def main():
     "main"
     skel()
     Cfg.user = getpass.getuser()
-    daemon(Cfg.pidfile, "-v" in sys.argv)
+    if "-d" in sys.argv:
+        daemon("-v" in sys.argv)
+    pidfile(Cfg.pidfile)
     privileges(Cfg.user)
     scan(modules, Cfg.mod)
     init(modules, Cfg.mod)
     while 1:
-        time.sleep(1.0)
-
+        try:
+            time.sleep(1.0)
+        except:
+            errors() 
 
 if __name__ == "__main__":
     main()
-    errors()
```

### Comparing `rssbot-556/pyproject.toml` & `rssbot-557/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "rssbot"
 description = "24/7 feed fetcher"
-version = "556"
+version = "557"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
```

### Comparing `rssbot-556/rssbot/broker.py` & `rssbot-557/rssbot/broker.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/client.py` & `rssbot-557/rssbot/client.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/disk.py` & `rssbot-557/rssbot/disk.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/find.py` & `rssbot-557/rssbot/find.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/handler.py` & `rssbot-557/rssbot/handler.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/modules/irc.py` & `rssbot-557/rssbot/modules/irc.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/modules/opm.py` & `rssbot-557/rssbot/modules/opm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # This file is placed in the Public Domain.
 
 
 "outline processor markup language"
 
 
+import uuid
+
+
 from ..disk   import sync
 from ..find   import find
 from ..object import Default, construct
-from ..run    import spl
+from ..utils  import shortid, spl
 
 
 from .rss import Rss
 
 
 TEMPLATE = """<opml version="1.0">
     <head>
@@ -104,17 +107,20 @@
         event.reply("imp <filename>")
         return
     fnm = event.args[0]
     with open(fnm, "r", encoding="utf-8") as file:
         txt = file.read()
     prs = Parser()
     nrs = 0
+    id = shortid()
     for obj in prs.parse(txt, 'outline', "name,display_list,xmlUrl"):
         nrs += 1
         if obj.xmlUrl and find("rss", {"rss": obj.xmlUrl}):
             event.reply(f"skipping {obj.xmlUrl}")
             continue
         rss = Rss()
         construct(rss, obj)
         rss.rss = rss.xmlUrl
+        rss.id = id
         sync(rss)
-        event.reply(obj)
+    if nrs:
+        event.reply(f"added {nrs} urls.")
```

### Comparing `rssbot-556/rssbot/modules/rss.py` & `rssbot-557/rssbot/modules/rss.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/modules/thr.py` & `rssbot-557/rssbot/modules/thr.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/object.py` & `rssbot-557/rssbot/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,19 @@
 
 def dumps(*args, **kw):
     "dump object to string."
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
 
 
+def cdir(pth):
+    path = pathlib.Path(pth)
+    path.parent.mkdir(parents=True, exist_ok=True)
+
+
 def __dir__():
     return (
         'Object',
         'Default',
         'construct',
         'dump',
         'dumps',
```

### Comparing `rssbot-556/rssbot/run.py` & `rssbot-557/rssbot/run.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot/thread.py` & `rssbot-557/rssbot/thread.py`

 * *Files identical despite different names*

### Comparing `rssbot-556/rssbot.egg-info/PKG-INFO` & `rssbot-557/rssbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 556
+Version: 557
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
@@ -113,15 +113,16 @@
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.rssbot
     ExecStart=/home/<user>/.local/pipx/venvs/rssbot/bin/rssbotd
-    RemainAfterExit=yes
+    PIDFile=/home/<user>/.rssbot/rssbot.pid
+    RemainAfterExit=no
 
     [Install]
     WantedBy=default.target
 
 
 then run this
```

### Comparing `rssbot-556/rssbot.egg-info/SOURCES.txt` & `rssbot-557/rssbot.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 README.rst
 pyproject.toml
 setup.py
 bin/rssbot
 bin/rssbotd
 rssbot/__init__.py
+rssbot/attrs.py
 rssbot/broker.py
 rssbot/client.py
 rssbot/disk.py
 rssbot/find.py
 rssbot/handler.py
 rssbot/log.py
 rssbot/object.py
 rssbot/run.py
 rssbot/thread.py
+rssbot/utils.py
 rssbot.egg-info/PKG-INFO
 rssbot.egg-info/SOURCES.txt
 rssbot.egg-info/dependency_links.txt
 rssbot.egg-info/top_level.txt
 rssbot/modules/__init__.py
 rssbot/modules/cmd.py
 rssbot/modules/err.py
```

