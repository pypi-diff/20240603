# Comparing `tmp/swh_journal-1.5.1.tar.gz` & `tmp/swh_journal-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_journal-1.5.1.tar", last modified: Tue May 28 10:55:23 2024, max compression
+gzip compressed data, was "swh_journal-1.5.2.tar", last modified: Mon Jun  3 10:56:34 2024, max compression
```

## Comparing `swh_journal-1.5.1.tar` & `swh_journal-1.5.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.693455 swh_journal-1.5.1/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      355 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1385 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-28 10:55:17.000000 swh_journal-1.5.1/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-28 10:55:17.000000 swh_journal-1.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-28 10:55:17.000000 swh_journal-1.5.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-28 10:55:17.000000 swh_journal-1.5.1/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-28 10:55:17.000000 swh_journal-1.5.1/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1909 2024-05-28 10:55:23.693455 swh_journal-1.5.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      339 2024-05-28 10:55:17.000000 swh_journal-1.5.1/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.681455 swh_journal-1.5.1/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.681455 swh_journal-1.5.1/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.681455 swh_journal-1.5.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      899 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/example-journal-client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      233 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3204 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/journal-clients.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      596 2024-05-28 10:55:17.000000 swh_journal-1.5.1/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1734 2024-05-28 10:55:17.000000 swh_journal-1.5.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-28 10:55:17.000000 swh_journal-1.5.1/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2024-05-28 10:55:17.000000 swh_journal-1.5.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-05-28 10:55:17.000000 swh_journal-1.5.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      405 2024-05-28 10:55:17.000000 swh_journal-1.5.1/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-28 10:55:23.697455 swh_journal-1.5.1/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.673455 swh_journal-1.5.1/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.685454 swh_journal-1.5.1/swh/journal/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      326 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18698 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8140 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3624 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/serializers.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.689455 swh_journal-1.5.1/swh/journal/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      521 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/journal_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/log4j.properties
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19252 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1517 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_inmemory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8731 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2183 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3181 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2465 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_stream.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.689455 swh_journal-1.5.1/swh/journal/writer/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2109 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1921 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/inmemory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1156 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11213 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/kafka.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1491 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/stream.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.689455 swh_journal-1.5.1/swh.journal.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1909 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1230 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      238 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1067 2024-05-28 10:55:17.000000 swh_journal-1.5.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.121018 swh_journal-1.5.2/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      355 2024-06-03 10:56:28.000000 swh_journal-1.5.2/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-06-03 10:56:28.000000 swh_journal-1.5.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-06-03 10:56:28.000000 swh_journal-1.5.2/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1385 2024-06-03 10:56:28.000000 swh_journal-1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-06-03 10:56:28.000000 swh_journal-1.5.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-06-03 10:56:28.000000 swh_journal-1.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-06-03 10:56:28.000000 swh_journal-1.5.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-06-03 10:56:28.000000 swh_journal-1.5.2/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-06-03 10:56:28.000000 swh_journal-1.5.2/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1909 2024-06-03 10:56:34.121018 swh_journal-1.5.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      339 2024-06-03 10:56:28.000000 swh_journal-1.5.2/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.109018 swh_journal-1.5.2/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.109018 swh_journal-1.5.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.109018 swh_journal-1.5.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      899 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/example-journal-client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      233 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3204 2024-06-03 10:56:28.000000 swh_journal-1.5.2/docs/journal-clients.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      596 2024-06-03 10:56:28.000000 swh_journal-1.5.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1734 2024-06-03 10:56:28.000000 swh_journal-1.5.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-06-03 10:56:28.000000 swh_journal-1.5.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2024-06-03 10:56:28.000000 swh_journal-1.5.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-06-03 10:56:28.000000 swh_journal-1.5.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      405 2024-06-03 10:56:28.000000 swh_journal-1.5.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-06-03 10:56:34.121018 swh_journal-1.5.2/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.101018 swh_journal-1.5.2/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.113018 swh_journal-1.5.2/swh/journal/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      326 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18418 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8140 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3624 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/serializers.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.117018 swh_journal-1.5.2/swh/journal/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      521 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/journal_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/log4j.properties
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19252 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/test_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1517 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/test_inmemory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8731 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2183 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3181 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2465 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/tests/test_stream.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.117018 swh_journal-1.5.2/swh/journal/writer/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2109 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/writer/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1921 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/writer/inmemory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1156 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/writer/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11213 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/writer/kafka.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1491 2024-06-03 10:56:28.000000 swh_journal-1.5.2/swh/journal/writer/stream.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 10:56:34.117018 swh_journal-1.5.2/swh.journal.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1909 2024-06-03 10:56:34.000000 swh_journal-1.5.2/swh.journal.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1230 2024-06-03 10:56:34.000000 swh_journal-1.5.2/swh.journal.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-06-03 10:56:34.000000 swh_journal-1.5.2/swh.journal.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-06-03 10:56:34.000000 swh_journal-1.5.2/swh.journal.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      238 2024-06-03 10:56:34.000000 swh_journal-1.5.2/swh.journal.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-06-03 10:56:34.000000 swh_journal-1.5.2/swh.journal.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1067 2024-06-03 10:56:28.000000 swh_journal-1.5.2/tox.ini
```

### Comparing `swh_journal-1.5.1/.pre-commit-config.yaml` & `swh_journal-1.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/CODE_OF_CONDUCT.md` & `swh_journal-1.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/LICENSE` & `swh_journal-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/PKG-INFO` & `swh_journal-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.5.1
+Version: 1.5.2
 Summary: Software Heritage Journal utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-journal
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-journal/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-journal/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-journal.git
```

### Comparing `swh_journal-1.5.1/docs/example-journal-client.py` & `swh_journal-1.5.2/docs/example-journal-client.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/docs/journal-clients.rst` & `swh_journal-1.5.2/docs/journal-clients.rst`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/mypy.ini` & `swh_journal-1.5.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/pyproject.toml` & `swh_journal-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/client.py` & `swh_journal-1.5.2/swh/journal/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from collections import defaultdict
 import enum
 from importlib import import_module
 from itertools import cycle
 import logging
 import os
-import time
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 import warnings
 
 from confluent_kafka import (
     OFFSET_BEGINNING,
     Consumer,
     KafkaError,
@@ -370,29 +369,27 @@
                 for i in cycle(reversed(range(10))):
                     messages = self.consumer.consume(
                         timeout=timeout, num_messages=batch_size
                     )
                     if messages:
                         break
 
-                    # do check for an EOF condition if we already consumed
+                    # do check for an EOF condition iff we already consumed
                     # messages, otherwise we could detect an EOF condition
                     # before messages had a chance to reach us (e.g. in tests)
                     if total_objects_processed > 0 and i == 0:
-                        assignment = self.get_assignment()
-
                         if self.on_eof == EofBehavior.STOP:
                             at_eof = all(
                                 (tp.topic, tp.partition) in self.eof_reached
-                                for tp in assignment
+                                for tp in self.consumer.assignment()
                             )
                             if at_eof:
                                 break
                         elif self.on_eof == EofBehavior.RESTART:
-                            for tp in assignment:
+                            for tp in self.consumer.assignment():
                                 if (tp.topic, tp.partition) in self.eof_reached:
                                     self.eof_reached.remove((tp.topic, tp.partition))
                                     self.statsd.increment("partition_restart_total")
                                     new_tp = TopicPartition(
                                         tp.topic,
                                         tp.partition,
                                         OFFSET_BEGINNING,
@@ -444,31 +441,23 @@
                 objects[object_type].append(deserialized_object)
 
         if objects:
             worker_fn(dict(objects))
         self.consumer.commit()
 
         if self.on_eof in (EofBehavior.STOP, EofBehavior.RESTART):
-            assignment = self.get_assignment()
-
             at_eof = all(
-                (tp.topic, tp.partition) in self.eof_reached for tp in assignment
+                (tp.topic, tp.partition) in self.eof_reached
+                for tp in self.consumer.assignment()
             )
         elif self.on_eof == EofBehavior.CONTINUE:
             at_eof = False
         else:
             assert False, f"Unexpected on_eof behavior: {self.on_eof}"
 
         return nb_processed, at_eof
 
     def deserialize_message(self, message, object_type=None):
         return self.value_deserializer(object_type, message.value())
 
     def close(self):
         self.consumer.close()
-
-    def get_assignment(self):
-        while not (assignment := self.consumer.assignment()):
-            logger.info("No partition assigned, waiting for a new assignment")
-            time.sleep(1)
-
-        return assignment
```

