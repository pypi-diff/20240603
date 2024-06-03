# Comparing `tmp/dask_databricks-0.3.1.tar.gz` & `tmp/dask_databricks-0.3.2.tar.gz`

## Comparing `dask_databricks-0.3.1.tar` & `dask_databricks-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/_version.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/cli.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/databrickscluster.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/tests/test_databricks.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.gitignore
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/LICENSE
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/README.md
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/dask_databricks/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/dask_databricks/_version.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/dask_databricks/cli.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/dask_databricks/databrickscluster.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/dask_databricks/tests/test_databricks.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/README.md
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 dask_databricks-0.3.2/PKG-INFO
```

### Comparing `dask_databricks-0.3.1/.pre-commit-config.yaml` & `dask_databricks-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/.github/workflows/release.yaml` & `dask_databricks-0.3.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/.github/workflows/test.yaml` & `dask_databricks-0.3.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/dask_databricks/__init__.py` & `dask_databricks-0.3.2/dask_databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/dask_databricks/cli.py` & `dask_databricks-0.3.2/dask_databricks/cli.py`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/dask_databricks/databrickscluster.py` & `dask_databricks-0.3.2/dask_databricks/databrickscluster.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,20 +19,27 @@
     """Connect to a Dask cluster deployed via databricks."""
 
     def __init__(
         self,
         loop: Optional[IOLoop] = None,
         asynchronous: bool = False,
     ):
-        self.spark_local_ip = os.getenv("SPARK_LOCAL_IP")
+        self.spark_local_ip = os.environ.get("SPARK_LOCAL_IP")
         if self.spark_local_ip is None:
             raise KeyError(
                 "Unable to find expected environment variable SPARK_LOCAL_IP. "
                 "Are you running this on a Databricks driver node?"
             )
+        if os.environ.get("MASTER") and "local[" in os.environ.get("MASTER"):
+            raise EnvironmentError(
+                "You appear to be trying to run a multi-node Dask cluster on a "
+                "single-node databricks cluster. Maybe you want "
+                "`dask.distributed.LocalCluster().get_client()` instead"
+
+            )
         try:
             name = spark.conf.get("spark.databricks.clusterUsageTags.clusterId")
         except AttributeError:
             name = "unknown-databricks-" + uuid.uuid4().hex[:10]
         super().__init__(name=name, loop=loop, asynchronous=asynchronous)
 
         if not self.called_from_running_loop:
```

### Comparing `dask_databricks-0.3.1/dask_databricks/tests/test_databricks.py` & `dask_databricks-0.3.2/dask_databricks/tests/test_databricks.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,22 @@
         del os.environ["SPARK_LOCAL_IP"]
 
 
 def test_databricks_cluster_raises_key_error_when_initialised_outside_of_databricks(remove_spark_local_ip):
     with pytest.raises(KeyError):
         DatabricksCluster()
 
+def test_databricks_cluster_raises_environment_error_when_master_variable_implies_single_node(
+    monkeypatch,
+    set_spark_local_ip,
+    dask_cluster,
+):
+    monkeypatch.setenv("MASTER", "local[8]")
+    with pytest.raises(EnvironmentError):
+        DatabricksCluster()
 
 def test_databricks_cluster_create(set_spark_local_ip, dask_cluster):
     cluster = DatabricksCluster()
     assert isinstance(cluster, Cluster)
 
 
 def test_databricks_cluster_create_client(set_spark_local_ip, dask_cluster):
```

### Comparing `dask_databricks-0.3.1/.gitignore` & `dask_databricks-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/LICENSE` & `dask_databricks-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/README.md` & `dask_databricks-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/pyproject.toml` & `dask_databricks-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.1/PKG-INFO` & `dask_databricks-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dask-databricks
-Version: 0.3.1
+Version: 0.3.2
 Project-URL: Documentation, https://github.com/dask-contrib/dask-databricks#readme
 Project-URL: Issues, https://github.com/dask-contrib/dask-databricks/issues
 Project-URL: Source, https://github.com/dask-contrib/dask-databricks
 Author-email: Jacob Tomlinson <jacob@tomlinson.email>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

