# Comparing `tmp/fink-client-7.2.tar.gz` & `tmp/fink-client-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fink-client-7.2.tar", last modified: Fri Dec  8 07:41:45 2023, max compression
+gzip compressed data, was "fink-client-8.0.tar", last modified: Mon Jun  3 13:22:04 2024, max compression
```

## Comparing `fink-client-7.2.tar` & `fink-client-8.0.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-12-08 07:41:45.598531 fink-client-7.2/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    11357 2022-08-16 12:31:59.000000 fink-client-7.2/LICENSE
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     6888 2023-12-08 07:41:45.598531 fink-client-7.2/PKG-INFO
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     6144 2023-09-08 11:59:23.000000 fink-client-7.2/README.md
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-12-08 07:41:45.598531 fink-client-7.2/bin/
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     1421 2022-08-16 12:31:59.000000 fink-client-7.2/bin/fink_client_test.sh
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-12-08 07:41:45.598531 fink-client-7.2/fink_client/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      686 2023-12-08 07:41:21.000000 fink-client-7.2/fink_client/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    13590 2023-09-08 11:35:13.000000 fink-client-7.2/fink_client/avroUtils.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     4494 2023-07-19 21:16:39.000000 fink-client-7.2/fink_client/configuration.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    12336 2023-09-08 11:35:13.000000 fink-client-7.2/fink_client/consumer.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-12-08 07:41:45.598531 fink-client-7.2/fink_client/scripts/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      606 2022-08-16 12:31:59.000000 fink-client-7.2/fink_client/scripts/__init__.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     3308 2022-08-16 12:31:59.000000 fink-client-7.2/fink_client/scripts/fink_alert_viewer.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     2547 2023-01-16 15:09:39.000000 fink-client-7.2/fink_client/scripts/fink_client_register.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     4719 2023-07-19 21:16:39.000000 fink-client-7.2/fink_client/scripts/fink_consumer.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)    18402 2023-11-06 14:57:52.000000 fink-client-7.2/fink_client/scripts/fink_datatransfer.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     8466 2023-02-27 14:53:47.000000 fink-client-7.2/fink_client/scripts/fink_datatransfer_mpi.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     9438 2023-03-02 09:51:35.000000 fink-client-7.2/fink_client/scripts/fink_datatransfer_offsets.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     1756 2022-08-16 12:31:59.000000 fink-client-7.2/fink_client/tester.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     3466 2022-08-16 12:31:59.000000 fink-client-7.2/fink_client/visualisation.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-12-08 07:41:45.598531 fink-client-7.2/fink_client.egg-info/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     6888 2023-12-08 07:41:45.000000 fink-client-7.2/fink_client.egg-info/PKG-INFO
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      718 2023-12-08 07:41:45.000000 fink-client-7.2/fink_client.egg-info/SOURCES.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        1 2023-12-08 07:41:45.000000 fink-client-7.2/fink_client.egg-info/dependency_links.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      268 2023-12-08 07:41:45.000000 fink-client-7.2/fink_client.egg-info/entry_points.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      121 2023-12-08 07:41:45.000000 fink-client-7.2/fink_client.egg-info/requires.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)       12 2023-12-08 07:41:45.000000 fink-client-7.2/fink_client.egg-info/top_level.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)       38 2023-12-08 07:41:45.598531 fink-client-7.2/setup.cfg
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     2169 2023-01-17 15:11:10.000000 fink-client-7.2/setup.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-12-08 07:41:45.598531 fink-client-7.2/tests/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     4141 2023-01-16 15:09:39.000000 fink-client-7.2/tests/test.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2024-06-03 13:22:04.082611 fink-client-8.0/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    11357 2022-08-16 12:31:59.000000 fink-client-8.0/LICENSE
+-rw-r--r--   0 peloton   (1000) peloton   (1000)     6916 2024-06-03 13:22:04.082611 fink-client-8.0/PKG-INFO
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     5800 2024-06-03 13:21:04.000000 fink-client-8.0/README.md
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2024-06-03 13:22:04.078611 fink-client-8.0/bin/
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     1421 2022-08-16 12:31:59.000000 fink-client-8.0/bin/fink_client_test.sh
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2024-06-03 13:22:04.078611 fink-client-8.0/fink_client/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      691 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    13588 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/avro_utils.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     4509 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/configuration.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    12840 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/consumer.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2024-06-03 13:22:04.082611 fink-client-8.0/fink_client/scripts/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      606 2022-08-16 12:31:59.000000 fink-client-8.0/fink_client/scripts/__init__.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     3463 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/scripts/fink_alert_viewer.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     2683 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/scripts/fink_client_register.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     5632 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/scripts/fink_consumer.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)    19724 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/scripts/fink_datatransfer.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     1754 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/tester.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     3423 2024-06-03 13:21:04.000000 fink-client-8.0/fink_client/visualisation.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2024-06-03 13:22:04.082611 fink-client-8.0/fink_client.egg-info/
+-rw-r--r--   0 peloton   (1000) peloton   (1000)     6916 2024-06-03 13:22:03.000000 fink-client-8.0/fink_client.egg-info/PKG-INFO
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      625 2024-06-03 13:22:04.000000 fink-client-8.0/fink_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        1 2024-06-03 13:22:03.000000 fink-client-8.0/fink_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      268 2024-06-03 13:22:03.000000 fink-client-8.0/fink_client.egg-info/entry_points.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      192 2024-06-03 13:22:03.000000 fink-client-8.0/fink_client.egg-info/requires.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)       12 2024-06-03 13:22:03.000000 fink-client-8.0/fink_client.egg-info/top_level.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)       38 2024-06-03 13:22:04.082611 fink-client-8.0/setup.cfg
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     2169 2023-01-17 15:11:10.000000 fink-client-8.0/setup.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2024-06-03 13:22:04.082611 fink-client-8.0/tests/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     4144 2024-06-03 13:21:04.000000 fink-client-8.0/tests/test.py
```

### Comparing `fink-client-7.2/LICENSE` & `fink-client-8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fink-client-7.2/PKG-INFO` & `fink-client-8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: fink-client
-Version: 7.2
-Summary: Light-weight client to manipulate alerts from Fink
-Home-page: https://fink-broker.readthedocs.io/en/latest/
-Author: AstroLab Software
-Author-email: peloton@lal.in2p3.fr
-Project-URL: Documentation, https://fink-broker.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/astrolabsoftware/fink-client
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![pypi](https://img.shields.io/pypi/v/fink-client.svg)](https://pypi.python.org/pypi/fink-client)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Sentinel](https://github.com/astrolabsoftware/fink-client/workflows/Sentinel/badge.svg)](https://github.com/astrolabsoftware/fink-client/actions?query=workflow%3ASentinel)
 [![codecov](https://codecov.io/gh/astrolabsoftware/fink-client/branch/master/graph/badge.svg)](https://codecov.io/gh/astrolabsoftware/fink-client)
 [![Documentation Status](https://readthedocs.org/projects/fink-broker/badge/?version=latest)](https://fink-broker.readthedocs.io/en/latest/?badge=latest)
 
@@ -33,81 +15,65 @@
 
 ### Install with pip
 
 ```bash
 pip install fink-client --upgrade
 ```
 
-You will also need to install `fastavro==1.6.0` separately (versions above are not compatible with alert schema):
-
-```
-# fastavro 1.6.0 requires Cython<3
-pip install "Cython<3"
-pip install --no-build-isolation "fastavro==1.6.0"
-```
-
 ### Use or develop in a controlled environment
 
-For usage:
-
-```bash
-conda env create -f https://raw.githubusercontent.com/astrolabsoftware/fink-client/master/environment.yml
-conda activate fink-client
-pip install "Cython<3"
-pip install --no-build-isolation "fastavro==1.6.0"
-pip install fink-client --upgrade
-```
-
-For development:
+For development, we recommend the use of a virtual environment:
 
 ```bash
 git clone https://github.com/astrolabsoftware/fink-client.git
 cd fink-client
-conda env create -f environment.yml
-conda activate fink-client
-pip install "Cython<3"
-pip install --no-build-isolation "fastavro==1.6.0"
-pip install -e .
+python -m venv .fc_env
+source .fc_env/bin/activate
+pip install -r requirements.txt
+pip install .
 ```
 
 ## Registration
 
 In order to connect and poll alerts from Fink, you need to get your credentials:
 
 1. Subscribe to one or more Fink streams by filling this [form](https://forms.gle/2td4jysT4e9pkf889).
 2. After filling the form, we will send your credentials. Register them on your laptop by simply running:
   ```
   fink_client_register -username <USERNAME> -group_id <GROUP_ID> ...
   ```
 
 ## Livestream usage
 
-Once you have your credentials, you are ready to poll streams!
+Once you have your credentials, you are ready to poll streams! You can easily access the documentation using `-h` or `--help`:
 
 ```bash
 fink_consumer -h
 usage: fink_consumer [-h] [--display] [-limit LIMIT] [--available_topics]
                      [--save] [-outdir OUTDIR] [-schema SCHEMA]
+                     [--dump_schema]
 
-Kafka consumer to listen and archive Fink streams from the Livestream service
+Kafka consumer to listen and archive Fink streams from the Livestream
+service
 
 optional arguments:
   -h, --help          show this help message and exit
-  --display           If specified, print on screen information about incoming
-                      alert.
+  --display           If specified, print on screen information about
+                      incoming alert.
   -limit LIMIT        If specified, download only `limit` alerts. Default is
                       None.
   --available_topics  If specified, print on screen information about
                       available topics.
   --save              If specified, save alert data on disk (Avro). See also
                       -outdir.
   -outdir OUTDIR      Folder to store incoming alerts if --save is set. It
                       must exist.
   -schema SCHEMA      Avro schema to decode the incoming alerts. Default is
-                      None (latest version downloaded from server)
+                      None (version taken from each alert)
+  --dump_schema       If specified, save the schema on disk (json file)
 ```
 
 You can also look at an alert on the disk:
 
 ```bash
 fink_alert_viewer -h
 usage: fink_alert_viewer [-h] [-filename FILENAME]
```

### Comparing `fink-client-7.2/bin/fink_client_test.sh` & `fink-client-8.0/bin/fink_client_test.sh`

 * *Files identical despite different names*

### Comparing `fink-client-7.2/fink_client/__init__.py` & `fink-client-8.0/fink_client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright 2019 AstroLab Software
+# Copyright 2019-2024 AstroLab Software
 # Author: Julien Peloton
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "7.2"
+__version__ = "8.0"
 __schema_version__ = "distribution_schema_fink_ztf_{}.avsc"
```

### Comparing `fink-client-7.2/fink_client/avroUtils.py` & `fink-client-8.0/fink_client/avro_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,27 +27,28 @@
 import pandas as pd
 
 import fastavro
 
 from fink_client.tester import regular_unit_tests
 from fink_client import __schema_version__
 
-class AlertReader():
-    """ Class to load alert Avro files.
+
+class AlertReader:
+    """Class to load alert Avro files.
 
     It accepts single avro file (.avro), gzipped avro file (.avro.gz), and
     folders containing several of these.
 
     Parameters
     ----------
     path: str
         Path to alert Avro file or folder containing alert Avro files.
 
     Examples
-    ----------
+    --------
     Load a single Avro alert
     >>> r = AlertReader(avro_single_alert)
     >>> list_of_alerts = r.to_list()
     >>> print(len(list_of_alerts))
     1
 
     Read a bunch of files
@@ -67,21 +68,22 @@
 
     If you give a list of files
     >>> r = AlertReader(avro_list)
     >>> print('{} alerts decoded'.format(len(r.to_list())))
     2 alerts decoded
 
     """
+
     def __init__(self, path: str):
-        """ Initialise the AlertReader class """
+        """Initialise the AlertReader class"""
         self.path = path
         self._load_avro_files()
 
     def _load_avro_files(self, ext_path: str = None):
-        """ Load Avro alert data
+        """Load Avro alert data
 
         Parameters
         ----------
         ext_path: str, optional
             If not None, load explicitly data under `ext_path`.
             Default is None (self.path is used).
         """
@@ -89,107 +91,107 @@
             path = ext_path
         else:
             path = self.path
 
         if isinstance(path, list):
             self.filenames = path
         elif os.path.isdir(path):
-            self.filenames = glob.glob(os.path.join(path, '*.avro*'))
-        elif path == '':
-            print('WARNING: path to avro files is empty')
+            self.filenames = glob.glob(os.path.join(path, "*.avro*"))
+        elif path == "":
+            print("WARNING: path to avro files is empty")
             self.filenames = []
         elif fastavro.is_avro(path):
             self.filenames = [path]
-        elif path.endswith('avro.gz'):
+        elif path.endswith("avro.gz"):
             self.filenames = [path]
         else:
             msg = """
             Data path not understood: {}
             You must give an avro file with
             its extension (.avro or .avro.gz), or a folder with avro files.
             """.format(path)
             raise IOError(msg)
 
     def _read_single_alert(self, name: str = None) -> dict:
-        """ Read an avro alert, and return data as dictionary
+        """Read an avro alert, and return data as dictionary
 
         Parameters
         ----------
         name: str, optional
             Name of the alert to read (avro format).
             Default is None (self.path is used).
 
         Returns
-        ----------
+        -------
         alert: dict
             Alert data in a dictionary
 
         Examples
-        ----------
+        --------
         >>> r = AlertReader("")
         WARNING: path to avro files is empty
 
         >>> alert = r._read_single_alert(name=avro_single_alert)
         """
         if name is None:
             name = self.path
 
         data = []
 
-        if name.endswith('avro'):
-            copen = lambda x: open(x, mode='rb')
-        elif name.endswith('avro.gz'):
-            copen = lambda x: gzip.open(x, mode='rb')
+        if name.endswith("avro"):
+            copen = lambda x: open(x, mode="rb")
+        elif name.endswith("avro.gz"):
+            copen = lambda x: gzip.open(x, mode="rb")
         else:
             msg = """
             Alert filename should end with `avro` or `avro.gz`.
             Currently trying to read: {}
             """.format(name)
             raise NotImplementedError(msg)
 
         with copen(name) as fo:
             avro_reader = reader(fo)
             for record in avro_reader:
-                data.append(record)
+                data.append(record)  # noqa: PERF402
         return data
 
     def to_pandas(self) -> pd.DataFrame:
-        """ Read Avro alert(s) and return data as Pandas DataFrame
+        """Read Avro alert(s) and return data as Pandas DataFrame
 
         Returns
-        ----------
+        -------
         alert: pd.DataFrame
             Alert data in a pandas DataFrame
 
         Examples
-        ----------
+        --------
         >>> r = AlertReader(avro_folder)
         >>> df = r.to_pandas()
         >>> assert('objectId' in r.to_pandas().columns)
 
         >>> r = AlertReader(avro_gzipped)
         >>> df = r.to_pandas()
         >>> assert('diaSource' in r.to_pandas().columns)
 
         """
         return pd.DataFrame(self.to_iterator())
 
     def to_list(self, size: int = None) -> list:
-        """ Read Avro alert and return data as list of dictionary
+        """Read Avro alert and return data as list of dictionary
 
         Returns
-        ----------
+        -------
         out: list of dictionary
             Alert data (dictionaries) in a list
         size: int, optional
             If not None, return only `size` alerts.
             Default is None.
 
         Examples
-        ----------
+        --------
         >>> r = AlertReader(avro_single_alert)
         >>> mylist = r.to_list()
         >>> print(len(mylist))
         1
 
         >>> r = AlertReader(avro_folder)
         >>> mylist = r.to_list(size=2)
@@ -201,47 +203,55 @@
         >>> print(len(mylist))
         1
         """
         nest = [self._read_single_alert(fn) for fn in self.filenames[:size]]
         return [item for sublist in nest for item in sublist][:size]
 
     def to_iterator(self) -> Iterable[dict]:
-        """ Return an iterator for alert data
+        """Return an iterator for alert data
 
         Returns
-        ----------
+        -------
         out: Iterable[dict]
             Alert data (dictionaries) in an iterator
 
         Examples
-        ----------
+        --------
         >>> r = AlertReader(avro_folder)
         >>> myiterator = r.to_iterator()
         >>> assert('objectId' in next(myiterator).keys())
 
         """
         for fn in self.filenames:
             for alert in self._read_single_alert(fn):
                 yield alert
 
-def write_alert(alert: dict, schema: str, path: str, overwrite: bool = False, id1: str = '', id2: str = ''):
-    """ Write avro alert on disk
+
+def write_alert(
+    alert: dict,
+    schema: str,
+    path: str,
+    overwrite: bool = False,
+    id1: str = "",
+    id2: str = "",
+):
+    """Write avro alert on disk
 
     Parameters
     ----------
     alert: dict
         Alert data to save (dictionary with avro syntax)
     schema: str or dict
         Path to Avro schema of the alert, or parsed schema.
     path: str
         Folder that will contain the alert. The filename will always be
         <objectID>.avro
 
     Examples
-    ----------
+    --------
     >>> r = AlertReader(avro_single_alert)
     >>> alert = r.to_list(size=1)[0]
 
     Write the alert on disk
     >>> write_alert(alert, schema_path, ".", overwrite=True, id1="objectId", id2="candid")
 
     For test purposes, you can overwrite alert data on disk, but that should
@@ -250,45 +260,43 @@
     >>> write_alert(
     ...     alert, schema_path, ".", overwrite=False, id1="objectId", id2="candid")
     ... # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
     Traceback (most recent call last):
       ...
     OSError: ./ZTF19acihgng_1060135832015015002.avro already exists!
     """
-    alert_filename = os.path.join(
-        path,
-        "{}_{}.avro".format(alert[id1], alert[id2])
-    )
+    alert_filename = os.path.join(path, "{}_{}.avro".format(alert[id1], alert[id2]))
 
     if isinstance(schema, str):
         schema = _get_alert_schema(schema)
     # Check if the alert already exist
     if os.path.exists(alert_filename) and not overwrite:
         raise IOError("{} already exists!".format(alert_filename))
 
-    with open(alert_filename, 'wb') as out:
+    with open(alert_filename, "wb") as out:
         writer(out, schema, [alert])
 
+
 def encode_into_avro(alert: dict, schema_file: str) -> str:
     """Encode a dict record into avro bytes
 
     Parameters
     ----------
     alert: dict
         A Dictionary of alert data
     schema_file: str
         Path of avro schema file
 
     Returns
-    ----------
+    -------
     value: str
         a bytes string with avro encoded alert data
 
     Examples
-    ----------
+    --------
     >>> r = AlertReader(avro_single_alert)
     >>> alert = r.to_list(size=1)[0]
     >>> avro_encoded = encode_into_avro(alert, schema_path)
     """
     with open(schema_file) as f:
         schema = json.load(f)
 
@@ -296,43 +304,46 @@
     b = io.BytesIO()
     fastavro.schemaless_writer(b, parsed_schema, alert)
 
     return b.getvalue()
 
 
 def get_legal_topic_name(topic: str) -> str:
-    """Returns a legal Kafka topic name
+    r"""Returns a legal Kafka topic name
 
     Special characters are not allowed in the name
     of a Kafka topic. This method returns a legal name
     after removing special characters and converting each
     letter to lowercase
 
     Parameters
     ----------
     topic: str
         topic name, essentially an alert parameter which is to be used
         to create a topic
 
     Returns
-    ----------
+    -------
     legal_topic: str
         A topic name that can be used as a Kafka topic
 
     Examples
-    ----------
+    --------
     >>> bad_name = 'IaMEvi\\l'
     >>> good_name = get_legal_topic_name(bad_name)
     >>> print(good_name)
     iamevil
     """
-    legal_topic = ''.join(a.lower() for a in topic if a.isalpha())
+    legal_topic = "".join(a.lower() for a in topic if a.isalpha())
     return legal_topic
 
-def _get_alert_schema(schema_path: str = None, key: str = None, timeout: int = 1) -> dict:
+
+def _get_alert_schema(
+    schema_path: str = None, key: str = None, timeout: int = 1
+) -> dict:
     """Returns schema for decoding Fink avro alerts
 
     This method downloads the latest schema available on the fink client server
     or falls back to using a custom schema provided by the user.
 
     Parameters
     ----------
@@ -341,20 +352,20 @@
         Note that schema doesn't get downloaded from Fink servers
         if schema_path is given
     timeout: int, optional
         Timeout (sec) when attempting to download the schema from Fink servers.
         Default is 1 second.
 
     Returns
-    ----------
+    -------
     parsed_schema: dict
         Dictionary of json format schema for decoding avro alerts from Fink
 
     Examples
-    ----------
+    --------
     direct download
     >>> schema = _get_alert_schema() # doctest: +NORMALIZE_WHITESPACE, +ELLIPSIS
     Traceback (most recent call last):
       ...
     NotImplementedError:
             The message cannot be decoded as there is no key (None). Either specify a
             key when writing the alert, or specify manually the schema path.
@@ -374,18 +385,18 @@
         msg = """
         The message cannot be decoded as there is no key (None). Either specify a
         key when writing the alert, or specify manually the schema path.
         """
         raise NotImplementedError(msg)
 
     # User-defined schema
-    if isinstance(schema_path, str) and schema_path != '':
+    if isinstance(schema_path, str) and schema_path != "":
         with open(schema_path) as f:
             schema = json.load(f)
-    elif isinstance(schema_path, str) and schema_path == '':
+    elif isinstance(schema_path, str) and schema_path == "":
         msg = """
         `schema_path` must be a non-empty string (path to a avsc file).
         """
         raise IOError(msg)
     # Finally using the key
     elif key is not None:
         # get schema from fink-client
@@ -401,40 +412,43 @@
             {} could not be downloaded. Check your internet connection, or the
             availability of the file at {}
             """.format(schema_name, os.path.join(base_url, tree))
             print(msg)
 
     return fastavro.parse_schema(schema)
 
+
 def _decode_avro_alert(avro_alert: io.IOBase, schema: dict) -> Any:
     """Decodes a file-like stream of avro data
 
     Parameters
     ----------
     avro_alert: io.IOBase
         a file-like stream with avro encoded data
 
     schema: dict
         Dictionary of json format schema to decode avro data
 
     Returns
-    ----------
+    -------
     record: Any
         Record obtained after decoding avro data (typically, dict)
     """
     avro_alert.seek(0)
     return fastavro.schemaless_reader(avro_alert, schema)
 
 
 if __name__ == "__main__":
     """ Run the test suite """
 
     args = globals()
-    args['avro_single_alert'] = 'datatest/ZTF19acihgng.avro'
-    args['avro_multi_file'] = 'datatest/avro_multi_alerts.avro'
-    args['avro_multi_file2'] = 'datatest/avro_multi_alerts_other.avro'
-    args['avro_list'] = ['datatest/ZTF19acihgng.avro', 'datatest/ZTF19acyfkzd.avro']
-    args['avro_folder'] = 'datatest'
-    args['avro_gzipped'] = 'datatest/elasticc/alert_mjd60674.0512_obj747_src1494043.avro.gz'
-    args['schema_path'] = 'schemas/tests/distribution_schema_0p2.avsc'
+    args["avro_single_alert"] = "datatest/ZTF19acihgng.avro"
+    args["avro_multi_file"] = "datatest/avro_multi_alerts.avro"
+    args["avro_multi_file2"] = "datatest/avro_multi_alerts_other.avro"
+    args["avro_list"] = ["datatest/ZTF19acihgng.avro", "datatest/ZTF19acyfkzd.avro"]
+    args["avro_folder"] = "datatest"
+    args["avro_gzipped"] = (
+        "datatest/elasticc/alert_mjd60674.0512_obj747_src1494043.avro.gz"
+    )
+    args["schema_path"] = "schemas/tests/distribution_schema_0p2.avsc"
 
     regular_unit_tests(global_args=args)
```

### Comparing `fink-client-7.2/fink_client/configuration.py` & `fink-client-8.0/fink_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,34 +14,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import yaml
 import os
 
 from fink_client.tester import regular_unit_tests
 
-_ROOTDIR = os.path.join(os.environ['HOME'], ".finkclient")
+_ROOTDIR = os.path.join(os.environ["HOME"], ".finkclient")
 _CREDNAME = "credentials.yml"
 
+
 def write_credentials(dict_file: dict, verbose: bool = False, tmp: bool = False):
-    """ Store user credentials on the computer.
+    """Store user credentials on the computer.
 
     To get your credentials, contact Fink admins or fill the registration form:
         https://forms.gle/2td4jysT4e9pkf889
 
     Parameters
     ----------
     dict_file: dict
         Dictionnary containing user credentials.
     verbose: bool, optional
         If True, print the credentials location. Default is False.
     tmp: bool, optional
         If True, store the credentials under /tmp. Default is False.
 
     Examples
-    ----------
+    --------
     >>> conf = {
     ...   'username': 'test',
     ...   'password': None,
     ...   'mytopics': ['rrlyr'],
     ...   'servers': 'localhost:9093',
     ...   'group_id': 'test_group',
     ...   'maxtimeout': 10
@@ -51,46 +52,50 @@
     if tmp:
         ROOTDIR = "/tmp"
     else:
         ROOTDIR = _ROOTDIR
 
     # check there are no missing information
     mandatory_keys = [
-        'username', 'password', 'group_id',
-        'mytopics', 'servers',
-        'maxtimeout'
+        "username",
+        "password",
+        "group_id",
+        "mytopics",
+        "servers",
+        "maxtimeout",
     ]
     for k in mandatory_keys:
-        assert k in dict_file.keys(), 'You need to specify {}'.format(k)
+        assert k in dict_file.keys(), "You need to specify {}".format(k)
 
     # Create the folder if it does not exist
     os.makedirs(ROOTDIR, exist_ok=True)
 
     # Store data into yml file
-    with open(os.path.join(ROOTDIR, _CREDNAME), 'w') as f:
+    with open(os.path.join(ROOTDIR, _CREDNAME), "w") as f:
         yaml.dump(dict_file, f)
 
     if verbose:
-        print('Credentials stored at {}/{}'.format(ROOTDIR, _CREDNAME))
+        print("Credentials stored at {}/{}".format(ROOTDIR, _CREDNAME))
+
 
 def load_credentials(tmp: bool = False) -> dict:
-    """ Load fink-client credentials.
+    """Load fink-client credentials.
 
     Parameters
     ----------
     tmp: bool, optional
         If True, load the credentials from /tmp. Default is False.
 
     Returns
-    --------
+    -------
     creds: dict
         Dictionnary containing user credentials.
 
     Examples
-    ----------
+    --------
     >>> conf_in = {
     ...   'username': 'test',
     ...   'password': None,
     ...   'mytopics': ['rrlyr'],
     ...   'servers': 'localhost:9093',
     ...   'group_id': 'test_group',
     ...   'maxtimeout': 10
@@ -130,22 +135,22 @@
         raise IOError(msg)
 
     with open(path) as f:
         creds = yaml.load(f, Loader=yaml.FullLoader)
 
     return creds
 
+
 def mm_topic_names():
-    """ Return list of topics with MMA schema
-    """
+    """Return list of topics with MMA schema"""
     out = [
-        'fink_grb_bronze',
-        'fink_grb_silver',
-        'fink_grb_gold',
-        'fink_gw_bronze',
+        "fink_grb_bronze",
+        "fink_grb_silver",
+        "fink_grb_gold",
+        "fink_gw_bronze",
     ]
     return out
 
 
 if __name__ == "__main__":
     """ Run the test suite """
```

### Comparing `fink-client-7.2/fink_client/consumer.py` & `fink-client-8.0/fink_client/consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2019-2020 AstroLab Software
+# Copyright 2019-2024 AstroLab Software
 # Author: Abhishek Chauhan, Julien Peloton
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,30 +14,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import json
 import time
 import fastavro
 import confluent_kafka
+from datetime import datetime, timezone
 
-from fink_client.avroUtils import write_alert
-from fink_client.avroUtils import _get_alert_schema
-from fink_client.avroUtils import _decode_avro_alert
+from fink_client.avro_utils import write_alert
+from fink_client.avro_utils import _get_alert_schema
+from fink_client.avro_utils import _decode_avro_alert
 from fink_client.configuration import mm_topic_names
 
+
 class AlertError(Exception):
+    """Base class for exception"""
+
     pass
 
 
 class AlertConsumer:
-    """
-    High level Kafka consumer to receive alerts from Fink broker
-    """
+    """High level Kafka consumer to receive alerts from Fink broker"""
 
-    def __init__(self, topics: list, config: dict, schema_path=None):
+    def __init__(self, topics: list, config: dict, schema_path=None, dump_schema=False):
         """Creates an instance of `AlertConsumer`
 
         Parameters
         ----------
         topics : list of str
             list of topics to subscribe
         config: dict
@@ -52,134 +54,141 @@
                 Kafka servers to connect to
         """
         self._topics = topics
         self._kafka_config = _get_kafka_config(config)
         self.schema_path = schema_path
         self._consumer = confluent_kafka.Consumer(self._kafka_config)
         self._consumer.subscribe(self._topics)
+        self.dump_schema = dump_schema
 
     def __enter__(self):
+        """Enter"""
         return self
 
     def __exit__(self, type, value, traceback):
+        """Exit"""
         self._consumer.close()
 
     def process_message(self, msg):
-        """ Process message from Kafka
+        """Process message from Kafka
 
         Parameters
         ----------
         msg: confluent_kafka.Message
             Object containing message information
 
         Returns
-        ----------
+        -------
         list: [tuple(str, dict, str)]
             list of topic, alert, key
             returns an empty list on timeout
         """
         # msg.error() returns None or KafkaError
         if msg.error():
             error_message = """
             Error: {} topic: {}[{}] at offset: {} with key: {}
             """.format(
-                msg.error(), msg.topic(),
-                msg.partition(), msg.offset(),
-                str(msg.key())
+                msg.error(), msg.topic(), msg.partition(), msg.offset(), str(msg.key())
             )
             raise AlertError(error_message)
 
         topic = msg.topic()
 
         # decode the key if it is bytes
         key = msg.key()
 
         if isinstance(key, bytes):
-            key = key.decode('utf8')
+            key = key.decode("utf8")
         if key is None:
             # compatibility with previous scheme
             key = ""
 
         try:
             _parsed_schema = fastavro.schema.parse_schema(json.loads(key))
+            if self.dump_schema:
+                today = datetime.now(timezone.utc).isoformat()
+                filename = "schema_{}.json".format(today)
+                with open(filename, "w") as json_file:
+                    json.dump(_parsed_schema, json_file, sort_keys=True, indent=4)
+                print("Schema saved as {}".format(filename))
             alert = self._decode_msg(_parsed_schema, msg)
-        except json.JSONDecodeError:
+        except json.JSONDecodeError as exc:
             # Old way
             if self.schema_path is not None:
                 _parsed_schema = _get_alert_schema(schema_path=self.schema_path)
                 alert = self._decode_msg(_parsed_schema, msg)
             elif key is not None:
                 try:
                     _parsed_schema = _get_alert_schema(key=key)
                     alert = self._decode_msg(_parsed_schema, msg)
                 except IndexError:
-                    _parsed_schema = _get_alert_schema(key=key + '_replayed')
+                    _parsed_schema = _get_alert_schema(key=key + "_replayed")
                     alert = self._decode_msg(_parsed_schema, msg)
             else:
                 msg = """
                 The message cannot be decoded as there is no key (None). Alternatively
                 specify manually the schema path when instantiating ``AlertConsumer`` (or from fink_consumer).
                 """
-                raise NotImplementedError(msg)
+                raise NotImplementedError(msg) from exc
 
         return topic, alert, key
 
     def poll(self, timeout: float = -1) -> (str, dict):
-        """ Consume one message from Fink server
+        """Consume one message from Fink server
 
         Parameters
         ----------
         timeout: float, optional
             maximum time to block waiting for a message
             if not set default is None i.e. wait indefinitely
 
         Returns
-        ----------
+        -------
         (topic, alert, key): tuple(str, dict, str)
             returns (None, None, None) on timeout
         """
         msg = self._consumer.poll(timeout)
         if msg is None:
             return None, None, None
 
         return self.process_message(msg)
 
     def _decode_msg(self, parsed_schema, msg) -> dict:
-        """ decode message using parsed schema
+        """Decode message using parsed schema
 
         Parameters
         ----------
         parsed_schema: dict
             Dictionary of json format schema for decoding avro alerts from Fink.
             Output of _get_alert_schema
         msg: bytes
             Message received
 
         Returns
-        ----------
+        -------
         alert: dict
             Decoded message
         """
         self._parsed_schema = parsed_schema
         avro_alert = io.BytesIO(msg.value())
         return _decode_avro_alert(avro_alert, self._parsed_schema)
 
     def consume(self, num_alerts: int = 1, timeout: float = -1) -> list:
-        """ Consume and return list of messages
+        """Consume and return list of messages
 
         Parameters
         ----------
         num_messages: int
             maximum number of messages to return
         timeout: float
             maximum time to block waiting for messages
             if not set default is None i.e. wait indefinitely
 
         Returns
-        ----------
+        -------
         list: [tuple(str, dict, str)]
             list of topic, alert, key
             returns an empty list on timeout
         """
         alerts = []
         msg_list = self._consumer.consume(num_alerts, timeout)
 
@@ -191,90 +200,93 @@
             topic, alert, key = self.process_message(msg)
 
             alerts.append((topic, alert, key))
 
         return alerts
 
     def poll_and_write(
-            self, outdir: str, timeout: float = -1,
-            overwrite: bool = False) -> (str, dict):
-        """ Consume one message from Fink server, save alert on disk and
-        return (topic, alert, key)
+        self, outdir: str, timeout: float = -1, overwrite: bool = False
+    ) -> (str, dict):
+        """Consume one message from Fink server
+
+        Notes
+        -----
+        It also saves the alert on disk and return (topic, alert, key)
 
         Parameters
         ----------
         outdir: str
             Folder to store the alert. It must exists.
         timeout: float, optional
             maximum time to block waiting for messages
             if not set default is None i.e. wait indefinitely
         overwrite: bool, optional
             If True, allow an existing alert to be overwritten.
             Default is False.
 
         Returns
-        ----------
+        -------
         (topic, alert): tuple(str, dict)
             returns (None, None) on timeout
 
         """
         topic, alert, key = self.poll(timeout)
         is_mma = topic in mm_topic_names()
 
         if is_mma:
-            id1 = 'objectId'
-            id2 = 'triggerId'
+            id1 = "objectId"
+            id2 = "triggerId"
         else:
-            id1 = 'objectId'
-            id2 = 'candid'
+            id1 = "objectId"
+            id2 = "candid"
 
         if topic is not None:
             write_alert(
                 alert,
                 self._parsed_schema,
                 outdir,
                 overwrite=overwrite,
                 id1=id1,
-                id2=id2
+                id2=id2,
             )
 
         return topic, alert, key
 
     def available_topics(self) -> dict:
-        """ Return available broker topics
+        """Return available broker topics
 
         Note, this routine only display topics, but users need
         to be authorized to poll data.
 
         Returns
-        ---------
+        -------
         topics: dict
             Keys are topic names, values are metadata
 
         """
         return self._consumer.list_topics().topics
 
     def available_brokers(self) -> dict:
-        """ Return available brokers
+        """Return available brokers
 
         Returns
-        ---------
+        -------
         brokers: dict
             Keys are broker ID, values are metadata with IP:PORT
 
         """
         return self._consumer.list_topics().brokers
 
     def close(self):
         """Close connection to Fink broker"""
         self._consumer.close()
 
 
 def return_offsets(consumer, topic, waitfor=1, timeout=10, verbose=False):
-    """ Poll servers to get the total committed offsets, and remaining lag
+    """Poll servers to get the total committed offsets, and remaining lag
 
     Parameters
     ----------
     consumer: confluent_kafka.Consumer
         Kafka consumer
     topic: str
         Topic name
@@ -282,28 +294,31 @@
         Time in second to wait before polling. Default is 1 second.
     timeout: int, optional
         Timeout in second when polling the servers. Default is 10.
     verbose: bool, optional
         If True, prints useful table. Default is False.
 
     Returns
-    ---------
+    -------
     total_offsets: int
         Total number of messages committed across all partitions
     total_lag: int
         Remaining messages in the topic across all partitions.
     """
     time.sleep(waitfor)
     # Get the topic's partitions
     metadata = consumer.list_topics(topic, timeout=timeout)
     if metadata.topics[topic].error is not None:
         raise confluent_kafka.KafkaException(metadata.topics[topic].error)
 
     # Construct TopicPartition list of partitions to query
-    partitions = [confluent_kafka.TopicPartition(topic, p) for p in metadata.topics[topic].partitions]
+    partitions = [
+        confluent_kafka.TopicPartition(topic, p)
+        for p in metadata.topics[topic].partitions
+    ]
 
     # Query committed offsets for this group and the given partitions
     try:
         committed = consumer.committed(partitions, timeout=timeout)
     except confluent_kafka.KafkaException as exception:
         kafka_error = exception.args[0]
         if kafka_error.code() == confluent_kafka.KafkaError._TIMED_OUT:
@@ -314,15 +329,17 @@
     total_offsets = 0
     total_lag = 0
     if verbose:
         print("%-50s  %9s  %9s" % ("Topic [Partition]", "Committed", "Lag"))
         print("=" * 72)
     for partition in committed:
         # Get the partitions low and high watermark offsets.
-        (lo, hi) = consumer.get_watermark_offsets(partition, timeout=timeout, cached=False)
+        (lo, hi) = consumer.get_watermark_offsets(
+            partition, timeout=timeout, cached=False
+        )
 
         if partition.offset == confluent_kafka.OFFSET_INVALID:
             offset = "-"
         else:
             offset = "%d" % (partition.offset)
 
         if hi < 0:
@@ -336,59 +353,55 @@
         else:
             lag = "%d" % (hi - partition.offset)
         #
         total_offsets = total_offsets + partition.offset
         total_lag = total_lag + int(lag)
 
         if verbose:
-            print("%-50s  %9s  %9s" % (
-                "{} [{}]".format(partition.topic, partition.partition), offset, lag))
+            print(
+                "%-50s  %9s  %9s"
+                % ("{} [{}]".format(partition.topic, partition.partition), offset, lag)
+            )
     if verbose:
         print("-" * 72)
-        print("%-50s  %9s  %9s" % (
-            "Total", total_offsets, total_lag))
+        print("%-50s  %9s  %9s" % ("Total", total_offsets, total_lag))
         print("-" * 72)
 
     return total_offsets, total_lag
 
+
 def _get_kafka_config(config: dict) -> dict:
     """Returns configurations for a consumer instance
 
     Parameters
     ----------
     config: dict
         Dictionary of configurations
 
     Returns
-    ----------
+    -------
     kafka_config: dict
         Dictionary with configurations for creating an instance of
         a secured Kafka consumer
     """
     kafka_config = {}
-    default_config = {
-        "auto.offset.reset": "earliest"
-    }
+    default_config = {"auto.offset.reset": "earliest"}
 
-    if 'username' in config and 'password' in config:
+    if "username" in config and "password" in config:
         kafka_config["security.protocol"] = "sasl_plaintext"
         kafka_config["sasl.mechanism"] = "SCRAM-SHA-512"
         kafka_config["sasl.username"] = config["username"]
         kafka_config["sasl.password"] = config["password"]
 
     kafka_config["group.id"] = config["group_id"]
 
     kafka_config.update(default_config)
 
     # use servers if given
-    if 'bootstrap.servers' in config:
+    if "bootstrap.servers" in config:
         kafka_config["bootstrap.servers"] = config["bootstrap.servers"]
     else:
         # use default fink_servers
-        fink_servers = [
-            "localhost:9093",
-            "localhost:9094",
-            "localhost:9095"
-        ]
+        fink_servers = ["localhost:9093", "localhost:9094", "localhost:9095"]
         kafka_config["bootstrap.servers"] = "{}".format(",".join(fink_servers))
 
     return kafka_config
```

### Comparing `fink-client-7.2/fink_client/scripts/__init__.py` & `fink-client-8.0/fink_client/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `fink-client-7.2/fink_client/scripts/fink_alert_viewer.py` & `fink-client-8.0/fink_client/scripts/fink_alert_viewer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 #!/usr/bin/env python
-# Copyright 2019-2020 AstroLab Software
+# Copyright 2019-2024 AstroLab Software
 # Author: Julien Peloton
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" Display cutouts and lightcurve from a ZTF alert """
+"""Display cutouts and lightcurve from a ZTF alert"""
+
 import argparse
 
 import matplotlib
 import matplotlib.pyplot as plt
 
 import numpy as np
 
-from fink_client.avroUtils import AlertReader
+from fink_client.avro_utils import AlertReader
 from fink_client.visualisation import show_stamps
 from fink_client.visualisation import extract_field
 
 # For plots
-font = {
-    'weight': 'bold',
-    'size': 22
-}
+font = {"weight": "bold", "size": 22}
 
-matplotlib.rc('font', **font)
+matplotlib.rc("font", **font)
 
 # Bands
-filter_color = {1: '#1f77b4', 2: '#ff7f0e', 3: '#2ca02c'}
+filter_color = {1: "#1f77b4", 2: "#ff7f0e", 3: "#2ca02c"}
 # [
 #     '#1f77b4',  # muted blue
 #     '#ff7f0e',  # safety orange
 #     '#2ca02c',  # cooked asparagus green
 #     '#d62728',  # brick red
 #     '#9467bd',  # muted purple
 #     '#8c564b',  # chestnut brown
 #     '#e377c2',  # raspberry yogurt pink
 #     '#7f7f7f',  # middle gray
 #     '#bcbd22',  # curry yellow-green
 #     '#17becf'   # blue-teal
 # ]
-filter_name = {1: 'g band', 2: 'r band', 3: 'i band'}
+filter_name = {1: "g band", 2: "r band", 3: "i band"}
+
 
 def main():
     """ """
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
-        '-filename', type=str, default='',
-        help="Path to an alert data file (avro format)")
+        "-filename",
+        type=str,
+        default="",
+        help="Path to an alert data file (avro format)",
+    )
     args = parser.parse_args(None)
 
     r = AlertReader(args.filename)
 
     # Display the cutouts contained in the alert
     alert = r.to_list(size=1)[0]
-    print(alert['objectId'])
+    print(alert["objectId"])
     fig = plt.figure(num=0, figsize=(12, 4))
     show_stamps(alert, fig)
 
     # extract current and historical data as one vector
-    mag = extract_field(alert, 'magpsf')
-    error = extract_field(alert, 'sigmapsf')
+    mag = extract_field(alert, "magpsf")
+    error = extract_field(alert, "sigmapsf")
     upper = extract_field(alert, "diffmaglim")
 
     # filter bands
     fid = extract_field(alert, "fid")
 
     # Rescale dates to end at 0
     jd = extract_field(alert, "jd")
@@ -88,27 +90,38 @@
         mask = np.where(fid == filt)[0]
 
         # Skip if no data
         if len(mask) == 0:
             continue
 
         # y data
-        maskNotNone = mag[mask] != None
+        maskNotNone = mag[mask] != None  # noqa: E711
         plt.errorbar(
-            dates[mask][maskNotNone], mag[mask][maskNotNone],
+            dates[mask][maskNotNone],
+            mag[mask][maskNotNone],
             yerr=error[mask][maskNotNone],
-            color=filter_color[filt], marker='o', ls='',
-            label=filter_name[filt], mew=4)
+            color=filter_color[filt],
+            marker="o",
+            ls="",
+            label=filter_name[filt],
+            mew=4,
+        )
         # Upper limits
         plt.plot(
-            dates[mask][~maskNotNone], upper[mask][~maskNotNone],
-            color=filter_color[filt], marker='v', ls='', mew=4, alpha=0.5)
+            dates[mask][~maskNotNone],
+            upper[mask][~maskNotNone],
+            color=filter_color[filt],
+            marker="v",
+            ls="",
+            mew=4,
+            alpha=0.5,
+        )
         plt.title(title)
     plt.legend()
     plt.gca().invert_yaxis()
-    plt.xlabel('Days to candidate')
-    plt.ylabel('Difference magnitude')
+    plt.xlabel("Days to candidate")
+    plt.ylabel("Difference magnitude")
     plt.show()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fink-client-7.2/fink_client/scripts/fink_client_register.py` & `fink-client-8.0/fink_client/scripts/fink_client_register.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,55 +14,75 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from fink_client.configuration import write_credentials
 from fink_client.configuration import load_credentials
 
 import argparse
 
+
 def main():
     """ """
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
-        '-username', type=str, default='',
-        help="username used for the authentication on the Kafka cluster")
-    parser.add_argument(
-        '-password', type=str, default=None,
-        help="If specified, password for the authentication. Default is None.")
-    parser.add_argument(
-        '-group_id', type=str, default='',
-        help="group_id used for the authentication on the Kafka cluster")
-    parser.add_argument(
-        '-mytopics', nargs='+', type=str, default=[],
-        help="Space-separated list of subscribed topics. E.g. --topics t1 t2")
-    parser.add_argument(
-        '-servers', type=str, default='.',
-        help="Comma-separated list of IP:PORT as a single string. e.g. 's1,s2'")
-    parser.add_argument(
-        '-maxtimeout', type=int, default=10,
-        help="Timeout when polling the servers. Default is 10 seconds.")
+        "-username",
+        type=str,
+        default="",
+        help="username used for the authentication on the Kafka cluster",
+    )
+    parser.add_argument(
+        "-password",
+        type=str,
+        default=None,
+        help="If specified, password for the authentication. Default is None.",
+    )
+    parser.add_argument(
+        "-group_id",
+        type=str,
+        default="",
+        help="group_id used for the authentication on the Kafka cluster",
+    )
+    parser.add_argument(
+        "-mytopics",
+        nargs="+",
+        type=str,
+        default=[],
+        help="Space-separated list of subscribed topics. E.g. --topics t1 t2",
+    )
+    parser.add_argument(
+        "-servers",
+        type=str,
+        default=".",
+        help="Comma-separated list of IP:PORT as a single string. e.g. 's1,s2'",
+    )
+    parser.add_argument(
+        "-maxtimeout",
+        type=int,
+        default=10,
+        help="Timeout when polling the servers. Default is 10 seconds.",
+    )
     parser.add_argument(
-        '--tmp', action='store_true',
-        help="If specified, register credentials in /tmp.")
+        "--tmp", action="store_true", help="If specified, register credentials in /tmp."
+    )
     parser.add_argument(
-        '--verbose', action='store_true',
-        help="If specified, print useful information.")
+        "--verbose", action="store_true", help="If specified, print useful information."
+    )
     args = parser.parse_args(None)
 
-    if args.password == 'None':
+    if args.password == "None":
         pwd = None
     else:
         pwd = args.password
 
     dict_file = {
-        'username': args.username,
-        'password': pwd,
-        'group_id': args.group_id,
-        'mytopics': args.mytopics,
-        'servers': args.servers,
-        'maxtimeout': args.maxtimeout
+        "username": args.username,
+        "password": pwd,
+        "group_id": args.group_id,
+        "mytopics": args.mytopics,
+        "servers": args.servers,
+        "maxtimeout": args.maxtimeout,
     }
 
     # Write credentials
     write_credentials(dict_file, args.verbose, args.tmp)
 
     # check credentials are correct
     if args.verbose:
```

### Comparing `fink-client-7.2/fink_client/scripts/fink_consumer.py` & `fink-client-8.0/fink_client/scripts/fink_consumer.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,121 +9,167 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" Kafka consumer to listen and archive Fink streams from the Livestream service """
+"""Kafka consumer to listen and archive Fink streams from the Livestream service"""
+
 import sys
 import os
 
 import argparse
 import time
 
 from tabulate import tabulate
+from astropy.time import Time
 
 from fink_client.consumer import AlertConsumer
 from fink_client.configuration import load_credentials
 from fink_client.configuration import mm_topic_names
 
+
 def main():
     """ """
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
-        '--display', action='store_true',
-        help="If specified, print on screen information about incoming alert.")
+        "--display",
+        action="store_true",
+        help="If specified, print on screen information about incoming alert.",
+    )
     parser.add_argument(
-        '-limit', type=int, default=None,
-        help="If specified, download only `limit` alerts. Default is None.")
+        "-limit",
+        type=int,
+        default=None,
+        help="If specified, download only `limit` alerts. Default is None.",
+    )
     parser.add_argument(
-        '--available_topics', action='store_true',
-        help="If specified, print on screen information about available topics.")
+        "--available_topics",
+        action="store_true",
+        help="If specified, print on screen information about available topics.",
+    )
     parser.add_argument(
-        '--save', action='store_true',
-        help="If specified, save alert data on disk (Avro). See also -outdir.")
+        "--save",
+        action="store_true",
+        help="If specified, save alert data on disk (Avro). See also -outdir.",
+    )
     parser.add_argument(
-        '-outdir', type=str, default='.',
-        help="Folder to store incoming alerts if --save is set. It must exist.")
+        "-outdir",
+        type=str,
+        default=".",
+        help="Folder to store incoming alerts if --save is set. It must exist.",
+    )
     parser.add_argument(
-        '-schema', type=str, default=None,
-        help="Avro schema to decode the incoming alerts. Default is None (version taken from each alert)"
+        "-schema",
+        type=str,
+        default=None,
+        help="Avro schema to decode the incoming alerts. Default is None (version taken from each alert)",
+    )
+    parser.add_argument(
+        "--dump_schema",
+        action="store_true",
+        help="If specified, save the schema on disk (json file)",
     )
     args = parser.parse_args(None)
 
     # load user configuration
     conf = load_credentials()
 
     myconfig = {
-        "username": conf['username'],
-        'bootstrap.servers': conf['servers'],
-        'group_id': conf['group_id']}
+        "username": conf["username"],
+        "bootstrap.servers": conf["servers"],
+        "group_id": conf["group_id"],
+    }
 
-    if conf['password'] is not None:
-        myconfig['password'] = conf['password']
+    if conf["password"] is not None:
+        myconfig["password"] = conf["password"]
 
     # Instantiate a consumer
     if args.schema is None:
         schema = None
     else:
         schema = args.schema
-    consumer = AlertConsumer(conf['mytopics'], myconfig, schema_path=schema)
+    consumer = AlertConsumer(
+        conf["mytopics"], myconfig, schema_path=schema, dump_schema=args.dump_schema
+    )
 
     if args.available_topics:
         print(consumer.available_topics().keys())
         sys.exit(0)
 
     # Time to wait before polling again if no alerts
-    maxtimeout = conf['maxtimeout']
+    maxtimeout = conf["maxtimeout"]
 
     if not os.path.isdir(args.outdir):
         os.makedirs(args.outdir, exist_ok=True)
 
     # infinite loop
     maxpoll = args.limit if args.limit else 1e10
     try:
         poll_number = 0
         while poll_number < maxpoll:
             if args.save:
                 # Save alerts on disk
                 topic, alert, key = consumer.poll_and_write(
-                    outdir=args.outdir,
-                    timeout=maxtimeout,
-                    overwrite=True
+                    outdir=args.outdir, timeout=maxtimeout, overwrite=True
                 )
             else:
                 # TODO: this is useless to get it and done nothing
                 # why not thinking about handler like Comet?
                 topic, alert, key = consumer.poll(timeout=maxtimeout)
 
             if topic is not None:
                 poll_number += 1
                 is_mma = topic in mm_topic_names()
 
             if args.display and topic is not None:
-                utc = time.strftime('%Y-%m-%d %H:%M:%S', time.gmtime())
+                utc = time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime())
                 if is_mma:
