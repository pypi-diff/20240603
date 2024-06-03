# Comparing `tmp/create_pip-0.1.tar.gz` & `tmp/create_pip-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_pip-0.1.tar", last modified: Sat Jun  1 17:05:42 2024, max compression
+gzip compressed data, was "create_pip-0.2.tar", last modified: Mon Jun  3 03:57:36 2024, max compression
```

## Comparing `create_pip-0.1.tar` & `create_pip-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 17:05:42.859040 create_pip-0.1/
--rw-rw-rw-   0        0        0       55 2024-06-01 17:05:42.856274 create_pip-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 17:05:42.842458 create_pip-0.1/create_pip/
--rw-rw-rw-   0        0        0       29 2024-06-01 17:05:13.000000 create_pip-0.1/create_pip/__init__.py
--rw-rw-rw-   0        0        0      242 2024-06-01 17:05:15.000000 create_pip-0.1/create_pip/main.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:05:42.854766 create_pip-0.1/create_pip.egg-info/
--rw-rw-rw-   0        0        0       55 2024-06-01 17:05:42.000000 create_pip-0.1/create_pip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-06-01 17:05:42.000000 create_pip-0.1/create_pip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 17:05:42.000000 create_pip-0.1/create_pip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 17:05:42.000000 create_pip-0.1/create_pip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 17:05:42.859040 create_pip-0.1/setup.cfg
--rw-rw-rw-   0        0        0      215 2024-06-01 17:03:46.000000 create_pip-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:57:36.503070 create_pip-0.2/
+-rw-rw-rw-   0        0        0       55 2024-06-03 03:57:36.503070 create_pip-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-03 03:57:36.481560 create_pip-0.2/create_pip/
+-rw-rw-rw-   0        0        0       29 2024-06-01 17:05:13.000000 create_pip-0.2/create_pip/__init__.py
+-rw-rw-rw-   0        0        0      242 2024-06-01 17:05:15.000000 create_pip-0.2/create_pip/main.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:57:36.498698 create_pip-0.2/create_pip.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-06-03 03:57:36.000000 create_pip-0.2/create_pip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-06-03 03:57:36.000000 create_pip-0.2/create_pip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 03:57:36.000000 create_pip-0.2/create_pip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-06-03 03:57:36.000000 create_pip-0.2/create_pip.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-06-03 03:57:36.000000 create_pip-0.2/create_pip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 03:57:36.505103 create_pip-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      340 2024-06-03 03:57:22.000000 create_pip-0.2/setup.py
```

