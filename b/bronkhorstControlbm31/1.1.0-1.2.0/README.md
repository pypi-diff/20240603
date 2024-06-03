# Comparing `tmp/bronkhorstcontrolbm31-1.1.0.tar.gz` & `tmp/bronkhorstcontrolbm31-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bronkhorstcontrolbm31-1.1.0.tar", last modified: Thu May 30 07:27:03 2024, max compression
+gzip compressed data, was "bronkhorstcontrolbm31-1.2.0.tar", last modified: Mon Jun  3 14:21:02 2024, max compression
```

## Comparing `bronkhorstcontrolbm31-1.1.0.tar` & `bronkhorstcontrolbm31-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:27:03.806406 bronkhorstcontrolbm31-1.1.0/
--rw-rw-rw-   0        0        0     2665 2024-05-30 07:27:03.803404 bronkhorstcontrolbm31-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2043 2024-05-29 13:21:57.000000 bronkhorstcontrolbm31-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 07:27:03.774404 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31/
--rw-rw-rw-   0        0        0     4905 2024-05-29 09:20:48.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31/bronkhorst.py
--rw-rw-rw-   0        0        0     8358 2024-05-29 14:14:12.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31/bronkhorstClient.py
--rw-rw-rw-   0        0        0     4973 2024-05-30 07:25:15.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31/bronkhorstServer.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:27:03.800407 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/
--rw-rw-rw-   0        0        0     2665 2024-05-30 07:27:03.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-05-30 07:27:03.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:27:03.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-30 07:27:03.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-30 07:27:03.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-30 07:27:03.000000 bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1023 2024-05-30 07:26:34.000000 bronkhorstcontrolbm31-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 07:27:03.806406 bronkhorstcontrolbm31-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 14:21:02.619863 bronkhorstcontrolbm31-1.2.0/
+-rw-rw-rw-   0        0        0     2740 2024-06-03 14:21:02.616861 bronkhorstcontrolbm31-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2118 2024-06-03 13:29:44.000000 bronkhorstcontrolbm31-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 14:21:02.595861 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31/
+-rw-rw-rw-   0        0        0     4905 2024-05-29 09:20:48.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31/bronkhorst.py
+-rw-rw-rw-   0        0        0     9611 2024-06-03 13:30:24.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31/bronkhorstClient.py
+-rw-rw-rw-   0        0        0     4973 2024-05-30 15:06:15.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31/bronkhorstServer.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:21:02.614862 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/
+-rw-rw-rw-   0        0        0     2740 2024-06-03 14:21:02.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-06-03 14:21:02.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:21:02.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      271 2024-06-03 14:21:02.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-06-03 14:21:02.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-06-03 14:21:02.000000 bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2024-06-03 14:19:35.000000 bronkhorstcontrolbm31-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:21:02.619863 bronkhorstcontrolbm31-1.2.0/setup.cfg
```

### Comparing `bronkhorstcontrolbm31-1.1.0/PKG-INFO` & `bronkhorstcontrolbm31-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bronkhorstControlbm31
-Version: 1.1.0
+Version: 1.2.0
 Summary: tools for communicating with Bronkhorst MFCs with the API for BM31
 Author-email: "Kenneth P. Marshall" <kenneth.marshall@esrf.fr>
 Maintainer-email: "Kenneth P. Marshall" <kenneth.marshall@esrf.fr>
 Project-URL: repository, https://github.com/msujas/bronkhorstControl
 Keywords: Bronkhorst,MFCs
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.12
@@ -41,10 +41,10 @@
 
 bronkhorstMultiServer remote
 
 then for the client use multi=True:
 
 MFCclient(3,'\<hostname or ip address\>', multi=True).pollAll()
 
-There are also 2 other functions in bronkhorstClient called plotLoop() and timePlot() which can be run in conjunction with the bronkhorstMultiServer. Takes host as a required aguement.
+There are also 2 other functions in bronkhorstClient called barPlot() and timePlot() which can be run in conjunction with the bronkhorstMultiServer. Takes host as a required aguement. These are also packaged as executables, so run e.g. 'timePlot \<hostname\>'
 
 I should mention this article https://realpython.com/python-sockets/ and the associated repository which helped me to make this.
```

### Comparing `bronkhorstcontrolbm31-1.1.0/README.md` & `bronkhorstcontrolbm31-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 
 bronkhorstMultiServer remote
 
 then for the client use multi=True:
 
 MFCclient(3,'\<hostname or ip address\>', multi=True).pollAll()
 
-There are also 2 other functions in bronkhorstClient called plotLoop() and timePlot() which can be run in conjunction with the bronkhorstMultiServer. Takes host as a required aguement.
+There are also 2 other functions in bronkhorstClient called barPlot() and timePlot() which can be run in conjunction with the bronkhorstMultiServer. Takes host as a required aguement. These are also packaged as executables, so run e.g. 'timePlot \<hostname\>'
 
 I should mention this article https://realpython.com/python-sockets/ and the associated repository which helped me to make this.
```

### Comparing `bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31/bronkhorst.py` & `bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31/bronkhorst.py`

 * *Files identical despite different names*

### Comparing `bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31/bronkhorstClient.py` & `bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31/bronkhorstClient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,41 @@
 import socket
 import pandas as pd
 import matplotlib.pyplot as plt
 import selectors,types
 import matplotlib
 matplotlib.rcParams.update({'font.size':14})
-import time 
+import time
+import argparse
 
 HOST = 'localhost'
 PORT = 61245
 