-                    table = [[alert['objectId'], alert['fink_class'], topic, alert['rate'], alert['observatory'], alert['triggerId']]]
-                    headers = ['ObjectId', 'Classification', 'Topic', 'Rate (mag/day)', 'Observatory', 'Trigger ID']
+                    table = [
+                        [
+                            alert["objectId"],
+                            alert["fink_class"],
+                            topic,
+                            alert["rate"],
+                            alert["observatory"],
+                            alert["triggerId"],
+                        ]
+                    ]
+                    headers = [
+                        "ObjectId",
+                        "Classification",
+                        "Topic",
+                        "Rate (mag/day)",
+                        "Observatory",
+                        "Trigger ID",
+                    ]
                 else:
                     table = [
                         [
-                            alert['timestamp'], utc, topic, alert['objectId'],
-                            alert['cdsxmatch'],
-                            alert['candidate']['magpsf']
+                            Time(alert["candidate"]["jd"], format="jd").iso,
+                            utc,
+                            topic,
+                            alert["objectId"],
+                            alert["cdsxmatch"],
+                            alert["candidate"]["magpsf"],
                         ],
                     ]
                     headers = [
-                        'Emitted at (UTC)', 'Received at (UTC)',
-                        'Topic', 'objectId', 'Simbad', 'Magnitude'
+                        "Emitted at (UTC)",
+                        "Received at (UTC)",
+                        "Topic",
+                        "objectId",
+                        "Simbad",
+                        "Magnitude",
                     ]
                 print(tabulate(table, headers, tablefmt="pretty"))
             elif args.display:
