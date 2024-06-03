# Comparing `tmp/symmetricjsonrpc3-0.2.0.tar.gz` & `tmp/symmetricjsonrpc3-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symmetricjsonrpc3-0.2.0.tar", last modified: Wed May 29 13:39:26 2024, max compression
+gzip compressed data, was "symmetricjsonrpc3-0.3.0.tar", last modified: Mon Jun  3 06:59:50 2024, max compression
```

## Comparing `symmetricjsonrpc3-0.2.0.tar` & `symmetricjsonrpc3-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-05-29 13:39:26.898848 symmetricjsonrpc3-0.2.0/
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      100 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/.gitignore
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)    17987 2022-04-25 11:45:00.000000 symmetricjsonrpc3-0.2.0/COPYING
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)    26434 2022-04-25 11:45:00.000000 symmetricjsonrpc3-0.2.0/COPYING.LESSER
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2402 2024-05-29 13:39:26.898848 symmetricjsonrpc3-0.2.0/PKG-INFO
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1568 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/README.txt
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-05-29 13:39:26.898848 symmetricjsonrpc3-0.2.0/examples/
--rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     2368 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/examples/client.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2059 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/examples/client_emulate.py
--rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     3184 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/examples/server.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1788 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/examples/server_emulate.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      915 2024-05-29 10:42:52.000000 symmetricjsonrpc3-0.2.0/examples/ssl_client.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1033 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/pyproject.toml
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       38 2024-05-29 13:39:26.898848 symmetricjsonrpc3-0.2.0/setup.cfg
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-05-29 13:39:26.898848 symmetricjsonrpc3-0.2.0/src/
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-05-29 13:39:26.898848 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/
--rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     1490 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/__init__.py
--rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     5063 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/dispatcher.py
--rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)    19706 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/json.py
--rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)    12935 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/rpc.py
--rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     5458 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/wrappers.py
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-05-29 13:39:26.898848 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3.egg-info/
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2402 2024-05-29 13:39:26.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3.egg-info/PKG-INFO
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      517 2024-05-29 13:39:26.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3.egg-info/SOURCES.txt
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2024-05-29 13:39:26.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3.egg-info/dependency_links.txt
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       18 2024-05-29 13:39:26.000000 symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3.egg-info/top_level.txt
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-06-03 06:59:50.540134 symmetricjsonrpc3-0.3.0/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      100 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.3.0/.gitignore
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)    17987 2022-04-25 11:45:00.000000 symmetricjsonrpc3-0.3.0/COPYING
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)    26434 2022-04-25 11:45:00.000000 symmetricjsonrpc3-0.3.0/COPYING.LESSER
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2372 2024-06-03 06:59:50.540134 symmetricjsonrpc3-0.3.0/PKG-INFO
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1537 2024-06-03 06:32:44.000000 symmetricjsonrpc3-0.3.0/README.txt
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-06-03 06:59:50.540134 symmetricjsonrpc3-0.3.0/examples/
+-rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     2368 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.3.0/examples/client.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2059 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.3.0/examples/client_emulate.py
+-rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     3184 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.3.0/examples/server.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1788 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.3.0/examples/server_emulate.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      915 2024-05-29 10:42:52.000000 symmetricjsonrpc3-0.3.0/examples/ssl_client.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1034 2024-06-03 06:36:01.000000 symmetricjsonrpc3-0.3.0/pyproject.toml
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       38 2024-06-03 06:59:50.540134 symmetricjsonrpc3-0.3.0/setup.cfg
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-06-03 06:59:50.536134 symmetricjsonrpc3-0.3.0/src/
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-06-03 06:59:50.540134 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/
+-rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     1490 2024-05-29 12:06:28.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/__init__.py
+-rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     5294 2024-06-03 06:32:44.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/dispatcher.py
+-rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)    15047 2024-06-03 06:32:44.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/json.py
+-rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     6804 2024-06-03 06:32:44.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/rpc.py
+-rwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)     5730 2024-06-03 06:32:44.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/wrappers.py
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-06-03 06:59:50.540134 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3.egg-info/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2372 2024-06-03 06:59:50.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3.egg-info/PKG-INFO
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      554 2024-06-03 06:59:50.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3.egg-info/SOURCES.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2024-06-03 06:59:50.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3.egg-info/dependency_links.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       18 2024-06-03 06:59:50.000000 symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3.egg-info/top_level.txt
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2024-06-03 06:59:50.540134 symmetricjsonrpc3-0.3.0/tests/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     6373 2024-06-03 06:54:49.000000 symmetricjsonrpc3-0.3.0/tests/test_json.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     7337 2024-06-03 06:43:24.000000 symmetricjsonrpc3-0.3.0/tests/test_rpc.py
```

### Comparing `symmetricjsonrpc3-0.2.0/COPYING` & `symmetricjsonrpc3-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/COPYING.LESSER` & `symmetricjsonrpc3-0.3.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/PKG-INFO` & `symmetricjsonrpc3-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: symmetricjsonrpc3
-Version: 0.2.0
+Version: 0.3.0
 Summary: A symmetric, transport-layer agnostic JSON RPC.
 Author-email: Egil Moeller <redhog@redhog.org>, Nicklas Lindgren <nili@gulmohar.se>, "Robert \"Robikz\" Zalewski" <zalewapl@gmail.com>
 Maintainer-email: "Robert \"Robikz\" Zalewski" <zalewapl@gmail.com>
 Project-URL: Source, https://github.com/Zalewa/python-symmetricjsonrpc3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8.1
 Description-Content-Type: text/plain
 License-File: COPYING
 License-File: COPYING.LESSER
 
 Python Symmetric JSON-RPC 3
 ===========================
 
