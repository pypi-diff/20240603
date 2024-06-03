# Comparing `tmp/mkdocs_ab6459-0.1.4.tar.gz` & `tmp/mkdocs_ab6459-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ab6459-0.1.4.tar", last modified: Mon Jun  3 08:22:28 2024, max compression
+gzip compressed data, was "mkdocs_ab6459-0.1.5.tar", last modified: Mon Jun  3 12:03:49 2024, max compression
```

## Comparing `mkdocs_ab6459-0.1.4.tar` & `mkdocs_ab6459-0.1.5.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/
--rw-r--r--   0 ian       (1000) ian       (1000)      171 2024-06-03 08:11:18.000000 mkdocs_ab6459-0.1.4/MANIFEST.in
--rw-r--r--   0 ian       (1000) ian       (1000)      432 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 07:48:26.000000 mkdocs_ab6459-0.1.4/README.md
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/mkdocs_ab6459/
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 08:04:03.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/__init__.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/
--rw-r--r--   0 ian       (1000) ian       (1000)    70329 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.css
--rw-r--r--   0 ian       (1000) ian       (1000)    51795 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)    70403 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)    51870 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)    12065 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.css
--rw-r--r--   0 ian       (1000) ian       (1000)    10126 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)    12058 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)    10198 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   107823 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.css
--rw-r--r--   0 ian       (1000) ian       (1000)    85352 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   107691 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)    85281 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   281046 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.css
--rw-r--r--   0 ian       (1000) ian       (1000)   232803 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.min.css
--rw-r--r--   0 ian       (1000) ian       (1000)   280259 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.rtl.css
--rw-r--r--   0 ian       (1000) ian       (1000)   232911 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.rtl.min.css
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/
--rw-r--r--   0 ian       (1000) ian       (1000)     1769 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/admonition.css
--rw-r--r--   0 ian       (1000) ian       (1000)     3971 2024-06-03 08:22:13.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/button.css
--rw-r--r--   0 ian       (1000) ian       (1000)     1201 2024-06-02 11:45:34.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/code.css
--rw-r--r--   0 ian       (1000) ian       (1000)     1986 2024-06-02 11:07:03.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/diagrams.css
--rw-r--r--   0 ian       (1000) ian       (1000)       53 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/footer.css
--rw-r--r--   0 ian       (1000) ian       (1000)      238 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/header.css
--rw-r--r--   0 ian       (1000) ian       (1000)      702 2024-06-02 12:39:44.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/headings.css
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-02 12:40:59.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/listings.css
--rw-r--r--   0 ian       (1000) ian       (1000)      533 2024-06-02 12:39:03.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/main.css
--rw-r--r--   0 ian       (1000) ian       (1000)      879 2024-06-02 11:48:34.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/sidebar.css
--rw-r--r--   0 ian       (1000) ian       (1000)     2003 2024-06-02 12:22:28.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/table.css
--rw-r--r--   0 ian       (1000) ian       (1000)      301 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/video.css
--rw-r--r--   0 ian       (1000) ian       (1000)     6414 2024-06-02 10:40:43.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/prism.css
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/mkdocs_ab6459/images/
--rw-r--r--   0 ian       (1000) ian       (1000)     8380 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/images/logo.svg
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/
--rw-r--r--   0 ian       (1000) ian       (1000)   207819 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.bundle.js
--rw-r--r--   0 ian       (1000) ian       (1000)    80721 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.bundle.min.js
--rw-r--r--   0 ian       (1000) ian       (1000)   135829 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.esm.js
--rw-r--r--   0 ian       (1000) ian       (1000)    73935 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.esm.min.js
--rw-r--r--   0 ian       (1000) ian       (1000)   145401 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.js
--rw-r--r--   0 ian       (1000) ian       (1000)    60635 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.min.js
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/custom/
--rw-r--r--   0 ian       (1000) ian       (1000)      499 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/custom/collapse_state.js
--rw-r--r--   0 ian       (1000) ian       (1000)      528 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/custom/darkmode.js
--rw-r--r--   0 ian       (1000) ian       (1000)    64049 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/prism.js
--rw-r--r--   0 ian       (1000) ian       (1000)     7503 2024-06-02 12:07:46.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/main.html
--rw-r--r--   0 ian       (1000) ian       (1000)       26 2024-06-03 07:47:24.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459/mkdocs_theme.yml
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)      432 2024-06-03 08:22:28.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)     1848 2024-06-03 08:22:28.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 08:22:28.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       39 2024-06-03 08:22:28.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 07:51:23.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/not-zip-safe
--rw-r--r--   0 ian       (1000) ian       (1000)        7 2024-06-03 08:22:28.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       14 2024-06-03 08:22:28.000000 mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/top_level.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       38 2024-06-03 08:22:28.335078 mkdocs_ab6459-0.1.4/setup.cfg
--rw-r--r--   0 ian       (1000) ian       (1000)      837 2024-06-03 08:22:22.000000 mkdocs_ab6459-0.1.4/setup.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/
+-rw-r--r--   0 ian       (1000) ian       (1000)      171 2024-06-03 08:11:18.000000 mkdocs_ab6459-0.1.5/MANIFEST.in
+-rw-r--r--   0 ian       (1000) ian       (1000)      432 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 07:48:26.000000 mkdocs_ab6459-0.1.5/README.md
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.350088 mkdocs_ab6459-0.1.5/mkdocs_ab6459/
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-03 08:04:03.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/__init__.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/
+-rw-r--r--   0 ian       (1000) ian       (1000)    70329 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    51795 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.min.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    70403 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    51870 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    12065 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    10126 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.min.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    12058 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    10198 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 ian       (1000) ian       (1000)   107823 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    85352 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.min.css
+-rw-r--r--   0 ian       (1000) ian       (1000)   107691 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 ian       (1000) ian       (1000)    85281 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 ian       (1000) ian       (1000)   281046 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.css
+-rw-r--r--   0 ian       (1000) ian       (1000)   232803 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.min.css
+-rw-r--r--   0 ian       (1000) ian       (1000)   280259 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.rtl.css
+-rw-r--r--   0 ian       (1000) ian       (1000)   232911 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.rtl.min.css
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/
+-rw-r--r--   0 ian       (1000) ian       (1000)     3339 2024-06-03 11:57:01.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/admonition.css
+-rw-r--r--   0 ian       (1000) ian       (1000)     3971 2024-06-03 08:21:21.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/button.css
+-rw-r--r--   0 ian       (1000) ian       (1000)     1201 2024-06-02 11:45:34.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/code.css
+-rw-r--r--   0 ian       (1000) ian       (1000)     1986 2024-06-02 11:07:03.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/diagrams.css
+-rw-r--r--   0 ian       (1000) ian       (1000)       53 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/footer.css
+-rw-r--r--   0 ian       (1000) ian       (1000)      238 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/header.css
+-rw-r--r--   0 ian       (1000) ian       (1000)      781 2024-06-03 08:51:12.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/headings.css
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2024-06-02 12:40:59.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/listings.css
+-rw-r--r--   0 ian       (1000) ian       (1000)      616 2024-06-03 11:05:27.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/main.css
+-rw-r--r--   0 ian       (1000) ian       (1000)      879 2024-06-02 11:48:34.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/sidebar.css
+-rw-r--r--   0 ian       (1000) ian       (1000)     2003 2024-06-02 12:22:28.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/table.css
+-rw-r--r--   0 ian       (1000) ian       (1000)      301 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/video.css
+-rw-r--r--   0 ian       (1000) ian       (1000)     6414 2024-06-02 10:40:43.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/prism.css
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/mkdocs_ab6459/images/
+-rw-r--r--   0 ian       (1000) ian       (1000)     8380 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/images/logo.svg
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/
+-rw-r--r--   0 ian       (1000) ian       (1000)   207819 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.bundle.js
+-rw-r--r--   0 ian       (1000) ian       (1000)    80721 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.bundle.min.js
+-rw-r--r--   0 ian       (1000) ian       (1000)   135829 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.esm.js
+-rw-r--r--   0 ian       (1000) ian       (1000)    73935 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.esm.min.js
+-rw-r--r--   0 ian       (1000) ian       (1000)   145401 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.js
+-rw-r--r--   0 ian       (1000) ian       (1000)    60635 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.min.js
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/custom/
+-rw-r--r--   0 ian       (1000) ian       (1000)     1292 2024-06-03 11:55:01.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/custom/check_stata.js
+-rw-r--r--   0 ian       (1000) ian       (1000)     1254 2024-06-03 10:20:53.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/custom/collapse_state.js
+-rw-r--r--   0 ian       (1000) ian       (1000)      528 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/custom/darkmode.js
+-rw-r--r--   0 ian       (1000) ian       (1000)    64049 2024-06-02 10:33:26.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/prism.js
+-rw-r--r--   0 ian       (1000) ian       (1000)     8734 2024-06-03 11:57:28.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/main.html
+-rw-r--r--   0 ian       (1000) ian       (1000)       26 2024-06-03 07:47:24.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459/mkdocs_theme.yml
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)      432 2024-06-03 12:03:49.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)     1887 2024-06-03 12:03:49.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 12:03:49.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/dependency_links.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       39 2024-06-03 12:03:49.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/entry_points.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2024-06-03 07:51:23.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/not-zip-safe
+-rw-r--r--   0 ian       (1000) ian       (1000)        7 2024-06-03 12:03:49.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/requires.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       14 2024-06-03 12:03:49.000000 mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/top_level.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       38 2024-06-03 12:03:49.359254 mkdocs_ab6459-0.1.5/setup.cfg
+-rw-r--r--   0 ian       (1000) ian       (1000)      837 2024-06-03 12:03:46.000000 mkdocs_ab6459-0.1.5/setup.py
```

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.rtl.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-grid.rtl.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.rtl.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-reboot.rtl.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.rtl.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap-utilities.rtl.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.rtl.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/bootstrap.rtl.min.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/admonition.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/admonition.css`

 * *Files 22% similar despite different names*

