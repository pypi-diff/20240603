# Comparing `tmp/swh.loader.cvs-0.8.2.tar.gz` & `tmp/swh_loader_cvs-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.loader.cvs-0.8.2.tar", last modified: Thu Jan 25 13:31:14 2024, max compression
+gzip compressed data, was "swh_loader_cvs-0.8.3.tar", last modified: Mon Jun  3 12:16:29 2024, max compression
```

## Comparing `swh.loader.cvs-0.8.2.tar` & `swh_loader_cvs-0.8.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.108508 swh.loader.cvs-0.8.2/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      376 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1133 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    34523 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9351 2024-01-25 13:31:14.108508 swh.loader.cvs-0.8.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7650 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      574 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.088508 swh.loader.cvs-0.8.2/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       47 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       45 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7650 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.088508 swh.loader.cvs-0.8.2/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.088508 swh.loader.cvs-0.8.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      265 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      613 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1803 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      159 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      226 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       42 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      247 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      193 2024-01-25 13:31:14.108508 swh.loader.cvs-0.8.2/setup.cfg
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      764 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/setup.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.080508 swh.loader.cvs-0.8.2/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.080508 swh.loader.cvs-0.8.2/swh/loader/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.092508 swh.loader.cvs-0.8.2/swh/loader/cvs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.092508 swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.080508 swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/.github/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.096508 swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/.github/workflows/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1102 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/.github/workflows/python-app.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5321 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2559 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/cvs2gitdump.1
--rw-r--r--   0 jenkins    (115) jenkins    (120)    27139 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/cvs2gitdump.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18155 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/cvsclient.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    28048 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/loader.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/py.typed
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.100508 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    34520 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/COPYRIGHT
--rw-r--r--   0 jenkins    (115) jenkins    (120)       81 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/Makefile.test
--rw-r--r--   0 jenkins    (115) jenkins    (120)       53 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/README
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2218 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/bar,v
--rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/extconf.rb
--rw-r--r--   0 jenkins    (115) jenkins    (120)      364 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/moo,v
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18806 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/py-rcsparse.c
--rw-r--r--   0 jenkins    (115) jenkins    (120)    23810 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/queue.h
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13359 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/rb-rcsparse.c
--rw-r--r--   0 jenkins    (115) jenkins    (120)    28501 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/rcsparse.c
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2480 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/rcsparse.h
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      210 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/setup.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1307 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/test.rb
--rw-r--r--   0 jenkins    (115) jenkins    (120)    25651 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/tree.h
--rw-r--r--   0 jenkins    (115) jenkins    (120)      914 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse.pyi
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18352 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/rlog.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      725 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tasks.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.100508 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.104508 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21731 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/alizagameapi.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18076 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/cpmixin.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17083 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/dino-commitid.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18140 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/dino-readded-file.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12305 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12421 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository2.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12376 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository3.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12675 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository4.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12380 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository5.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12408 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository6.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12387 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository7.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12967 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository8.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12431 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository9.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)   536935 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/nano.rlog.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    31678 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/rcsbase-log-kw-test-repo.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15002 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/runbaby.tgz
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3228 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/unsafe_rlog_with_unsafe_relative_path.rlog
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/unsafe_rlog_wrong_arborescence.rlog
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2542 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/test_cvsclient.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    42919 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1449 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/swh/loader/cvs/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-25 13:31:14.104508 swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9351 2024-01-25 13:31:14.000000 swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-01-25 13:31:14.000000 swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-01-25 13:31:14.000000 swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       51 2024-01-25 13:31:14.000000 swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-01-25 13:31:14.000000 swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-01-25 13:31:14.000000 swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-01-25 13:31:06.000000 swh.loader.cvs-0.8.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.399427 swh_loader_cvs-0.8.3/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      376 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1575 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    34523 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9418 2024-06-03 12:16:29.399427 swh_loader_cvs-0.8.3/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7650 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      574 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.379427 swh_loader_cvs-0.8.3/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       47 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       45 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7650 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.379427 swh_loader_cvs-0.8.3/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.379427 swh_loader_cvs-0.8.3/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      266 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      613 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1803 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      227 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       74 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      247 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      193 2024-06-03 12:16:29.399427 swh_loader_cvs-0.8.3/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      764 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/setup.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.371427 swh_loader_cvs-0.8.3/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.371427 swh_loader_cvs-0.8.3/swh/loader/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.383427 swh_loader_cvs-0.8.3/swh/loader/cvs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.383427 swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.371427 swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/.github/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.383427 swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/.github/workflows/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1102 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/.github/workflows/python-app.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5321 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2559 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/cvs2gitdump.1
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    27139 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/cvs2gitdump.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18155 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/cvsclient.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    27946 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/loader.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/py.typed
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.387427 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    34520 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/COPYRIGHT
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       81 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/Makefile.test
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       53 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/README
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2218 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/bar,v
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/extconf.rb
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      364 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/moo,v
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18806 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/py-rcsparse.c
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    23810 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/queue.h
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13359 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/rb-rcsparse.c
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    28501 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/rcsparse.c
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2480 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/rcsparse.h
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      210 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/setup.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1307 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/test.rb
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    25651 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/tree.h
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      914 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse.pyi
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18352 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/rlog.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      725 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tasks.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.387427 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.391427 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21731 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/alizagameapi.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18076 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/cpmixin.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17083 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/dino-commitid.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18140 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/dino-readded-file.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12305 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12421 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository2.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12376 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository3.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12675 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository4.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12380 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository5.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12408 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository6.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12387 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository7.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12967 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository8.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12431 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository9.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   536935 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/nano.rlog.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    31678 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/rcsbase-log-kw-test-repo.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15002 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/runbaby.tgz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3228 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/unsafe_rlog_with_unsafe_relative_path.rlog
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/unsafe_rlog_wrong_arborescence.rlog
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2542 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/test_cvsclient.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    42919 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1449 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/swh/loader/cvs/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 12:16:29.391427 swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9418 2024-06-03 12:16:29.000000 swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-06-03 12:16:29.000000 swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-06-03 12:16:29.000000 swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       51 2024-06-03 12:16:29.000000 swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      329 2024-06-03 12:16:29.000000 swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-06-03 12:16:29.000000 swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-06-03 12:16:23.000000 swh_loader_cvs-0.8.3/tox.ini
```

### Comparing `swh.loader.cvs-0.8.2/CODE_OF_CONDUCT.md` & `swh_loader_cvs-0.8.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/LICENSE` & `swh_loader_cvs-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/PKG-INFO` & `swh_loader_cvs-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.cvs
-Version: 0.8.2
+Version: 0.8.3
 Summary: Software Heritage CVS Loader
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-loader-cvs
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-loader-cvs/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-cvs/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-loader-cvs.git
@@ -17,27 +17,28 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity
 Requires-Dist: swh.core[http]>=0.3
 Requires-Dist: swh.storage>=0.11.3