-"A symmetric, transport-layer agnostic JSON-RPC implemenation in python."
+"A symmetric, transport-layer agnostic JSON-RPC implementation in Python."
 
-A JSON-RPC (see https://jsonrpc.org) implementation for Python, with
+A JSON-RPC (see https://jsonrpc.org) implementation for Python with
 the following features:
 
- * Symmetric - both the connecting and the listening process can send
-   and receive method calls, there is no specific "server" or "client"
+ * Symmetric - both the connecting and the listening processes can send
+   and receive method calls. There is no specific "server" or "client"
    process, and no difference between the two connection ends apart
    from who initiates the connection.
 
- * Asynchronous - calls can be interlieved with new calls initiated
+ * Asynchronous - calls can be interleaved with new calls initiated
    before a previous call has returned.
 
  * Thread-safe - calls to the remote side can be done from multiple
    threads without any locking.
 
  * Transport agnostic - can run on top of anything that resembles a
-   socket the slightest (e.g. OpenSSL)
+   socket in the slightest (e.g. OpenSSL)
 
-  * Dependency free
+ * Dependency free
 
-What this really drills down to is that this library implements the
-full specification of JSON-RPC over sockets.
+This library implements the full specification of JSON-RPC over sockets.
 
   This is a fork of niligulmohar's "symmetricjsonrpc" with the intent
   of bringing it up-to-date with current Python and publishing it
   to PyPI.
 
 For usage details, look at the examples in the "examples" directory.
 
 Conventions
 ===========
 
-The conventions apply only since forking from the original repository.
+The conventions apply only after the point of forking from the original
+repository.
 
-This project uses/follows/adheres to:
+This project adheres to:
 
 - Conventional Commits 1.0.0 (https://www.conventionalcommits.org/)
 - PyPA version scheme (https://packaging.python.org/en/latest/specifications/version-specifiers/)
 
 Git tags are prefixed with 'v'.
 
-Module's version is automatically deduced from the git tag in the
+The package's version is automatically deduced from the git tag in the
 "no-guess-dev" mode.
```

### Comparing `symmetricjsonrpc3-0.2.0/README.txt` & `symmetricjsonrpc3-0.3.0/README.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Python Symmetric JSON-RPC 3
 ===========================
 
-"A symmetric, transport-layer agnostic JSON-RPC implemenation in python."
+"A symmetric, transport-layer agnostic JSON-RPC implementation in Python."
 
-A JSON-RPC (see https://jsonrpc.org) implementation for Python, with
+A JSON-RPC (see https://jsonrpc.org) implementation for Python with
 the following features:
 
- * Symmetric - both the connecting and the listening process can send
-   and receive method calls, there is no specific "server" or "client"
+ * Symmetric - both the connecting and the listening processes can send
+   and receive method calls. There is no specific "server" or "client"
    process, and no difference between the two connection ends apart
    from who initiates the connection.
 
- * Asynchronous - calls can be interlieved with new calls initiated
+ * Asynchronous - calls can be interleaved with new calls initiated
    before a previous call has returned.
 
  * Thread-safe - calls to the remote side can be done from multiple
    threads without any locking.
 
  * Transport agnostic - can run on top of anything that resembles a
-   socket the slightest (e.g. OpenSSL)
+   socket in the slightest (e.g. OpenSSL)
 
-  * Dependency free
+ * Dependency free
 
-What this really drills down to is that this library implements the
-full specification of JSON-RPC over sockets.
+This library implements the full specification of JSON-RPC over sockets.
 
   This is a fork of niligulmohar's "symmetricjsonrpc" with the intent
   of bringing it up-to-date with current Python and publishing it
   to PyPI.
 
 For usage details, look at the examples in the "examples" directory.
 
 Conventions
 ===========
 
-The conventions apply only since forking from the original repository.
+The conventions apply only after the point of forking from the original
+repository.
 
-This project uses/follows/adheres to:
+This project adheres to:
 
 - Conventional Commits 1.0.0 (https://www.conventionalcommits.org/)
 - PyPA version scheme (https://packaging.python.org/en/latest/specifications/version-specifiers/)
 
 Git tags are prefixed with 'v'.
 
-Module's version is automatically deduced from the git tag in the
+The package's version is automatically deduced from the git tag in the
 "no-guess-dev" mode.
```

### Comparing `symmetricjsonrpc3-0.2.0/examples/client.py` & `symmetricjsonrpc3-0.3.0/examples/client.py`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/examples/client_emulate.py` & `symmetricjsonrpc3-0.3.0/examples/client_emulate.py`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/examples/server.py` & `symmetricjsonrpc3-0.3.0/examples/server.py`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/examples/server_emulate.py` & `symmetricjsonrpc3-0.3.0/examples/server_emulate.py`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/examples/ssl_client.py` & `symmetricjsonrpc3-0.3.0/examples/ssl_client.py`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/pyproject.toml` & `symmetricjsonrpc3-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     { name = 'Robert "Robikz" Zalewski', email = "zalewapl@gmail.com" },
 ]
 maintainers = [
     { name = 'Robert "Robikz" Zalewski', email = "zalewapl@gmail.com" },
 ]
 readme = "README.txt"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
     "Topic :: System :: Networking",
 ]
 requires-python = ">=3.8.1"
```

### Comparing `symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/__init__.py` & `symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/__init__.py`

 * *Files identical despite different names*

### Comparing `symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/dispatcher.py` & `symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/dispatcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 # -*- coding: utf-8 -*-
 # vim: set fileencoding=UTF-8 :
 
 # python-symmetricjsonrpc3
 # Copyright (C) 2009 Egil Moeller <redhog@redhog.org>
 # Copyright (C) 2009 Nicklas Lindgren <nili@gulmohar.se>
 # Copyright (C) 2024 Robert "Robikz" Zalewski <zalewapl@gmail.com>
-
+#
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
-
+#
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Lesser General Public License for more details.
-
+#
 # You should have received a copy of the GNU Lesser General Public
 # License along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307
 # USA
 
-"""Facilities for managing a hirearchy of threads each providing a
+"""Facilities for managing a hierarchy of threads each providing a
 synchronous I/O interface."""
 
 import select
 import threading
-import traceback
+from logging import getLogger
+
+
+logger = getLogger(__name__)
 
 
 class Thread(threading.Thread):
     """This class is the base class for a set of threading.Thread
     subclasses that provides automatic start, some debugging print-out
     for start/stop, a subject resource to manage (like a socket), and
     possibly a child/parent relationship with another thread."""
@@ -48,64 +51,78 @@
         self.subject = subject
         self.parent = parent
         if hasattr(self.parent, "children"):
             self.parent.children.append(self)
         self._shutdown = False
         if 'name' not in kw:
             if self.parent:
-                kw['name'] = "%s/%s" % (self.parent.getName(), type(self).__name__)
+                kw['name'] = "%s/%s" % (self.parent.name, type(self).__name__)
             else:
                 kw['name'] = type(self).__name__
         threading.Thread.__init__(self, *arg, **kw)
 
     def _exit(self):
         for child in list(self.children):
             child.join()
         if hasattr(self.parent, "children"):
             self.parent.children.remove(self)
 
     def run(self, *arg, **kw):
-        if self.debug_thread: print("%s: BEGIN" % self.getName())
+        self._dbg("%s: BEGIN", self.name)
         self.run_thread(*arg, **kw)
-        if self.debug_thread: print("%s: TEARDOWN: %s" % (self.getName(), ', '.join(child.getName() for child in self.children)))
+        if self.debug_thread:  # perf check -- avoid the unnecessary join loop
+            self._dbg("%s: TEARDOWN: %s", self.name,
+                      ', '.join(child.name for child in self.children))
         self._exit()
-        if self.debug_thread: print("%s: END" % self.getName())
+        self._dbg("%s: END", self.name)
 
     def shutdown(self):
-        if self.debug_thread: print("%s: shutdown: %s" % (threading.currentThread().getName(), self.getName(),))
+        self._dbg("%s: shutdown: %s",
+                  threading.current_thread().name, self.name)
         for child in list(self.children):
             child.shutdown()
         self._shutdown = True
-        if self.debug_thread: print("%s: shutdown done: %s" % (threading.currentThread().getName(), self.getName(),))
+        self._dbg("%s: shutdown done: %s",
+                  threading.current_thread().name, self.name)
 
     def run_parent(self):
         pass
 
     def run_thread(self, *arg, **kw):
         pass
 
+    def _dbg(self, fmt, *args, **kwargs):
+        if self.debug_thread:
+            logger.debug(fmt, *args, **kwargs)
+
+
 class Connection(Thread):
     """A connection manager thread base class."""
 
     debug_dispatch = False
 
     _dispatcher_class = "Request"
 
     def run_thread(self):
         for value in self.read():
-            if self.debug_dispatch: print("%s: DISPATCH: %s" % (self.getName(), value))
+            self._dbg("%s: DISPATCH: %s", self.name, value)
             self.dispatch(value)
-            if self.debug_dispatch: print("%s: DISPATCH DONE: %s" % (self.getName(), value))
+            self._dbg("%s: DISPATCH DONE: %s", self.name, value)
 
     def read(self):
         pass
 
     def dispatch(self, subject):
         getattr(self, self._dispatcher_class)(parent=self, subject=subject)
 
+    def _dbg(self, fmt, *args, **kwargs):
+        if self.debug_dispatch:
+            logger.debug(fmt, *args, **kwargs)
+
+
 class ServerConnection(Connection):
     """Connection manager thread handling a listening socket,
     dispatching inbound connections."""
 
     _dispatcher_class = "InboundConnection"
 
     def read(self):
@@ -117,17 +134,18 @@
                 self.subject.close()
                 return
             status = poll.poll(100)
             if status:
                 socket, address = self.subject.accept()
                 yield socket
 
+
 class ThreadedClient(Thread):
     """A dispatch manager that can be used to wrap some other dispatch
-    manager to have it started and entierly run inside an extra
+    manager to have it started and entirely run inside an extra
     thread. This is actually useful to wrap connection managers with
     too, to have their run_parent() run inside a separate thread
     too. See the RPC module for a good example of this."""
 
     _dispatcher_class = "Thread"
 
     def _init(self, subject, parent=None, *arg, **kw):
```

### Comparing `symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/json.py` & `symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/json.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,67 +2,73 @@
 # -*- coding: utf-8 -*-
 # vim: set fileencoding=UTF-8 :
 
 # python-symmetricjsonrpc3
 # Copyright (C) 2009 Egil Moeller <redhog@redhog.org>
 # Copyright (C) 2009 Nicklas Lindgren <nili@gulmohar.se>
 # Copyright (C) 2024 Robert "Robikz" Zalewski <zalewapl@gmail.com>
-
+#
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
-
+#
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Lesser General Public License for more details.
-
+#
 # You should have received a copy of the GNU Lesser General Public
 # License along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307
 # USA
 
 """JSON (de)serialization facilities."""
 
-import sys
 import io
-import unittest
+import sys
+from logging import getLogger
 
 from . import wrappers
 
+
+logger = getLogger(__name__)
+
+
 def from_json(str):
-    """Return a python object representing the json value in str."""
+    """Return a Python object representing the JSON value in str."""
     r = Reader(str)
     return r.read_value()
 
+
 def to_json(obj):
-    """Return a json string representing the python object obj."""
+    """Return a JSON string representing the Python object obj."""
     i = io.StringIO()
     w = Writer(i, encoding='UTF-8')
     w.write_value(obj)
     return i.getvalue()
 
+
 class Writer:
-    """A serializer for python values to JSON. Allowed types for
+    """A serializer for Python values to JSON. Allowed types for
     values to serialize are:
 
         * None
         * True
         * False
-        * Integer
-        * Float
-        * String
-        * Unicode
-        * List
-        * Dict (keys must be String or Unicode)
+        * int
+        * float
+        * str
+        * bytes
+        * list
+        * dict (keys must be str)
         * any object with a __to_json__ method
 
     The writer must be instantiated with a file-like object to write
-    the serialized json to as sole argument. To actually serialize
+    the serialized JSON to as sole argument. To actually serialize
     data, call the write_value() or write_values() methods."""
 
     def __init__(self, s, encoding=None):
         self.encoding = encoding
         self.s = wrappers.WriterWrapper(s)
 
     def close(self):
@@ -130,14 +136,15 @@
         else:
             raise Exception("Cannot encode %s of type %s to json" % (value,type(value)))
 
     def unflushed_write_values(self, values):
         for value in values:
             self.unflushed_write_value(value)
 
+
 class Tokenizer:
     """A SAX-like recursive-descent parser for JSON.
 
     This class does not actually parse JSON into Python objects, it
     only provides tokenization (just like a SAX parser for XML).
 
     This class must be subclassed to be useful. See Reader for
@@ -223,15 +230,15 @@
             elif c == 'r': c = '\r'
             elif c == 't': c = '\t'
             elif c == 'u':
                 d1 = self.s.next()
                 d2 = self.s.next()
                 d3 = self.s.next()
                 d4 = self.s.next()
-                c = unichr(int(d1+d2+d3+d4, 16))
+                c = chr(int(d1+d2+d3+d4, 16))
             else: self._assert(c, '"\\/')
         self.char(c)
 
     def _read_string(self):
         self.string_begin()
         self._assert(self.s.next(), '"')
         while self.s.peek() != '"':
@@ -311,14 +318,15 @@
     def read_value(self):
         return self._read_value()
 
     def read_values(self):
         while True:
             self._read_value()
 
+
 class Reader(Tokenizer):
     """A JSON parser that parses JSON strings read from a file-like
     object or character iterator (for example a string) into Python
     values.
 
     The parser must be instantiated with the file-like object or
     string as its sole argument. To actually parse any values, call
@@ -372,170 +380,86 @@
             while True:
                 self.state = [[]]
                 self._read_value()
                 yield self.state[-1][-1]
         except EOFError:
             return
 
-class DebugTokenizer:
-    def pair_begin(self): print('('); print(self.state); return super(DebugTokenizer, self).pair_begin()
-    def pair_end(self): print(')'); print(self.state); return super(DebugTokenizer, self).pair_end()
-    def object_begin(self): print('{'); print(self.state); return super(DebugTokenizer, self).object_begin()
-    def object_end(self): print('}'); print(self.state); return super(DebugTokenizer, self).object_end()
-    def array_begin(self): print('['); print(self.state); return super(DebugTokenizer, self).array_begin()
-    def array_end(self): print(']'); print(self.state); return super(DebugTokenizer, self).array_end()
-    def string_begin(self): print('"'); print(self.state); return super(DebugTokenizer, self).string_begin()
-    def string_end(self): print('"'); print(self.state); return super(DebugTokenizer, self).string_end()
-    def number_begin(self): print('<'); print(self.state); return super(DebugTokenizer, self).number_begin()
-    def number_end(self): print('>'); print(self.state); return super(DebugTokenizer, self).number_end()
-    def char(self, c): print(repr(c)); print(self.state); return super(DebugTokenizer, self).char(c)
-    def true(self): print("TRUE"); print(self.state); return super(DebugTokenizer, self).true()
-    def false(self): print("FALSE"); print(self.state); return super(DebugTokenizer, self).false()
-    def null(self): print("NULL"); print(self.state); return super(DebugTokenizer, self).null()
-    def fail(self, msg): super(DebugTokenizer, self).fail(); raise Exception(msg)
-
-class DebugReader(DebugTokenizer, Reader): pass
-
-#### Test code ####
-
-class TestJson(unittest.TestCase):
-    import socket
-    import tempfile
-    import threading
-
-    def assertReadEqual(self, str, obj):
-        reader = Reader(str)
-        read_obj = reader.read_value()
-        self.assertEqual(obj, read_obj)
-        io = self.tempfile.TemporaryFile()
-        Writer(io).write_value(obj)
-        io.seek(0)
-        reader1 = Reader(io)
-        read_obj1 = reader1.read_value()
-        self.assertEqual(obj, read_obj1)
-    def assertWriteEqual(self, str, obj):
-        self.assertEqual(str, to_json(obj))
-    def test_to_json(self):
-        STR = '["string",false,null]'
-        OBJ = [u"string", False, None]
-        self.assertEqual(to_json(OBJ), STR)
-    def test_from_json(self):
-        STR = '{"array": ["string",false,null],"object":{"number":4711,"bool":true}}'
-        OBJ = {u"array": [u"string", False, None], u"object": {u"number": 4711, u"bool": True}}
-        self.assertEqual(from_json(STR), OBJ)
-    def test_single_number_from_json(self):
-        STR = '3.33'
-        OBJ = 3.33
-        self.assertEqual(from_json(STR), OBJ)
-    def test_read_value(self):
-        STR = '{"array": ["string",false,null],"object":{"number":4711,"bool":true}}'
-        OBJ = {u"array": [u"string", False, None], u"object": {u"number": 4711, u"bool": True}}
-        self.assertReadEqual(STR, OBJ)
-    def test_read_numbers(self):
-        STR = '[0, -1, 0.2, 1e+4, -2.5E-5, 1e20]'
-        self.assertReadEqual(STR, eval(STR))
-    def test_read_escape_string(self):
-        STR = r'"\b\f\n\r\t\u1234"'
-        OBJ = u"\b\f\n\r\t\u1234"
-        self.assertReadEqual(STR, OBJ)
-    def test_read_quote_string(self):
-        STR = r'"\""'
-        OBJ = u"\""
-        self.assertReadEqual(STR, OBJ)
-    def test_read_solidus_string(self):
-        STR = r'"\/"'
-        OBJ = u"/"
-        self.assertReadEqual(STR, OBJ)
-    def test_read_reverse_solidus_string(self):
-        STR = r'"\\"'
-        OBJ = u"\\"
-        self.assertReadEqual(STR, OBJ)
-    def test_read_whitespace(self):
-        STR = ''' {
-"array" : [ ] ,
-"object" : { }
-} '''
-        self.assertReadEqual(STR, eval(STR))
-    def test_read_values(self):
-        STR = "{}[]true false null"
-        reader = Reader(STR)
-        values = [{}, [], True, False, None]
-
-        for i, r in enumerate(reader.read_values()):
-            self.assertEqual(r, values[i])
-    def test_encode_invalid_control_character(self):
-        self.assertRaises(Exception, lambda: json('\x00', self.tempfile.TemporaryFile()))
-    def test_encode_invalid_object(self):
-        self.assertRaises(Exception, lambda: json(Tokenizer(""), self.tempfile.TemporaryFile()))
-    def test_read_object(self):
-        STR = '{"__jsonclass__":["foo","bar"],"naja":123}'
-        def foo(arg, kw):
-            assert arg == ["bar"]
-            assert kw == {"naja":123}
-            return True
-        reader = Reader(STR, {'foo': foo})
-        assert reader.read_value() is True
-    def test_broken_socket(self):
-        sockets = self.socket.socketpair()
-        reader = Reader(sockets[0])
-        sockets[0].close()
-        self.assertRaises(self.socket.error, lambda: reader.read_value())
-
-    def test_eof(self):
-        import cStringIO
-
-        obj = {'foo':1, 'bar':[1, 2]}
-        io0 = self.tempfile.TemporaryFile()
-        Writer(io0).write_value(obj)
-        io0.seek(0)
-        full_json_string = io0.read()
-
-        for json_string, eof_error in ((full_json_string, False), (full_json_string[0:10], True), ('', True)):
-            io1 = self.tempfile.TemporaryFile()
-            io1.write(json_string)
-            io1.seek(0)
-            reader = Reader(io1)
-            if eof_error:
-                self.assertRaises(EOFError, lambda: reader.read_value())
-            else:
-                self.assertEqual(obj, reader.read_value())
 
+class DebugTokenizer:
+    def pair_begin(self):
+        logger.debug('(')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).pair_begin()
+
+    def pair_end(self):
+        logger.debug(')')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).pair_end()
+
+    def object_begin(self):
+        logger.debug('{')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).object_begin()
 
-    def test_closed_socket(self):
-        class Timeout(self.threading.Thread):
-            def run(self1):
-                obj = {'foo':1, 'bar':[1, 2]}
-                io = self.tempfile.TemporaryFile()
-                Writer(io).write_value(obj)
-                io.seek(0)
-                full_json_string = io.read()
-
-                for json_string, eof_error in ((full_json_string, False), (full_json_string[0:10], True), ('', True)):
-                    sockets = self.socket.socketpair()
-                    reader = Reader(sockets[0])
-
-                    for c in json_string:
-                        while not sockets[1].send(c): pass
-                    sockets[1].close()
-                    if eof_error:
-                        self.assertRaises(EOFError, lambda: reader.read_value())
-                    else:
-                        self.assertEqual(obj, reader.read_value())
-
-        timeout = Timeout()
-        timeout.start()
-        timeout.join(3)
-        if timeout.is_alive():
-            self.fail('Reader has hung.')
-
-    def test_write_object(self):
-        class SomeObj:
-            def __init__(self, x):
-                self.x = x
+    def object_end(self):
+        logger.debug('}')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).object_end()
+
+    def array_begin(self):
+        logger.debug('[')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).array_begin()
+
+    def array_end(self):
+        logger.debug(']')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).array_end()
+
+    def string_begin(self):
+        logger.debug('"')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).string_begin()
+
+    def string_end(self):
+        logger.debug('"')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).string_end()
+
+    def number_begin(self):
+        logger.debug('<')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).number_begin()
 
