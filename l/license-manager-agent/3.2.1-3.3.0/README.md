# Comparing `tmp/license_manager_agent-3.2.1.tar.gz` & `tmp/license_manager_agent-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_agent-3.2.1.tar", max compression
+gzip compressed data, was "license_manager_agent-3.3.0.tar", max compression
```

## Comparing `license_manager_agent-3.2.1.tar` & `license_manager_agent-3.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1911 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/__init__.py
--rw-r--r--   0        0        0      288 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/constants.py
--rw-r--r--   0        0        0     1808 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/models.py
--rw-r--r--   0        0        0     9582 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/utils.py
--rw-r--r--   0        0        0     3473 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/config.py
--rw-r--r--   0        0        0     1150 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/exceptions.py
--rw-r--r--   0        0        0     2519 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/logs.py
--rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/__init__.py
--rw-r--r--   0        0        0     4942 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/flexlm.py
--rw-r--r--   0        0        0     3953 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/lmx.py
--rw-r--r--   0        0        0     4521 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/lsdyna.py
--rw-r--r--   0        0        0     4860 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/olicense.py
--rw-r--r--   0        0        0     3405 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/rlm.py
--rwxr-xr-x   0        0        0     1063 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/reconcile.py
--rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/__init__.py
--rw-r--r--   0        0        0     3002 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/flexlm.py
--rw-r--r--   0        0        0     1871 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/license_server_interface.py
--rw-r--r--   0        0        0     2844 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/lmx.py
--rw-r--r--   0        0        0     2810 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/lsdyna.py
--rw-r--r--   0        0        0     2802 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/olicense.py
--rw-r--r--   0        0        0     2737 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/rlm.py
--rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/__init__.py
--rw-r--r--   0        0        0     9881 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/clean_jobs_and_bookings.py
--rw-r--r--   0        0        0     4721 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/license_report.py
--rw-r--r--   0        0        0      496 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/models.py
--rw-r--r--   0        0        0     6323 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/reconciliation.py
--rw-r--r--   0        0        0     1269 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/utils.py
--rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/__init__.py
--rw-r--r--   0        0        0     9717 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/cmd_utils.py
--rw-r--r--   0        0        0      990 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/common.py
--rw-r--r--   0        0        0     3735 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/reservations.py
--rw-r--r--   0        0        0     1616 2024-05-02 17:08:19.580136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py
--rw-r--r--   0        0        0     3945 2024-05-02 17:08:19.580136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py
--rw-r--r--   0        0        0     1825 2024-05-02 17:08:19.580136 license_manager_agent-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 license_manager_agent-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1911 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/backend_utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/backend_utils/constants.py
+-rw-r--r--   0        0        0     1808 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/backend_utils/models.py
+-rw-r--r--   0        0        0    10018 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/backend_utils/utils.py
+-rw-r--r--   0        0        0     3567 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/config.py
+-rw-r--r--   0        0        0     1150 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/exceptions.py
+-rw-r--r--   0        0        0     2519 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/logs.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/parsing/__init__.py
+-rw-r--r--   0        0        0     4942 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/parsing/flexlm.py
+-rw-r--r--   0        0        0     3953 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/parsing/lmx.py
+-rw-r--r--   0        0        0     4521 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/parsing/lsdyna.py
+-rw-r--r--   0        0        0     4860 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/parsing/olicense.py
+-rw-r--r--   0        0        0     3405 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/parsing/rlm.py
+-rwxr-xr-x   0        0        0     1120 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/reconcile.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/server_interfaces/__init__.py
+-rw-r--r--   0        0        0     3002 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/server_interfaces/flexlm.py
+-rw-r--r--   0        0        0     1871 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/server_interfaces/license_server_interface.py
+-rw-r--r--   0        0        0     2844 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/server_interfaces/lmx.py
+-rw-r--r--   0        0        0     2810 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/server_interfaces/lsdyna.py
+-rw-r--r--   0        0        0     2802 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/server_interfaces/olicense.py
+-rw-r--r--   0        0        0     2737 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/server_interfaces/rlm.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/services/__init__.py
+-rw-r--r--   0        0        0     9881 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/services/clean_jobs_and_bookings.py
+-rw-r--r--   0        0        0     4721 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/services/license_report.py
+-rw-r--r--   0        0        0      496 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/services/models.py
+-rw-r--r--   0        0        0     6323 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/services/reconciliation.py
+-rw-r--r--   0        0        0     1269 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/workload_managers/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/__init__.py
+-rw-r--r--   0        0        0     9717 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/cmd_utils.py
+-rw-r--r--   0        0        0      990 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/common.py
+-rw-r--r--   0        0        0     3735 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/reservations.py
+-rw-r--r--   0        0        0     1616 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py
+-rw-r--r--   0        0        0     3945 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py
+-rw-r--r--   0        0        0     1825 2024-06-03 10:25:26.511722 license_manager_agent-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 license_manager_agent-3.3.0/PKG-INFO
```

### Comparing `license_manager_agent-3.2.1/README.md` & `license_manager_agent-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/backend_utils/models.py` & `license_manager_agent-3.3.0/lm_agent/backend_utils/models.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/backend_utils/utils.py` & `license_manager_agent-3.3.0/lm_agent/backend_utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,14 +130,28 @@
     async with AsyncBackendClient() as backend_client:
         resp = await backend_client.get("/lm/health")
     if resp.status_code != 204:
         logger.error(f"Backend health-check request failed with status code: {resp.status_code}")
         raise LicenseManagerBackendConnectionError("Could not connect to the backend health-check endpoint")
 
 
