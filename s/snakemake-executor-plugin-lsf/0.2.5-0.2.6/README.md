# Comparing `tmp/snakemake_executor_plugin_lsf-0.2.5.tar.gz` & `tmp/snakemake_executor_plugin_lsf-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_lsf-0.2.5.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_lsf-0.2.6.tar", max compression
```

## Comparing `snakemake_executor_plugin_lsf-0.2.5.tar` & `snakemake_executor_plugin_lsf-0.2.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/LICENSE
--rw-r--r--   0        0        0     5668 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/README.md
--rw-r--r--   0        0        0     1193 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    25828 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/snakemake_executor_plugin_lsf/__init__.py
--rw-r--r--   0        0        0     6714 1970-01-01 00:00:00.000000 snakemake_executor_plugin_lsf-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-06-03 14:47:07.019170 snakemake_executor_plugin_lsf-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5668 2024-06-03 14:47:07.019170 snakemake_executor_plugin_lsf-0.2.6/README.md
+-rw-r--r--   0        0        0     1193 2024-06-03 14:47:07.019170 snakemake_executor_plugin_lsf-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    26291 2024-06-03 14:47:07.019170 snakemake_executor_plugin_lsf-0.2.6/snakemake_executor_plugin_lsf/__init__.py
+-rw-r--r--   0        0        0     6714 1970-01-01 00:00:00.000000 snakemake_executor_plugin_lsf-0.2.6/PKG-INFO
```

### Comparing `snakemake_executor_plugin_lsf-0.2.5/LICENSE` & `snakemake_executor_plugin_lsf-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_lsf-0.2.5/README.md` & `snakemake_executor_plugin_lsf-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_lsf-0.2.5/pyproject.toml` & `snakemake_executor_plugin_lsf-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-lsf"
-version = "0.2.5"
+version = "0.2.6"
 description = "A Snakemake executor plugin for submitting jobs to a LSF cluster."
 authors = [
     "Brian Fulton-Howard <brian.fulton-howard@mssm.edu>",
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
```

### Comparing `snakemake_executor_plugin_lsf-0.2.5/snakemake_executor_plugin_lsf/__init__.py` & `snakemake_executor_plugin_lsf-0.2.6/snakemake_executor_plugin_lsf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,29 @@
         # You can access the job's resources, etc.
         # via the job object.
         # After submitting the job, you have to call
         # self.report_job_submission(job_info).
         # with job_info being of type
         # snakemake_interface_executor_plugins.executors.base.SubmittedJobInfo.
 
-        log_folder = f"group_{job.name}" if job.is_group() else f"rule_{job.name}"
+        if job.is_group():
+            # use the group name, which is in groupid
+            log_folder = f"group_{job.groupid}"
+            # get all wildcards of all the jobs in the group and
+            # prepend each with job name, as wildcards of same
+            # name can contain different values across jobs
+            wildcard_dict = {
+                f"{j.name}__{k}": v
+                for j in job.jobs
+                for k, v in j.wildcards_dict.items()
+            }
+        else:
+            log_folder = f"rule_{job.name}"
+            wildcard_dict = job.wildcards_dict
 
-        wildcard_dict = job.wildcards_dict
         if wildcard_dict:
             wildcard_dict_noslash = {
                 k: v.replace("/", "___") for k, v in wildcard_dict.items()
             }
             wildcard_str = "..".join(
                 [f"{k}={v}" for k, v in wildcard_dict_noslash.items()]
             )
```

### Comparing `snakemake_executor_plugin_lsf-0.2.5/PKG-INFO` & `snakemake_executor_plugin_lsf-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-lsf
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Snakemake executor plugin for submitting jobs to a LSF cluster.
 Home-page: https://github.com/befh/snakemake-executor-plugin-lsf
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,lsf
 Author: Brian Fulton-Howard
 Author-email: brian.fulton-howard@mssm.edu
 Requires-Python: >=3.11,<4.0
```