-            def __to_json__(self):
-                return {'__jsonclass__': ['SomeObj'], 'x': self.x}
+    def number_end(self):
+        logger.debug('>')
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).number_end()
+
+    def char(self, c):
+        logger.debug(repr(c))
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).char(c)
+
+    def true(self):
+        logger.debug("TRUE")
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).true()
+
+    def false(self):
+        logger.debug("FALSE")
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).false()
+
+    def null(self):
+        logger.debug("NULL")
+        logger.debug(self.state)
+        return super(DebugTokenizer, self).null()
+
+    def fail(self, msg):
+        super(DebugTokenizer, self).fail()
+        raise Exception(msg)
 
-        self.assertWriteEqual('{"x":4711,"__jsonclass__":["SomeObj"]}', SomeObj(4711))
 
-if __name__ == "__main__":
-    unittest.main()
+class DebugReader(DebugTokenizer, Reader):
+    pass
```

### Comparing `symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3/wrappers.py` & `symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3/wrappers.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,42 @@
 # -*- coding: utf-8 -*-
 # vim: set fileencoding=UTF-8 :
 
 # python-symmetricjsonrpc3
 # Copyright (C) 2009 Egil Moeller <redhog@redhog.org>
 # Copyright (C) 2009 Nicklas Lindgren <nili@gulmohar.se>
 # Copyright (C) 2024 Robert "Robikz" Zalewski <zalewapl@gmail.com>
