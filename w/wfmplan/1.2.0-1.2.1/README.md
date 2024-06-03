# Comparing `tmp/wfmplan-1.2.0.tar.gz` & `tmp/wfmplan-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfmplan-1.2.0.tar", last modified: Sun Jun  2 16:57:13 2024, max compression
+gzip compressed data, was "wfmplan-1.2.1.tar", last modified: Sun Jun  2 22:54:28 2024, max compression
```

## Comparing `wfmplan-1.2.0.tar` & `wfmplan-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.284753 wfmplan-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-02 16:57:09.000000 wfmplan-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-06-02 16:57:13.280753 wfmplan-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-06-02 16:57:09.000000 wfmplan-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:57:13.284753 wfmplan-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-06-02 16:57:09.000000 wfmplan-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.280753 wfmplan-1.2.0/wfmplan/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.280753 wfmplan-1.2.0/wfmplan/AgentOptimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/AgentOptimizer/BatchOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/AgentOptimizer/Optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/AgentOptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.280753 wfmplan-1.2.0/wfmplan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:54:28.078637 wfmplan-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-02 22:54:24.000000 wfmplan-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-06-02 22:54:28.078637 wfmplan-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-06-02 22:54:24.000000 wfmplan-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:54:28.078637 wfmplan-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-06-02 22:54:24.000000 wfmplan-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:54:28.078637 wfmplan-1.2.1/wfmplan/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:54:28.078637 wfmplan-1.2.1/wfmplan/AgentOptimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-06-02 22:54:24.000000 wfmplan-1.2.1/wfmplan/AgentOptimizer/BatchOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-06-02 22:54:24.000000 wfmplan-1.2.1/wfmplan/AgentOptimizer/Optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 22:54:24.000000 wfmplan-1.2.1/wfmplan/AgentOptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 22:54:24.000000 wfmplan-1.2.1/wfmplan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:54:28.078637 wfmplan-1.2.1/wfmplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-06-02 22:54:28.000000 wfmplan-1.2.1/wfmplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-02 22:54:28.000000 wfmplan-1.2.1/wfmplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:54:28.000000 wfmplan-1.2.1/wfmplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 22:54:28.000000 wfmplan-1.2.1/wfmplan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 22:54:28.000000 wfmplan-1.2.1/wfmplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 22:54:28.000000 wfmplan-1.2.1/wfmplan.egg-info/top_level.txt
```

### Comparing `wfmplan-1.2.0/LICENSE.txt` & `wfmplan-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wfmplan-1.2.0/PKG-INFO` & `wfmplan-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: wfmplan
-Version: 1.2.0
+Version: 1.2.1
 Summary: Optimization library for workforce management planning
 Home-page: https://github.com/laddha-rishi/wfmplan
 Author: Rishi Laddha
 Author-email: laddha.rishi@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/laddha-rishi/wfmplan
+Project-URL: Documentation, https://medium.com/@laddha.rishi/queueing-up-success-revolutionize-workforce-planning-with-python-6c9d7edbb6cd
 Keywords: workforce management optimization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -78,15 +79,15 @@
 
 batch_optimizer = BatchOptimizer(df, operational_targets)
 result_df = batch_optimizer.run_optimization()
 
 print(result_df)
 ```
 
-For more details and advanced usage, refer to the [documentation](https://github.com/laddha-rishi/wfmplan).
+For more details and advanced usage, refer to the [documentation](https://medium.com/@laddha.rishi/queueing-up-success-revolutionize-workforce-planning-with-python-6c9d7edbb6cd).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ---
 If you're interested in collaborating to enhance the library further, please don't hesitate to contact me. This project is open source because I believe in empowering everyone and avoiding redundant work.
```

### Comparing `wfmplan-1.2.0/README.md` & `wfmplan-1.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 batch_optimizer = BatchOptimizer(df, operational_targets)
 result_df = batch_optimizer.run_optimization()
 
 print(result_df)
 ```
 
-For more details and advanced usage, refer to the [documentation](https://github.com/laddha-rishi/wfmplan).
+For more details and advanced usage, refer to the [documentation](https://medium.com/@laddha.rishi/queueing-up-success-revolutionize-workforce-planning-with-python-6c9d7edbb6cd).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ---
-If you're interested in collaborating to enhance the library further, please don't hesitate to contact me. This project is open source because I believe in empowering everyone and avoiding redundant work.
+If you're interested in collaborating to enhance the library further, please don't hesitate to contact me. This project is open source because I believe in empowering everyone and avoiding redundant work.
```

### Comparing `wfmplan-1.2.0/setup.py` & `wfmplan-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="wfmplan",
-    version="1.2.0",
+    version="1.2.1",
     description="Optimization library for workforce management planning",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/laddha-rishi/wfmplan",
     author="Rishi Laddha",
     author_email="laddha.rishi@gmail.com",
     license="MIT",
@@ -19,15 +19,16 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     project_urls={
-        "Source Code": "https://github.com/laddha-rishi/wfmplan"
+        "Source Code": "https://github.com/laddha-rishi/wfmplan",
+        "Documentation": "https://medium.com/@laddha.rishi/queueing-up-success-revolutionize-workforce-planning-with-python-6c9d7edbb6cd",
     },
     packages=find_packages(include=['wfmplan', 'wfmplan.*']),
     install_requires=[
         'numpy>=1.23.0',
         'pandas>=1.3.5',
     ],
     include_package_data=True,
```

### Comparing `wfmplan-1.2.0/wfmplan/AgentOptimizer/BatchOptimizer.py` & `wfmplan-1.2.1/wfmplan/AgentOptimizer/BatchOptimizer.py`

 * *Files identical despite different names*

### Comparing `wfmplan-1.2.0/wfmplan/AgentOptimizer/Optimizer.py` & `wfmplan-1.2.1/wfmplan/AgentOptimizer/Optimizer.py`

 * *Files identical despite different names*

### Comparing `wfmplan-1.2.0/wfmplan.egg-info/PKG-INFO` & `wfmplan-1.2.1/wfmplan.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: wfmplan
-Version: 1.2.0
+Version: 1.2.1
 Summary: Optimization library for workforce management planning
 Home-page: https://github.com/laddha-rishi/wfmplan
 Author: Rishi Laddha
 Author-email: laddha.rishi@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/laddha-rishi/wfmplan
+Project-URL: Documentation, https://medium.com/@laddha.rishi/queueing-up-success-revolutionize-workforce-planning-with-python-6c9d7edbb6cd
 Keywords: workforce management optimization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -78,15 +79,15 @@
 
 batch_optimizer = BatchOptimizer(df, operational_targets)
 result_df = batch_optimizer.run_optimization()
 
 print(result_df)
 ```
 
-For more details and advanced usage, refer to the [documentation](https://github.com/laddha-rishi/wfmplan).
+For more details and advanced usage, refer to the [documentation](https://medium.com/@laddha.rishi/queueing-up-success-revolutionize-workforce-planning-with-python-6c9d7edbb6cd).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ---
 If you're interested in collaborating to enhance the library further, please don't hesitate to contact me. This project is open source because I believe in empowering everyone and avoiding redundant work.
```

