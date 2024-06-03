# Comparing `tmp/koji-1.34.1.tar.gz` & `tmp/koji-1.34.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji-1.34.1.tar", last modified: Thu May 30 11:20:17 2024, max compression
+gzip compressed data, was "koji-1.34.2.tar", last modified: Mon Jun  3 07:53:29 2024, max compression
```

## Comparing `koji-1.34.1.tar` & `koji-1.34.2.tar`

### file list

```diff
@@ -1,59 +1,46 @@
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.768725 koji-1.34.1/
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.34.1/COPYING
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-05-30 11:20:17.768725 koji-1.34.1/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2024-03-05 12:28:44.000000 koji-1.34.1/README.md
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.763725 koji-1.34.1/cli/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2024-03-25 10:23:32.000000 koji-1.34.1/cli/koji
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.763725 koji-1.34.1/cli/koji_cli/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        0 2024-02-21 12:05:04.000000 koji-1.34.1/cli/koji_cli/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   356649 2024-05-30 11:20:13.000000 koji-1.34.1/cli/koji_cli/commands.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32592 2024-05-06 11:41:24.000000 koji-1.34.1/cli/koji_cli/lib.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.766725 koji-1.34.1/koji/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   139313 2024-05-30 11:20:13.000000 koji-1.34.1/koji/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    66938 2024-04-24 12:57:03.000000 koji-1.34.1/koji/__init__.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2024-05-30 11:11:41.000000 koji-1.34.1/koji/_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       82 2023-06-21 10:16:25.000000 koji-1.34.1/koji/_version.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2024-02-21 12:05:04.000000 koji-1.34.1/koji/arch.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1348 2023-06-21 10:16:25.000000 koji-1.34.1/koji/arch.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2024-02-21 12:05:04.000000 koji-1.34.1/koji/context.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      301 2023-06-21 10:16:25.000000 koji-1.34.1/koji/context.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    64208 2024-05-30 11:20:13.000000 koji-1.34.1/koji/daemon.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4292 2024-03-26 14:42:02.000000 koji-1.34.1/koji/daemon.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7590 2024-03-20 11:41:52.000000 koji-1.34.1/koji/plugin.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1358 2024-03-26 14:45:09.000000 koji-1.34.1/koji/plugin.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2024-05-30 11:20:13.000000 koji-1.34.1/koji/policy.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1428 2024-03-26 14:25:42.000000 koji-1.34.1/koji/policy.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        8 2024-03-26 15:30:24.000000 koji-1.34.1/koji/py.typed
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2024-03-05 12:28:44.000000 koji-1.34.1/koji/rpmdiff.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      756 2023-06-21 10:16:25.000000 koji-1.34.1/koji/rpmdiff.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2024-03-05 12:28:44.000000 koji-1.34.1/koji/server.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      169 2023-06-21 10:16:25.000000 koji-1.34.1/koji/server.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    34036 2024-05-30 11:08:06.000000 koji-1.34.1/koji/tasks.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     5770 2024-03-26 14:32:23.000000 koji-1.34.1/koji/tasks.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    35966 2024-05-30 11:08:06.000000 koji-1.34.1/koji/util.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     6451 2024-05-23 10:47:54.000000 koji-1.34.1/koji/util.pyi
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3846 2024-05-06 11:41:24.000000 koji-1.34.1/koji/xmlrpcplus.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      920 2024-03-26 15:13:04.000000 koji-1.34.1/koji/xmlrpcplus.pyi
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.767725 koji-1.34.1/koji.egg-info/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      867 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/SOURCES.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/dependency_links.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       56 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/requires.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/top_level.txt
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.762725 koji-1.34.1/plugins/
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.767725 koji-1.34.1/plugins/cli/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/dud.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2024-05-20 09:41:52.000000 koji-1.34.1/plugins/cli/kiwi.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/runroot.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/save_failed_tree.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/sidetag_cli.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2024-05-30 11:20:17.768725 koji-1.34.1/setup.cfg
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2434 2024-05-23 09:54:45.000000 koji-1.34.1/setup.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.767725 koji-1.34.1/tests/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2024-03-05 12:28:44.000000 koji-1.34.1/tests/test_docs_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2024-03-05 12:28:44.000000 koji-1.34.1/tests/test_scm.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.768725 koji-1.34.1/util/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41430 2024-05-06 11:41:24.000000 koji-1.34.1/util/koji-gc
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2024-03-05 12:28:44.000000 koji-1.34.1/util/koji-shadow
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    11387 2024-05-06 11:41:24.000000 koji-1.34.1/util/koji-sweep-db
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    54617 2024-05-30 11:08:06.000000 koji-1.34.1/util/kojira
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.674674 koji-1.34.2/
+-rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.34.2/COPYING
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-06-03 07:53:29.673674 koji-1.34.2/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2024-03-05 12:28:44.000000 koji-1.34.2/README.md
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.669674 koji-1.34.2/cli/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2024-03-25 10:23:32.000000 koji-1.34.2/cli/koji
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.670674 koji-1.34.2/cli/koji_cli/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        0 2024-02-21 12:05:04.000000 koji-1.34.2/cli/koji_cli/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   356649 2024-06-03 07:40:10.000000 koji-1.34.2/cli/koji_cli/commands.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32592 2024-05-06 11:41:24.000000 koji-1.34.2/cli/koji_cli/lib.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.672674 koji-1.34.2/koji/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   139313 2024-06-03 07:40:10.000000 koji-1.34.2/koji/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2024-06-03 07:46:41.000000 koji-1.34.2/koji/_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2024-02-21 12:05:04.000000 koji-1.34.2/koji/arch.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2024-02-21 12:05:04.000000 koji-1.34.2/koji/context.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    64208 2024-06-03 07:40:10.000000 koji-1.34.2/koji/daemon.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7590 2024-03-20 11:41:52.000000 koji-1.34.2/koji/plugin.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2024-06-03 07:40:10.000000 koji-1.34.2/koji/policy.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2024-03-05 12:28:44.000000 koji-1.34.2/koji/rpmdiff.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2024-03-05 12:28:44.000000 koji-1.34.2/koji/server.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    34036 2024-05-30 11:08:06.000000 koji-1.34.2/koji/tasks.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    35966 2024-05-30 11:08:06.000000 koji-1.34.2/koji/util.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3846 2024-05-06 11:41:24.000000 koji-1.34.2/koji/xmlrpcplus.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.672674 koji-1.34.2/koji.egg-info/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-06-03 07:53:29.000000 koji-1.34.2/koji.egg-info/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      656 2024-06-03 07:53:29.000000 koji-1.34.2/koji.egg-info/SOURCES.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2024-06-03 07:53:29.000000 koji-1.34.2/koji.egg-info/dependency_links.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       56 2024-06-03 07:53:29.000000 koji-1.34.2/koji.egg-info/requires.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2024-06-03 07:53:29.000000 koji-1.34.2/koji.egg-info/top_level.txt
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.669674 koji-1.34.2/plugins/
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.673674 koji-1.34.2/plugins/cli/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2024-03-05 12:28:44.000000 koji-1.34.2/plugins/cli/dud.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2024-05-20 09:41:52.000000 koji-1.34.2/plugins/cli/kiwi.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2024-03-05 12:28:44.000000 koji-1.34.2/plugins/cli/runroot.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2024-03-05 12:28:44.000000 koji-1.34.2/plugins/cli/save_failed_tree.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2024-03-05 12:28:44.000000 koji-1.34.2/plugins/cli/sidetag_cli.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2024-06-03 07:53:29.674674 koji-1.34.2/setup.cfg
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2434 2024-05-23 09:54:45.000000 koji-1.34.2/setup.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.673674 koji-1.34.2/tests/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2024-03-05 12:28:44.000000 koji-1.34.2/tests/test_docs_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2024-03-05 12:28:44.000000 koji-1.34.2/tests/test_scm.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-06-03 07:53:29.673674 koji-1.34.2/util/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41430 2024-05-06 11:41:24.000000 koji-1.34.2/util/koji-gc
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2024-03-05 12:28:44.000000 koji-1.34.2/util/koji-shadow
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    11387 2024-05-06 11:41:24.000000 koji-1.34.2/util/koji-sweep-db
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    54617 2024-05-30 11:08:06.000000 koji-1.34.2/util/kojira
```

### Comparing `koji-1.34.1/COPYING` & `koji-1.34.2/COPYING`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/PKG-INFO` & `koji-1.34.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.34.1
+Version: 1.34.2
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.34.1/README.md` & `koji-1.34.2/README.md`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/cli/koji` & `koji-1.34.2/cli/koji`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/cli/koji_cli/commands.py` & `koji-1.34.2/cli/koji_cli/commands.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/cli/koji_cli/lib.py` & `koji-1.34.2/cli/koji_cli/lib.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/__init__.py` & `koji-1.34.2/koji/__init__.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/arch.py` & `koji-1.34.2/koji/arch.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/context.py` & `koji-1.34.2/koji/context.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/daemon.py` & `koji-1.34.2/koji/daemon.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/plugin.py` & `koji-1.34.2/koji/plugin.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/policy.py` & `koji-1.34.2/koji/policy.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/rpmdiff.py` & `koji-1.34.2/koji/rpmdiff.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/server.py` & `koji-1.34.2/koji/server.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/tasks.py` & `koji-1.34.2/koji/tasks.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/util.py` & `koji-1.34.2/koji/util.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji/xmlrpcplus.py` & `koji-1.34.2/koji/xmlrpcplus.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/koji.egg-info/PKG-INFO` & `koji-1.34.2/koji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.34.1
+Version: 1.34.2
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.34.1/koji.egg-info/SOURCES.txt` & `koji-1.34.2/koji.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,38 +2,25 @@
 README.md
 setup.py
 cli/koji
 cli/koji_cli/__init__.py
 cli/koji_cli/commands.py
 cli/koji_cli/lib.py
 koji/__init__.py
-koji/__init__.pyi
 koji/_version.py
-koji/_version.pyi
 koji/arch.py
-koji/arch.pyi
 koji/context.py
-koji/context.pyi
 koji/daemon.py
-koji/daemon.pyi
 koji/plugin.py
-koji/plugin.pyi
 koji/policy.py
-koji/policy.pyi
-koji/py.typed
 koji/rpmdiff.py
-koji/rpmdiff.pyi
 koji/server.py
-koji/server.pyi
 koji/tasks.py
-koji/tasks.pyi
 koji/util.py
-koji/util.pyi
 koji/xmlrpcplus.py
-koji/xmlrpcplus.pyi
 koji.egg-info/PKG-INFO
 koji.egg-info/SOURCES.txt
 koji.egg-info/dependency_links.txt
 koji.egg-info/requires.txt
 koji.egg-info/top_level.txt
 plugins/cli/dud.py
 plugins/cli/kiwi.py
```

### Comparing `koji-1.34.1/plugins/cli/dud.py` & `koji-1.34.2/plugins/cli/dud.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/plugins/cli/kiwi.py` & `koji-1.34.2/plugins/cli/kiwi.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/plugins/cli/runroot.py` & `koji-1.34.2/plugins/cli/runroot.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/plugins/cli/save_failed_tree.py` & `koji-1.34.2/plugins/cli/save_failed_tree.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/plugins/cli/sidetag_cli.py` & `koji-1.34.2/plugins/cli/sidetag_cli.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/setup.py` & `koji-1.34.2/setup.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/tests/test_docs_version.py` & `koji-1.34.2/tests/test_docs_version.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/tests/test_scm.py` & `koji-1.34.2/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/util/koji-gc` & `koji-1.34.2/util/koji-gc`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/util/koji-shadow` & `koji-1.34.2/util/koji-shadow`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/util/koji-sweep-db` & `koji-1.34.2/util/koji-sweep-db`

 * *Files identical despite different names*

### Comparing `koji-1.34.1/util/kojira` & `koji-1.34.2/util/kojira`

 * *Files identical despite different names*