+async def report_cluster_status():
+    """
+    Report the cluster status to the backend.
+    """
+    interval = settings.STAT_INTERVAL
+
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.put("/lm/cluster_statuses", params={"interval": interval})
+
+    LicenseManagerBackendConnectionError.require_condition(
+        resp.status_code == 202, f"Failed to report cluster status: {resp.text}"
+    )
+
+
 async def get_cluster_jobs_from_backend() -> List[JobSchema]:
     """
     Get all jobs for the cluster with its bookings from the backend.
     """
     async with AsyncBackendClient() as backend_client:
         resp = await backend_client.get("/lm/jobs/by_client_id")
```

### Comparing `license_manager_agent-3.2.1/lm_agent/config.py` & `license_manager_agent-3.3.0/lm_agent/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 
     # Token cache directory
     CACHE_DIR: Path = DEFAULT_CACHE_DIR
 
     # If set to `True`, reconcile will be triggered by Prolog/Epilog. Set to `False` to disable this.
     USE_RECONCILE_IN_PROLOG_EPILOG: bool = True
 
+    # Stat interval used to report the cluster status to the API
+    STAT_INTERVAL: int = 60
+
     class Config:
         env_prefix = "LM2_AGENT_"
         if DEFAULT_DOTENV_PATH.is_file():
             env_file = DEFAULT_DOTENV_PATH
         else:
             env_file = Path(".env")
```

### Comparing `license_manager_agent-3.2.1/lm_agent/exceptions.py` & `license_manager_agent-3.3.0/lm_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/logs.py` & `license_manager_agent-3.3.0/lm_agent/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/parsing/flexlm.py` & `license_manager_agent-3.3.0/lm_agent/parsing/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/parsing/lmx.py` & `license_manager_agent-3.3.0/lm_agent/parsing/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/parsing/lsdyna.py` & `license_manager_agent-3.3.0/lm_agent/parsing/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/parsing/olicense.py` & `license_manager_agent-3.3.0/lm_agent/parsing/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/parsing/rlm.py` & `license_manager_agent-3.3.0/lm_agent/parsing/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/reconcile.py` & `license_manager_agent-3.3.0/lm_agent/reconcile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import asyncio
 import logging
 import typing
 
 import sentry_sdk
 
-from lm_agent.backend_utils.utils import check_backend_health
+from lm_agent.backend_utils.utils import check_backend_health, report_cluster_status
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
 from lm_agent.services.reconciliation import reconcile
 
 if settings.SENTRY_DSN:
     sentry_sdk.init(
         dsn=settings.SENTRY_DSN,
@@ -28,13 +28,14 @@
 
 
 async def run_reconcile():
     """Main function to setup the env and call the reconcile function."""
     begin_logging()
     logger.info("Starting reconcile script")
     await check_backend_health()
+    await report_cluster_status()
     await reconcile()
     logger.info("Reconcile completed successfully")
 
 
 def main():
     asyncio.run(run_reconcile())
```

### Comparing `license_manager_agent-3.2.1/lm_agent/server_interfaces/flexlm.py` & `license_manager_agent-3.3.0/lm_agent/server_interfaces/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/server_interfaces/license_server_interface.py` & `license_manager_agent-3.3.0/lm_agent/server_interfaces/license_server_interface.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/server_interfaces/lmx.py` & `license_manager_agent-3.3.0/lm_agent/server_interfaces/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/server_interfaces/lsdyna.py` & `license_manager_agent-3.3.0/lm_agent/server_interfaces/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/server_interfaces/olicense.py` & `license_manager_agent-3.3.0/lm_agent/server_interfaces/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/server_interfaces/rlm.py` & `license_manager_agent-3.3.0/lm_agent/server_interfaces/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/services/clean_jobs_and_bookings.py` & `license_manager_agent-3.3.0/lm_agent/services/clean_jobs_and_bookings.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/services/license_report.py` & `license_manager_agent-3.3.0/lm_agent/services/license_report.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/services/reconciliation.py` & `license_manager_agent-3.3.0/lm_agent/services/reconciliation.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/utils.py` & `license_manager_agent-3.3.0/lm_agent/utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/cmd_utils.py` & `license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/common.py` & `license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/common.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/reservations.py` & `license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/reservations.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py` & `license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py` & `license_manager_agent-3.3.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.1/pyproject.toml` & `license_manager_agent-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-agent"
-version = "3.2.1"
+version = "3.3.0"
 description = "Provides an agent for interacting with license manager"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_agent" }]
```

### Comparing `license_manager_agent-3.2.1/PKG-INFO` & `license_manager_agent-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-agent
-Version: 3.2.1
+Version: 3.3.0
 Summary: Provides an agent for interacting with license manager
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

