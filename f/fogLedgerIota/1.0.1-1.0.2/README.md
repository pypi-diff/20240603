# Comparing `tmp/fogLedgerIota-1.0.1.tar.gz` & `tmp/fogledgeriota-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fogLedgerIota-1.0.1.tar", last modified: Tue Mar 26 02:14:41 2024, max compression
+gzip compressed data, was "fogledgeriota-1.0.2.tar", last modified: Sun Jun  2 19:35:33 2024, max compression
```

## Comparing `fogLedgerIota-1.0.1.tar` & `fogledgeriota-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:14:41.611761 fogLedgerIota-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-26 02:14:41.611761 fogLedgerIota-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:14:41.611761 fogLedgerIota-1.0.1/fogLedgerIota.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-26 02:14:41.000000 fogLedgerIota-1.0.1/fogLedgerIota.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-26 02:14:41.000000 fogLedgerIota-1.0.1/fogLedgerIota.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 02:14:41.000000 fogLedgerIota-1.0.1/fogLedgerIota.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 02:14:41.000000 fogLedgerIota-1.0.1/fogLedgerIota.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 02:14:41.000000 fogLedgerIota-1.0.1/fogLedgerIota.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 02:14:41.000000 fogLedgerIota-1.0.1/fogLedgerIota.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:14:41.607761 fogLedgerIota-1.0.1/fogledgerIota/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:14:41.607761 fogLedgerIota-1.0.1/fogledgerIota/iota/
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/IotaBasic.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:14:41.611761 fogLedgerIota-1.0.1/fogledgerIota/iota/config/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/config/ApiConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/config/CoordConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/config/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/config/SpammerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/config/WebAppConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/fogledgerIota/iota/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 02:14:41.611761 fogLedgerIota-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-26 02:14:36.000000 fogLedgerIota-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:35:33.658276 fogledgeriota-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-06-02 19:35:33.658276 fogledgeriota-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:35:33.658276 fogledgeriota-1.0.2/fogLedgerIota.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-06-02 19:35:33.000000 fogledgeriota-1.0.2/fogLedgerIota.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-02 19:35:33.000000 fogledgeriota-1.0.2/fogLedgerIota.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:35:33.000000 fogledgeriota-1.0.2/fogLedgerIota.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:35:33.000000 fogledgeriota-1.0.2/fogLedgerIota.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 19:35:33.000000 fogledgeriota-1.0.2/fogLedgerIota.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 19:35:33.000000 fogledgeriota-1.0.2/fogLedgerIota.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:35:33.654276 fogledgeriota-1.0.2/fogledgerIota/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:35:33.658276 fogledgeriota-1.0.2/fogledgerIota/iota/
+-rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/IotaBasic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:35:33.658276 fogledgeriota-1.0.2/fogledgerIota/iota/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/config/ApiConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/config/CoordConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/config/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/config/SpammerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/config/WebAppConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/fogledgerIota/iota/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 19:35:33.658276 fogledgeriota-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-06-02 19:35:29.000000 fogledgeriota-1.0.2/setup.py
```

### Comparing `fogLedgerIota-1.0.1/LICENSE.txt` & `fogledgeriota-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fogLedgerIota-1.0.1/PKG-INFO` & `fogledgeriota-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedgerIota
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger-Iota/tree/v1.0.0
 Author: Weslei Santos
 Author-email: weslei.eng.comp@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,iota,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedgerIota-1.0.1/README.md` & `fogledgeriota-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 ```
 sudo ansible-playbook -i "localhost," -c local containernet/ansible/install.yml
 ```
 
 #### 2. Install Fogbed
 
 ```
-sudo pip install -U git+https://github.com/EsauM10/fogbed.git
+sudo pip install fogbed
 ```
 
 #### 3. Install FogLedger
 
 ```
-sudo pip install -U git+https://github.com/larsid/FogLedger.git
+sudo pip install -U git+https://github.com/larsid/FogLedger-Iota.git
 ```
 
 ## Get Started
 
 ## Preparing Blockchain Test
 
 ## Run example iota
@@ -55,20 +55,20 @@
 ```
 sudo python3 test-distributed-network.py
 ```
 
 ## Example: A local network with four nodes
 
 ```python
-from fogledger.iota.IotaBasic import (IotaBasic)
-from fogledger.iota.config.NodeConfig import (NodeConfig)
-from fogledger.iota.config.CoordConfig import (CoordConfig)
-from fogledger.iota.config.SpammerConfig import (SpammerConfig)
-from fogledger.iota.config.ApiConfig import (ApiConfig)
-from fogledger.iota.config.WebAppConfig import (WebAppConfig)
+from fogledgerIota.iota.IotaBasic import (IotaBasic)
+from fogledgerIota.iota.config.NodeConfig import (NodeConfig)
+from fogledgerIota.iota.config.CoordConfig import (CoordConfig)
+from fogledgerIota.iota.config.SpammerConfig import (SpammerConfig)
+from fogledgerIota.iota.config.ApiConfig import (ApiConfig)
+from fogledgerIota.iota.config.WebAppConfig import (WebAppConfig)
 from typing import List
 from fogbed import (
     VirtualInstance, setLogLevel, FogbedDistributedExperiment, Worker, Controller
 )
 
 setLogLevel('info')
```

### Comparing `fogLedgerIota-1.0.1/fogLedgerIota.egg-info/PKG-INFO` & `fogledgeriota-1.0.2/fogLedgerIota.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedgerIota
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger-Iota/tree/v1.0.0
 Author: Weslei Santos
 Author-email: weslei.eng.comp@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,iota,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedgerIota-1.0.1/fogLedgerIota.egg-info/SOURCES.txt` & `fogledgeriota-1.0.2/fogLedgerIota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fogLedgerIota-1.0.1/fogledgerIota/iota/IotaBasic.py` & `fogledgeriota-1.0.2/fogledgerIota/iota/IotaBasic.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     @staticmethod
     def read_file(file_path):
         with open(file_path, 'r') as file:
             return file.read()
 
     def installPrivateTangle(self):
         print("install tangle")
-        path_script = pkg_resources.resource_filename('fogledger.iota', 'data')
+        path_script = pkg_resources.resource_filename('fogledgerIota.iota', 'data')
         path_private_tangle = os.path.join(path_script, "private-tangle.sh")
         subprocess.run(["/bin/bash", path_private_tangle, "install"], check=True, cwd=path_script)
         print("finished script...")
     
     def define_nodes(self, index: int, node_conf: NodeConfig = None):
         name = node_conf.name if node_conf and node_conf.name is not None else f'{self.prefix}node{index}'
         ip = node_conf.ip if node_conf and node_conf.ip is not None else None
```

### Comparing `fogLedgerIota-1.0.1/setup.py` & `fogledgeriota-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fogLedgerIota",
-    version="1.0.1",
+    version="1.0.2",
     description='Plugin to build DLTs in Fogbed.',
     long_description='Plugin to build DLT in Fogbed. Suport IOTA. \
         The FogLedger is a plugin for [Fogbed](https://github.com/larsid/FogLedger-Iota). It allows you to emulate a fog network with distributed ledgers. \
         Currently, FogLedger has suport for IOTA. IOTA is a groundbreaking cryptocurrency designed for the Internet of Things (IoT), \
         Offering feeless transactions and scalability for machine-to-machine communication. \
         Its unique Tangle ledger utilizes a directed acyclic graph (DAG) for efficient data transfer and decentralized consensus, \
         making it ideal for securing and facilitating microtransactions in IoT ecosystems.',
```