-                print('No alerts the last {} seconds'.format(maxtimeout))
+                print("No alerts the last {} seconds".format(maxtimeout))
     except KeyboardInterrupt:
-        sys.stderr.write('%% Aborted by user\n')
+        sys.stderr.write("%% Aborted by user\n")
     finally:
         consumer.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fink-client-7.2/fink_client/scripts/fink_datatransfer.py` & `fink-client-8.0/fink_client/scripts/fink_datatransfer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python
-# Copyright 2023 AstroLab Software
+# Copyright 2023-2024 AstroLab Software
 # Author: Julien Peloton, Saikou Oumar BAH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" Kafka consumer to listen and archive Fink streams
-    from the data transfer service
-"""
+"""Kafka consumer to listen and archive Fink streams from the data transfer service"""
+
 import sys
 import os
 import io
 import json
 import argparse
 import logging
 import psutil
@@ -38,73 +37,79 @@
 
 from fink_client.configuration import load_credentials
 
 from fink_client.consumer import return_offsets
 
 
 def print_offsets(kafka_config, topic, maxtimeout=10, verbose=True):
-    """ Wrapper around `consumer.return_offsets`
+    """Wrapper around `consumer.return_offsets`
 
     If the server is rebalancing the offsets, it will exit the program.
 
     Parameters
     ----------
     kafka_config: dic
         Dictionary with consumer parameters
     topic: str
         Topic name
     maxtimeout: int, optional
         Timeout in second, when polling the servers
 
     Returns
-    ----------
+    -------
     total_offsets: int
         Total number of messages committed across all partitions
     total_lag: int
         Remaining messages in the topic across all partitions.
     """
     consumer = confluent_kafka.Consumer(kafka_config)
 
