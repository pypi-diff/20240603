# Comparing `tmp/hfutils-0.2.6.tar.gz` & `tmp/hfutils-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.2.6.tar", last modified: Thu May 16 13:09:49 2024, max compression
+gzip compressed data, was "hfutils-0.2.7.tar", last modified: Sun Jun  2 22:05:59 2024, max compression
```

## Comparing `hfutils-0.2.6.tar` & `hfutils-0.2.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.808173 hfutils-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-16 13:09:28.000000 hfutils-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 13:09:28.000000 hfutils-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-16 13:09:49.808173 hfutils-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-16 13:09:28.000000 hfutils-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.796173 hfutils-0.2.6/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/ls_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/index/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/make.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.804173 hfutils-0.2.6/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/irregular_repo.json
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.804173 hfutils-0.2.6/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:09:49.808173 hfutils-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-16 13:09:28.000000 hfutils-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.167052 hfutils-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-02 22:05:40.000000 hfutils-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-02 22:05:40.000000 hfutils-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-06-02 22:05:59.167052 hfutils-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-06-02 22:05:40.000000 hfutils-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.155052 hfutils-0.2.7/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.159052 hfutils-0.2.7/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.159052 hfutils-0.2.7/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.159052 hfutils-0.2.7/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/ls_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/entry/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.159052 hfutils-0.2.7/hfutils/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/index/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/index/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/index/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.159052 hfutils-0.2.7/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.159052 hfutils-0.2.7/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/irregular_repo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-06-02 22:05:40.000000 hfutils-0.2.7/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:05:59.163052 hfutils-0.2.7/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-06-02 22:05:59.000000 hfutils-0.2.7/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-06-02 22:05:59.000000 hfutils-0.2.7/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:05:59.000000 hfutils-0.2.7/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 22:05:59.000000 hfutils-0.2.7/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-02 22:05:59.000000 hfutils-0.2.7/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 22:05:59.000000 hfutils-0.2.7/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-02 22:05:40.000000 hfutils-0.2.7/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 22:05:40.000000 hfutils-0.2.7/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-02 22:05:40.000000 hfutils-0.2.7/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 22:05:40.000000 hfutils-0.2.7/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-02 22:05:40.000000 hfutils-0.2.7/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 22:05:40.000000 hfutils-0.2.7/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 22:05:40.000000 hfutils-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:05:59.167052 hfutils-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-02 22:05:40.000000 hfutils-0.2.7/setup.py
```

### Comparing `hfutils-0.2.6/LICENSE` & `hfutils-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/PKG-INFO` & `hfutils-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.6
+Version: 0.2.7
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,22 +17,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
-Requires-Dist: huggingface_hub>=0.22
+Requires-Dist: huggingface_hub>=0.23
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
 Requires-Dist: tzlocal
 Requires-Dist: natsort
 Provides-Extra: build
 Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
+Requires-Dist: setuptools<70; extra == "build"
 Provides-Extra: doc
 Requires-Dist: Jinja2>=3.0.0; extra == "doc"
 Requires-Dist: sphinx>=3.2.0; extra == "doc"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "doc"
 Requires-Dist: enum_tools>=0.9.0; extra == "doc"
 Requires-Dist: sphinx-toolbox; extra == "doc"
 Requires-Dist: plantumlcli>=0.0.2; extra == "doc"
```

### Comparing `hfutils-0.2.6/README.md` & `hfutils-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/archive/__init__.py` & `hfutils-0.2.7/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/archive/base.py` & `hfutils-0.2.7/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/archive/rar.py` & `hfutils-0.2.7/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/archive/sevenz.py` & `hfutils-0.2.7/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/archive/tar.py` & `hfutils-0.2.7/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/archive/zip.py` & `hfutils-0.2.7/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/entry/base.py` & `hfutils-0.2.7/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/entry/dispatch.py` & `hfutils-0.2.7/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/entry/download.py` & `hfutils-0.2.7/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/entry/ls.py` & `hfutils-0.2.7/hfutils/entry/ls.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/entry/ls_repo.py` & `hfutils-0.2.7/hfutils/entry/ls_repo.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/entry/upload.py` & `hfutils-0.2.7/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/entry/whoami.py` & `hfutils-0.2.7/hfutils/entry/whoami.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/index/fetch.py` & `hfutils-0.2.7/hfutils/index/fetch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/index/hash.py` & `hfutils-0.2.7/hfutils/index/hash.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/index/make.py` & `hfutils-0.2.7/hfutils/index/make.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/index/validate.py` & `hfutils-0.2.7/hfutils/index/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/operate/base.py` & `hfutils-0.2.7/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/operate/download.py` & `hfutils-0.2.7/hfutils/operate/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,14 @@
         try:
             hf_client.hf_hub_download(
                 repo_id=repo_id,
                 repo_type=repo_type,
                 filename=hf_normpath(file_in_repo),
                 revision=revision,
                 local_dir=td,
-                force_download=True,
-                local_dir_use_symlinks=False,
                 resume_download=resume_download,
             )
         finally:
             if os.path.exists(temp_path):
                 if os.path.dirname(local_file):
                     os.makedirs(os.path.dirname(local_file), exist_ok=True)
                 shutil.move(temp_path, local_file)
```

### Comparing `hfutils-0.2.6/hfutils/operate/upload.py` & `hfutils-0.2.7/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/operate/validate.py` & `hfutils-0.2.7/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/utils/binary.py` & `hfutils-0.2.7/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/utils/download.py` & `hfutils-0.2.7/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/utils/path.py` & `hfutils-0.2.7/hfutils/utils/path.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/utils/temp.py` & `hfutils-0.2.7/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/utils/tqdm_.py` & `hfutils-0.2.7/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils/utils/walk.py` & `hfutils-0.2.7/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils.egg-info/PKG-INFO` & `hfutils-0.2.7/hfutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.6
+Version: 0.2.7
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,22 +17,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
-Requires-Dist: huggingface_hub>=0.22
+Requires-Dist: huggingface_hub>=0.23
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
 Requires-Dist: tzlocal
 Requires-Dist: natsort
 Provides-Extra: build
 Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
+Requires-Dist: setuptools<70; extra == "build"
 Provides-Extra: doc
 Requires-Dist: Jinja2>=3.0.0; extra == "doc"
 Requires-Dist: sphinx>=3.2.0; extra == "doc"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "doc"
 Requires-Dist: enum_tools>=0.9.0; extra == "doc"
 Requires-Dist: sphinx-toolbox; extra == "doc"
 Requires-Dist: plantumlcli>=0.0.2; extra == "doc"
```

### Comparing `hfutils-0.2.6/hfutils.egg-info/SOURCES.txt` & `hfutils-0.2.7/hfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.6/hfutils.egg-info/requires.txt` & `hfutils-0.2.7/hfutils.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 hbutils>=0.9.0
-huggingface_hub>=0.22
+huggingface_hub>=0.23
 tqdm
 requests
 click>=7
 tzlocal
 natsort
 
 [7z]
 py7zr
 
 [build]
 pyinstaller<5,>=4.7
+setuptools<70
 
 [doc]
 Jinja2>=3.0.0
 sphinx>=3.2.0
 sphinx_rtd_theme>=0.4.3
 enum_tools>=0.9.0
 sphinx-toolbox
```

### Comparing `hfutils-0.2.6/setup.py` & `hfutils-0.2.7/setup.py`

 * *Files identical despite different names*