-Requires-Dist: swh.model>=6.6.0
+Requires-Dist: swh.model>=6.13.0
 Requires-Dist: swh.scheduler>=0.0.39
 Requires-Dist: swh.loader.core>=5.7.3
 Provides-Extra: testing
 Requires-Dist: sentry-sdk; extra == "testing"
 Requires-Dist: tenacity; extra == "testing"
 Requires-Dist: swh.core[http]>=0.3; extra == "testing"
 Requires-Dist: swh.storage>=0.11.3; extra == "testing"
-Requires-Dist: swh.model>=6.6.0; extra == "testing"
+Requires-Dist: swh.model>=6.13.0; extra == "testing"
 Requires-Dist: swh.scheduler>=0.0.39; extra == "testing"
 Requires-Dist: swh.loader.core>=5.7.3; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
+Requires-Dist: swh.loader.core[testing]; extra == "testing"
 Requires-Dist: swh.scheduler[testing]; extra == "testing"
 
 Software Heritage - CVS loader
 ==============================
 
 The Software Heritage CVS Loader imports the history of CVS repositories
 into the SWH dataset.
```

### Comparing `swh.loader.cvs-0.8.2/README.rst` & `swh_loader_cvs-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/conftest.py` & `swh_loader_cvs-0.8.3/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/docs/README.rst` & `swh_loader_cvs-0.8.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/mypy.ini` & `swh_loader_cvs-0.8.3/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/pyproject.toml` & `swh_loader_cvs-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/setup.py` & `swh_loader_cvs-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/.github/workflows/python-app.yml` & `swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/README.md` & `swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/README.md`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/cvs2gitdump.1` & `swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/cvs2gitdump.1`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/cvs2gitdump/cvs2gitdump.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/cvs2gitdump/cvs2gitdump.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/cvsclient.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/cvsclient.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/loader.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,18 +311,15 @@
             contents: List[Content] = []
             skipped_contents: List[SkippedContent] = []
             directories: List[Directory] = []
 
             for obj_node in swh_dir.collect():
                 obj = obj_node.to_model()  # type: ignore
                 obj_type = obj.object_type
-                if obj_type in (
-                    Content.object_type,
-                    from_disk.DiskBackedContent.object_type,
-                ):
+                if obj_type == Content.object_type:
                     contents.append(obj.with_data())
                 elif obj_type == SkippedContent.object_type:
                     skipped_contents.append(obj)
                 elif obj_type == Directory.object_type:
                     directories.append(obj)
                 else:
                     assert False, obj_type
