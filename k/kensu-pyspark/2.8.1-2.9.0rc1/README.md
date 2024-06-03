# Comparing `tmp/kensu-pyspark-2.8.1.tar.gz` & `tmp/kensu_pyspark-2.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kensu-pyspark-2.8.1.tar", last modified: Wed Apr  3 15:29:39 2024, max compression
+gzip compressed data, was "kensu_pyspark-2.9.0rc1.tar", last modified: Mon Jun  3 09:59:52 2024, max compression
```

## Comparing `kensu-pyspark-2.8.1.tar` & `kensu_pyspark-2.9.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:39.298626 kensu-pyspark-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-03 15:29:39.298626 kensu-pyspark-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:39.286626 kensu-pyspark-2.8.1/kensu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:39.290626 kensu-pyspark-2.8.1/kensu/pyspark/
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/pyspark/KensuDataFrameWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58723 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/pyspark/spark_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:39.286626 kensu-pyspark-2.8.1/kensu/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:39.290626 kensu-pyspark-2.8.1/kensu/utils/kensu_conf_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/utils/kensu_conf_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/utils/kensu_conf_file/conf_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:39.290626 kensu-pyspark-2.8.1/kensu/utils/remote/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/kensu/utils/remote/circuit_breakers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:29:39.290626 kensu-pyspark-2.8.1/kensu_pyspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-03 15:29:39.000000 kensu-pyspark-2.8.1/kensu_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 15:29:39.000000 kensu-pyspark-2.8.1/kensu_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:29:39.000000 kensu-pyspark-2.8.1/kensu_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-03 15:29:39.000000 kensu-pyspark-2.8.1/kensu_pyspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 15:29:39.000000 kensu-pyspark-2.8.1/kensu_pyspark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 15:29:39.298626 kensu-pyspark-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-03 15:29:34.000000 kensu-pyspark-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:52.507543 kensu_pyspark-2.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-06-03 09:59:52.507543 kensu_pyspark-2.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:52.495543 kensu_pyspark-2.9.0rc1/kensu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:52.495543 kensu_pyspark-2.9.0rc1/kensu/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/pyspark/KensuDataFrameWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58723 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/pyspark/spark_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:52.491543 kensu_pyspark-2.9.0rc1/kensu/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:52.495543 kensu_pyspark-2.9.0rc1/kensu/utils/kensu_conf_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/utils/kensu_conf_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/utils/kensu_conf_file/conf_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:52.495543 kensu_pyspark-2.9.0rc1/kensu/utils/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/kensu/utils/remote/circuit_breakers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:59:52.495543 kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-06-03 09:59:52.000000 kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 09:59:52.000000 kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:59:52.000000 kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-06-03 09:59:52.000000 kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 09:59:52.000000 kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-03 09:59:52.507543 kensu_pyspark-2.9.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-06-03 09:59:49.000000 kensu_pyspark-2.9.0rc1/setup.py
```

### Comparing `kensu-pyspark-2.8.1/LICENSE` & `kensu_pyspark-2.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kensu-pyspark-2.8.1/PKG-INFO` & `kensu_pyspark-2.9.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kensu-pyspark
-Version: 2.8.1
+Version: 2.9.0rc1
 Home-page: 
 Author-email: 
 Keywords: DODD,Data Observability Driven Development,Data Observability,Analytics Observability
 Platform: Posix; MacOS X; Windows
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: urllib3>=1.15.1
@@ -37,123 +37,123 @@
 Requires-Dist: sqllineage>=1.3.7; extra == "boto"
 Requires-Dist: boto3; extra == "boto"
 Provides-Extra: sqllineage
 Requires-Dist: sqllineage>=1.3.7; extra == "sqllineage"
 Provides-Extra: psycopg2-binary
 Requires-Dist: psycopg2-binary==2.9.3; extra == "psycopg2-binary"
 Provides-Extra: pg
+Requires-Dist: pglast==v3.4; extra == "pg"
 Requires-Dist: sqlparse>=0.4.2; extra == "pg"
 Requires-Dist: psycopg2-binary==2.9.3; extra == "pg"
-Requires-Dist: pglast==v3.4; extra == "pg"
 Provides-Extra: pglast
 Requires-Dist: pglast==v3.4; extra == "pglast"
 Provides-Extra: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "google-cloud-bigquery"
 Provides-Extra: gbq