### Comparing `swh_journal-1.5.1/swh/journal/pytest_plugin.py` & `swh_journal-1.5.2/swh/journal/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/serializers.py` & `swh_journal-1.5.2/swh/journal/serializers.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/tests/journal_data.py` & `swh_journal-1.5.2/swh/journal/tests/journal_data.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/tests/test_client.py` & `swh_journal-1.5.2/swh/journal/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/tests/test_inmemory.py` & `swh_journal-1.5.2/swh/journal/tests/test_inmemory.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/tests/test_kafka_writer.py` & `swh_journal-1.5.2/swh/journal/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/tests/test_pytest_plugin.py` & `swh_journal-1.5.2/swh/journal/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/tests/test_serializers.py` & `swh_journal-1.5.2/swh/journal/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/tests/test_stream.py` & `swh_journal-1.5.2/swh/journal/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/writer/__init__.py` & `swh_journal-1.5.2/swh/journal/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/writer/inmemory.py` & `swh_journal-1.5.2/swh/journal/writer/inmemory.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/writer/interface.py` & `swh_journal-1.5.2/swh/journal/writer/interface.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/writer/kafka.py` & `swh_journal-1.5.2/swh/journal/writer/kafka.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh/journal/writer/stream.py` & `swh_journal-1.5.2/swh/journal/writer/stream.py`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/swh.journal.egg-info/PKG-INFO` & `swh_journal-1.5.2/swh.journal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.5.1
+Version: 1.5.2
 Summary: Software Heritage Journal utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-journal
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-journal/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-journal/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-journal.git
```

### Comparing `swh_journal-1.5.1/swh.journal.egg-info/SOURCES.txt` & `swh_journal-1.5.2/swh.journal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh_journal-1.5.1/tox.ini` & `swh_journal-1.5.2/tox.ini`

 * *Files identical despite different names*