-    topics = ['{}'.format(topic)]
+    topics = ["{}".format(topic)]
     consumer.subscribe(topics)
-    total_offset, total_lag = return_offsets(consumer, topic, timeout=maxtimeout, waitfor=0, verbose=verbose)
+    total_offset, total_lag = return_offsets(
+        consumer, topic, timeout=maxtimeout, waitfor=0, verbose=verbose
+    )
     if (total_offset, total_lag) == (-1, -1):
-        print("Warning: Consumer group '{}' is rebalancing. Please wait.".format(kafka_config['group.id']))
+        print(
+            "Warning: Consumer group '{}' is rebalancing. Please wait.".format(
+                kafka_config["group.id"]
+            )
+        )
         sys.exit()
     consumer.close()
 
     return total_lag, total_offset
 
 
 def get_schema(kafka_config, topic, maxtimeout):
-    """ Poll the schema data from the schema topic
+    """Poll the schema data from the schema topic
 
     Parameters
     ----------
     kafka_config: dic
         Dictionary with consumer parameters
     topic: str
         Topic name
     timeout: int, optional
         Timeout in second, when polling the servers
 
     Returns
-    ----------
+    -------
     schema: None or dic
         Schema data. None if the poll was not successful.
         Reasons to get None:
             1. timeout has been reached (increase timeout)
             2. topic is empty (produce new data)
             3. topic does not exist (create the topic)
     """
     # Instantiate a consumer
     consumer_schema = confluent_kafka.Consumer(kafka_config)
 
     # Subscribe to schema topic
-    topics = ['{}_schema'.format(topic)]
+    topics = ["{}_schema".format(topic)]
     consumer_schema.subscribe(topics)
 
     # Poll
     msg = consumer_schema.poll(maxtimeout)
     if msg is not None:
         schema = fastavro.schema.parse_schema(json.loads(msg.key()))
     else:
@@ -112,15 +117,15 @@
 
     consumer_schema.close()
 
     return schema
 
 
 def my_assign(consumer, partitions):
-    """ Function to reset offsets when (re)polling
+    """Function to reset offsets when (re)polling
 
     It must be passed when subscribing to a topic:
         `consumer.subscribe(topics, on_assign=my_assign)`
 
     Parameters
     ----------
     consumer: confluent_kafka.Consumer
@@ -130,64 +135,63 @@
     """
     for p in partitions:
         p.offset = 0
     consumer.assign(partitions)
 
 
 def reset_offset(kafka_config, topic):