-Requires-Dist: sqlparse>=0.4.2; extra == "gbq"
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "gbq"
+Requires-Dist: sqlparse>=0.4.2; extra == "gbq"
 Provides-Extra: sqlparse
 Requires-Dist: sqlparse>=0.4.2; extra == "sqlparse"
-Provides-Extra: apache-airflow-google
-Requires-Dist: apache-airflow[google]==2.2.3; extra == "apache-airflow-google"
-Provides-Extra: airflow
-Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow"
 Provides-Extra: airflow-google
-Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow-google"
+Requires-Dist: gcsfs; extra == "airflow-google"
 Requires-Dist: twine<=3.8.0; extra == "airflow-google"
+Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow-google"
 Requires-Dist: fsspec; extra == "airflow-google"
-Requires-Dist: gcsfs; extra == "airflow-google"
+Provides-Extra: airflow
+Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow"
+Provides-Extra: apache-airflow-google
+Requires-Dist: apache-airflow[google]==2.2.3; extra == "apache-airflow-google"
 Provides-Extra: twine
 Requires-Dist: twine<=3.8.0; extra == "twine"
 Provides-Extra: gcsfs
 Requires-Dist: gcsfs; extra == "gcsfs"
 Provides-Extra: fsspec
 Requires-Dist: fsspec; extra == "fsspec"
 Provides-Extra: packaging
 Requires-Dist: packaging; extra == "packaging"
 Provides-Extra: sdk
 Requires-Dist: packaging; extra == "sdk"
-Provides-Extra: kafka
-Requires-Dist: confluent-kafka; extra == "kafka"
 Provides-Extra: confluent-kafka
 Requires-Dist: confluent-kafka; extra == "confluent-kafka"
-Provides-Extra: gitpython
-Requires-Dist: GitPython; extra == "gitpython"
+Provides-Extra: kafka
+Requires-Dist: confluent-kafka; extra == "kafka"
 Provides-Extra: git
 Requires-Dist: GitPython; extra == "git"
+Provides-Extra: gitpython
+Requires-Dist: GitPython; extra == "gitpython"
 Provides-Extra: pytest-sftpserver
 Requires-Dist: pytest-sftpserver; extra == "pytest-sftpserver"
 Provides-Extra: test
-Requires-Dist: pytest>=6.2.4; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
-Requires-Dist: pytest-vcr; extra == "test"
+Requires-Dist: pytest>=6.2.4; extra == "test"
 Requires-Dist: pytest-sftpserver; extra == "test"
+Requires-Dist: pytest-vcr; extra == "test"
 Provides-Extra: pytest
 Requires-Dist: pytest>=6.2.4; extra == "pytest"
 Provides-Extra: pytest-mock
 Requires-Dist: pytest-mock; extra == "pytest-mock"
 Provides-Extra: pytest-vcr
 Requires-Dist: pytest-vcr; extra == "pytest-vcr"
-Provides-Extra: setuptools
-Requires-Dist: setuptools>=21.0.0; extra == "setuptools"
 Provides-Extra: build
-Requires-Dist: setuptools>=21.0.0; extra == "build"
 Requires-Dist: wheel; extra == "build"
 Requires-Dist: twine>=3.4.1; extra == "build"
+Requires-Dist: setuptools>=21.0.0; extra == "build"
+Provides-Extra: setuptools
+Requires-Dist: setuptools>=21.0.0; extra == "setuptools"
 Requires-Dist: twine>=3.4.1; extra == "twine"
 Provides-Extra: wheel
 Requires-Dist: wheel; extra == "wheel"
 Provides-Extra: all
-Requires-Dist: boto3; extra == "all"
-Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: numpy>=1.19.5; extra == "all"
-Requires-Dist: sqlparse>=0.4.2; extra == "all"
-Requires-Dist: psycopg2-binary==2.9.3; extra == "all"
-Requires-Dist: pysftp>=0.2.9; extra == "all"
-Requires-Dist: packaging; extra == "all"
 Requires-Dist: setuptools>=21.0.0; extra == "all"
-Requires-Dist: gcsfs; extra == "all"
+Requires-Dist: pysftp>=0.2.9; extra == "all"
+Requires-Dist: twine>=3.4.1; extra == "all"
+Requires-Dist: pytest>=6.2.4; extra == "all"
 Requires-Dist: pytest-sftpserver; extra == "all"
