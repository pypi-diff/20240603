# Comparing `tmp/apache_airflow_providers_teradata-2.2.0.tar.gz` & `tmp/apache_airflow_providers_teradata-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_teradata-2.2.0.tar", last modified: Thu May 30 06:45:06 2024, max compression
+gzip compressed data, was "apache_airflow_providers_teradata-2.2.0rc1.tar", last modified: Thu May 30 06:45:06 2024, max compression
```

## Comparing `apache_airflow_providers_teradata-2.2.0.tar` & `apache_airflow_providers_teradata-2.2.0rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4671 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/README.rst
--rw-r--r--   0        0        0    13569 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/LICENSE
--rw-r--r--   0        0        0     1495 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/__init__.py
--rw-r--r--   0        0        0     3854 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/hooks/__init__.py
--rw-r--r--   0        0        0     9511 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/hooks/teradata.py
--rw-r--r--   0        0        0      787 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/operators/__init__.py
--rw-r--r--   0        0        0     3628 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/operators/teradata.py
--rw-r--r--   0        0        0      785 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/__init__.py
--rw-r--r--   0        0        0     4293 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/azure_blob_to_teradata.py
--rw-r--r--   0        0        0     4523 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/s3_to_teradata.py
--rw-r--r--   0        0        0     3834 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/teradata_to_teradata.py
--rw-r--r--   0        0        0     3286 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 apache_airflow_providers_teradata-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4675 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/LICENSE
+-rw-r--r--   0        0        0     1495 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/__init__.py
+-rw-r--r--   0        0        0     3854 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/__init__.py
+-rw-r--r--   0        0        0     9511 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/teradata.py
+-rw-r--r--   0        0        0      787 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/operators/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/operators/teradata.py
+-rw-r--r--   0        0        0      785 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/__init__.py
+-rw-r--r--   0        0        0     4293 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/azure_blob_to_teradata.py
+-rw-r--r--   0        0        0     4523 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/s3_to_teradata.py
+-rw-r--r--   0        0        0     3834 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/teradata_to_teradata.py
+-rw-r--r--   0        0        0     3296 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6799 1970-01-01 00:00:00.000000 apache_airflow_providers_teradata-2.2.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_teradata-2.2.0/README.rst` & `apache_airflow_providers_teradata-2.2.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-teradata``
 
-Release: ``2.2.0``
+Release: ``2.2.0.rc1``
 
 
 `Teradata <https://www.teradata.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/LICENSE` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/get_provider_info.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/hooks/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/hooks/teradata.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/teradata.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/operators/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/operators/teradata.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/operators/teradata.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/azure_blob_to_teradata.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/azure_blob_to_teradata.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/s3_to_teradata.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/s3_to_teradata.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/airflow/providers/teradata/transfers/teradata_to_teradata.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/teradata_to_teradata.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.2.0/pyproject.toml` & `apache_airflow_providers_teradata-2.2.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-teradata"
-version = "2.2.0"
+version = "2.2.0.rc1"
 description = "Provider package apache-airflow-providers-teradata for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,16 +52,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow-providers-common-sql>=1.3.1",
-    "apache-airflow>=2.7.0",
+    "apache-airflow-providers-common-sql>=1.3.1rc0",
+    "apache-airflow>=2.7.0rc0",
     "teradatasql>=17.20.0.28",
     "teradatasqlalchemy>=17.20.0.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/changelog.html"
```

### Comparing `apache_airflow_providers_teradata-2.2.0/PKG-INFO` & `apache_airflow_providers_teradata-2.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-teradata
-Version: 2.2.0
+Version: 2.2.0rc1
 Summary: Provider package apache-airflow-providers-teradata for Apache Airflow
 Keywords: airflow-provider,teradata,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.3.1
-Requires-Dist: apache-airflow>=2.7.0
+Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: teradatasql>=17.20.0.28
 Requires-Dist: teradatasqlalchemy>=17.20.0.0
 Requires-Dist: apache-airflow-providers-amazon ; extra == "amazon"
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-microsoft-azure ; extra == "microsoft.azure"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/changelog.html
@@ -79,15 +79,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-teradata``
 
-Release: ``2.2.0``
+Release: ``2.2.0.rc1``
 
 
 `Teradata <https://www.teradata.com/>`__
 
 
 Provider package
 ----------------
```