-
+#
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
-
+#
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Lesser General Public License for more details.
-
+#
 # You should have received a copy of the GNU Lesser General Public
 # License along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307
 # USA
 
 """Utilities for abstracting I/O for sockets or file-like objects
 behind an identical interface."""
+import io
+import select
+from logging import getLogger
+
+
+logger = getLogger(__name__)
 
 debug_write = False
 debug_read = False
 
-import select
 
 class WriterWrapper:
     """Provides a unified interface for writing to sockets or
     file-like objects.
 
     Its instances will actually belong to one of its subclasses,
     depending on what type of object it wraps."""
@@ -49,15 +54,15 @@
         else:
             return f
 
     def __init__(self, f):
         self.f = f
         self.buff = None
         self.poll = None
-        if hasattr(f, 'fileno'):
+        if _is_real_file(f):
             self.poll = select.poll()
             self.poll.register(f, select.POLLOUT | select.POLLERR | select.POLLHUP | select.POLLNVAL)
         self.closed = False
 
     @property
     def buff_len(self):
         return len(self.buff) if self.buff else 0
@@ -73,15 +78,16 @@
             self.buff += s
         if self.buff_len > self.buff_maxsize:
             self.flush()
 
     def flush(self):
         data = self.buff
         self.buff = None
-        if debug_write: print("write(%s)" % (repr(data),))
+        if debug_write:
+            logger.debug("write(%s)", repr(data))
         while data:
             self._wait()
             data = data[self._write(data):]
 
     def _wait(self):
         if not self.poll:
             return