-    """ Rest offsets for a given topic
+    """Rest offsets for a given topic
 
     Parameters
     ----------
     kafka_config: dict
         Kafka server parameters
     topic: str
         Topic name
     """
     consumer = confluent_kafka.Consumer(kafka_config)
-    topics = ['{}'.format(topic)]
+    topics = ["{}".format(topic)]
     consumer.subscribe(topics, on_assign=my_assign)
     consumer.close()
 
 
 def return_partition_offset(consumer, topic, partition):
-    """ Return the offset and the remaining lag of a partition
+    """Return the offset and the remaining lag of a partition
 
     consumer: confluent_kafka.Consumer
         Kafka consumer
     topic: str
         Topic name
     partition: int
         The partition number
 
     Returns
-    ----------
+    -------
     offset : int
         Total number of offsets in the topic
     """
-
     topicPartition = confluent_kafka.TopicPartition(topic, partition)
     low_offset, high_offset = consumer.get_watermark_offsets(topicPartition)
     partition_size = high_offset - low_offset
 
     return partition_size
 
 
 def return_npartitions(topic, kafka_config):
-    """ Get the number of partitions
+    """Get the number of partitions
 
     Parameters
     ----------
     kafka_config: dic
         Dictionary with consumer parameters
     topic: str
         Topic name
 
     Returns
