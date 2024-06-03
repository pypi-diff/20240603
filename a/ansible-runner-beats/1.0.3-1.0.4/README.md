# Comparing `tmp/ansible-runner-beats-1.0.3.tar.gz` & `tmp/ansible_runner_beats-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-runner-beats-1.0.3.tar", last modified: Tue Mar  7 16:23:50 2023, max compression
+gzip compressed data, was "ansible_runner_beats-1.0.4.tar", last modified: Mon Jun  3 13:23:10 2024, max compression
```

## Comparing `ansible-runner-beats-1.0.3.tar` & `ansible_runner_beats-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:50.570783 ansible-runner-beats-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-03-07 16:23:41.000000 ansible-runner-beats-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-07 16:23:50.570783 ansible-runner-beats-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-07 16:23:41.000000 ansible-runner-beats-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:50.566783 ansible-runner-beats-1.0.3/ansible_runner_beats/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-07 16:23:41.000000 ansible-runner-beats-1.0.3/ansible_runner_beats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-03-07 16:23:41.000000 ansible-runner-beats-1.0.3/ansible_runner_beats/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:50.570783 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-07 16:23:50.000000 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-07 16:23:50.000000 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 16:23:50.000000 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-07 16:23:50.000000 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 16:23:50.000000 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-07 16:23:50.000000 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-07 16:23:50.000000 ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 16:23:50.570783 ansible-runner-beats-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-07 16:23:41.000000 ansible-runner-beats-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:10.612089 ansible_runner_beats-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-06-03 13:23:05.000000 ansible_runner_beats-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-06-03 13:23:10.608090 ansible_runner_beats-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-06-03 13:23:05.000000 ansible_runner_beats-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:10.608090 ansible_runner_beats-1.0.4/ansible_runner_beats/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 13:23:05.000000 ansible_runner_beats-1.0.4/ansible_runner_beats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-06-03 13:23:05.000000 ansible_runner_beats-1.0.4/ansible_runner_beats/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:10.608090 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-06-03 13:23:10.000000 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 13:23:10.000000 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:23:10.000000 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-03 13:23:10.000000 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:23:10.000000 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-03 13:23:10.000000 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-03 13:23:10.000000 ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:23:10.612089 ansible_runner_beats-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-06-03 13:23:05.000000 ansible_runner_beats-1.0.4/setup.py
```

### Comparing `ansible-runner-beats-1.0.3/LICENSE` & `ansible_runner_beats-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-runner-beats-1.0.3/PKG-INFO` & `ansible_runner_beats-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: ansible-runner-beats
-Version: 1.0.3
-Home-page: https://github.com/claranet/ansible-runner-beats
-Author: Claranet
-License: MPL2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ansible Runner beats Event Emitter
 [![Maintainer](https://img.shields.io/badge/maintained%20by-claranet-e00000?style=flat-square)](https://www.claranet.fr/)
 [![License](https://img.shields.io/github/license/claranet/ansible-runner-beats?style=flat-square)](LICENSE)
 [![Release](https://img.shields.io/pypi/v/ansible-runner-beats?style=flat-square)](https://pypi.org/project/ansible-runner-beats/#history)
 
 This project is a plugin for [Ansible Runner](https://github.com/ansible/ansible-runner) that allows emitting Ansible status and events to Logstash through the Beats protocol. This can allow `Runner` to notify other systems as Ansible jobs are run and to deliver key events to that system if it's interested.
```

### Comparing `ansible-runner-beats-1.0.3/README.md` & `ansible_runner_beats-1.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: ansible-runner-beats
+Version: 1.0.4
+Home-page: https://github.com/claranet/ansible-runner-beats
+Author: Claranet
+License: MPL2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pylogbeat
+Requires-Dist: deepmerge
+
 # Ansible Runner beats Event Emitter
 [![Maintainer](https://img.shields.io/badge/maintained%20by-claranet-e00000?style=flat-square)](https://www.claranet.fr/)
 [![License](https://img.shields.io/github/license/claranet/ansible-runner-beats?style=flat-square)](LICENSE)
 [![Release](https://img.shields.io/pypi/v/ansible-runner-beats?style=flat-square)](https://pypi.org/project/ansible-runner-beats/#history)
 
 This project is a plugin for [Ansible Runner](https://github.com/ansible/ansible-runner) that allows emitting Ansible status and events to Logstash through the Beats protocol. This can allow `Runner` to notify other systems as Ansible jobs are run and to deliver key events to that system if it's interested.
```

### Comparing `ansible-runner-beats-1.0.3/ansible_runner_beats/events.py` & `ansible_runner_beats-1.0.4/ansible_runner_beats/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -56,14 +56,25 @@
         configuration[c] = get_conf(c, default=v)
 
     return configuration
 
 
 def status_handler(runner_config, data):
     plugin_config = get_configuration(runner_config)
+
+    def log_error(error, message):
+        prefix = "ERROR: "
+        logger.error(
+            f"{prefix}Connection to {plugin_config['runner_beats_host']}:{plugin_config['runner_beats_port']} {message}!\n",
+            f"{prefix}Please check if the beats server is running and reachable.\n",
+            f"{prefix}Skipping beats plugin for the rest of the run.\n",
+            str(error),
+            file=sys.stderr,
+        )
+
     if (
         plugin_config["runner_beats_host"] is not None
         and plugin_config["runner_beats_port"] is not None
     ):
         message = {
             "@timestamp": datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S"),
             "type": "ansible-runner",
@@ -99,25 +110,20 @@
                     message,
                     certificate=plugin_config["runner_beats_ssl_cert"],
                     key=plugin_config["runner_beats_ssl_key"],
                     ca=plugin_config["runner_beats_ssl_ca"],
                 )
         except (TimeoutError, socket.timeout) as e:
             os.environ["RUNNER_BEATS_TIMEDOUT"] = "true"
-            print(
-                f"Connection to {plugin_config['runner_beats_host']}:{plugin_config['runner_beats_port']} timed out!\n{e}",
-                file=sys.stderr,
-            )
+            log_error(e, "timed out")
         except (
             ConnectionResetError,
+            ConnectionRefusedError,
             pylogbeat.ConnectionException,
         ) as e:
-            print(
-                f"{e} ({plugin_config['runner_beats_host']}:{plugin_config['runner_beats_port']})",
-                file=sys.stderr,
-            )
+            log_error(e, "refused")
     else:
         logger.info("Beats Plugin Skipped")
 
 
 def event_handler(runner_config, data):
     status_handler(runner_config, data)
```

### Comparing `ansible-runner-beats-1.0.3/ansible_runner_beats.egg-info/PKG-INFO` & `ansible_runner_beats-1.0.4/ansible_runner_beats.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: ansible-runner-beats
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/claranet/ansible-runner-beats
 Author: Claranet
 License: MPL2
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pylogbeat
+Requires-Dist: deepmerge
 
 # Ansible Runner beats Event Emitter
 [![Maintainer](https://img.shields.io/badge/maintained%20by-claranet-e00000?style=flat-square)](https://www.claranet.fr/)
 [![License](https://img.shields.io/github/license/claranet/ansible-runner-beats?style=flat-square)](LICENSE)
 [![Release](https://img.shields.io/pypi/v/ansible-runner-beats?style=flat-square)](https://pypi.org/project/ansible-runner-beats/#history)
 
 This project is a plugin for [Ansible Runner](https://github.com/ansible/ansible-runner) that allows emitting Ansible status and events to Logstash through the Beats protocol. This can allow `Runner` to notify other systems as Ansible jobs are run and to deliver key events to that system if it's interested.
```

### Comparing `ansible-runner-beats-1.0.3/setup.py` & `ansible_runner_beats-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-with open('requirements.txt') as f:
+with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="ansible-runner-beats",
-    version="1.0.3",
+    version="1.0.4",
     author="Claranet",
     url="https://github.com/claranet/ansible-runner-beats",
     license="MPL2",
     packages=find_packages(),
     install_requires=required,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

