# Comparing `tmp/proxpi-1.2.0b0.tar.gz` & `tmp/proxpi-1.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxpi-1.2.0b0.tar", last modified: Tue Mar 19 05:47:02 2024, max compression
+gzip compressed data, was "proxpi-1.2.0rc0.tar", last modified: Mon Jun  3 05:00:31 2024, max compression
```

## Comparing `proxpi-1.2.0b0.tar` & `proxpi-1.2.0rc0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.540002 proxpi-1.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.528002 proxpi-1.2.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.528002 proxpi-1.2.0b0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.528002 proxpi-1.2.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.github/workflows/publish-docker-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.github/workflows/publish-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-03-19 05:47:02.540002 proxpi-1.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)    23893 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/app.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.528002 proxpi-1.2.0b0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/scripts/benchmark-json-api-response-size.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-19 05:47:02.540002 proxpi-1.2.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.524002 proxpi-1.2.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.532002 proxpi-1.2.0b0/src/proxpi/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/src/proxpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30315 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/src/proxpi/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/src/proxpi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.532002 proxpi-1.2.0b0/src/proxpi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/src/proxpi/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/src/proxpi/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/src/proxpi/templates/packages.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.536002 proxpi-1.2.0b0/src/proxpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-03-19 05:47:02.000000 proxpi-1.2.0b0/src/proxpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-19 05:47:02.000000 proxpi-1.2.0b0/src/proxpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 05:47:02.000000 proxpi-1.2.0b0/src/proxpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-19 05:47:02.000000 proxpi-1.2.0b0/src/proxpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-19 05:47:02.000000 proxpi-1.2.0b0/src/proxpi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.532002 proxpi-1.2.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.524002 proxpi-1.2.0b0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.524002 proxpi-1.2.0b0/tests/data/indexes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.532002 proxpi-1.2.0b0/tests/data/indexes/extra/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.532002 proxpi-1.2.0b0/tests/data/indexes/extra/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/numpy/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/numpy/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/numpy/numpy-1.23.1-cp310-cp310-macosx_10_9_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/numpy/yanked.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.536002 proxpi-1.2.0b0/tests/data/indexes/extra/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/scipy/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/scipy/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/scipy/scipy-1.9.0-cp310-cp310-manylinux_2_17_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/scipy/scipy-1.9.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/extra/scipy/yanked.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.536002 proxpi-1.2.0b0/tests/data/indexes/root/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.536002 proxpi-1.2.0b0/tests/data/indexes/root/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_17_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_24_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_24_x86_64.whl.metadata
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_28_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_28_x86_64.whl.metadata
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-win_amd64.whl
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/numpy-1.23.1.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/numpy/yanked.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 05:47:02.536002 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/proxpi-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/proxpi-1.0.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/proxpi-1.1.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/proxpi-1.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/data/indexes/root/proxpi/yanked.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1016 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/test-docker-image.sh
--rw-r--r--   0 runner    (1001) docker     (127)    16750 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-19 05:46:53.000000 proxpi-1.2.0b0/tests/test_pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.388653 proxpi-1.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.376653 proxpi-1.2.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.376653 proxpi-1.2.0rc0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.380653 proxpi-1.2.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.github/workflows/publish-docker-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.github/workflows/publish-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-06-03 05:00:31.388653 proxpi-1.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    28058 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/app.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.380653 proxpi-1.2.0rc0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/scripts/benchmark-json-api-response-size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-06-03 05:00:31.388653 proxpi-1.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.372653 proxpi-1.2.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.380653 proxpi-1.2.0rc0/src/proxpi/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/src/proxpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/src/proxpi/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/src/proxpi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.380653 proxpi-1.2.0rc0/src/proxpi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/src/proxpi/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/src/proxpi/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/src/proxpi/templates/packages.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.388653 proxpi-1.2.0rc0/src/proxpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-06-03 05:00:31.000000 proxpi-1.2.0rc0/src/proxpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-06-03 05:00:31.000000 proxpi-1.2.0rc0/src/proxpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 05:00:31.000000 proxpi-1.2.0rc0/src/proxpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-03 05:00:31.000000 proxpi-1.2.0rc0/src/proxpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 05:00:31.000000 proxpi-1.2.0rc0/src/proxpi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.380653 proxpi-1.2.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.372653 proxpi-1.2.0rc0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.376653 proxpi-1.2.0rc0/tests/data/indexes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.380653 proxpi-1.2.0rc0/tests/data/indexes/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.384653 proxpi-1.2.0rc0/tests/data/indexes/extra/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/numpy/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/numpy/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/numpy/numpy-1.23.1-cp310-cp310-macosx_10_9_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/numpy/yanked.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.384653 proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/scipy-1.9.0-cp310-cp310-manylinux_2_17_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/scipy-1.9.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/yanked.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.384653 proxpi-1.2.0rc0/tests/data/indexes/root/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.384653 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_17_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_24_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_24_x86_64.whl.metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_28_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_28_x86_64.whl.metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-win_amd64.whl
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/numpy-1.23.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/numpy/yanked.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 05:00:31.388653 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/proxpi-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/proxpi-1.0.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/proxpi-1.1.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/proxpi-1.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/yanked.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1016 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/test-docker-image.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    16750 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-03 05:00:26.000000 proxpi-1.2.0rc0/tests/test_pypi.py
```

### Comparing `proxpi-1.2.0b0/.github/ISSUE_TEMPLATE/bug_report.md` & `proxpi-1.2.0rc0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/.github/workflows/publish-docker-image.yml` & `proxpi-1.2.0rc0/.github/workflows/publish-docker-image.yml`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/.github/workflows/publish-python-package.yml` & `proxpi-1.2.0rc0/.github/workflows/publish-python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 on:
   release:
     types: [created]
 
 jobs:
   release:
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install build tools
       run: |
         pip install -U pip
         pip install build
     - name: Build package
@@ -24,10 +26,7 @@
       run: pip install dist/*.whl
     - name: Run unit-tests
       run: |
         pip install -r tests/requirements.txt
         pytest -vvra
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: ${{ secrets.PYPI_USERNAME }}
-        password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `proxpi-1.2.0b0/.github/workflows/test-python-package.yml` & `proxpi-1.2.0rc0/.github/workflows/test-python-package.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.7, 3.8, 3.9, '3.10', '3.11', '3.12']
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
     - name: Update pip
       run: pip install -U pip
     - name: Install package
       run: pip install .