-Requires-Dist: twine<=3.8.0; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: pandas>=1.2.4; extra == "all"
-Requires-Dist: sqllineage>=1.3.7; extra == "all"
-Requires-Dist: pglast==v3.4; extra == "all"
-Requires-Dist: pytest-vcr; extra == "all"
+Requires-Dist: boto3; extra == "all"
 Requires-Dist: confluent-kafka; extra == "all"
+Requires-Dist: psycopg2-binary==2.9.3; extra == "all"
 Requires-Dist: apache-airflow[google]==2.2.3; extra == "all"
-Requires-Dist: twine>=3.4.1; extra == "all"
+Requires-Dist: packaging; extra == "all"
+Requires-Dist: pandas>=1.2.4; extra == "all"
+Requires-Dist: gcsfs; extra == "all"
 Requires-Dist: gluonts==0.6.5; extra == "all"
-Requires-Dist: fsspec; extra == "all"
+Requires-Dist: pytest-vcr; extra == "all"
+Requires-Dist: twine<=3.8.0; extra == "all"
 Requires-Dist: scikit-learn>=0.24.2; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: pytest>=6.2.4; extra == "all"
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "all"
+Requires-Dist: pytest-mock; extra == "all"
+Requires-Dist: sqllineage>=1.3.7; extra == "all"
+Requires-Dist: wheel; extra == "all"
+Requires-Dist: sqlparse>=0.4.2; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: fsspec; extra == "all"
+Requires-Dist: pglast==v3.4; extra == "all"
+Requires-Dist: numpy>=1.19.5; extra == "all"
 Provides-Extra: all-but-test
-Requires-Dist: boto3; extra == "all-but-test"
-Requires-Dist: pytest-mock; extra == "all-but-test"
-Requires-Dist: numpy>=1.19.5; extra == "all-but-test"
-Requires-Dist: sqlparse>=0.4.2; extra == "all-but-test"
-Requires-Dist: psycopg2-binary==2.9.3; extra == "all-but-test"
-Requires-Dist: pysftp>=0.2.9; extra == "all-but-test"
-Requires-Dist: packaging; extra == "all-but-test"
 Requires-Dist: setuptools>=21.0.0; extra == "all-but-test"
-Requires-Dist: gcsfs; extra == "all-but-test"
+Requires-Dist: pysftp>=0.2.9; extra == "all-but-test"
+Requires-Dist: twine>=3.4.1; extra == "all-but-test"
+Requires-Dist: pytest>=6.2.4; extra == "all-but-test"
 Requires-Dist: pytest-sftpserver; extra == "all-but-test"
-Requires-Dist: twine<=3.8.0; extra == "all-but-test"
-Requires-Dist: wheel; extra == "all-but-test"
-Requires-Dist: pandas>=1.2.4; extra == "all-but-test"
-Requires-Dist: sqllineage>=1.3.7; extra == "all-but-test"
-Requires-Dist: pglast==v3.4; extra == "all-but-test"
-Requires-Dist: pytest-vcr; extra == "all-but-test"
+Requires-Dist: boto3; extra == "all-but-test"
 Requires-Dist: confluent-kafka; extra == "all-but-test"
+Requires-Dist: psycopg2-binary==2.9.3; extra == "all-but-test"
 Requires-Dist: apache-airflow[google]==2.2.3; extra == "all-but-test"
-Requires-Dist: twine>=3.4.1; extra == "all-but-test"
+Requires-Dist: packaging; extra == "all-but-test"
+Requires-Dist: pandas>=1.2.4; extra == "all-but-test"
+Requires-Dist: gcsfs; extra == "all-but-test"
 Requires-Dist: gluonts==0.6.5; extra == "all-but-test"
-Requires-Dist: fsspec; extra == "all-but-test"
+Requires-Dist: pytest-vcr; extra == "all-but-test"
+Requires-Dist: twine<=3.8.0; extra == "all-but-test"
 Requires-Dist: scikit-learn>=0.24.2; extra == "all-but-test"