```diff
@@ -61,8 +61,80 @@
     margin: 0;
     padding: 0.5rem 0.75rem;
 }
 
 summary + p {
     margin: 0;
     padding: 0.5rem 0.75rem;
+}
+
+/* Lab Activity Styling */
+
+.activity summary strong {
+    font-weight: 600;
+    margin-right: 0.5rem;
+}
+
+.activity summary {
+    align-items: center;
+    color: rgb(var(--bs-body-color-rgb));
+    display: inline-flex;
+    font-size: 1.35rem;
+    font-weight: lighter;
+    line-height: 0;
+    margin-bottom: 0;
+    text-align: left;
+}
+
+.activity {
+    background: rgba(var(--bs-body-color-rgb), 0.03);
+    border: var(--bs-border-width) solid var(--bs-border-color-translucent);
+    border-radius: var(--bs-border-radius-xl);
+    padding: 1rem;
+    margin-bottom: 1rem;
+    width: 100%;
+}
+
+.activity summary {
+    display: flex;
+    justify-content: start;
+    align-items: center;
+}
+
+.activity summary:after {
+    content: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='15' height='15' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='rgba%280,0,0,.5%29' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M5 14l6-6-6-6'/%3e%3c/svg%3e");
+    line-height: 0;
+    margin: 0 0 0 auto;
+    text-align: right;
+    transition: transform .35s ease;
+    transform-origin: .5em 50%;
+}
+
+.activity summary::marker {
+    content: "";
+}
+
+[open].activity summary:after {
+    transform: rotate(90deg);
+}
+
+.activity p {
+    margin: 0 0 0 0;
+    padding-left: 0;
+    padding-right: 0;
+    padding-top: 0.5rem;
+    padding-bottom: 0.5rem;
+}
+
+.activity p:last-of-type {
+    padding-bottom: 0;
+}
+
+.activity .tip summary {
+    font-size: unset !important;
+    font-weight: unset;
+}
+
+.activity .tip p {
+    margin: 0 0 0 0;
+    padding: 0.5rem;
 }
```

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/button.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/button.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/code.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/code.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/diagrams.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/diagrams.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/headings.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/headings.css`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 /*    display: inline-flex;*/
 /*    font-size: 1.45rem;*/
 /*    font-weight: 600;*/
 /*    margin-right: 0.5rem;*/
 /*}*/
 
 h2 {
+    display: inline-flex;
     font-size: 1.45rem;
     font-weight: 600;
+    margin-right: 0.25rem;
     margin-bottom: 0;
     text-align: left;
 }
 
 h3 {
     color: rgb(var(--bs-body-color-rgb));
+    display: inline-flex;
     font-size: 1.35rem;
     font-weight: lighter;
     margin-bottom: 0;
     text-align: left;
 }
 
 /*h3 {*/
```

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/main.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/main.css`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,14 @@
 
 .wrapper {
     background: rgba(var(--bs-body-color-rgb), 0.03);
     border: var(--bs-border-width) solid var(--bs-border-color-translucent);
     border-radius: var(--bs-border-radius-xl);
     padding: 1rem;
     margin-bottom: 1rem;
+}
+
+.wrapped {
+    display: flex;
+    flex-direction: row;
+    margin-bottom: 1rem;
 }
```

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/sidebar.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/sidebar.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/custom/table.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/custom/table.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/css/prism.css` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/css/prism.css`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/images/logo.svg` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.bundle.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.bundle.min.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.esm.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.esm.min.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/bootstrap.min.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/custom/darkmode.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/custom/darkmode.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/js/prism.js` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/js/prism.js`

 * *Files identical despite different names*

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459/main.html` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459/main.html`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     <link href="{{ 'css/custom/admonition.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/button.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/code.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/diagrams.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/footer.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/header.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/headings.css' | url }}" rel="stylesheet" type="text/css"/>
+    <link href="{{ 'css/custom/input.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/listings.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/main.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/sidebar.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/table.css' | url }}" rel="stylesheet" type="text/css"/>
     <link href="{{ 'css/custom/video.css' | url }}" rel="stylesheet" type="text/css"/>
     <!--- External JS --->
     <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.1/jquery.min.js"></script>
@@ -103,26 +104,27 @@
                         <span class="d-none d-sm-none d-md-none d-lg-inline-block d-xl-inline-block">{{ nav_item.title }}</span>
                     </button>
                     {% endif %}
                 </li>
                 {% endfor %}
             </ul>
         </article>
-        <article class="col-lg-10">
+        <article class="col-lg-10 pe-0">
             {{ page.content }}
         </article>
     </section>
 </main>
 
 <footer class="bg-body-secondary p-3 rounded-4 small text-center text-muted">
     Errors or Questions? Contact Ian Cornelius, <a href="mailto:ab6459@coventry.ac.uk">ab6459@coventry.ac.uk</a>
 </footer>
 
 <script src=" {{ 'js/prism.js' | url }} "></script>
 <script src=" {{ 'js/bootstrap.bundle.min.js' | url }} "></script>
+<script src=" {{ 'js/custom/check_stata.js' | url }} "></script>
 <script src=" {{ 'js/custom/collapse_state.js' | url }} "></script>
 <script src=" {{ 'js/custom/darkmode.js' | url }} "></script>
 {%- for script in config.extra_javascript %}
 {{ script | script_tag }}
 {%- endfor %}
 </body>
 <script>
@@ -134,10 +136,46 @@
         $(this).nextUntil('div.wrapper').addBack().wrapAll('<div class="wrapper">');
     })
 
     $('table').wrap(`<div id="table"><div class="table">`)
 
     $('.mermaid').wrap(`<div id="mermaid">`)
 
+    var counter = 1;
+    $('details.activity').each(function() {
+        $(this).attr('id', `task-${counter}`);
+        counter += 1;
+    });
+
+    $('details.activity > summary').each(function() {
+        $(this).prepend(`
+            <input type="checkbox" hidden />
+            <span class="me-2 badge">Not Completed</span>
+        `);
+    })
+
+    $('details.activity p:first-of-type').each(function() {
+        $(this).before(`
+            <input class="mt-2 btn btn-sm btn-success" type="button" value="Mark as Completed"/>
+        `);
+    })
+
+    var counter2 = 1;
+    $('details.activity > summary span').each(function() {
+        $(this).attr('id', `task-check-${counter2}`);
+        counter2 += 1;
+    });
+
+    var counter3 = 1;
+    $('details.activity > input[type="button"]').each(function() {
+        $(this).attr('id', `task-check-${counter3}`);
+        counter3 += 1;
+    });
+
+    var counter4 = 1;
+    $('details.activity > summary input[type="checkbox"]').each(function() {
+        $(this).attr('id', `task-check-${counter4}`);
+        counter4 += 1;
+    });
 
 </script>
 </html>
```

### Comparing `mkdocs_ab6459-0.1.4/mkdocs_ab6459.egg-info/SOURCES.txt` & `mkdocs_ab6459-0.1.5/mkdocs_ab6459.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,9 +44,10 @@
 mkdocs_ab6459/js/bootstrap.bundle.js
 mkdocs_ab6459/js/bootstrap.bundle.min.js
 mkdocs_ab6459/js/bootstrap.esm.js
 mkdocs_ab6459/js/bootstrap.esm.min.js
 mkdocs_ab6459/js/bootstrap.js
 mkdocs_ab6459/js/bootstrap.min.js
 mkdocs_ab6459/js/prism.js
+mkdocs_ab6459/js/custom/check_stata.js
 mkdocs_ab6459/js/custom/collapse_state.js
 mkdocs_ab6459/js/custom/darkmode.js
```

### Comparing `mkdocs_ab6459-0.1.4/setup.py` & `mkdocs_ab6459-0.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_desc = fh.read()
 
 setup(
     name="mkdocs_ab6459",
-    version="0.1.4",
+    version="0.1.5",
     url='https://github.coventry.ac.uk/ab6459/mkdocs_ab6459',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Topic :: Documentation',
         'Topic :: Text Processing',
     ],
     install_requires=[
```