-    ----------
+    -------
     nbpartitions: int
         Number of partitions in the topic
 
     """
     consumer = confluent_kafka.Consumer(kafka_config)
 
     # Details to get
@@ -207,52 +211,55 @@
 
     consumer.close()
 
     return nbpartitions
 
 
 def return_last_offsets(kafka_config, topic):
-    """ Return the last offsets
+    """Return the last offsets
 
     Parameters
     ----------
     kafka_config: dict
         Kafka consumer config
     topic: str
         Topic name
 
     Returns
-    ----------
+    -------
     offsets: list
         Last offsets of each partition
     """
     consumer = confluent_kafka.Consumer(kafka_config)
-    topics = ['{}'.format(topic)]
+    topics = ["{}".format(topic)]
     consumer.subscribe(topics)
 
     metadata = consumer.list_topics(topic)
     if metadata.topics[topic].error is not None:
         raise confluent_kafka.KafkaException(metadata.topics[topic].error)
 
     # List of partitions
-    partitions = [confluent_kafka.TopicPartition(topic, p) for p in metadata.topics[topic].partitions]
+    partitions = [
+        confluent_kafka.TopicPartition(topic, p)
+        for p in metadata.topics[topic].partitions
+    ]
     committed = consumer.committed(partitions)
     offsets = []
     for partition in committed:
         if partition.offset != confluent_kafka.OFFSET_INVALID:
             offsets.append(partition.offset)
         else:
             offsets.append(0)
 
     consumer.close()
     return offsets
 
 
 def poll(process_id, nconsumers, queue, schema, kafka_config, rng, args):
-    """ Poll data from Kafka servers
+    """Poll data from Kafka servers
 
     Parameters
     ----------
     process_id: int
         ID of the process used for multiprocessing
     nconsumers: int
         Number of consumers (cores) in parallel
@@ -277,203 +284,264 @@
     disable = not args.verbose
 
     poll_number = 0
     while not queue.empty() and poll_number < maxpoll:
         # Getting a partition from the queue
         partition = queue.get()
         tp = confluent_kafka.TopicPartition(
-            args.topic,
-            partition["partition"],
-            offset=partition["offset"]
+            args.topic, partition["partition"], offset=partition["offset"]
         )
         consumer.assign([tp])
         # Getting the total number of alert in the partition
-        offset = return_partition_offset(
-            consumer,
-            args.topic,
-            partition["partition"]
-        )
+        offset = return_partition_offset(consumer, args.topic, partition["partition"])
         # Resuming from the last consumed alert
         initial = partition["offset"]
 
         max_end_check = 4
 
         if offset == initial:
             if partition["status"] < max_end_check:
                 # After max_end_check time if no alerts added,
                 # it is supposed finished
-                queue.put({
-                    "partition": partition["partition"],
-                    "offset": partition["offset"],
-                    "status": partition["status"] + 1
-                })
+                queue.put(
+                    {
+                        "partition": partition["partition"],
+                        "offset": partition["offset"],
+                        "status": partition["status"] + 1,
+                    }
+                )
         else:
             poll_number = initial
             total = offset
-            with trange(total, position=partition["partition"], initial=initial, colour='#F5622E', unit='alerts', disable=disable) as pbar:
+            with trange(
+                total,
+                position=partition["partition"],
+                initial=initial,
+                colour="#F5622E",
+                unit="alerts",
+                disable=disable,
+            ) as pbar:
                 try:
                     while poll_number < maxpoll:
-                        msgs = consumer.consume(
-                            args.batchsize,
-                            args.maxtimeout
-                        )
+                        msgs = consumer.consume(args.batchsize, args.maxtimeout)
                         # Decode the message
                         if msgs is not None:
                             if len(msgs) == 0:
-                                print('[{}] No alerts the last {} seconds ({} polled)... Have to exit(1)\n'.format(process_id, args.maxtimeout, poll_number))
+                                print(
+                                    "[{}] No alerts the last {} seconds ({} polled)... Have to exit(1)\n".format(
+                                        process_id, args.maxtimeout, poll_number
+                                    )
+                                )
                                 # Alerts can be added in the partition later
                                 # putting it again in the queue
                                 # changing the offset to continue where we stopped
-                                queue.put({
-                                    "partition": partition["partition"],
-                                    "offset": poll_number,
-                                    "status": 0
-                                })
+                                queue.put(
+                                    {
+                                        "partition": partition["partition"],
+                                        "offset": poll_number,
+                                        "status": 0,
+                                    }
+                                )
                                 break
 
                             pdf = pd.DataFrame.from_records(
-                                [fastavro.schemaless_reader(io.BytesIO(msg.value()), schema) for msg in msgs],
+                                [
+                                    fastavro.schemaless_reader(
+                                        io.BytesIO(msg.value()), schema
+                                    )
+                                    for msg in msgs
+                                ],
                             )
                             if pdf.empty:
                                 # print('[{}] No alerts the last {} seconds ({} polled)... Exiting\n'.format(process_id, args.maxtimeout, poll_number))
                                 break
 
                             # known mismatches between partitions
                             # see https://github.com/astrolabsoftware/fink-client/issues/165
-                            if 'cats_broad_max_prob' in pdf.columns:
-                                pdf['cats_broad_max_prob'] = pdf['cats_broad_max_prob'].astype('float')
-
-                            if 'cats_broad_class' in pdf.columns:
-                                pdf['cats_broad_class'] = pdf['cats_broad_class'].astype('float')
+                            if "cats_broad_max_prob" in pdf.columns:
+                                pdf["cats_broad_max_prob"] = pdf[
+                                    "cats_broad_max_prob"
+                                ].astype("float")
+
+                            if "cats_broad_class" in pdf.columns:
+                                pdf["cats_broad_class"] = pdf[
+                                    "cats_broad_class"
+                                ].astype("float")
 