-Requires-Dist: GitPython; extra == "all-but-test"
-Requires-Dist: pytest>=6.2.4; extra == "all-but-test"
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "all-but-test"
+Requires-Dist: pytest-mock; extra == "all-but-test"
+Requires-Dist: sqllineage>=1.3.7; extra == "all-but-test"
+Requires-Dist: wheel; extra == "all-but-test"
+Requires-Dist: sqlparse>=0.4.2; extra == "all-but-test"
+Requires-Dist: GitPython; extra == "all-but-test"
+Requires-Dist: fsspec; extra == "all-but-test"
+Requires-Dist: pglast==v3.4; extra == "all-but-test"
+Requires-Dist: numpy>=1.19.5; extra == "all-but-test"
 Provides-Extra: no-extra-deps
 
     DODD Python Agent: enable Data Observability Driven Development in your Python script
```

### Comparing `kensu-pyspark-2.8.1/README.md` & `kensu_pyspark-2.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `kensu-pyspark-2.8.1/kensu/itertools.py` & `kensu_pyspark-2.9.0rc1/kensu/itertools.py`

 * *Files identical despite different names*

### Comparing `kensu-pyspark-2.8.1/kensu/pyspark/KensuDataFrameWriter.py` & `kensu_pyspark-2.9.0rc1/kensu/pyspark/KensuDataFrameWriter.py`

 * *Files identical despite different names*

### Comparing `kensu-pyspark-2.8.1/kensu/pyspark/spark_connector.py` & `kensu_pyspark-2.9.0rc1/kensu/pyspark/spark_connector.py`

 * *Files identical despite different names*

### Comparing `kensu-pyspark-2.8.1/kensu/utils/kensu_conf_file/conf_file.py` & `kensu_pyspark-2.9.0rc1/kensu/utils/kensu_conf_file/conf_file.py`

 * *Files identical despite different names*

### Comparing `kensu-pyspark-2.8.1/kensu/utils/remote/circuit_breakers.py` & `kensu_pyspark-2.9.0rc1/kensu/utils/remote/circuit_breakers.py`

 * *Files identical despite different names*

### Comparing `kensu-pyspark-2.8.1/kensu_pyspark.egg-info/PKG-INFO` & `kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kensu-pyspark
-Version: 2.8.1
+Version: 2.9.0rc1
 Home-page: 
 Author-email: 
 Keywords: DODD,Data Observability Driven Development,Data Observability,Analytics Observability
 Platform: Posix; MacOS X; Windows
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: urllib3>=1.15.1
@@ -37,123 +37,123 @@
 Requires-Dist: sqllineage>=1.3.7; extra == "boto"
 Requires-Dist: boto3; extra == "boto"
 Provides-Extra: sqllineage
 Requires-Dist: sqllineage>=1.3.7; extra == "sqllineage"
 Provides-Extra: psycopg2-binary
 Requires-Dist: psycopg2-binary==2.9.3; extra == "psycopg2-binary"
 Provides-Extra: pg
+Requires-Dist: pglast==v3.4; extra == "pg"
 Requires-Dist: sqlparse>=0.4.2; extra == "pg"
 Requires-Dist: psycopg2-binary==2.9.3; extra == "pg"
-Requires-Dist: pglast==v3.4; extra == "pg"
 Provides-Extra: pglast
 Requires-Dist: pglast==v3.4; extra == "pglast"
 Provides-Extra: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "google-cloud-bigquery"
 Provides-Extra: gbq
-Requires-Dist: sqlparse>=0.4.2; extra == "gbq"
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "gbq"
+Requires-Dist: sqlparse>=0.4.2; extra == "gbq"
 Provides-Extra: sqlparse
 Requires-Dist: sqlparse>=0.4.2; extra == "sqlparse"
-Provides-Extra: apache-airflow-google
-Requires-Dist: apache-airflow[google]==2.2.3; extra == "apache-airflow-google"
-Provides-Extra: airflow
-Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow"
 Provides-Extra: airflow-google
-Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow-google"
+Requires-Dist: gcsfs; extra == "airflow-google"
 Requires-Dist: twine<=3.8.0; extra == "airflow-google"
+Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow-google"
 Requires-Dist: fsspec; extra == "airflow-google"
-Requires-Dist: gcsfs; extra == "airflow-google"
+Provides-Extra: airflow
+Requires-Dist: apache-airflow[google]==2.2.3; extra == "airflow"
+Provides-Extra: apache-airflow-google
+Requires-Dist: apache-airflow[google]==2.2.3; extra == "apache-airflow-google"
 Provides-Extra: twine
 Requires-Dist: twine<=3.8.0; extra == "twine"
 Provides-Extra: gcsfs
 Requires-Dist: gcsfs; extra == "gcsfs"
 Provides-Extra: fsspec
 Requires-Dist: fsspec; extra == "fsspec"
 Provides-Extra: packaging
 Requires-Dist: packaging; extra == "packaging"
 Provides-Extra: sdk
 Requires-Dist: packaging; extra == "sdk"