@@ -90,24 +96,27 @@
             res = self.poll.poll(self.poll_timeout)
         if self.closed:
             raise EOFError
 
     def _write(self, s):
         raise NotImplementedError
 
+
 class FileWriter(WriterWrapper):
     def _write(self, s):
         self.f.write(s)
         return len(s)
 
+
 class SocketWriter(WriterWrapper):
     def _write(self, s):
         res = self.f.send(s.encode('ascii'))
         return res
 
+
 class ReaderWrapper:
     """Provides a unified interface for reading from sockets or
     file-like objects.
 
     Its instances will actually belong to one of its subclasses,
     depending on what type of object it wraps."""
     poll_timeout = 1000
@@ -121,15 +130,15 @@
             return FileReader(f)
         else:
             return f
 
     def __init__(self, f):
         self.file = f
         self.poll = None
-        if hasattr(f, 'fileno'):
+        if _is_real_file(f):
             self.poll = select.poll()
             self.poll.register(f, select.POLLIN | select.POLLPRI | select.POLLERR | select.POLLHUP | select.POLLNVAL)
         self.closed = False
 
     def __iter__(self):
         return self
 
@@ -139,15 +148,15 @@
         except EOFError:
             raise StopIteration
         result = self._read()
         if result == '':
             raise StopIteration
         else:
             if debug_read:
-                print("read(%s)" % (repr(result),))
+                logger.debug("read(%s)", repr(result))
             return result
 
     def close(self):
         self.closed = True
         self.file.close()
 
     def _wait(self):
@@ -158,22 +167,25 @@
             res = self.poll.poll(self.poll_timeout)
         if self.closed:
             raise EOFError
 
     def _read(self):
         raise NotImplementedError
 
+
 class FileReader(ReaderWrapper):
     def _read(self):
         return self.file.read(1)
 
+
 class SocketReader(ReaderWrapper):
     def _read(self):
         return self.file.recv(1).decode('ascii')
 
+
 class ReIterator:
     """An iterator wrapper that provides lookahead through the peek
     method."""
     def __init__(self, i):
         self._prefix = [] # In reverse order!
         self._i = iter(i)
 
@@ -191,7 +203,16 @@
     def peek(self):
         try:
             if not self._prefix:
                 self._put(next(self._i))
             return self._prefix[-1]
         except StopIteration:
             raise EOFError()
+
+
+def _is_real_file(f):
+    if hasattr(f, 'fileno'):
+        try:
+            return f.fileno() is not None
+        except io.UnsupportedOperation:
+            pass
+    return False
```

### Comparing `symmetricjsonrpc3-0.2.0/src/symmetricjsonrpc3.egg-info/PKG-INFO` & `symmetricjsonrpc3-0.3.0/src/symmetricjsonrpc3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: symmetricjsonrpc3
-Version: 0.2.0
+Version: 0.3.0
 Summary: A symmetric, transport-layer agnostic JSON RPC.
 Author-email: Egil Moeller <redhog@redhog.org>, Nicklas Lindgren <nili@gulmohar.se>, "Robert \"Robikz\" Zalewski" <zalewapl@gmail.com>
 Maintainer-email: "Robert \"Robikz\" Zalewski" <zalewapl@gmail.com>
 Project-URL: Source, https://github.com/Zalewa/python-symmetricjsonrpc3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8.1
 Description-Content-Type: text/plain
 License-File: COPYING
 License-File: COPYING.LESSER
 
 Python Symmetric JSON-RPC 3
 ===========================
 