-                            if 'tracklet' in pdf.columns:
-                                pdf['tracklet'] = pdf['tracklet'].astype('str')
+                            if "tracklet" in pdf.columns:
+                                pdf["tracklet"] = pdf["tracklet"].astype("str")
 
                             # if 'jd' in pdf.columns:
                             #     # create columns year, month, day
 
                             table = pa.Table.from_pandas(pdf)
 
                             if poll_number == initial:
                                 table_schema = table.schema
 
-                            if args.partitionby == 'time':
-                                partitioning = ['year', 'month', 'day']
-                            elif args.partitionby == 'finkclass':
-                                partitioning = ['finkclass']
-                            elif args.partitionby == 'tnsclass':
-                                partitioning = ['tnsclass']
-                            elif args.partitionby == 'classId':
-                                partitioning = ['classId']
+                            if args.partitionby == "time":
+                                partitioning = ["year", "month", "day"]
+                            elif args.partitionby == "finkclass":
+                                partitioning = ["finkclass"]
+                            elif args.partitionby == "tnsclass":
+                                partitioning = ["tnsclass"]
+                            elif args.partitionby == "classId":
+                                partitioning = ["classId"]
 
                             part_num = rng.randint(0, 1e6)
                             try:
                                 pq.write_to_dataset(
                                     table,
                                     args.outdir,
                                     schema=table_schema,
-                                    basename_template='part-{}-{{i}}-{}.parquet'.format(process_id, part_num),
+                                    basename_template="part-{}-{{i}}-{}.parquet".format(
+                                        process_id, part_num
+                                    ),
                                     partition_cols=partitioning,
-                                    existing_data_behavior='overwrite_or_ignore'
+                                    existing_data_behavior="overwrite_or_ignore",
                                 )
                             except pa.lib.ArrowTypeError:
-                                print('Schema mismatch detected')
+                                print("Schema mismatch detected")
                                 table_schema_ = table.schema
                                 pq.write_to_dataset(
                                     table,
                                     args.outdir,
                                     schema=table_schema_,
-                                    basename_template='part-{}-{{i}}-{}.parquet'.format(process_id, part_num),
+                                    basename_template="part-{}-{{i}}-{}.parquet".format(
+                                        process_id, part_num
+                                    ),
                                     partition_cols=partitioning,
-                                    existing_data_behavior='overwrite_or_ignore'
+                                    existing_data_behavior="overwrite_or_ignore",
                                 )
 
                             poll_number += len(msgs)
                             pbar.update(len(msgs))
 
                             if len(msgs) < args.batchsize:
-                                queue.put({
-                                    "partition": partition["partition"],
-                                    "offset": poll_number,
-                                    "status": 0
-                                })
+                                queue.put(
+                                    {
+                                        "partition": partition["partition"],
+                                        "offset": poll_number,
+                                        "status": 0,
+                                    }
+                                )
                                 break
                         else:
-                            logging.info('[{}] No alerts the last {} seconds ({} polled)\n'.format(process_id, args.maxtimeout, poll_number))
+                            logging.info(
+                                "[{}] No alerts the last {} seconds ({} polled)\n".format(
+                                    process_id, args.maxtimeout, poll_number
+                                )
+                            )
                 except KeyboardInterrupt:
-                    sys.stderr.write('%% Aborted by user\n')
+                    sys.stderr.write("%% Aborted by user\n")
                     consumer.close()
     consumer.close()
 
 
 def main():
     """ """
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
-        '-topic', type=str, default='.',
-        help="Topic name for the stream that contains the data.")
+        "-topic",
+        type=str,
+        default=".",
+        help="Topic name for the stream that contains the data.",
+    )
     parser.add_argument(
-        '-limit', type=int, default=None,
-        help="If specified, download only `limit` alerts from the stream. Default is None, that is download all alerts.")
+        "-limit",
+        type=int,
+        default=None,
+        help="If specified, download only `limit` alerts from the stream. Default is None, that is download all alerts.",
+    )
     parser.add_argument(
-        '-outdir', type=str, default='.',
-        help="Folder to store incoming alerts. It will be created if it does not exist.")
+        "-outdir",
+        type=str,
+        default=".",
+        help="Folder to store incoming alerts. It will be created if it does not exist.",
+    )
     parser.add_argument(
-        '-partitionby', type=str, default='time',
-        help="Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). `classId` is also available for ELASTiCC data. Default is time.")
+        "-partitionby",
+        type=str,
+        default="time",
+        help="Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). `classId` is also available for ELASTiCC data. Default is time.",
+    )
     parser.add_argument(
-        '-batchsize', type=int, default=1000,
-        help="Maximum number of alert within the `maxtimeout` (see conf). Default is 1000 alerts.")
+        "-batchsize",
+        type=int,
+        default=1000,
+        help="Maximum number of alert within the `maxtimeout` (see conf). Default is 1000 alerts.",
+    )
     parser.add_argument(
-        '-nconsumers', type=int, default=-1,
-        help="Number of parallel consumer to use. Default (-1) is the number of logical CPUs in the system.")
+        "-nconsumers",
+        type=int,
+        default=-1,
+        help="Number of parallel consumer to use. Default (-1) is the number of logical CPUs in the system.",
+    )
     parser.add_argument(
-        '-maxtimeout', type=float, default=None,
-        help="Overwrite the default timeout (in seconds) from user configuration. Default is None.")
+        "-maxtimeout",
+        type=float,
+        default=None,
+        help="Overwrite the default timeout (in seconds) from user configuration. Default is None.",
+    )
     parser.add_argument(
-        '-number_partitions', type=int, default=10,
-        help="Number of partitions for the topic in the distant Kafka cluster. Do not touch unless you know what your are doing. Default is 10 (Fink Kafka cluster)")
+        "-number_partitions",
+        type=int,
+        default=10,
+        help="Number of partitions for the topic in the distant Kafka cluster. Do not touch unless you know what your are doing. Default is 10 (Fink Kafka cluster)",
+    )
     parser.add_argument(
-        '--restart_from_beginning', action='store_true',
-        help="If specified, restart downloading from the 1st alert in the stream. Default is False.")
+        "--restart_from_beginning",
+        action="store_true",
+        help="If specified, restart downloading from the 1st alert in the stream. Default is False.",
+    )
     parser.add_argument(
-        '--verbose', action='store_true',
-        help="If specified, print on screen information about the consuming.")
+        "--verbose",
+        action="store_true",
+        help="If specified, print on screen information about the consuming.",
+    )
     args = parser.parse_args(None)
 
-    if args.partitionby not in ['time', 'finkclass', 'tnsclass', 'classId']:
-        print("{} is an unknown partitioning. `-partitionby` should be in ['time', 'finkclass', 'tnsclass', 'classId']".format(args.partitionby))
+    if args.partitionby not in ["time", "finkclass", "tnsclass", "classId"]:
+        print(
+            "{} is an unknown partitioning. `-partitionby` should be in ['time', 'finkclass', 'tnsclass', 'classId']".format(
+                args.partitionby
+            )
+        )
         sys.exit()
 
     # load user configuration
     conf = load_credentials()
 
     # Time to wait before polling again if no alerts
     if args.maxtimeout is None:
-        args.maxtimeout = conf['maxtimeout']
+        args.maxtimeout = conf["maxtimeout"]
 
     # Number of consumers to use
     if args.nconsumers == -1:
         nconsumers = psutil.cpu_count(logical=True)
     else:
         nconsumers = args.nconsumers
 
     kafka_config = {
-        'bootstrap.servers': conf['servers'],
-        'group.id': conf['group_id'],
-        "auto.offset.reset": "earliest"
+        "bootstrap.servers": conf["servers"],
+        "group.id": conf["group_id"],
+        "auto.offset.reset": "earliest",
     }
 
     if args.restart_from_beginning:
-        total_lag, total_offset = print_offsets(kafka_config, args.topic, args.maxtimeout, verbose=False)
+        total_lag, total_offset = print_offsets(
+            kafka_config, args.topic, args.maxtimeout, verbose=False
+        )
         args.total_lag = total_offset
         args.total_offset = 0
         offsets = [0 for _ in range(args.number_partitions)]
     else:
-        total_lag, total_offset = print_offsets(kafka_config, args.topic, args.maxtimeout)
+        total_lag, total_offset = print_offsets(
+            kafka_config, args.topic, args.maxtimeout
+        )
         args.total_lag = total_lag
         args.total_offset = total_offset
         offsets = return_last_offsets(kafka_config, args.topic)
         if total_lag == 0:
             print("All alerts have been polled. Exiting.")
             sys.exit()
 
@@ -482,33 +550,34 @@
 
     if (args.limit is not None) and (args.limit < args.batchsize):
         args.batchsize = args.limit
 
     schema = get_schema(kafka_config, args.topic, args.maxtimeout)
     if schema is None:
         # TBD: raise error
-        print('No schema found -- wait a few seconds and relaunch. If the error persists, maybe the queue is empty.')
+        print(
+            "No schema found -- wait a few seconds and relaunch. If the error persists, maybe the queue is empty."
+        )
     else:
         nbpart = return_npartitions(args.topic, kafka_config)
         print("Number of partitions for topic {}: {}".format(args.topic, nbpart))
         available = Queue()
         # Queue loading
         for key in range(nbpart):
-            available.put({
-                "partition": key,
-                "offset": offsets[key],
-                "status": 0
-            })
+            available.put({"partition": key, "offset": offsets[key], "status": 0})
 
         # Processes Creation
         random_state = 0
         rng = np.random.RandomState(random_state)
         procs = []
         for i in range(nconsumers):
-            proc = Process(target=poll, args=(i, nconsumers, available, schema, kafka_config, rng, args))
+            proc = Process(
+                target=poll,
+                args=(i, nconsumers, available, schema, kafka_config, rng, args),
+            )
             procs.append(proc)
             proc.start()
 
         for proc in procs:
             proc.join()
 
         print_offsets(kafka_config, args.topic, args.maxtimeout)
```

### Comparing `fink-client-7.2/fink_client/tester.py` & `fink-client-8.0/fink_client/tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import sys
 import doctest
 import numpy as np
 
+
 def regular_unit_tests(global_args: dict = None, verbose: bool = False):
-    """ Base commands for the regular unit test suite
+    """Base commands for the regular unit test suite
 
     Include this routine in the main of a module, and execute:
     python3 mymodule.py
     to run the tests.
 
     It should exit gracefully if no error (exit code 0),
     otherwise it will print on the screen the failure.