-Provides-Extra: kafka
-Requires-Dist: confluent-kafka; extra == "kafka"
 Provides-Extra: confluent-kafka
 Requires-Dist: confluent-kafka; extra == "confluent-kafka"
-Provides-Extra: gitpython
-Requires-Dist: GitPython; extra == "gitpython"
+Provides-Extra: kafka
+Requires-Dist: confluent-kafka; extra == "kafka"
 Provides-Extra: git
 Requires-Dist: GitPython; extra == "git"
+Provides-Extra: gitpython
+Requires-Dist: GitPython; extra == "gitpython"
 Provides-Extra: pytest-sftpserver
 Requires-Dist: pytest-sftpserver; extra == "pytest-sftpserver"
 Provides-Extra: test
-Requires-Dist: pytest>=6.2.4; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
-Requires-Dist: pytest-vcr; extra == "test"
+Requires-Dist: pytest>=6.2.4; extra == "test"
 Requires-Dist: pytest-sftpserver; extra == "test"
+Requires-Dist: pytest-vcr; extra == "test"
 Provides-Extra: pytest
 Requires-Dist: pytest>=6.2.4; extra == "pytest"
 Provides-Extra: pytest-mock
 Requires-Dist: pytest-mock; extra == "pytest-mock"
 Provides-Extra: pytest-vcr
 Requires-Dist: pytest-vcr; extra == "pytest-vcr"
-Provides-Extra: setuptools
-Requires-Dist: setuptools>=21.0.0; extra == "setuptools"
 Provides-Extra: build
-Requires-Dist: setuptools>=21.0.0; extra == "build"
 Requires-Dist: wheel; extra == "build"
 Requires-Dist: twine>=3.4.1; extra == "build"
+Requires-Dist: setuptools>=21.0.0; extra == "build"
+Provides-Extra: setuptools
+Requires-Dist: setuptools>=21.0.0; extra == "setuptools"
 Requires-Dist: twine>=3.4.1; extra == "twine"
 Provides-Extra: wheel
 Requires-Dist: wheel; extra == "wheel"
 Provides-Extra: all
-Requires-Dist: boto3; extra == "all"
-Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: numpy>=1.19.5; extra == "all"
-Requires-Dist: sqlparse>=0.4.2; extra == "all"
-Requires-Dist: psycopg2-binary==2.9.3; extra == "all"
-Requires-Dist: pysftp>=0.2.9; extra == "all"
-Requires-Dist: packaging; extra == "all"
 Requires-Dist: setuptools>=21.0.0; extra == "all"
-Requires-Dist: gcsfs; extra == "all"
+Requires-Dist: pysftp>=0.2.9; extra == "all"
+Requires-Dist: twine>=3.4.1; extra == "all"
+Requires-Dist: pytest>=6.2.4; extra == "all"
 Requires-Dist: pytest-sftpserver; extra == "all"
-Requires-Dist: twine<=3.8.0; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: pandas>=1.2.4; extra == "all"
-Requires-Dist: sqllineage>=1.3.7; extra == "all"
-Requires-Dist: pglast==v3.4; extra == "all"
-Requires-Dist: pytest-vcr; extra == "all"
+Requires-Dist: boto3; extra == "all"
 Requires-Dist: confluent-kafka; extra == "all"
+Requires-Dist: psycopg2-binary==2.9.3; extra == "all"
 Requires-Dist: apache-airflow[google]==2.2.3; extra == "all"
-Requires-Dist: twine>=3.4.1; extra == "all"
+Requires-Dist: packaging; extra == "all"
+Requires-Dist: pandas>=1.2.4; extra == "all"
+Requires-Dist: gcsfs; extra == "all"
 Requires-Dist: gluonts==0.6.5; extra == "all"