-"A symmetric, transport-layer agnostic JSON-RPC implemenation in python."
+"A symmetric, transport-layer agnostic JSON-RPC implementation in Python."
 
-A JSON-RPC (see https://jsonrpc.org) implementation for Python, with
+A JSON-RPC (see https://jsonrpc.org) implementation for Python with
 the following features:
 
- * Symmetric - both the connecting and the listening process can send
-   and receive method calls, there is no specific "server" or "client"
+ * Symmetric - both the connecting and the listening processes can send
+   and receive method calls. There is no specific "server" or "client"
    process, and no difference between the two connection ends apart
    from who initiates the connection.
 
- * Asynchronous - calls can be interlieved with new calls initiated
+ * Asynchronous - calls can be interleaved with new calls initiated
    before a previous call has returned.
 
  * Thread-safe - calls to the remote side can be done from multiple
    threads without any locking.
 
  * Transport agnostic - can run on top of anything that resembles a
-   socket the slightest (e.g. OpenSSL)
+   socket in the slightest (e.g. OpenSSL)
 
-  * Dependency free
+ * Dependency free
 
-What this really drills down to is that this library implements the
-full specification of JSON-RPC over sockets.
+This library implements the full specification of JSON-RPC over sockets.
 
   This is a fork of niligulmohar's "symmetricjsonrpc" with the intent
   of bringing it up-to-date with current Python and publishing it
   to PyPI.
 
 For usage details, look at the examples in the "examples" directory.
 
 Conventions
 ===========
 
-The conventions apply only since forking from the original repository.
+The conventions apply only after the point of forking from the original
+repository.
 
-This project uses/follows/adheres to:
+This project adheres to:
 
 - Conventional Commits 1.0.0 (https://www.conventionalcommits.org/)
 - PyPA version scheme (https://packaging.python.org/en/latest/specifications/version-specifiers/)
 
 Git tags are prefixed with 'v'.
 
-Module's version is automatically deduced from the git tag in the
+The package's version is automatically deduced from the git tag in the
 "no-guess-dev" mode.
```