@@ -32,15 +33,15 @@
         Dictionary containing user-defined variables to
         be passed to the test suite. Default is None.
     verbose: bool
         If True, print useful debug messages.
         Default is False.
 
     Examples
-    ----------
+    --------
     Set "toto" to "myvalue", such that it can be used during tests:
     >>> globs = globals()
     >>> globs["toto"] = "myvalue"
     >>> regular_unit_tests(global_args=globs)
     """
     if global_args is None:
         global_args = globals()
```

### Comparing `fink-client-7.2/fink_client/visualisation.py` & `fink-client-8.0/fink_client/visualisation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2019-2020 AstroLab Software
+# Copyright 2019-2024 AstroLab Software
 # Author: Julien Peloton
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -18,25 +18,26 @@
 
 import matplotlib.pyplot as plt
 
 from astropy.io import fits
 
 import numpy as np
 
+
 def plot_cutout(stamp: bytes, fig=None, subplot=None, **kwargs):
-    """ Plot one cutout contained in an alert (2D array)
+    """Plot one cutout contained in an alert (2D array)
 
     Adapted from ZTF alert tools.
 
     Parameters
     ----------
     stamp: bytes
         Cutout data as raw binary from the alert
     """
-    with gzip.open(io.BytesIO(stamp), 'rb') as f:
+    with gzip.open(io.BytesIO(stamp), "rb") as f:
         with fits.open(io.BytesIO(f.read()), ignore_missing_simple=True) as hdul:
             if fig is None:
                 fig = plt.figure(figsize=(4, 4))
             if subplot is None:
                 subplot = (1, 1, 1)
 
             ax = fig.add_subplot(*subplot)
@@ -46,72 +47,71 @@
 
             data = data[::-1]
 
             ax.imshow(data)
 
     return ax
 
+
 def show_stamps(alert: dict, fig=None):
-    """ Plot the 3 cutouts contained in an alert.
+    """Plot the 3 cutouts contained in an alert.
 
     Parameters
     ----------
     alert: dict
         Dictionnary containing alert data.
     """
-    for i, cutout in enumerate(['Science', 'Template', 'Difference']):
-        stamp = alert['cutout{}'.format(cutout)]['stampData']
+    for i, cutout in enumerate(["Science", "Template", "Difference"]):
+        stamp = alert["cutout{}".format(cutout)]["stampData"]
         ffig = plot_cutout(stamp, fig=fig, subplot=(1, 3, i + 1))
         ffig.set_title(cutout)
         # remove axis labels
-        plt.xlabel('')
-        plt.ylabel('')
+        plt.xlabel("")
+        plt.ylabel("")
+
 
 def extract_history(history_list: list, field: str) -> list:
-    """Extract the historical measurements contained in the alerts
-    for the parameter `field`.
+    """Extract the historical measurements contained in the alerts for the parameter `field`.
 
     Parameters
     ----------
     history_list: list of dict
         List of dictionary from alert['prv_candidates'].
     field: str
         The field name for which you want to extract the data. It must be
         a key of elements of history_list (alert['prv_candidates'])
 
     Returns
-    ----------
+    -------
     measurement: list
         List of all the `field` measurements contained in the alerts.
     """
     try:
         measurement = [obs[field] for obs in history_list]
     except KeyError:
-        print('{} not in history data'.format(field))
+        print("{} not in history data".format(field))
         measurement = [None] * len(history_list)
 
     return measurement
 
+
 def extract_field(alert: dict, field: str) -> np.array:
-    """ Concatenate current and historical observation data for a given field.
+    """Concatenate current and historical observation data for a given field.
 
     Parameters
     ----------
     alert: dict
         Dictionnary containing alert data
     field: str
         Name of the field to extract.
 
     Returns
-    ----------
+    -------
     data: np.array
         List containing previous measurements and current measurement at the
         end. If `field` is not in `prv_candidates fields, data will be
         [None, None, ..., alert['candidate'][field]].
     """
     data = np.concatenate(
-        [
-            [alert["candidate"][field]],
-            extract_history(alert['prv_candidates'], field)
-        ]
+        [[alert["candidate"][field]], extract_history(alert["prv_candidates"], field)]
     )
     return data
```

### Comparing `fink-client-7.2/fink_client.egg-info/PKG-INFO` & `fink-client-8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 Metadata-Version: 2.1
 Name: fink-client
-Version: 7.2
+Version: 8.0
 Summary: Light-weight client to manipulate alerts from Fink
 Home-page: https://fink-broker.readthedocs.io/en/latest/
 Author: AstroLab Software
 Author-email: peloton@lal.in2p3.fr
 Project-URL: Documentation, https://fink-broker.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/astrolabsoftware/fink-client
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: astropy==6.0.1
+Requires-Dist: confluent-kafka==2.4.0
+Requires-Dist: coverage==7.5.3
+Requires-Dist: coveralls==4.0.1
+Requires-Dist: fastavro==1.9.4
+Requires-Dist: matplotlib==3.9.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: pandas==2.2.2
+Requires-Dist: pyarrow==16.1.0
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: tqdm==4.66.4
 
 [![pypi](https://img.shields.io/pypi/v/fink-client.svg)](https://pypi.python.org/pypi/fink-client)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Sentinel](https://github.com/astrolabsoftware/fink-client/workflows/Sentinel/badge.svg)](https://github.com/astrolabsoftware/fink-client/actions?query=workflow%3ASentinel)
 [![codecov](https://codecov.io/gh/astrolabsoftware/fink-client/branch/master/graph/badge.svg)](https://codecov.io/gh/astrolabsoftware/fink-client)
 [![Documentation Status](https://readthedocs.org/projects/fink-broker/badge/?version=latest)](https://fink-broker.readthedocs.io/en/latest/?badge=latest)
@@ -33,81 +45,65 @@
 
 ### Install with pip
 
 ```bash
 pip install fink-client --upgrade
 ```
 
-You will also need to install `fastavro==1.6.0` separately (versions above are not compatible with alert schema):
-
-```
-# fastavro 1.6.0 requires Cython<3
-pip install "Cython<3"
-pip install --no-build-isolation "fastavro==1.6.0"
-```
-
 ### Use or develop in a controlled environment
 
-For usage:
-
-```bash
-conda env create -f https://raw.githubusercontent.com/astrolabsoftware/fink-client/master/environment.yml
-conda activate fink-client
-pip install "Cython<3"
-pip install --no-build-isolation "fastavro==1.6.0"
-pip install fink-client --upgrade
-```
-
-For development:
+For development, we recommend the use of a virtual environment:
 
 ```bash
 git clone https://github.com/astrolabsoftware/fink-client.git
 cd fink-client
-conda env create -f environment.yml
-conda activate fink-client
-pip install "Cython<3"
-pip install --no-build-isolation "fastavro==1.6.0"
-pip install -e .
+python -m venv .fc_env
+source .fc_env/bin/activate
+pip install -r requirements.txt
+pip install .
 ```
 
 ## Registration
 
 In order to connect and poll alerts from Fink, you need to get your credentials:
 
 1. Subscribe to one or more Fink streams by filling this [form](https://forms.gle/2td4jysT4e9pkf889).
 2. After filling the form, we will send your credentials. Register them on your laptop by simply running:
   ```
   fink_client_register -username <USERNAME> -group_id <GROUP_ID> ...
   ```
 
 ## Livestream usage
 
-Once you have your credentials, you are ready to poll streams!
+Once you have your credentials, you are ready to poll streams! You can easily access the documentation using `-h` or `--help`:
 
 ```bash
 fink_consumer -h
 usage: fink_consumer [-h] [--display] [-limit LIMIT] [--available_topics]
                      [--save] [-outdir OUTDIR] [-schema SCHEMA]
+                     [--dump_schema]
 
-Kafka consumer to listen and archive Fink streams from the Livestream service
+Kafka consumer to listen and archive Fink streams from the Livestream
+service
 
 optional arguments:
   -h, --help          show this help message and exit
-  --display           If specified, print on screen information about incoming
-                      alert.
+  --display           If specified, print on screen information about
+                      incoming alert.
   -limit LIMIT        If specified, download only `limit` alerts. Default is
                       None.
   --available_topics  If specified, print on screen information about
                       available topics.
   --save              If specified, save alert data on disk (Avro). See also
                       -outdir.
   -outdir OUTDIR      Folder to store incoming alerts if --save is set. It
                       must exist.
   -schema SCHEMA      Avro schema to decode the incoming alerts. Default is
-                      None (latest version downloaded from server)
+                      None (version taken from each alert)
+  --dump_schema       If specified, save the schema on disk (json file)
 ```
 
 You can also look at an alert on the disk:
 
 ```bash
 fink_alert_viewer -h
 usage: fink_alert_viewer [-h] [-filename FILENAME]
```

### Comparing `fink-client-7.2/fink_client.egg-info/SOURCES.txt` & `fink-client-8.0/fink_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 setup.py
 bin/fink_client_test.sh
 fink_client/__init__.py
-fink_client/avroUtils.py
+fink_client/avro_utils.py
 fink_client/configuration.py
 fink_client/consumer.py
 fink_client/tester.py
 fink_client/visualisation.py
 fink_client.egg-info/PKG-INFO
 fink_client.egg-info/SOURCES.txt
 fink_client.egg-info/dependency_links.txt
@@ -15,10 +15,8 @@
 fink_client.egg-info/requires.txt
 fink_client.egg-info/top_level.txt
 fink_client/scripts/__init__.py
 fink_client/scripts/fink_alert_viewer.py
 fink_client/scripts/fink_client_register.py
 fink_client/scripts/fink_consumer.py
 fink_client/scripts/fink_datatransfer.py
-fink_client/scripts/fink_datatransfer_mpi.py
-fink_client/scripts/fink_datatransfer_offsets.py
 tests/test.py
```

### Comparing `fink-client-7.2/setup.py` & `fink-client-8.0/setup.py`

 * *Files identical despite different names*

### Comparing `fink-client-7.2/tests/test.py` & `fink-client-8.0/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2019-2020 AstroLab Software
+# Copyright 2019-2024 AstroLab Software
 # Author: Abhishek Chauhan, Julien Peloton
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,17 +15,17 @@
 # limitations under the License.
 import unittest
 import os
 import io
 import confluent_kafka
 import fastavro
 from fink_client.consumer import AlertConsumer
-from fink_client.avroUtils import AlertReader
-from fink_client.avroUtils import encode_into_avro
-from fink_client.avroUtils import get_legal_topic_name
+from fink_client.avro_utils import AlertReader
+from fink_client.avro_utils import encode_into_avro
+from fink_client.avro_utils import get_legal_topic_name
 
 from fink_client.configuration import load_credentials
 
 
 class TestIntegration(unittest.TestCase):
 
     def setUp(self):
```