-Requires-Dist: fsspec; extra == "all"
+Requires-Dist: pytest-vcr; extra == "all"
+Requires-Dist: twine<=3.8.0; extra == "all"
 Requires-Dist: scikit-learn>=0.24.2; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: pytest>=6.2.4; extra == "all"
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "all"
+Requires-Dist: pytest-mock; extra == "all"
+Requires-Dist: sqllineage>=1.3.7; extra == "all"
+Requires-Dist: wheel; extra == "all"
+Requires-Dist: sqlparse>=0.4.2; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: fsspec; extra == "all"
+Requires-Dist: pglast==v3.4; extra == "all"
+Requires-Dist: numpy>=1.19.5; extra == "all"
 Provides-Extra: all-but-test
-Requires-Dist: boto3; extra == "all-but-test"
-Requires-Dist: pytest-mock; extra == "all-but-test"
-Requires-Dist: numpy>=1.19.5; extra == "all-but-test"
-Requires-Dist: sqlparse>=0.4.2; extra == "all-but-test"
-Requires-Dist: psycopg2-binary==2.9.3; extra == "all-but-test"
-Requires-Dist: pysftp>=0.2.9; extra == "all-but-test"
-Requires-Dist: packaging; extra == "all-but-test"
 Requires-Dist: setuptools>=21.0.0; extra == "all-but-test"
-Requires-Dist: gcsfs; extra == "all-but-test"
+Requires-Dist: pysftp>=0.2.9; extra == "all-but-test"
+Requires-Dist: twine>=3.4.1; extra == "all-but-test"
+Requires-Dist: pytest>=6.2.4; extra == "all-but-test"
 Requires-Dist: pytest-sftpserver; extra == "all-but-test"
-Requires-Dist: twine<=3.8.0; extra == "all-but-test"
-Requires-Dist: wheel; extra == "all-but-test"
-Requires-Dist: pandas>=1.2.4; extra == "all-but-test"
-Requires-Dist: sqllineage>=1.3.7; extra == "all-but-test"
-Requires-Dist: pglast==v3.4; extra == "all-but-test"
-Requires-Dist: pytest-vcr; extra == "all-but-test"
+Requires-Dist: boto3; extra == "all-but-test"
 Requires-Dist: confluent-kafka; extra == "all-but-test"
+Requires-Dist: psycopg2-binary==2.9.3; extra == "all-but-test"
 Requires-Dist: apache-airflow[google]==2.2.3; extra == "all-but-test"
-Requires-Dist: twine>=3.4.1; extra == "all-but-test"
+Requires-Dist: packaging; extra == "all-but-test"
+Requires-Dist: pandas>=1.2.4; extra == "all-but-test"
+Requires-Dist: gcsfs; extra == "all-but-test"
 Requires-Dist: gluonts==0.6.5; extra == "all-but-test"
-Requires-Dist: fsspec; extra == "all-but-test"
+Requires-Dist: pytest-vcr; extra == "all-but-test"
+Requires-Dist: twine<=3.8.0; extra == "all-but-test"
 Requires-Dist: scikit-learn>=0.24.2; extra == "all-but-test"
-Requires-Dist: GitPython; extra == "all-but-test"
-Requires-Dist: pytest>=6.2.4; extra == "all-but-test"
 Requires-Dist: google-cloud-bigquery>=2.26.0; extra == "all-but-test"
+Requires-Dist: pytest-mock; extra == "all-but-test"
+Requires-Dist: sqllineage>=1.3.7; extra == "all-but-test"
+Requires-Dist: wheel; extra == "all-but-test"
+Requires-Dist: sqlparse>=0.4.2; extra == "all-but-test"
+Requires-Dist: GitPython; extra == "all-but-test"
+Requires-Dist: fsspec; extra == "all-but-test"
+Requires-Dist: pglast==v3.4; extra == "all-but-test"
+Requires-Dist: numpy>=1.19.5; extra == "all-but-test"
 Provides-Extra: no-extra-deps
 
     DODD Python Agent: enable Data Observability Driven Development in your Python script
```

### Comparing `kensu-pyspark-2.8.1/kensu_pyspark.egg-info/requires.txt` & `kensu_pyspark-2.9.0rc1/kensu_pyspark.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -11,97 +11,97 @@
 [GitPython]
 GitPython
 
 [airflow]
 apache-airflow[google]==2.2.3
 
 [airflow-google]
-apache-airflow[google]==2.2.3
+gcsfs
 twine<=3.8.0
+apache-airflow[google]==2.2.3
 fsspec
-gcsfs
 
 [all]
