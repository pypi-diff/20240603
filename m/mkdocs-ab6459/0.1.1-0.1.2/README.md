# Comparing `tmp/mkdocs_ab6459-0.1.1.tar.gz` & `tmp/mkdocs_ab6459-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ab6459-0.1.1.tar", last modified: Mon Jun  3 08:05:19 2024, max compression
+gzip compressed data, was "mkdocs_ab6459-0.1.2.tar", last modified: Mon Jun  3 08:07:39 2024, max compression
```

## Comparing `mkdocs_ab6459-0.1.1.tar` & `mkdocs_ab6459-0.1.2.tar`

### file list

```diff
@@ -1,62 +1,16 @@
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.486475 mkdocs_ab6459-0.1.1/
--rw-r--r--   0 ian       (1000) ian       (1000)      163 2024-06-03 07:48:14.000000 mkdocs_ab6459-0.1.1/MANIFEST.in
--rw-r--r--   0 ian       (1000) ian       (1000)      435 2024-06-03 08:05:19.486475 mkdocs_ab6459-0.1.1/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 07:48:26.000000 mkdocs_ab6459-0.1.1/README.md
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.486475 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)      435 2024-06-03 08:05:19.000000 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)     1512 2024-06-03 08:05:19.000000 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 08:05:19.000000 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       39 2024-06-03 08:05:19.000000 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 07:51:23.000000 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/not-zip-safe
--rw-r--r--   0 ian       (1000) ian       (1000)        7 2024-06-03 08:05:19.000000 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        6 2024-06-03 08:05:19.000000 mkdocs_ab6459-0.1.1/mkdocs_ab6459.egg-info/top_level.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       38 2024-06-03 08:05:19.486475 mkdocs_ab6459-0.1.1/setup.cfg
--rw-r--r--   0 ian       (1000) ian       (1000)      840 2024-06-03 08:05:00.000000 mkdocs_ab6459-0.1.1/setup.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.477309 mkdocs_ab6459-0.1.1/theme/
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 08:04:03.000000 mkdocs_ab6459-0.1.1/theme/__init__.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.477309 mkdocs_ab6459-0.1.1/theme/css/
--rw-r--r--   0 ian       (1000) ian       (1000)    70329 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-grid.css
--rw-r--r--   0 ian       (1000) ian       (1000)    51795 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-grid.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)    70403 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-grid.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)    51870 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)    12065 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-reboot.css
--rw-r--r--   0 ian       (1000) ian       (1000)    10126 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-reboot.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)    12058 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)    10198 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   107823 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-utilities.css
--rw-r--r--   0 ian       (1000) ian       (1000)    85352 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-utilities.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   107691 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)    85281 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   281046 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap.css
--rw-r--r--   0 ian       (1000) ian       (1000)   232803 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   280259 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)   232911 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/bootstrap.rtl.min.css
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.477309 mkdocs_ab6459-0.1.1/theme/css/custom/
--rw-r--r--   0 ian       (1000) ian       (1000)     1769 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/custom/admonition.css
--rw-r--r--   0 ian       (1000) ian       (1000)     3215 2024-06-02 12:53:24.000000 mkdocs_ab6459-0.1.1/theme/css/custom/button.css
--rw-r--r--   0 ian       (1000) ian       (1000)     1201 2024-06-02 11:45:34.000000 mkdocs_ab6459-0.1.1/theme/css/custom/code.css
--rw-r--r--   0 ian       (1000) ian       (1000)     1986 2024-06-02 11:07:03.000000 mkdocs_ab6459-0.1.1/theme/css/custom/diagrams.css
--rw-r--r--   0 ian       (1000) ian       (1000)       53 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/custom/footer.css
--rw-r--r--   0 ian       (1000) ian       (1000)      238 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/custom/header.css
--rw-r--r--   0 ian       (1000) ian       (1000)      702 2024-06-02 12:39:44.000000 mkdocs_ab6459-0.1.1/theme/css/custom/headings.css
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-02 12:40:59.000000 mkdocs_ab6459-0.1.1/theme/css/custom/listings.css
--rw-r--r--   0 ian       (1000) ian       (1000)      533 2024-06-02 12:39:03.000000 mkdocs_ab6459-0.1.1/theme/css/custom/main.css
--rw-r--r--   0 ian       (1000) ian       (1000)      879 2024-06-02 11:48:34.000000 mkdocs_ab6459-0.1.1/theme/css/custom/sidebar.css
--rw-r--r--   0 ian       (1000) ian       (1000)     2003 2024-06-02 12:22:28.000000 mkdocs_ab6459-0.1.1/theme/css/custom/table.css
--rw-r--r--   0 ian       (1000) ian       (1000)      301 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/css/custom/video.css
--rw-r--r--   0 ian       (1000) ian       (1000)     6414 2024-06-02 10:40:43.000000 mkdocs_ab6459-0.1.1/theme/css/prism.css
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.477309 mkdocs_ab6459-0.1.1/theme/images/
--rw-r--r--   0 ian       (1000) ian       (1000)     8380 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/images/logo.svg
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.486475 mkdocs_ab6459-0.1.1/theme/js/
--rw-r--r--   0 ian       (1000) ian       (1000)   207819 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/bootstrap.bundle.js
--rw-r--r--   0 ian       (1000) ian       (1000)    80721 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/bootstrap.bundle.min.js
--rw-r--r--   0 ian       (1000) ian       (1000)   135829 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/bootstrap.esm.js
--rw-r--r--   0 ian       (1000) ian       (1000)    73935 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/bootstrap.esm.min.js
--rw-r--r--   0 ian       (1000) ian       (1000)   145401 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/bootstrap.js
--rw-r--r--   0 ian       (1000) ian       (1000)    60635 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/bootstrap.min.js
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:05:19.486475 mkdocs_ab6459-0.1.1/theme/js/custom/
--rw-r--r--   0 ian       (1000) ian       (1000)      499 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/custom/collapse_state.js
--rw-r--r--   0 ian       (1000) ian       (1000)      528 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/custom/darkmode.js
--rw-r--r--   0 ian       (1000) ian       (1000)    64049 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.1/theme/js/prism.js
--rw-r--r--   0 ian       (1000) ian       (1000)     7503 2024-06-02 12:07:46.000000 mkdocs_ab6459-0.1.1/theme/main.html
--rw-r--r--   0 ian       (1000) ian       (1000)       26 2024-06-03 07:47:24.000000 mkdocs_ab6459-0.1.1/theme/mkdocs_theme.yml
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:07:39.607577 mkdocs_ab6459-0.1.2/
+-rw-r--r--   0 ian       (1000) ian       (1000)      163 2024-06-03 07:48:14.000000 mkdocs_ab6459-0.1.2/MANIFEST.in
+-rw-r--r--   0 ian       (1000) ian       (1000)      432 2024-06-03 08:07:39.607577 mkdocs_ab6459-0.1.2/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 07:48:26.000000 mkdocs_ab6459-0.1.2/README.md
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:07:39.607577 mkdocs_ab6459-0.1.2/mkdocs_ab6459/
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 08:04:03.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459/__init__.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:07:39.607577 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)      432 2024-06-03 08:07:39.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)      316 2024-06-03 08:07:39.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 08:07:39.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/dependency_links.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       39 2024-06-03 08:07:39.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/entry_points.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 07:51:23.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/not-zip-safe
+-rw-r--r--   0 ian       (1000) ian       (1000)        7 2024-06-03 08:07:39.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/requires.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       14 2024-06-03 08:07:39.000000 mkdocs_ab6459-0.1.2/mkdocs_ab6459.egg-info/top_level.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       38 2024-06-03 08:07:39.607577 mkdocs_ab6459-0.1.2/setup.cfg
+-rw-r--r--   0 ian       (1000) ian       (1000)      837 2024-06-03 08:07:32.000000 mkdocs_ab6459-0.1.2/setup.py
```

### Comparing `mkdocs_ab6459-0.1.1/setup.py` & `mkdocs_ab6459-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_desc = fh.read()
 
 setup(
     name="mkdocs_ab6459",
-    version="0.1.1",
-    url='https://github.coventry.ac.uk/ab6459/mkdocs_cu_ab6459',
+    version="0.1.2",
+    url='https://github.coventry.ac.uk/ab6459/mkdocs_ab6459',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Topic :: Documentation',
         'Topic :: Text Processing',
     ],
     install_requires=[
         'mkdocs',
```