@@ -36,10 +36,10 @@
         pip install -r tests/requirements.txt
         pytest -vvra \
           --cov proxpi \
           --cov-report xml \
           --cov-report term \
           --cov-config setup.cfg
     - name: Upload coverage
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `proxpi-1.2.0b0/CODE_OF_CONDUCT.md` & `proxpi-1.2.0rc0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/CONTRIBUTING.md` & `proxpi-1.2.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/Dockerfile` & `proxpi-1.2.0rc0/Dockerfile`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/LICENSE` & `proxpi-1.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/PKG-INFO` & `proxpi-1.2.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxpi
-Version: 1.2.0b0
+Version: 1.2.0rc0
 Summary: PyPI caching mirror
 Home-page: https://github.com/EpicWink/proxpi
 Author: Laurie O
 Author-email: laurie_opperman@hotmail.com
 License: MIT
 Keywords: pypi,index,mirror,cache
 Classifier: Environment :: Console
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses>=0.6; python_version < "3.7"
 Requires-Dist: flask<4.0,>=2.0
 Requires-Dist: jinja2~=3.0
-Requires-Dist: lxml~=4.8
+Requires-Dist: lxml<6.0,>=4.8
 Requires-Dist: requests~=2.27
 
 # proxpi
 [![Build status](
 https://github.com/EpicWink/proxpi/workflows/test/badge.svg?branch=master)](
 https://github.com/EpicWink/proxpi/actions?query=branch%3Amaster+workflow%3Atest)
 [![codecov](https://codecov.io/gh/EpicWink/proxpi/branch/master/graph/badge.svg)](
```

### Comparing `proxpi-1.2.0b0/README.md` & `proxpi-1.2.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/app.requirements.txt` & `proxpi-1.2.0rc0/app.requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile --generate-hashes --output-file=app.requirements.txt
 #
-blinker==1.7.0 \
-    --hash=sha256:c3f865d4d54db7abc53758a01601cf343fe55b84c1de4e3fa910e420b438d5b9 \
-    --hash=sha256:e6820ff6fa4e4d1d8e2747c2283749c3f547e4fee112b98555cdcdae32996182
+blinker==1.8.2 \
+    --hash=sha256:1779309f71bf239144b9399d06ae925637cf6634cf6bd131104184531bf67c01 \
+    --hash=sha256:8f77b09d3bf7c795e969e9486f39c2c5e9c39d4ee07424be2bc594ece9642d83
     # via flask
-certifi==2024.2.2 \
-    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
-    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
+certifi==2024.6.2 \
+    --hash=sha256:3cd43f1c6fa7dedc5899d69d3ad0398fd018ad1a17fba83ddaf78aa46c747516 \
+    --hash=sha256:ddc6c8ce995e6987e7faf5e3f1b02b302836a0e5d98ece18392cb1a36c72ad56
     # via requests
 charset-normalizer==3.3.2 \
     --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
     --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
     --hash=sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786 \
     --hash=sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8 \
     --hash=sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09 \
@@ -108,134 +108,183 @@
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via flask
 coloredlogs==15.0.1 \
     --hash=sha256:612ee75c546f53e92e70049c9dbfcc18c935a2b9a53b66085ce9ef6a6e5c0934 \
     --hash=sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0
     # via proxpi (setup.py)
-flask==3.0.2 \
-    --hash=sha256:3232e0e9c850d781933cf0207523d1ece087eb8d87b23777ae38456e2fbe7c6e \
-    --hash=sha256:822c03f4b799204250a7ee84b1eddc40665395333973dfb9deebfe425fefcb7d
+flask==3.0.3 \
+    --hash=sha256:34e815dfaa43340d1d15a5c3a02b8476004037eb4840b34910c6e21679d288f3 \
+    --hash=sha256:ceb27b0af3823ea2737928a4d99d125a06175b8512c445cbd9a9ce200ef76842
     # via proxpi (setup.py)
-gunicorn==21.2.0 \
-    --hash=sha256:3213aa5e8c24949e792bcacfc176fef362e7aac80b76c56f6b5122bf350722f0 \
-    --hash=sha256:88ec8bff1d634f98e61b9f65bc4bf3cd918a90806c6f5c48bc5603849ec81033
+gunicorn==22.0.0 \
+    --hash=sha256:350679f91b24062c86e386e198a15438d53a7a8207235a78ba1b53df4c4378d9 \
+    --hash=sha256:4a0b436239ff76fb33f11c07a16482c521a7e09c1ce3cc293c2330afe01bec63
     # via proxpi (setup.py)
 humanfriendly==10.0 \
     --hash=sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477 \
     --hash=sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc
     # via coloredlogs
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
-itsdangerous==2.1.2 \
-    --hash=sha256:2c2349112351b88699d8d4b6b075022c0808887cb7ad10069318a8b0bc88db44 \
-    --hash=sha256:5dbbc68b317e5e42f327f9021763545dc3fc3bfe22e6deb96aaf1fc38874156a
+itsdangerous==2.2.0 \
+    --hash=sha256:c6242fc49e35958c8b15141343aa660db5fc54d4f13a1db01a3f5891b98700ef \
+    --hash=sha256:e0050c0b7da1eea53ffaf149c0cfbb5c6e2e2b69c4bef22c81fa6eb73e5f6173
     # via flask
-jinja2==3.1.3 \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+jinja2==3.1.4 \
+    --hash=sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369 \
+    --hash=sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d
     # via
     #   flask
     #   proxpi (setup.py)
-lxml==4.9.4 \
-    --hash=sha256:00e91573183ad273e242db5585b52670eddf92bacad095ce25c1e682da14ed91 \
-    --hash=sha256:01bf1df1db327e748dcb152d17389cf6d0a8c5d533ef9bab781e9d5037619229 \
-    --hash=sha256:056a17eaaf3da87a05523472ae84246f87ac2f29a53306466c22e60282e54ff8 \
-    --hash=sha256:0a08c89b23117049ba171bf51d2f9c5f3abf507d65d016d6e0fa2f37e18c0fc5 \
-    --hash=sha256:1343df4e2e6e51182aad12162b23b0a4b3fd77f17527a78c53f0f23573663545 \
-    --hash=sha256:1449f9451cd53e0fd0a7ec2ff5ede4686add13ac7a7bfa6988ff6d75cff3ebe2 \
-    --hash=sha256:16b9ec51cc2feab009e800f2c6327338d6ee4e752c76e95a35c4465e80390ccd \
-    --hash=sha256:1f10f250430a4caf84115b1e0f23f3615566ca2369d1962f82bef40dd99cd81a \
-    --hash=sha256:231142459d32779b209aa4b4d460b175cadd604fed856f25c1571a9d78114771 \
-    --hash=sha256:232fd30903d3123be4c435fb5159938c6225ee8607b635a4d3fca847003134ba \
-    --hash=sha256:23d891e5bdc12e2e506e7d225d6aa929e0a0368c9916c1fddefab88166e98b20 \
-    --hash=sha256:266f655d1baff9c47b52f529b5f6bec33f66042f65f7c56adde3fcf2ed62ae8b \
-    --hash=sha256:273473d34462ae6e97c0f4e517bd1bf9588aa67a1d47d93f760a1282640e24ac \
-    --hash=sha256:2bd9ac6e44f2db368ef8986f3989a4cad3de4cd55dbdda536e253000c801bcc7 \
-    --hash=sha256:33714fcf5af4ff7e70a49731a7cc8fd9ce910b9ac194f66eaa18c3cc0a4c02be \
-    --hash=sha256:359a8b09d712df27849e0bcb62c6a3404e780b274b0b7e4c39a88826d1926c28 \
-    --hash=sha256:365005e8b0718ea6d64b374423e870648ab47c3a905356ab6e5a5ff03962b9a9 \
-    --hash=sha256:389d2b2e543b27962990ab529ac6720c3dded588cc6d0f6557eec153305a3622 \
-    --hash=sha256:3b505f2bbff50d261176e67be24e8909e54b5d9d08b12d4946344066d66b3e43 \
-    --hash=sha256:3d74d4a3c4b8f7a1f676cedf8e84bcc57705a6d7925e6daef7a1e54ae543a197 \
-    --hash=sha256:3f3f00a9061605725df1816f5713d10cd94636347ed651abdbc75828df302b20 \
-    --hash=sha256:43498ea734ccdfb92e1886dfedaebeb81178a241d39a79d5351ba2b671bff2b2 \
-    --hash=sha256:4855161013dfb2b762e02b3f4d4a21cc7c6aec13c69e3bffbf5022b3e708dd97 \
-    --hash=sha256:4d973729ce04784906a19108054e1fd476bc85279a403ea1a72fdb051c76fa48 \
-    --hash=sha256:4ece9cca4cd1c8ba889bfa67eae7f21d0d1a2e715b4d5045395113361e8c533d \
-    --hash=sha256:506becdf2ecaebaf7f7995f776394fcc8bd8a78022772de66677c84fb02dd33d \
-    --hash=sha256:520486f27f1d4ce9654154b4494cf9307b495527f3a2908ad4cb48e4f7ed7ef7 \
-    --hash=sha256:5557461f83bb7cc718bc9ee1f7156d50e31747e5b38d79cf40f79ab1447afd2d \
-    --hash=sha256:562778586949be7e0d7435fcb24aca4810913771f845d99145a6cee64d5b67ca \
-    --hash=sha256:59bb5979f9941c61e907ee571732219fa4774d5a18f3fa5ff2df963f5dfaa6bc \
-    --hash=sha256:606d445feeb0856c2b424405236a01c71af7c97e5fe42fbc778634faef2b47e4 \
-    --hash=sha256:6197c3f3c0b960ad033b9b7d611db11285bb461fc6b802c1dd50d04ad715c225 \
-    --hash=sha256:647459b23594f370c1c01768edaa0ba0959afc39caeeb793b43158bb9bb6a663 \
-    --hash=sha256:647bfe88b1997d7ae8d45dabc7c868d8cb0c8412a6e730a7651050b8c7289cf2 \
-    --hash=sha256:6bee9c2e501d835f91460b2c904bc359f8433e96799f5c2ff20feebd9bb1e590 \
-    --hash=sha256:6dbdacf5752fbd78ccdb434698230c4f0f95df7dd956d5f205b5ed6911a1367c \
-    --hash=sha256:701847a7aaefef121c5c0d855b2affa5f9bd45196ef00266724a80e439220e46 \
-    --hash=sha256:786d6b57026e7e04d184313c1359ac3d68002c33e4b1042ca58c362f1d09ff58 \
-    --hash=sha256:7b378847a09d6bd46047f5f3599cdc64fcb4cc5a5a2dd0a2af610361fbe77b16 \
-    --hash=sha256:7d1d6c9e74c70ddf524e3c09d9dc0522aba9370708c2cb58680ea40174800013 \
-    --hash=sha256:857d6565f9aa3464764c2cb6a2e3c2e75e1970e877c188f4aeae45954a314e0c \
-    --hash=sha256:8671622256a0859f5089cbe0ce4693c2af407bc053dcc99aadff7f5310b4aa02 \
-    --hash=sha256:88f7c383071981c74ec1998ba9b437659e4fd02a3c4a4d3efc16774eb108d0ec \
-    --hash=sha256:8aecb5a7f6f7f8fe9cac0bcadd39efaca8bbf8d1bf242e9f175cbe4c925116c3 \
-    --hash=sha256:91bbf398ac8bb7d65a5a52127407c05f75a18d7015a270fdd94bbcb04e65d573 \
-    --hash=sha256:936e8880cc00f839aa4173f94466a8406a96ddce814651075f95837316369899 \
-    --hash=sha256:953dd5481bd6252bd480d6ec431f61d7d87fdcbbb71b0d2bdcfc6ae00bb6fb10 \
-    --hash=sha256:95ae6c5a196e2f239150aa4a479967351df7f44800c93e5a975ec726fef005e2 \
-    --hash=sha256:9a2b5915c333e4364367140443b59f09feae42184459b913f0f41b9fed55794a \
-    --hash=sha256:9ae6c3363261021144121427b1552b29e7b59de9d6a75bf51e03bc072efb3c37 \
-    --hash=sha256:9b556596c49fa1232b0fff4b0e69b9d4083a502e60e404b44341e2f8fb7187f5 \
-    --hash=sha256:9c131447768ed7bc05a02553d939e7f0e807e533441901dd504e217b76307745 \
-    --hash=sha256:9d9d5726474cbbef279fd709008f91a49c4f758bec9c062dfbba88eab00e3ff9 \
-    --hash=sha256:a1bdcbebd4e13446a14de4dd1825f1e778e099f17f79718b4aeaf2403624b0f7 \
-    --hash=sha256:a602ed9bd2c7d85bd58592c28e101bd9ff9c718fbde06545a70945ffd5d11868 \
-    --hash=sha256:a8edae5253efa75c2fc79a90068fe540b197d1c7ab5803b800fccfe240eed33c \
-    --hash=sha256:a905affe76f1802edcac554e3ccf68188bea16546071d7583fb1b693f9cf756b \
-    --hash=sha256:a9e7c6d89c77bb2770c9491d988f26a4b161d05c8ca58f63fb1f1b6b9a74be45 \
-    --hash=sha256:aa9b5abd07f71b081a33115d9758ef6077924082055005808f68feccb27616bd \
-    --hash=sha256:aaa5c173a26960fe67daa69aa93d6d6a1cd714a6eb13802d4e4bd1d24a530644 \
-    --hash=sha256:ac7674d1638df129d9cb4503d20ffc3922bd463c865ef3cb412f2c926108e9a4 \
-    --hash=sha256:b1541e50b78e15fa06a2670157a1962ef06591d4c998b998047fff5e3236880e \
-    --hash=sha256:b1980dbcaad634fe78e710c8587383e6e3f61dbe146bcbfd13a9c8ab2d7b1192 \
-    --hash=sha256:bafa65e3acae612a7799ada439bd202403414ebe23f52e5b17f6ffc2eb98c2be \
-    --hash=sha256:bb5bd6212eb0edfd1e8f254585290ea1dadc3687dd8fd5e2fd9a87c31915cdab \
-    --hash=sha256:bbdd69e20fe2943b51e2841fc1e6a3c1de460d630f65bde12452d8c97209464d \
-    --hash=sha256:bc354b1393dce46026ab13075f77b30e40b61b1a53e852e99d3cc5dd1af4bc85 \
-    --hash=sha256:bcee502c649fa6351b44bb014b98c09cb00982a475a1912a9881ca28ab4f9cd9 \
-    --hash=sha256:bdd9abccd0927673cffe601d2c6cdad1c9321bf3437a2f507d6b037ef91ea307 \
-    --hash=sha256:c42ae7e010d7d6bc51875d768110c10e8a59494855c3d4c348b068f5fb81fdcd \
-    --hash=sha256:c71b5b860c5215fdbaa56f715bc218e45a98477f816b46cfde4a84d25b13274e \
-    --hash=sha256:c7721a3ef41591341388bb2265395ce522aba52f969d33dacd822da8f018aff8 \
-    --hash=sha256:ca8e44b5ba3edb682ea4e6185b49661fc22b230cf811b9c13963c9f982d1d964 \
-    --hash=sha256:cb53669442895763e61df5c995f0e8361b61662f26c1b04ee82899c2789c8f69 \
-    --hash=sha256:cc02c06e9e320869d7d1bd323df6dd4281e78ac2e7f8526835d3d48c69060683 \
-    --hash=sha256:d3caa09e613ece43ac292fbed513a4bce170681a447d25ffcbc1b647d45a39c5 \
-    --hash=sha256:d82411dbf4d3127b6cde7da0f9373e37ad3a43e89ef374965465928f01c2b979 \
-    --hash=sha256:dbcb2dc07308453db428a95a4d03259bd8caea97d7f0776842299f2d00c72fc8 \
-    --hash=sha256:dd4fda67f5faaef4f9ee5383435048ee3e11ad996901225ad7615bc92245bc8e \
-    --hash=sha256:ddd92e18b783aeb86ad2132d84a4b795fc5ec612e3545c1b687e7747e66e2b53 \
-    --hash=sha256:de362ac8bc962408ad8fae28f3967ce1a262b5d63ab8cefb42662566737f1dc7 \
-    --hash=sha256:e214025e23db238805a600f1f37bf9f9a15413c7bf5f9d6ae194f84980c78722 \
-    --hash=sha256:e8f9f93a23634cfafbad6e46ad7d09e0f4a25a2400e4a64b1b7b7c0fbaa06d9d \
-    --hash=sha256:e96a1788f24d03e8d61679f9881a883ecdf9c445a38f9ae3f3f193ab6c591c66 \
-    --hash=sha256:ec53a09aee61d45e7dbe7e91252ff0491b6b5fee3d85b2d45b173d8ab453efc1 \
-    --hash=sha256:f10250bb190fb0742e3e1958dd5c100524c2cc5096c67c8da51233f7448dc137 \
-    --hash=sha256:f1faee2a831fe249e1bae9cbc68d3cd8a30f7e37851deee4d7962b17c410dd56 \
-    --hash=sha256:f610d980e3fccf4394ab3806de6065682982f3d27c12d4ce3ee46a8183d64a6a \
-    --hash=sha256:f6c35b2f87c004270fa2e703b872fcc984d714d430b305145c39d53074e1ffe0 \
-    --hash=sha256:f836f39678cb47c9541f04d8ed4545719dc31ad850bf1832d6b4171e30d65d23 \
-    --hash=sha256:f99768232f036b4776ce419d3244a04fe83784bce871b16d2c2e984c7fcea847 \
-    --hash=sha256:fd814847901df6e8de13ce69b84c31fc9b3fb591224d6762d0b256d510cbf382 \
-    --hash=sha256:fdb325b7fba1e2c40b9b1db407f85642e32404131c08480dd652110fc908561b
+lxml==5.2.2 \
+    --hash=sha256:02437fb7308386867c8b7b0e5bc4cd4b04548b1c5d089ffb8e7b31009b961dc3 \
+    --hash=sha256:02f6a8eb6512fdc2fd4ca10a49c341c4e109aa6e9448cc4859af5b949622715a \
+    --hash=sha256:05f8757b03208c3f50097761be2dea0aba02e94f0dc7023ed73a7bb14ff11eb0 \
+    --hash=sha256:06668e39e1f3c065349c51ac27ae430719d7806c026fec462e5693b08b95696b \
+    --hash=sha256:07542787f86112d46d07d4f3c4e7c760282011b354d012dc4141cc12a68cef5f \
+    --hash=sha256:08ea0f606808354eb8f2dfaac095963cb25d9d28e27edcc375d7b30ab01abbf6 \
+    --hash=sha256:0969e92af09c5687d769731e3f39ed62427cc72176cebb54b7a9d52cc4fa3b73 \
+    --hash=sha256:0a028b61a2e357ace98b1615fc03f76eb517cc028993964fe08ad514b1e8892d \
+    --hash=sha256:0b3f5016e00ae7630a4b83d0868fca1e3d494c78a75b1c7252606a3a1c5fc2ad \
+    --hash=sha256:13e69be35391ce72712184f69000cda04fc89689429179bc4c0ae5f0b7a8c21b \
+    --hash=sha256:16a8326e51fcdffc886294c1e70b11ddccec836516a343f9ed0f82aac043c24a \
+    --hash=sha256:19b4e485cd07b7d83e3fe3b72132e7df70bfac22b14fe4bf7a23822c3a35bff5 \
+    --hash=sha256:1a2569a1f15ae6c8c64108a2cd2b4a858fc1e13d25846be0666fc144715e32ab \
+    --hash=sha256:1a7aca7964ac4bb07680d5c9d63b9d7028cace3e2d43175cb50bba8c5ad33316 \
+    --hash=sha256:1b590b39ef90c6b22ec0be925b211298e810b4856909c8ca60d27ffbca6c12e6 \
+    --hash=sha256:1d8a701774dfc42a2f0b8ccdfe7dbc140500d1049e0632a611985d943fcf12df \
+    --hash=sha256:1e275ea572389e41e8b039ac076a46cb87ee6b8542df3fff26f5baab43713bca \
+    --hash=sha256:2304d3c93f2258ccf2cf7a6ba8c761d76ef84948d87bf9664e14d203da2cd264 \
+    --hash=sha256:23441e2b5339bc54dc949e9e675fa35efe858108404ef9aa92f0456929ef6fe8 \
+    --hash=sha256:23cfafd56887eaed93d07bc4547abd5e09d837a002b791e9767765492a75883f \
+    --hash=sha256:28bf95177400066596cdbcfc933312493799382879da504633d16cf60bba735b \
+    --hash=sha256:2eb2227ce1ff998faf0cd7fe85bbf086aa41dfc5af3b1d80867ecfe75fb68df3 \
+    --hash=sha256:2fb0ba3e8566548d6c8e7dd82a8229ff47bd8fb8c2da237607ac8e5a1b8312e5 \
+    --hash=sha256:303f540ad2dddd35b92415b74b900c749ec2010e703ab3bfd6660979d01fd4ed \
+    --hash=sha256:339ee4a4704bc724757cd5dd9dc8cf4d00980f5d3e6e06d5847c1b594ace68ab \
+    --hash=sha256:33ce9e786753743159799fdf8e92a5da351158c4bfb6f2db0bf31e7892a1feb5 \
+    --hash=sha256:343ab62e9ca78094f2306aefed67dcfad61c4683f87eee48ff2fd74902447726 \
+    --hash=sha256:34e17913c431f5ae01d8658dbf792fdc457073dcdfbb31dc0cc6ab256e664a8d \
+    --hash=sha256:364d03207f3e603922d0d3932ef363d55bbf48e3647395765f9bfcbdf6d23632 \
+    --hash=sha256:38b67afb0a06b8575948641c1d6d68e41b83a3abeae2ca9eed2ac59892b36706 \
+    --hash=sha256:3a745cc98d504d5bd2c19b10c79c61c7c3df9222629f1b6210c0368177589fb8 \
+    --hash=sha256:3b019d4ee84b683342af793b56bb35034bd749e4cbdd3d33f7d1107790f8c472 \
+    --hash=sha256:3b6a30a9ab040b3f545b697cb3adbf3696c05a3a68aad172e3fd7ca73ab3c835 \
+    --hash=sha256:3d1e35572a56941b32c239774d7e9ad724074d37f90c7a7d499ab98761bd80cf \
+    --hash=sha256:3d98de734abee23e61f6b8c2e08a88453ada7d6486dc7cdc82922a03968928db \
+    --hash=sha256:453d037e09a5176d92ec0fd282e934ed26d806331a8b70ab431a81e2fbabf56d \
+    --hash=sha256:45f9494613160d0405682f9eee781c7e6d1bf45f819654eb249f8f46a2c22545 \
+    --hash=sha256:4820c02195d6dfb7b8508ff276752f6b2ff8b64ae5d13ebe02e7667e035000b9 \
+    --hash=sha256:49095a38eb333aaf44c06052fd2ec3b8f23e19747ca7ec6f6c954ffea6dbf7be \
+    --hash=sha256:4aefd911793b5d2d7a921233a54c90329bf3d4a6817dc465f12ffdfe4fc7b8fe \
+    --hash=sha256:4bc6cb140a7a0ad1f7bc37e018d0ed690b7b6520ade518285dc3171f7a117905 \
+    --hash=sha256:4c30a2f83677876465f44c018830f608fa3c6a8a466eb223535035fbc16f3438 \
+    --hash=sha256:50127c186f191b8917ea2fb8b206fbebe87fd414a6084d15568c27d0a21d60db \
+    --hash=sha256:50ccb5d355961c0f12f6cf24b7187dbabd5433f29e15147a67995474f27d1776 \
+    --hash=sha256:519895c99c815a1a24a926d5b60627ce5ea48e9f639a5cd328bda0515ea0f10c \
+    --hash=sha256:54401c77a63cc7d6dc4b4e173bb484f28a5607f3df71484709fe037c92d4f0ed \
+    --hash=sha256:546cf886f6242dff9ec206331209db9c8e1643ae642dea5fdbecae2453cb50fd \
+    --hash=sha256:55ce6b6d803890bd3cc89975fca9de1dff39729b43b73cb15ddd933b8bc20484 \
+    --hash=sha256:56793b7a1a091a7c286b5f4aa1fe4ae5d1446fe742d00cdf2ffb1077865db10d \
+    --hash=sha256:57f0a0bbc9868e10ebe874e9f129d2917750adf008fe7b9c1598c0fbbfdde6a6 \
+    --hash=sha256:5b8c041b6265e08eac8a724b74b655404070b636a8dd6d7a13c3adc07882ef30 \
+    --hash=sha256:5e097646944b66207023bc3c634827de858aebc226d5d4d6d16f0b77566ea182 \
+    --hash=sha256:60499fe961b21264e17a471ec296dcbf4365fbea611bf9e303ab69db7159ce61 \
+    --hash=sha256:610b5c77428a50269f38a534057444c249976433f40f53e3b47e68349cca1425 \
+    --hash=sha256:625e3ef310e7fa3a761d48ca7ea1f9d8718a32b1542e727d584d82f4453d5eeb \
+    --hash=sha256:657a972f46bbefdbba2d4f14413c0d079f9ae243bd68193cb5061b9732fa54c1 \
+    --hash=sha256:69ab77a1373f1e7563e0fb5a29a8440367dec051da6c7405333699d07444f511 \
+    --hash=sha256:6a520b4f9974b0a0a6ed73c2154de57cdfd0c8800f4f15ab2b73238ffed0b36e \
+    --hash=sha256:6d68ce8e7b2075390e8ac1e1d3a99e8b6372c694bbe612632606d1d546794207 \
+    --hash=sha256:6dcc3d17eac1df7859ae01202e9bb11ffa8c98949dcbeb1069c8b9a75917e01b \
+    --hash=sha256:6dfdc2bfe69e9adf0df4915949c22a25b39d175d599bf98e7ddf620a13678585 \
+    --hash=sha256:739e36ef7412b2bd940f75b278749106e6d025e40027c0b94a17ef7968d55d56 \
+    --hash=sha256:7429e7faa1a60cad26ae4227f4dd0459efde239e494c7312624ce228e04f6391 \
+    --hash=sha256:74da9f97daec6928567b48c90ea2c82a106b2d500f397eeb8941e47d30b1ca85 \
+    --hash=sha256:74e4f025ef3db1c6da4460dd27c118d8cd136d0391da4e387a15e48e5c975147 \
+    --hash=sha256:75a9632f1d4f698b2e6e2e1ada40e71f369b15d69baddb8968dcc8e683839b18 \
+    --hash=sha256:76acba4c66c47d27c8365e7c10b3d8016a7da83d3191d053a58382311a8bf4e1 \
+    --hash=sha256:79d1fb9252e7e2cfe4de6e9a6610c7cbb99b9708e2c3e29057f487de5a9eaefa \
+    --hash=sha256:7ce7ad8abebe737ad6143d9d3bf94b88b93365ea30a5b81f6877ec9c0dee0a48 \
+    --hash=sha256:7ed07b3062b055d7a7f9d6557a251cc655eed0b3152b76de619516621c56f5d3 \
+    --hash=sha256:7ff762670cada8e05b32bf1e4dc50b140790909caa8303cfddc4d702b71ea184 \
+    --hash=sha256:8268cbcd48c5375f46e000adb1390572c98879eb4f77910c6053d25cc3ac2c67 \
+    --hash=sha256:875a3f90d7eb5c5d77e529080d95140eacb3c6d13ad5b616ee8095447b1d22e7 \
+    --hash=sha256:89feb82ca055af0fe797a2323ec9043b26bc371365847dbe83c7fd2e2f181c34 \
+    --hash=sha256:8a7e24cb69ee5f32e003f50e016d5fde438010c1022c96738b04fc2423e61706 \
+    --hash=sha256:8ab6a358d1286498d80fe67bd3d69fcbc7d1359b45b41e74c4a26964ca99c3f8 \
+    --hash=sha256:8b8df03a9e995b6211dafa63b32f9d405881518ff1ddd775db4e7b98fb545e1c \
+    --hash=sha256:8cf85a6e40ff1f37fe0f25719aadf443686b1ac7652593dc53c7ef9b8492b115 \
+    --hash=sha256:8e8d351ff44c1638cb6e980623d517abd9f580d2e53bfcd18d8941c052a5a009 \
+    --hash=sha256:9164361769b6ca7769079f4d426a41df6164879f7f3568be9086e15baca61466 \
+    --hash=sha256:96e85aa09274955bb6bd483eaf5b12abadade01010478154b0ec70284c1b1526 \
+    --hash=sha256:981a06a3076997adf7c743dcd0d7a0415582661e2517c7d961493572e909aa1d \
+    --hash=sha256:9cd5323344d8ebb9fb5e96da5de5ad4ebab993bbf51674259dbe9d7a18049525 \
+    --hash=sha256:9d6c6ea6a11ca0ff9cd0390b885984ed31157c168565702959c25e2191674a14 \
+    --hash=sha256:a02d3c48f9bb1e10c7788d92c0c7db6f2002d024ab6e74d6f45ae33e3d0288a3 \
+    --hash=sha256:a233bb68625a85126ac9f1fc66d24337d6e8a0f9207b688eec2e7c880f012ec0 \
+    --hash=sha256:a2f6a1bc2460e643785a2cde17293bd7a8f990884b822f7bca47bee0a82fc66b \
+    --hash=sha256:a6d17e0370d2516d5bb9062c7b4cb731cff921fc875644c3d751ad857ba9c5b1 \
+    --hash=sha256:a6d2092797b388342c1bc932077ad232f914351932353e2e8706851c870bca1f \
+    --hash=sha256:ab67ed772c584b7ef2379797bf14b82df9aa5f7438c5b9a09624dd834c1c1aaf \
+    --hash=sha256:ac6540c9fff6e3813d29d0403ee7a81897f1d8ecc09a8ff84d2eea70ede1cdbf \
+    --hash=sha256:ae4073a60ab98529ab8a72ebf429f2a8cc612619a8c04e08bed27450d52103c0 \
+    --hash=sha256:ae791f6bd43305aade8c0e22f816b34f3b72b6c820477aab4d18473a37e8090b \
+    --hash=sha256:aef5474d913d3b05e613906ba4090433c515e13ea49c837aca18bde190853dff \
+    --hash=sha256:b0b3f2df149efb242cee2ffdeb6674b7f30d23c9a7af26595099afaf46ef4e88 \
+    --hash=sha256:b128092c927eaf485928cec0c28f6b8bead277e28acf56800e972aa2c2abd7a2 \
+    --hash=sha256:b16db2770517b8799c79aa80f4053cd6f8b716f21f8aca962725a9565ce3ee40 \
+    --hash=sha256:b336b0416828022bfd5a2e3083e7f5ba54b96242159f83c7e3eebaec752f1716 \
+    --hash=sha256:b47633251727c8fe279f34025844b3b3a3e40cd1b198356d003aa146258d13a2 \
+    --hash=sha256:b537bd04d7ccd7c6350cdaaaad911f6312cbd61e6e6045542f781c7f8b2e99d2 \
+    --hash=sha256:b5e4ef22ff25bfd4ede5f8fb30f7b24446345f3e79d9b7455aef2836437bc38a \
+    --hash=sha256:b74b9ea10063efb77a965a8d5f4182806fbf59ed068b3c3fd6f30d2ac7bee734 \
+    --hash=sha256:bb2dc4898180bea79863d5487e5f9c7c34297414bad54bcd0f0852aee9cfdb87 \
+    --hash=sha256:bbc4b80af581e18568ff07f6395c02114d05f4865c2812a1f02f2eaecf0bfd48 \
+    --hash=sha256:bcc98f911f10278d1daf14b87d65325851a1d29153caaf146877ec37031d5f36 \
+    --hash=sha256:be49ad33819d7dcc28a309b86d4ed98e1a65f3075c6acd3cd4fe32103235222b \
+    --hash=sha256:bec4bd9133420c5c52d562469c754f27c5c9e36ee06abc169612c959bd7dbb07 \
+    --hash=sha256:c2faf60c583af0d135e853c86ac2735ce178f0e338a3c7f9ae8f622fd2eb788c \
+    --hash=sha256:c689d0d5381f56de7bd6966a4541bff6e08bf8d3871bbd89a0c6ab18aa699573 \
+    --hash=sha256:c7079d5eb1c1315a858bbf180000757db8ad904a89476653232db835c3114001 \
+    --hash=sha256:cb3942960f0beb9f46e2a71a3aca220d1ca32feb5a398656be934320804c0df9 \
+    --hash=sha256:cd9e78285da6c9ba2d5c769628f43ef66d96ac3085e59b10ad4f3707980710d3 \
+    --hash=sha256:cf2a978c795b54c539f47964ec05e35c05bd045db5ca1e8366988c7f2fe6b3ce \
+    --hash=sha256:d14a0d029a4e176795cef99c056d58067c06195e0c7e2dbb293bf95c08f772a3 \
+    --hash=sha256:d237ba6664b8e60fd90b8549a149a74fcc675272e0e95539a00522e4ca688b04 \
+    --hash=sha256:d26a618ae1766279f2660aca0081b2220aca6bd1aa06b2cf73f07383faf48927 \
+    --hash=sha256:d28cb356f119a437cc58a13f8135ab8a4c8ece18159eb9194b0d269ec4e28083 \
+    --hash=sha256:d4ed0c7cbecde7194cd3228c044e86bf73e30a23505af852857c09c24e77ec5d \
+    --hash=sha256:d83e2d94b69bf31ead2fa45f0acdef0757fa0458a129734f59f67f3d2eb7ef32 \
+    --hash=sha256:d8bbcd21769594dbba9c37d3c819e2d5847656ca99c747ddb31ac1701d0c0ed9 \
+    --hash=sha256:d9b342c76003c6b9336a80efcc766748a333573abf9350f4094ee46b006ec18f \
+    --hash=sha256:dc911208b18842a3a57266d8e51fc3cfaccee90a5351b92079beed912a7914c2 \
+    --hash=sha256:dfa7c241073d8f2b8e8dbc7803c434f57dbb83ae2a3d7892dd068d99e96efe2c \
+    --hash=sha256:e282aedd63c639c07c3857097fc0e236f984ceb4089a8b284da1c526491e3f3d \
+    --hash=sha256:e290d79a4107d7d794634ce3e985b9ae4f920380a813717adf61804904dc4393 \
+    --hash=sha256:e3d9d13603410b72787579769469af730c38f2f25505573a5888a94b62b920f8 \
+    --hash=sha256:e481bba1e11ba585fb06db666bfc23dbe181dbafc7b25776156120bf12e0d5a6 \
+    --hash=sha256:e49b052b768bb74f58c7dda4e0bdf7b79d43a9204ca584ffe1fb48a6f3c84c66 \
+    --hash=sha256:eb00b549b13bd6d884c863554566095bf6fa9c3cecb2e7b399c4bc7904cb33b5 \
+    --hash=sha256:ec87c44f619380878bd49ca109669c9f221d9ae6883a5bcb3616785fa8f94c97 \
+    --hash=sha256:edcfa83e03370032a489430215c1e7783128808fd3e2e0a3225deee278585196 \
+    --hash=sha256:f11ae142f3a322d44513de1018b50f474f8f736bc3cd91d969f464b5bfef8836 \
+    --hash=sha256:f2a09f6184f17a80897172863a655467da2b11151ec98ba8d7af89f17bf63dae \
+    --hash=sha256:f5b65529bb2f21ac7861a0e94fdbf5dc0daab41497d18223b46ee8515e5ad297 \
+    --hash=sha256:f60fdd125d85bf9c279ffb8e94c78c51b3b6a37711464e1f5f31078b45002421 \
+    --hash=sha256:f61efaf4bed1cc0860e567d2ecb2363974d414f7f1f124b1df368bbf183453a6 \
+    --hash=sha256:f90e552ecbad426eab352e7b2933091f2be77115bb16f09f78404861c8322981 \
+    --hash=sha256:f956196ef61369f1685d14dad80611488d8dc1ef00be57c0c5a03064005b0f30 \
+    --hash=sha256:fb91819461b1b56d06fa4bcf86617fac795f6a99d12239fb0c68dbeba41a0a30 \
+    --hash=sha256:fbc9d316552f9ef7bba39f4edfad4a734d3d6f93341232a9dddadec4f15d425f \
+    --hash=sha256:ff69a9a0b4b17d78170c73abe2ab12084bdf1691550c5629ad1fe7849433f324 \
+    --hash=sha256:ffb2be176fed4457e445fe540617f0252a72a8bc56208fd65a690fdb1f57660b
     # via proxpi (setup.py)
 markupsafe==2.1.5 \
     --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
     --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
     --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
     --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
     --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
@@ -297,19 +346,19 @@
     # via
     #   jinja2
     #   werkzeug
 packaging==24.0 \
     --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
     --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
     # via gunicorn
-requests==2.31.0 \
-    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
-    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+requests==2.32.3 \
+    --hash=sha256:55365417734eb18255590a9ff9eb97e9e1da868d4ccd6402399eaf68af20a760 \
+    --hash=sha256:70761cfe03c773ceb22aa2f671b4757976145175cdfca038c02654d061d6dcc6
     # via proxpi (setup.py)
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
-werkzeug==3.0.1 \
-    --hash=sha256:507e811ecea72b18a404947aded4b3390e1db8f826b494d76550ef45bb3b1dcc \
-    --hash=sha256:90a285dc0e42ad56b34e696398b8122ee4c681833fb35b8334a095d82c56da10
+werkzeug==3.0.3 \
+    --hash=sha256:097e5bfda9f0aba8da6b8545146def481d06aa7d3266e7448e2cccf67dd8bd18 \
+    --hash=sha256:fc9645dc43e03e4d630d23143a04a7f947a9a3b5727cd535fdfe155a17cc48c8
     # via flask
```

### Comparing `proxpi-1.2.0b0/scripts/benchmark-json-api-response-size.py` & `proxpi-1.2.0rc0/scripts/benchmark-json-api-response-size.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/setup.cfg` & `proxpi-1.2.0rc0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	Operating System :: Microsoft :: Windows
 
 [options]
 install_requires = 
 	dataclasses >= 0.6; python_version < "3.7"
 	flask >= 2.0, < 4.0
 	jinja2 ~= 3.0
-	lxml ~= 4.8
+	lxml >= 4.8, < 6.0
 	requests ~= 2.27
 python_requires = ~= 3.6
 packages = find:
 package_dir = 
 	=src
 
 [options.packages.find]
```

### Comparing `proxpi-1.2.0b0/src/proxpi/_cache.py` & `proxpi-1.2.0rc0/src/proxpi/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Package index interfacing and caching."""
 
-import io
 import os
 import re
 import abc
 import time
 import shutil
 import logging
 import tempfile
@@ -46,15 +45,14 @@
     if os.environ.get("PROXPI_READ_TIMEOUT")
     else None
 )
 
 logger = logging.getLogger(__name__)
 _name_normalise_re = re.compile("[-_.]+")
 _hostname_normalise_pattern = re.compile(r"[^a-z0-9]+")
-_html_parser = lxml.etree.HTMLParser()
 _time_offset = time.time()
 
 
 def _now() -> float:
     return time.monotonic() + _time_offset
 
 
@@ -385,33 +383,30 @@
 
     def _list_packages(self):
         """List projects using or updating cache."""
         if self._index_t is not None and _now() < self._index_t + self.ttl:
             return
 
         logger.info(f"Listing packages in index '{self._index_url_masked}'")
-        response = self.session.get(self.index_url, headers=self._headers)
+        response = self.session.get(self.index_url, headers=self._headers, stream=True)
         response.raise_for_status()
         self._index_t = _now()
 
         if response.headers["Content-Type"] == "application/vnd.pypi.simple.v1+json":
             response_data = response.json()
             for project in response_data["projects"]:
                 name_normalised = _name_normalise_re.sub("-", project["name"]).lower()
                 self._index[name_normalised] = f"{name_normalised}/"
             logger.debug(
                 f"Finished listing packages in index '{self._index_url_masked}'",
             )
             return
 
-        tree = lxml.etree.parse(io.BytesIO(response.content), _html_parser)
-        root = tree.getroot()
-        body = next((b for b in root if b.tag == "body"), root)
-        for child in body:
-            if child.tag == "a":
+        for _, child in lxml.etree.iterparse(response.raw, tag="a", html=True):
+            if True:  # minimise Git diff
                 name = _name_normalise_re.sub("-", child.text).lower()
                 self._index[name] = child.attrib["href"]
         logger.debug(f"Finished listing packages in index '{self._index_url_masked}'")
 
     def list_packages(self) -> t.KeysView[str]:
         """List packages.
 
@@ -446,41 +441,38 @@
             return
 
         logger.debug(f"Listing files in package '{package_name}'")
         response = None
         if self._index_t is None or _now() > self._index_t + self.ttl:
             url = urllib.parse.urljoin(self.index_url, package_name)
             logger.debug(f"Refreshing '{package_name}'")
-            response = self.session.get(url, headers=self._headers)
+            response = self.session.get(url, headers=self._headers, stream=True)
         if not response or not response.ok:
             logger.debug(f"List-files response: {response}")
             package_name_normalised = _name_normalise_re.sub("-", package_name).lower()
             if package_name_normalised not in self.list_projects():
                 raise NotFound(package_name)
             package_url = self._index[package_name]
             url = urllib.parse.urljoin(self.index_url, package_url)
-            response = self.session.get(url, headers=self._headers)
+            response = self.session.get(url, headers=self._headers, stream=True)
             response.raise_for_status()
 
         package = Package(package_name, files={}, refreshed=_now())
 
         if response.headers["Content-Type"] == "application/vnd.pypi.simple.v1+json":
             response_data = response.json()
             for file_data in response_data["files"]:
                 file = FileFromJSON.from_json_response(file_data, response.request.url)
                 package.files[file.name] = file
             self._packages[package_name] = package
             logger.debug(f"Finished listing files in package '{package_name}'")
             return
 
-        tree = lxml.etree.parse(io.BytesIO(response.content), _html_parser)
-        root = tree.getroot()
-        body = next((b for b in root if b.tag == "body"), root)
-        for child in body:
-            if child.tag == "a":
+        for _, child in lxml.etree.iterparse(response.raw, tag="a", html=True):
+            if True:  # minimise Git diff
                 file = FileFromHTML.from_html_element(child, response.request.url)
                 package.files[file.name] = file
         self._packages[package_name] = package
         logger.debug(f"Finished listing files in package '{package_name}'")
 
     def list_files(self, package_name: str) -> t.ValuesView[File]:
         """List project files.
```

### Comparing `proxpi-1.2.0b0/src/proxpi/server.py` & `proxpi-1.2.0rc0/src/proxpi/server.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/src/proxpi/templates/index.html` & `proxpi-1.2.0rc0/src/proxpi/templates/index.html`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/src/proxpi.egg-info/PKG-INFO` & `proxpi-1.2.0rc0/src/proxpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxpi
-Version: 1.2.0b0
+Version: 1.2.0rc0
 Summary: PyPI caching mirror
 Home-page: https://github.com/EpicWink/proxpi
 Author: Laurie O
 Author-email: laurie_opperman@hotmail.com
 License: MIT
 Keywords: pypi,index,mirror,cache
 Classifier: Environment :: Console
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses>=0.6; python_version < "3.7"
 Requires-Dist: flask<4.0,>=2.0
 Requires-Dist: jinja2~=3.0
-Requires-Dist: lxml~=4.8
+Requires-Dist: lxml<6.0,>=4.8
 Requires-Dist: requests~=2.27
 
 # proxpi
 [![Build status](
 https://github.com/EpicWink/proxpi/workflows/test/badge.svg?branch=master)](
 https://github.com/EpicWink/proxpi/actions?query=branch%3Amaster+workflow%3Atest)
 [![codecov](https://codecov.io/gh/EpicWink/proxpi/branch/master/graph/badge.svg)](
```

### Comparing `proxpi-1.2.0b0/src/proxpi.egg-info/SOURCES.txt` & `proxpi-1.2.0rc0/src/proxpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/_utils.py` & `proxpi-1.2.0rc0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/extra/scipy/index.html` & `proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/index.html`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/extra/scipy/index.json` & `proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/index.json`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/extra/scipy/yanked.json` & `proxpi-1.2.0rc0/tests/data/indexes/extra/scipy/yanked.json`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/root/numpy/index.html` & `proxpi-1.2.0rc0/tests/data/indexes/root/numpy/index.html`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/root/numpy/index.json` & `proxpi-1.2.0rc0/tests/data/indexes/root/numpy/index.json`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/root/numpy/yanked.json` & `proxpi-1.2.0rc0/tests/data/indexes/root/numpy/yanked.json`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/root/proxpi/index.html` & `proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/index.html`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/root/proxpi/index.json` & `proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/index.json`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/data/indexes/root/proxpi/yanked.json` & `proxpi-1.2.0rc0/tests/data/indexes/root/proxpi/yanked.json`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/test-docker-image.sh` & `proxpi-1.2.0rc0/tests/test-docker-image.sh`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/test_integration.py` & `proxpi-1.2.0rc0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0b0/tests/test_pypi.py` & `proxpi-1.2.0rc0/tests/test_pypi.py`

 * *Files identical despite different names*