-boto3
-pytest-mock
-numpy>=1.19.5
-sqlparse>=0.4.2
-psycopg2-binary==2.9.3
-pysftp>=0.2.9
-packaging
 setuptools>=21.0.0
-gcsfs
+pysftp>=0.2.9
+twine>=3.4.1
+pytest>=6.2.4
 pytest-sftpserver
-twine<=3.8.0
-wheel
-pandas>=1.2.4
-sqllineage>=1.3.7
-pglast==v3.4
-pytest-vcr
+boto3
 confluent-kafka
+psycopg2-binary==2.9.3
 apache-airflow[google]==2.2.3
-twine>=3.4.1
+packaging
+pandas>=1.2.4
+gcsfs
 gluonts==0.6.5
-fsspec
+pytest-vcr
+twine<=3.8.0
 scikit-learn>=0.24.2
-GitPython
-pytest>=6.2.4
 google-cloud-bigquery>=2.26.0
-
-[all-but-test]
-boto3
 pytest-mock
-numpy>=1.19.5
+sqllineage>=1.3.7
+wheel
 sqlparse>=0.4.2
-psycopg2-binary==2.9.3
-pysftp>=0.2.9
-packaging
+GitPython
+fsspec
+pglast==v3.4
+numpy>=1.19.5
+
+[all-but-test]
 setuptools>=21.0.0
-gcsfs
+pysftp>=0.2.9
+twine>=3.4.1
+pytest>=6.2.4
 pytest-sftpserver
-twine<=3.8.0
-wheel
-pandas>=1.2.4
-sqllineage>=1.3.7
-pglast==v3.4
-pytest-vcr
+boto3
 confluent-kafka
+psycopg2-binary==2.9.3
 apache-airflow[google]==2.2.3
-twine>=3.4.1
+packaging
+pandas>=1.2.4
+gcsfs
 gluonts==0.6.5
-fsspec
+pytest-vcr
+twine<=3.8.0
 scikit-learn>=0.24.2
-GitPython
-pytest>=6.2.4
 google-cloud-bigquery>=2.26.0
+pytest-mock
+sqllineage>=1.3.7
+wheel
+sqlparse>=0.4.2
+GitPython
+fsspec
+pglast==v3.4
+numpy>=1.19.5
 
 [apache-airflow[google]]
 apache-airflow[google]==2.2.3
 
 [boto]
 sqllineage>=1.3.7
 boto3
 
 [boto3]
 boto3
 
 [build]
-setuptools>=21.0.0
 wheel
 twine>=3.4.1
+setuptools>=21.0.0
 
 [confluent-kafka]
 confluent-kafka
 
 [fsspec]
 fsspec
 
 [gbq]
-sqlparse>=0.4.2
 google-cloud-bigquery>=2.26.0
+sqlparse>=0.4.2
 
 [gcsfs]
 gcsfs
 
 [git]
 GitPython
 
@@ -126,17 +126,17 @@
 packaging
 
 [pandas]
 numpy>=1.19.5
 pandas>=1.2.4
 
 [pg]
+pglast==v3.4
 sqlparse>=0.4.2
 psycopg2-binary==2.9.3
-pglast==v3.4
 
 [pglast]
 pglast==v3.4
 
 [psycopg2-binary]
 psycopg2-binary==2.9.3
 
@@ -171,18 +171,18 @@
 [sqllineage ]
 sqllineage>=1.3.7
 
 [sqlparse ]
 sqlparse>=0.4.2
 
 [test]
-pytest>=6.2.4
 pytest-mock
-pytest-vcr
+pytest>=6.2.4
 pytest-sftpserver
+pytest-vcr
 
 [twine]
 twine<=3.8.0
 
 [twine ]
 twine>=3.4.1
```

### Comparing `kensu-pyspark-2.8.1/setup.py` & `kensu_pyspark-2.9.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 NAME = artifact_name()
 
 
 BUILD_FLAVOR = os.environ["BUILD_FLAVOR"] if "BUILD_FLAVOR" in os.environ else ""
 BUILD_NUMBER = os.environ["BUILD_NUMBER"] if "BUILD_NUMBER" in os.environ else ""
 # https://semver.org/
-VERSION = "2.8.1" + BUILD_FLAVOR + BUILD_NUMBER
+VERSION = "2.9.0-rc1" + BUILD_FLAVOR + BUILD_NUMBER
 
 
 
 
 # To install the library, run the following
 #
 # python setup.py install
```