```

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/COPYRIGHT` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/bar,v` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/bar,v`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/py-rcsparse.c` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/py-rcsparse.c`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/queue.h` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/queue.h`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/rb-rcsparse.c` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/rb-rcsparse.c`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/rcsparse.c` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/rcsparse.c`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/rcsparse.h` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/rcsparse.h`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/test.rb` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/test.rb`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse/tree.h` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse/tree.h`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rcsparse.pyi` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rcsparse.pyi`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/rlog.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/rlog.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tasks.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/alizagameapi.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/alizagameapi.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/cpmixin.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/cpmixin.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/dino-commitid.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/dino-commitid.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/dino-readded-file.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/dino-readded-file.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository2.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository2.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository3.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository3.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository4.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository4.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository5.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository5.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository6.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository6.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository7.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository7.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository8.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository8.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/greek-repository9.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/greek-repository9.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/nano.rlog.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/nano.rlog.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/rcsbase-log-kw-test-repo.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/rcsbase-log-kw-test-repo.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/runbaby.tgz` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/runbaby.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/unsafe_rlog_with_unsafe_relative_path.rlog` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/unsafe_rlog_with_unsafe_relative_path.rlog`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/data/unsafe_rlog_wrong_arborescence.rlog` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/data/unsafe_rlog_wrong_arborescence.rlog`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/test_cvsclient.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/test_cvsclient.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/test_loader.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh/loader/cvs/tests/test_tasks.py` & `swh_loader_cvs-0.8.3/swh/loader/cvs/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/PKG-INFO` & `swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.cvs
-Version: 0.8.2
+Version: 0.8.3
 Summary: Software Heritage CVS Loader
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-loader-cvs
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-loader-cvs/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-cvs/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-loader-cvs.git
@@ -17,27 +17,28 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity
 Requires-Dist: swh.core[http]>=0.3
 Requires-Dist: swh.storage>=0.11.3
-Requires-Dist: swh.model>=6.6.0
+Requires-Dist: swh.model>=6.13.0
 Requires-Dist: swh.scheduler>=0.0.39
 Requires-Dist: swh.loader.core>=5.7.3
 Provides-Extra: testing
 Requires-Dist: sentry-sdk; extra == "testing"
 Requires-Dist: tenacity; extra == "testing"
 Requires-Dist: swh.core[http]>=0.3; extra == "testing"
 Requires-Dist: swh.storage>=0.11.3; extra == "testing"
-Requires-Dist: swh.model>=6.6.0; extra == "testing"
+Requires-Dist: swh.model>=6.13.0; extra == "testing"
 Requires-Dist: swh.scheduler>=0.0.39; extra == "testing"
 Requires-Dist: swh.loader.core>=5.7.3; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
+Requires-Dist: swh.loader.core[testing]; extra == "testing"
 Requires-Dist: swh.scheduler[testing]; extra == "testing"
 
 Software Heritage - CVS loader
 ==============================
 
 The Software Heritage CVS Loader imports the history of CVS repositories
 into the SWH dataset.
```

### Comparing `swh.loader.cvs-0.8.2/swh.loader.cvs.egg-info/SOURCES.txt` & `swh_loader_cvs-0.8.3/swh.loader.cvs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.cvs-0.8.2/tox.ini` & `swh_loader_cvs-0.8.3/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,29 @@
 envlist =
   black
   flake8
   mypy
   py3
 
 [testenv]
+usedevelop = true
 extras =
   testing
 deps =
   pytest-cov
   # the dependency below is needed for now as a workaround for
   #   https://github.com/pypa/pip/issues/6239
   # TODO: remove when this issue is fixed
   swh.scheduler[testing]
 commands =
   pytest --doctest-modules \
-         --rootdir {envsitepackagesdir} \
-         --cov={envsitepackagesdir}/swh/loader/cvs \
+         --cov=swh/loader/cvs \
          --cov-branch \
-         {envsitepackagesdir}/swh/loader/cvs \
+         swh/loader/cvs \
          {posargs}
-# --rootdir (with --import-mode from pytest.ini) are required to make tests
-# that depends on the test file to be a proper submodule of the swh namespace
-# after migration to PEP420 (implicit namespace).
 
 [testenv:black]
 skip_install = true
 deps =
   black==23.1.0
 commands =
   {envpython} -m black --check swh
@@ -42,15 +39,15 @@
 commands =
   {envpython} -m flake8
 
 [testenv:mypy]
 extras =
   testing
 deps =
-  mypy==1.0.1
+  mypy==1.8.0
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
```

