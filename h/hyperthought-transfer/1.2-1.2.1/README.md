# Comparing `tmp/hyperthought-transfer-1.2.tar.gz` & `tmp/hyperthought-transfer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmp0gr0i2cb\hyperthought-transfer-1.2.tar", last modified: Fri Apr 26 14:26:54 2024, max compression
+gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmp2kun9hrz\hyperthought-transfer-1.2.1.tar", last modified: Mon Jun  3 13:02:41 2024, max compression
```

## Comparing `hyperthought-transfer-1.2.tar` & `hyperthought-transfer-1.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/
--rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/.coveragerc
--rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-1.2/.gitignore
--rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-1.2/.readthedocs.yml
--rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-1.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-1.2/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/docs/
--rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/changelog.rst
--rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/contributing.rst
--rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/index.rst
--rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/license.rst
--rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/Makefile
--rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/readme.rst
--rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/docs/_static/
--rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/docs/_static/.gitignore
--rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2764 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-1.2/README.rst
--rw-rw-rw-   0        0        0     1335 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1023 2024-04-26 13:16:43.000000 hyperthought-transfer-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/antivirus/
--rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/antivirus/base.py
--rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/antivirus/_mcafee.py
--rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/antivirus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/
--rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/data.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/
--rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/connect.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/template/
--rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/template/create.py
--rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/template/template.db
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/template/__init__.py
--rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/process/
--rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/process/filebinner.py
--rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/process/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/
--rw-rw-rw-   0        0        0     3273 2023-05-31 09:22:05.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/connect.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/template/
--rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/template/create.py
--rw-rw-rw-   0        0        0   147456 2024-01-28 19:41:19.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/template/template.db
--rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/template/__init__.py
--rw-rw-rw-   0        0        0    77845 2024-01-28 19:41:19.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/processes/
--rw-rw-rw-   0        0        0     6857 2023-05-31 09:04:03.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/processes/rules.py
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/processes/__init__.py
--rw-rw-rw-   0        0        0     2010 2024-01-28 19:41:19.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/utils.py
--rw-rw-rw-   0        0        0    52517 2024-01-28 19:41:19.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/__init__.py
--rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2/src/hyperthought_transfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2764 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1840 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2024-04-26 14:26:53.000000 hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 14:26:54.000000 hyperthought-transfer-1.2/tests/
--rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/tests/conftest.py
--rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2/tox.ini
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/
+-rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/.coveragerc
+-rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-1.2.1/.gitignore
+-rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-1.2.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-1.2.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-1.2.1/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/docs/
+-rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/license.rst
+-rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/readme.rst
+-rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/docs/_static/
+-rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2766 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-1.2.1/README.rst
+-rw-rw-rw-   0        0        0     1335 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2024-06-03 13:02:08.000000 hyperthought-transfer-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/antivirus/
+-rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/antivirus/base.py
+-rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/antivirus/_mcafee.py
+-rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/antivirus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/
+-rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/data.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/
+-rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/connect.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/template/
+-rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/template/create.py
+-rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/template/template.db
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/template/__init__.py
+-rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/process/
+-rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/process/filebinner.py
+-rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/process/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/
+-rw-rw-rw-   0        0        0     3273 2023-05-31 09:22:05.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/connect.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/template/
+-rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/template/create.py
+-rw-rw-rw-   0        0        0   147456 2024-01-28 19:41:19.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/template/template.db
+-rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/template/__init__.py
+-rw-rw-rw-   0        0        0    77845 2024-01-28 19:41:19.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/processes/
+-rw-rw-rw-   0        0        0     6857 2023-05-31 09:04:03.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/processes/rules.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/processes/__init__.py
+-rw-rw-rw-   0        0        0     2010 2024-01-28 19:41:19.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/utils.py
+-rw-rw-rw-   0        0        0    52577 2024-06-03 13:02:08.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2766 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1840 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2024-06-03 13:02:40.000000 hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 13:02:41.000000 hyperthought-transfer-1.2.1/tests/
+-rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-1.2.1/tox.ini
```

### Comparing `hyperthought-transfer-1.2/.coveragerc` & `hyperthought-transfer-1.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/.gitignore` & `hyperthought-transfer-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/.readthedocs.yml` & `hyperthought-transfer-1.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/CONTRIBUTING.rst` & `hyperthought-transfer-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/docs/conf.py` & `hyperthought-transfer-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/docs/index.rst` & `hyperthought-transfer-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/docs/Makefile` & `hyperthought-transfer-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/LICENSE.txt` & `hyperthought-transfer-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/PKG-INFO` & `hyperthought-transfer-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 1.2
+Version: 1.2.1
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-1.2/README.rst` & `hyperthought-transfer-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/setup.cfg` & `hyperthought-transfer-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/setup.py` & `hyperthought-transfer-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from setuptools import setup, find_packages
 
 
 if __name__ == "__main__":
     try:
         setup(
-            version="1.2",
+            version="1.2.1",
             use_scm_version={
                 "version_scheme": "no-guess-dev",
                 "local-scheme": "no-local-version",
             },
             packages=find_packages(where="src"),
             package_dir={"": "src"},
             include_package_data=True,
```

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/antivirus/base.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/antivirus/base.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/antivirus/_mcafee.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/antivirus/_mcafee.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/antivirus/__init__.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/antivirus/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/data.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/data.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/connect.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/template/create.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/template/template.db` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/template/template.db`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/database/__init__.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/database/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/filebinner/process/filebinner.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/filebinner/process/filebinner.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/connect.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/template/create.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/template/template.db` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/template/template.db`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/database/__init__.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/database/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/processes/rules.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/processes/rules.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/utils.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/manifest/__init__.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/manifest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1042,14 +1042,18 @@
             The id of the Metadata record of interest.
 
         Returns
         -------
         A list of MetadataItem objects.
         """
         metadata_record = self.database.get_metadata(metadata_id=metadata_id)
+
+        if not metadata_record:
+            return []
+
         metadata = metadata_record["metadata"]
         return ht.metadata.from_api_format(metadata=metadata)
 
     def delete_metadata(self, metadata_id: int) -> None:
         """Remove a Metadata record."""
         self.database.delete_metadata(metadata_id=metadata_id)
```

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer/__init__.py` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/PKG-INFO` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 1.2
+Version: 1.2.1
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-1.2/src/hyperthought_transfer.egg-info/SOURCES.txt` & `hyperthought-transfer-1.2.1/src/hyperthought_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.2/tox.ini` & `hyperthought-transfer-1.2.1/tox.ini`

 * *Files identical despite different names*