+def getArgs(host=HOST, port=PORT, connid = socket.gethostname(),waitTime = 0.5, plotTime = 1):
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument('host',nargs='?', default=host, type= str, help = 'host name/address')
+    parser.add_argument('-p','--port',default=port, type=int, help = 'port number')
+    parser.add_argument('-c','--connid',default=connid, type = str, help='name for connection')
+    parser.add_argument('-wt','--waittime',default=waitTime, type = float, help = 'time to wait between iterations (default 0.5 s)')
+    parser.add_argument('-pt','--plotTime',default=plotTime, type = float, 
+                        help = 'total time to plot on x-axis (only for timePlot, default 1 hour)')
+    args = parser.parse_args()
+
+    host = args.host
+    port = args.port
+    connid = args.connid
+    waitTime = args.waittime
+    plotTime = args.plotTime
+
+    print(host)
+    print(port)
+    print(connid)
+    return host, port, connid, waitTime, plotTime
+
 def connect(host=HOST, port=PORT):
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.connect((host,port))
     return s
 
 class MFCclient():
     def __init__(self,address, host=HOST,port=PORT, multi=False,connid = socket.gethostname()):
@@ -160,15 +183,16 @@
             if not data.outb and data.messages:
                 data.outb = data.messages.pop(0)
             if data.outb:
                 print(f"Sending {data.outb} to connection {data.connid}")
                 sent = sock.send(data.outb)  # Should be ready to write
                 data.outb = data.outb[sent:]      
 
-def plotLoop(host, port = PORT,waittime = 1, multi = True, connid = 'plotLoop'):
+def barPlot(host=HOST, port = PORT,waittime = 0.5, multi = True, connid = 'plotLoop'):
+    host,port,connid, waittime, xlim=getArgs(host=host,port=port,connid=connid, waitTime=waittime,plotTime=1)
     fig,(ax1,ax2) = plt.subplots(2,1)
 
     while True:
         try:
             ax1.set_ylabel('MFC/BPR Measure')
             ax2.set_ylabel('MFC/BPR Setpoint')
 
@@ -181,15 +205,16 @@
             plt.pause(waittime)
             ax1.cla()
             ax2.cla()
         except (KeyboardInterrupt, AttributeError):
             plt.close(fig)
             return
 
-def timePlot(host, port = PORT,waittime = 1, multi = True, connid = 'timePlot',xlim = 1):
+def timePlot(host=HOST, port = PORT,waittime = 0.5, multi = True, connid = 'timePlot',xlim = 1):
+    host,port,connid, waittime, xlim=getArgs(host=host,port=port,connid=connid, waitTime=waittime,plotTime=xlim)
     measure = {}
     c=0
     fig,ax = plt.subplots()
     tlist = []
     xlims = xlim*3600
     while True:
         try:
```

### Comparing `bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31/bronkhorstServer.py` & `bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31/bronkhorstServer.py`

 * *Files identical despite different names*

### Comparing `bronkhorstcontrolbm31-1.1.0/bronkhorstControlbm31.egg-info/PKG-INFO` & `bronkhorstcontrolbm31-1.2.0/bronkhorstControlbm31.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bronkhorstControlbm31
-Version: 1.1.0
+Version: 1.2.0
 Summary: tools for communicating with Bronkhorst MFCs with the API for BM31
 Author-email: "Kenneth P. Marshall" <kenneth.marshall@esrf.fr>
 Maintainer-email: "Kenneth P. Marshall" <kenneth.marshall@esrf.fr>
 Project-URL: repository, https://github.com/msujas/bronkhorstControl
 Keywords: Bronkhorst,MFCs
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.12
@@ -41,10 +41,10 @@
 
 bronkhorstMultiServer remote
 
 then for the client use multi=True:
 
 MFCclient(3,'\<hostname or ip address\>', multi=True).pollAll()
 
-There are also 2 other functions in bronkhorstClient called plotLoop() and timePlot() which can be run in conjunction with the bronkhorstMultiServer. Takes host as a required aguement.
+There are also 2 other functions in bronkhorstClient called barPlot() and timePlot() which can be run in conjunction with the bronkhorstMultiServer. Takes host as a required aguement. These are also packaged as executables, so run e.g. 'timePlot \<hostname\>'
 
 I should mention this article https://realpython.com/python-sockets/ and the associated repository which helped me to make this.
```

### Comparing `bronkhorstcontrolbm31-1.1.0/pyproject.toml` & `bronkhorstcontrolbm31-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools >= 59.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bronkhorstControlbm31"
-version = "1.1.0"
+version = "1.2.0"
 requires-python = ">= 3.10"
-dependencies = ["bronkhorst-propar",
-                "pandas",
-                "matplotlib"]
+dependencies = ["bronkhorst-propar", "pandas", "matplotlib"]
 authors = [{name = "Kenneth P. Marshall", email = "kenneth.marshall@esrf.fr"}]
 maintainers = [{name = "Kenneth P. Marshall", email = "kenneth.marshall@esrf.fr"}]
 description = "tools for communicating with Bronkhorst MFCs with the API for BM31"
 readme = {file = "README.MD", content-type = "text/markdown"}
 keywords = ["Bronkhorst", "MFCs"]
 classifiers = [
 "Development Status :: 4 - Beta",
 "Programming Language :: Python :: 3.12"]
 
 [project.scripts]
 bronkhorstServer = "bronkhorstControlbm31.bronkhorstServer:run"
 bronkhorstMultiServer = "bronkhorstControlbm31.bronkhorstServer:multiServer"
+timePlot = "bronkhorstControlbm31.bronkhorstClient:timePlot"
+barPlot = "bronkhorstControlbm31.bronkhorstClient:barPlot"
 
 [tool.setuptools]
 packages = ["bronkhorstControlbm31"]
 
 [project.urls]
 repository = "https://github.com/msujas/bronkhorstControl"
```

