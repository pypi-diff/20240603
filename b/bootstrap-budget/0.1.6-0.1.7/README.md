# Comparing `tmp/bootstrap-budget-0.1.6.tar.gz` & `tmp/bootstrap_budget-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrap-budget-0.1.6.tar", last modified: Sun Mar 10 23:29:21 2024, max compression
+gzip compressed data, was "bootstrap_budget-0.1.7.tar", last modified: Mon Jun  3 05:04:54 2024, max compression
```

## Comparing `bootstrap-budget-0.1.6.tar` & `bootstrap_budget-0.1.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.432624 bootstrap-budget-0.1.6/
--rw-rw-rw-   0        0        0     1104 2022-09-24 06:48:13.000000 bootstrap-budget-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      226 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1512 2024-03-10 23:29:21.431623 bootstrap-budget-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-11-05 03:52:44.000000 bootstrap-budget-0.1.6/README.md
--rw-rw-rw-   0        0        0     1826 2024-03-10 23:28:54.000000 bootstrap-budget-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-10 23:29:21.432624 bootstrap-budget-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.373621 bootstrap-budget-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.383622 bootstrap-budget-0.1.6/src/bootstrap_budget/
--rw-rw-rw-   0        0        0     2509 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/__init__.py
--rw-rw-rw-   0        0        0      624 2024-03-08 21:20:46.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/account.py
--rw-rw-rw-   0        0        0     1203 2024-03-10 03:37:17.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/admin.py
--rw-rw-rw-   0        0        0     3714 2024-03-10 03:31:20.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/auth.py
--rw-rw-rw-   0        0        0      605 2024-03-08 21:22:49.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/budget.py
--rw-rw-rw-   0        0        0      659 2024-03-08 21:22:54.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/budget_item.py
--rw-rw-rw-   0        0        0    14183 2024-03-04 03:26:36.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/cli.py
--rw-rw-rw-   0        0        0      433 2024-03-08 21:21:47.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/dashboard.py
--rw-rw-rw-   0        0        0     8210 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/entities.py
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.398621 bootstrap-budget-0.1.6/src/bootstrap_budget/sample_data/
--rw-rw-rw-   0        0        0      100 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/sample_data/__init__.py
--rw-rw-rw-   0        0        0      193 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/sample_data/account.csv
--rw-rw-rw-   0        0        0       99 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/sample_data/budget.csv
--rw-rw-rw-   0        0        0      486 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/sample_data/budget_item.csv
--rw-rw-rw-   0        0        0    20631 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/sample_data/transaction.csv
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.406621 bootstrap-budget-0.1.6/src/bootstrap_budget/static/
--rw-rw-rw-   0        0        0    10076 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    37997 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     8957 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/apple-touch-icon.png
--rw-rw-rw-   0        0        0    85875 2024-03-09 03:24:19.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/bootstrap-icons.min.css
--rw-rw-rw-   0        0        0    80669 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   232953 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/bootstrap.min.css
--rw-rw-rw-   0        0        0      550 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/favicon-16x16.png
--rw-rw-rw-   0        0        0     1112 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/favicon-32x32.png
--rw-rw-rw-   0        0        0    15406 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/favicon.ico
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.411622 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/
--rw-rw-rw-   0        0        0   176032 2024-03-09 03:24:19.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   130396 2024-03-09 03:24:19.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/bootstrap-icons.woff2
--rw-rw-rw-   0        0        0    20127 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   109025 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.419621 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/
--rw-rw-rw-   0        0        0        0 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-hi-res-v2.png
--rw-rw-rw-   0        0        0   172694 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.jpeg
--rw-rw-rw-   0        0        0    15532 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.pdf
--rw-rw-rw-   0        0        0    28312 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.png
--rw-rw-rw-   0        0        0    34053 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.svg
--rw-rw-rw-   0        0        0    15270 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.png
--rw-rw-rw-   0        0        0    63938 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.xcf
--rw-rw-rw-   0        0        0    47699 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-hi-res-v2.png
--rw-rw-rw-   0        0        0    55131 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.jpeg
--rw-rw-rw-   0        0        0     5964 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.pdf
--rw-rw-rw-   0        0        0    13388 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.svg
--rw-rw-rw-   0        0        0     8700 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-web-v2.png
--rw-rw-rw-   0        0        0    12314 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-v1.png
--rw-rw-rw-   0        0        0     2749 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-v1.svg
--rw-rw-rw-   0        0        0     1054 2024-03-10 21:05:51.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/login.css
--rw-rw-rw-   0        0        0      118 2024-03-10 22:49:39.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/main.css
--rw-rw-rw-   0        0        0      263 2024-03-03 00:23:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/static/site.webmanifest
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.425623 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/
--rw-rw-rw-   0        0        0      924 2024-03-10 22:52:47.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/account.html
--rw-rw-rw-   0        0        0      724 2024-03-10 23:26:13.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/admin.html
--rw-rw-rw-   0        0        0    13558 2024-03-10 23:23:26.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/base.html
--rw-rw-rw-   0        0        0      982 2024-03-10 23:25:19.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/budget-item.html
--rw-rw-rw-   0        0        0      984 2024-03-10 23:25:11.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/budget.html
--rw-rw-rw-   0        0        0      496 2024-03-10 23:25:11.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/dashboard.html
--rw-rw-rw-   0        0        0     3620 2024-03-09 22:22:16.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/login.html
--rw-rw-rw-   0        0        0      496 2024-03-10 23:25:30.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/transaction.html
--rw-rw-rw-   0        0        0      379 2024-03-10 23:25:57.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/templates/user_admin.html
--rw-rw-rw-   0        0        0      440 2024-03-08 21:23:06.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/transaction.py
--rw-rw-rw-   0        0        0     1826 2024-03-10 23:21:35.000000 bootstrap-budget-0.1.6/src/bootstrap_budget/user.py
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.430621 bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/
--rw-rw-rw-   0        0        0     1512 2024-03-10 23:29:21.000000 bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3253 2024-03-10 23:29:21.000000 bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 23:29:21.000000 bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-03-10 23:29:21.000000 bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      165 2024-03-10 23:29:21.000000 bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-10 23:29:21.000000 bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-10 23:29:21.429624 bootstrap-budget-0.1.6/tests/
--rw-rw-rw-   0        0        0      539 2023-11-11 02:01:35.000000 bootstrap-budget-0.1.6/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.563794 bootstrap_budget-0.1.7/
+-rw-rw-rw-   0        0        0     1104 2022-09-24 06:48:13.000000 bootstrap_budget-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      226 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3298 2024-06-03 05:04:54.563794 bootstrap_budget-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1887 2024-06-03 05:04:21.000000 bootstrap_budget-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1826 2024-05-28 05:13:56.000000 bootstrap_budget-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 05:04:54.563794 bootstrap_budget-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.482776 bootstrap_budget-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.491777 bootstrap_budget-0.1.7/src/bootstrap_budget/
+-rw-rw-rw-   0        0        0     2512 2024-05-14 04:00:53.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/__init__.py
+-rw-rw-rw-   0        0        0     3024 2024-06-03 03:23:04.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/account.py
+-rw-rw-rw-   0        0        0     1165 2024-03-11 02:06:28.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/admin.py
+-rw-rw-rw-   0        0        0     3677 2024-03-11 02:06:37.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/auth.py
+-rw-rw-rw-   0        0        0     2661 2024-06-03 03:26:01.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/budget.py
+-rw-rw-rw-   0        0        0     3003 2024-06-03 04:23:18.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/budget_item.py
+-rw-rw-rw-   0        0        0    14669 2024-05-27 04:41:17.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/cli.py
+-rw-rw-rw-   0        0        0      396 2024-03-11 02:06:52.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/dashboard.py
+-rw-rw-rw-   0        0        0     8274 2024-06-02 23:53:38.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/entities.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.511776 bootstrap_budget-0.1.7/src/bootstrap_budget/sample_data/
+-rw-rw-rw-   0        0        0      100 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/sample_data/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/sample_data/account.csv
+-rw-rw-rw-   0        0        0       99 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/sample_data/budget.csv
+-rw-rw-rw-   0        0        0      486 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/sample_data/budget_item.csv
+-rw-rw-rw-   0        0        0    20631 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/sample_data/transaction.csv
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.518775 bootstrap_budget-0.1.7/src/bootstrap_budget/static/
+-rw-rw-rw-   0        0        0    10076 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    37997 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     8957 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/apple-touch-icon.png
+-rw-rw-rw-   0        0        0    85875 2024-03-09 03:24:19.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/bootstrap-icons.min.css
+-rw-rw-rw-   0        0        0    80669 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   232953 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/bootstrap.min.css
+-rw-rw-rw-   0        0        0      550 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1112 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/favicon-32x32.png
+-rw-rw-rw-   0        0        0    15406 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/favicon.ico
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.523775 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/
+-rw-rw-rw-   0        0        0   176032 2024-03-09 03:24:19.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   130396 2024-03-09 03:24:19.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/bootstrap-icons.woff2
+-rw-rw-rw-   0        0        0    20127 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   109025 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.531775 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/
+-rw-rw-rw-   0        0        0        0 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-hi-res-v2.png
+-rw-rw-rw-   0        0        0   172694 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.jpeg
+-rw-rw-rw-   0        0        0    15532 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.pdf
+-rw-rw-rw-   0        0        0    28312 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.png
+-rw-rw-rw-   0        0        0    34053 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.svg
+-rw-rw-rw-   0        0        0    15270 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.png
+-rw-rw-rw-   0        0        0    63938 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.xcf
+-rw-rw-rw-   0        0        0    47699 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-hi-res-v2.png
+-rw-rw-rw-   0        0        0    55131 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.jpeg
+-rw-rw-rw-   0        0        0     5964 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.pdf
+-rw-rw-rw-   0        0        0    13388 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.svg
+-rw-rw-rw-   0        0        0     8700 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-web-v2.png
+-rw-rw-rw-   0        0        0    12314 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-v1.png
+-rw-rw-rw-   0        0        0     2749 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-v1.svg
+-rw-rw-rw-   0        0        0     1054 2024-03-10 21:05:51.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/login.css
+-rw-rw-rw-   0        0        0       76 2024-03-13 04:12:06.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/main.css
+-rw-rw-rw-   0        0        0      263 2024-03-03 00:23:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/static/site.webmanifest
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.557794 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/
+-rw-rw-rw-   0        0        0     5517 2024-06-03 04:37:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/account.html
+-rw-rw-rw-   0        0        0      724 2024-03-10 23:26:13.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/admin.html
+-rw-rw-rw-   0        0        0    12808 2024-06-03 04:40:15.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/base.html
+-rw-rw-rw-   0        0        0     5577 2024-06-03 04:38:33.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/budget-item.html
+-rw-rw-rw-   0        0        0     5054 2024-06-03 04:38:20.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/budget.html
+-rw-rw-rw-   0        0        0      496 2024-03-10 23:25:11.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/dashboard.html
+-rw-rw-rw-   0        0        0     3620 2024-03-09 22:22:16.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/login.html
+-rw-rw-rw-   0        0        0      496 2024-03-10 23:25:30.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/transaction.html
+-rw-rw-rw-   0        0        0      379 2024-03-10 23:25:57.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/templates/user_admin.html
+-rw-rw-rw-   0        0        0      403 2024-03-11 02:07:00.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/transaction.py
+-rw-rw-rw-   0        0        0     2547 2024-06-03 02:59:17.000000 bootstrap_budget-0.1.7/src/bootstrap_budget/user.py
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.562794 bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/
+-rw-rw-rw-   0        0        0     3298 2024-06-03 05:04:54.000000 bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3253 2024-06-03 05:04:54.000000 bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 05:04:54.000000 bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-06-03 05:04:54.000000 bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      165 2024-06-03 05:04:54.000000 bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-06-03 05:04:54.000000 bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 05:04:54.561797 bootstrap_budget-0.1.7/tests/
+-rw-rw-rw-   0        0        0      539 2023-11-11 02:01:35.000000 bootstrap_budget-0.1.7/tests/test_version.py
```

### Comparing `bootstrap-budget-0.1.6/LICENSE` & `bootstrap_budget-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/pyproject.toml` & `bootstrap_budget-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='bootstrap-budget'
-version='0.1.6'
+version='0.1.7'
 authors = [
     {name = 'forgineer', email = 'blake.phillips86@gmail.com'},
 ]
 description='A simple financial application to help you pull your budget up by its bootstraps.'
 readme = 'README.md' # Long description
 license = {text = 'MIT License'}
 requires-python = ">=3.8"
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/__init__.py` & `bootstrap_budget-0.1.7/src/bootstrap_budget/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from flask import Flask
 from logging.config import dictConfig
 from pony.flask import Pony
 
 # Define database and entities (Pony ORM)
 from .entities import (
-    db, User, Config, Budget, UserBudget, BudgetItem, Account, Transaction
+    db, User, Config, Budget, BudgetAccount, BudgetItem, Account, Transaction
 )
 
 
 # Set Bootstrap Budget globals
 __admin__: str = 'admin'
 __version__: str = importlib.metadata.version('bootstrap_budget')
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/admin.py` & `bootstrap_budget-0.1.7/src/bootstrap_budget/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 )
 from werkzeug.security import check_password_hash
 
 # Import bootstrap-budget blueprints/modules/classes/functions
 from .auth import login_required, admin_only
 
 
-# Define as a Flask blueprint: Admin
 bp = Blueprint('admin', __name__, url_prefix='/admin')
 
 
 # TODO: Enable user registration
 # - Adds a link for self registration on the login page
 # - Otherwise users can only be added through the admin console
 # - Default is unchecked
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/auth.py` & `bootstrap_budget-0.1.7/src/bootstrap_budget/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from werkzeug.security import check_password_hash
 
 # Import bootstrap-budget blueprints/modules/classes/functions
 from . import __admin__
 from .entities import User
 
 
-# Define as a Flask blueprint: Auth
 bp = Blueprint('auth', __name__, url_prefix='/auth')
 
 
 def login_required(view) -> Any:
     """
     Decorator for initiating a required login to a view or resource
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/cli.py` & `bootstrap_budget-0.1.7/src/bootstrap_budget/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from bootstrap_budget import __admin__, __version__, sample_data
 from datetime import datetime
 from pony import orm
 from werkzeug.security import generate_password_hash
 
 # Define database and entities (Pony ORM)
 from .entities import (
-    db as database, User, Config, Budget, UserBudget, BudgetItem, Account, Transaction
+    db as database, User, Config, Budget, BudgetAccount, BudgetItem, Account, Transaction
 )
 
 # Define Bootstrap Budget configuration file
 CONFIG_FILE: str = 'config.py'
 
 # Define standard provider and filename for SQLite database integration
 SQLITE_PROVIDER: str = 'sqlite'
@@ -210,14 +210,24 @@
     accounts_lookup: dict = {}
     budget_items_lookup: dict = {}
 
     accounts = orm.select(a for a in db_entity.Account if a.user_id == user)
     for account in accounts:
         accounts_lookup[account.name] = account.id
 
+    # Insert BUDGET_ACCOUNT records
+    budgets = orm.select(b for b in db_entity.Budget if b.user_id == user)
+    for budget in budgets:
+        for account in accounts:
+            db_entity.BudgetAccount(created_dt_tm=datetime.now(),
+                                    updated_dt_tm=datetime.now(),
+                                    user_id=user.id,
+                                    account_id=account.id,
+                                    budget_id=budget.id)
+
     budget_items = orm.select(bi for bi in db_entity.BudgetItem if bi.user_id == user)
     for budget_item in budget_items:
         budget_items_lookup[budget_item.name] = budget_item.id
 
     # Insert TRANSACTION records
     with open(transaction_csv_path, mode='r') as csv_file:
         transaction_csv: csv.DictReader = csv.DictReader(csv_file)
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/entities.py` & `bootstrap_budget-0.1.7/src/bootstrap_budget/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,37 +24,37 @@
     hash = orm.Required(str)
     created_dt_tm = orm.Required(datetime)
     updated_dt_tm = orm.Required(datetime)
     is_active = orm.Required(bool, default=True)
     accounts = orm.Set('Account')
     configs = orm.Set('Config')
     budgets = orm.Set('Budget')
+    budget_accounts = orm.Set('BudgetAccount')
     budget_items = orm.Set('BudgetItem')
     transactions = orm.Set('Transaction')
-    user_budgets = orm.Set('UserBudget')
 
 
 """
 CREATE TABLE "USER" (
-    "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-    "last_name" TEXT,
-    "first_name" TEXT,
-    "middle_name" TEXT,
-    "username" TEXT UNIQUE NOT NULL,
-    "address_line_1" TEXT,
-    "address_line_2" TEXT,
-    "city" TEXT,
-    "state" TEXT,
-    "zipcode" TEXT,
-    "email" TEXT,
-    "phone_number" TEXT,
-    "hash" TEXT NOT NULL,
-    "created_dt_tm" DATETIME NOT NULL,
-    "updated_dt_tm" DATETIME NOT NULL,
-    "is_active" BOOLEAN NOT NULL
+  "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+  "last_name" TEXT,
+  "first_name" TEXT,
+  "middle_name" TEXT,
+  "username" TEXT UNIQUE NOT NULL,
+  "address_line_1" TEXT,
+  "address_line_2" TEXT,
+  "city" TEXT,
+  "state" TEXT,
+  "zipcode" TEXT,
+  "email" TEXT,
+  "phone_number" TEXT,
+  "hash" TEXT NOT NULL,
+  "created_dt_tm" DATETIME NOT NULL,
+  "updated_dt_tm" DATETIME NOT NULL,
+  "is_active" BOOLEAN NOT NULL
 );
 """
 
 
 class Config(db.Entity):
     _table_ = 'CONFIG'
 
@@ -68,24 +68,24 @@
     is_active = orm.Required(bool, default=True)
     user_id = orm.Required(User)
     orm.composite_key(name, user_id)
 
 
 """
 CREATE TABLE "CONFIG" (
-    "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-    "name" TEXT UNIQUE NOT NULL,
-    "description" TEXT,
-    "config_value" TEXT,
-    "config_value_type" INTEGER NOT NULL,
-    "created_dt_tm" DATETIME NOT NULL,
-    "updated_dt_tm" DATETIME NOT NULL,
-    "is_active" BOOLEAN NOT NULL,
-    "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
-    CONSTRAINT "unq_config__name_user_id" UNIQUE ("name", "user_id")
+  "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+  "name" TEXT UNIQUE NOT NULL,
+  "description" TEXT,
+  "config_value" TEXT,
+  "config_value_type" INTEGER NOT NULL,
+  "created_dt_tm" DATETIME NOT NULL,
+  "updated_dt_tm" DATETIME NOT NULL,
+  "is_active" BOOLEAN NOT NULL,
+  "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
+  CONSTRAINT "unq_config__name_user_id" UNIQUE ("name", "user_id")
 );
 
 CREATE INDEX "idx_config__user_id" ON "CONFIG" ("user_id");
 """
 
 
 class Budget(db.Entity):
@@ -95,60 +95,61 @@
     name = orm.Required(str)
     description = orm.Optional(str, nullable=True)
     budget_year = orm.Required(int)
     created_dt_tm = orm.Required(datetime)
     updated_dt_tm = orm.Required(datetime)
     is_active = orm.Required(bool, default=True)
     user_id = orm.Required(User)
-    user_budgets = orm.Set('UserBudget')
+    budget_accounts = orm.Set('BudgetAccount')
     orm.composite_key(name, user_id)
 
 
 """
 CREATE TABLE "BUDGET" (
-    "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-    "name" TEXT NOT NULL,
-    "description" TEXT,
-    "budget_year" INTEGER NOT NULL,
-    "created_dt_tm" DATETIME NOT NULL,
-    "updated_dt_tm" DATETIME NOT NULL,
-    "is_active" BOOLEAN NOT NULL,
-    "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
-    CONSTRAINT "unq_budget__name_user_id" UNIQUE ("name", "user_id")
+  "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+  "name" TEXT NOT NULL,
+  "description" TEXT,
+  "budget_year" INTEGER NOT NULL,
+  "created_dt_tm" DATETIME NOT NULL,
+  "updated_dt_tm" DATETIME NOT NULL,
+  "is_active" BOOLEAN NOT NULL,
+  "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
+  CONSTRAINT "unq_budget__name_user_id" UNIQUE ("name", "user_id")
 );
 
 CREATE INDEX "idx_budget__user_id" ON "BUDGET" ("user_id");
 """
 
 
-class UserBudget(db.Entity):
-    _table_ = 'USER_BUDGET'
+class BudgetAccount(db.Entity):
+    _table_ = 'BUDGET_ACCOUNT'
 
     id = orm.PrimaryKey(int, auto=True)
-    permissions = orm.Required(int)
     created_dt_tm = orm.Required(datetime)
     updated_dt_tm = orm.Required(datetime)
     is_active = orm.Required(bool, default=True)
     user_id = orm.Required(User)
+    account_id = orm.Required('Account')
     budget_id = orm.Required(Budget)
 
 
 """
-CREATE TABLE "USER_BUDGET" (
-    "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-    "permissions" INTEGER NOT NULL,
-    "created_dt_tm" DATETIME NOT NULL,
-    "updated_dt_tm" DATETIME NOT NULL,
-    "is_active" BOOLEAN NOT NULL,
-    "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
-    "budget_id" INTEGER NOT NULL REFERENCES "BUDGET" ("id") ON DELETE CASCADE
+CREATE TABLE "BUDGET_ACCOUNT" (
+  "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+  "created_dt_tm" DATETIME NOT NULL,
+  "updated_dt_tm" DATETIME NOT NULL,
+  "is_active" BOOLEAN NOT NULL,
+  "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
+  "account_id" INTEGER NOT NULL REFERENCES "ACCOUNT" ("id") ON DELETE CASCADE,
+  "budget_id" INTEGER NOT NULL REFERENCES "BUDGET" ("id") ON DELETE CASCADE
 );
 
-CREATE INDEX "idx_user_budget__budget_id" ON "USER_BUDGET" ("budget_id");
-CREATE INDEX "idx_user_budget__user_id" ON "USER_BUDGET" ("user_id");
+CREATE INDEX "idx_budget_account__account_id" ON "BUDGET_ACCOUNT" ("account_id");
+CREATE INDEX "idx_budget_account__budget_id" ON "BUDGET_ACCOUNT" ("budget_id");
+CREATE INDEX "idx_budget_account__user_id" ON "BUDGET_ACCOUNT" ("user_id");
 """
 
 
 class BudgetItem(db.Entity):
     _table_ = 'BUDGET_ITEM'
 
     id = orm.PrimaryKey(int, auto=True)
@@ -162,24 +163,24 @@
     user_id = orm.Required(User)
     transactions = orm.Set('Transaction')
     orm.composite_key(name, user_id)
 
 
 """
 CREATE TABLE "BUDGET_ITEM" (
-    "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-    "name" TEXT NOT NULL,
-    "description" TEXT,
-    "budget_amount" REAL NOT NULL,
-    "sequence_order" INTEGER NOT NULL,
-    "created_dt_tm" DATETIME NOT NULL,
-    "updated_dt_tm" DATETIME NOT NULL,
-    "is_active" BOOLEAN NOT NULL,
-    "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
-    CONSTRAINT "unq_budget_item__name_user_id" UNIQUE ("name", "user_id")
+  "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+  "name" TEXT NOT NULL,
+  "description" TEXT,
+  "budget_amount" REAL NOT NULL,
+  "sequence_order" INTEGER NOT NULL,
+  "created_dt_tm" DATETIME NOT NULL,
+  "updated_dt_tm" DATETIME NOT NULL,
+  "is_active" BOOLEAN NOT NULL,
+  "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
+  CONSTRAINT "unq_budget_item__name_user_id" UNIQUE ("name", "user_id")
 );
 
 CREATE INDEX "idx_budget_item__user_id" ON "BUDGET_ITEM" ("user_id");
 """
 
 
 class Account(db.Entity):
@@ -191,31 +192,32 @@
     account_number = orm.Optional(str, nullable=True)
     account_route_nbr = orm.Optional(str, nullable=True)
     opening_amount = orm.Required(float, default=0)
     created_dt_tm = orm.Required(datetime)
     updated_dt_tm = orm.Required(datetime)
     is_active = orm.Required(bool, default=True)
     user_id = orm.Required(User)
+    budget_accounts = orm.Set(BudgetAccount)
     transactions = orm.Set('Transaction')
     orm.composite_key(name, user_id)
 
 
 """
 CREATE TABLE "ACCOUNT" (
-    "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-    "name" TEXT NOT NULL,
-    "description" TEXT,
-    "account_number" TEXT,
-    "account_route_nbr" TEXT,
-    "opening_amount" REAL NOT NULL,
-    "created_dt_tm" DATETIME NOT NULL,
-    "updated_dt_tm" DATETIME NOT NULL,
-    "is_active" BOOLEAN NOT NULL,
-    "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
-    CONSTRAINT "unq_account__name_user_id" UNIQUE ("name", "user_id")
+  "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+  "name" TEXT NOT NULL,
+  "description" TEXT,
+  "account_number" TEXT,
+  "account_route_nbr" TEXT,
+  "opening_amount" REAL NOT NULL,
+  "created_dt_tm" DATETIME NOT NULL,
+  "updated_dt_tm" DATETIME NOT NULL,
+  "is_active" BOOLEAN NOT NULL,
+  "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
+  CONSTRAINT "unq_account__name_user_id" UNIQUE ("name", "user_id")
 );
 
 CREATE INDEX "idx_account__user_id" ON "ACCOUNT" ("user_id");
 """
 
 
 class Transaction(db.Entity):
@@ -232,24 +234,24 @@
     user_id = orm.Required(User)
     account_id = orm.Required(Account)
     budget_item_id = orm.Required(BudgetItem)
 
 
 """
 CREATE TABLE "TRANSACTION" (
-    "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-    "description" TEXT,
-    "amount" REAL NOT NULL,
-    "transaction_dt_tm" DATETIME NOT NULL,
-    "note" TEXT,
-    "created_dt_tm" DATETIME NOT NULL,
-    "updated_dt_tm" DATETIME,
-    "is_active" BOOLEAN NOT NULL,
-    "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
-    "account_id" INTEGER NOT NULL REFERENCES "ACCOUNT" ("id") ON DELETE CASCADE,
-    "budget_item_id" INTEGER NOT NULL REFERENCES "BUDGET_ITEM" ("id") ON DELETE CASCADE
+  "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+  "description" TEXT,
+  "amount" REAL NOT NULL,
+  "transaction_dt_tm" DATETIME NOT NULL,
+  "note" TEXT,
+  "created_dt_tm" DATETIME NOT NULL,
+  "updated_dt_tm" DATETIME,
+  "is_active" BOOLEAN NOT NULL,
+  "user_id" INTEGER NOT NULL REFERENCES "USER" ("id") ON DELETE CASCADE,
+  "account_id" INTEGER NOT NULL REFERENCES "ACCOUNT" ("id") ON DELETE CASCADE,
+  "budget_item_id" INTEGER NOT NULL REFERENCES "BUDGET_ITEM" ("id") ON DELETE CASCADE
 );
 
 CREATE INDEX "idx_transaction__account_id" ON "TRANSACTION" ("account_id");
 CREATE INDEX "idx_transaction__budget_item_id" ON "TRANSACTION" ("budget_item_id");
 CREATE INDEX "idx_transaction__user_id" ON "TRANSACTION" ("user_id");
 """
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/sample_data/transaction.csv` & `bootstrap_budget-0.1.7/src/bootstrap_budget/sample_data/transaction.csv`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/android-chrome-192x192.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/android-chrome-512x512.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/apple-touch-icon.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/bootstrap-icons.min.css` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/bootstrap.bundle.min.js` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/bootstrap.min.css` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/favicon-16x16.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/favicon-32x32.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/favicon.ico` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/bootstrap-icons.woff` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/bootstrap-icons.woff2` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.eot` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.svg` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.ttf` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff2` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.jpeg` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.jpeg`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.pdf` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.pdf`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.svg` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-000000-v2.svg`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.xcf` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-ffffff-v2.xcf`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-hi-res-v2.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-hi-res-v2.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.jpeg` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.jpeg`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.pdf` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.pdf`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.svg` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-v2.svg`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-web-v2.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-mini-000000-web-v2.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-v1.png` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-v1.png`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/images/bootstrap-logo-v1.svg` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/images/bootstrap-logo-v1.svg`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/static/login.css` & `bootstrap_budget-0.1.7/src/bootstrap_budget/static/login.css`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/templates/admin.html` & `bootstrap_budget-0.1.7/src/bootstrap_budget/templates/admin.html`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/templates/base.html` & `bootstrap_budget-0.1.7/src/bootstrap_budget/templates/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+{% macro add_form_input(id, label, value='', type='text', required=False, number_step='1', placeholder='') -%}
+<div class="mb-2">
+    {% if type != 'hidden' %}
+    <label for="{{ id }}" class="col-form-label"><strong>{{ label }}</strong></label>
+    {% endif %}
+    <input type="{{ type }}" class="form-control" name="{{ id }}" id="{{ id }}" {% if type == 'number' -%}step="{{ number_step }}"{%- endif %} placeholder="{% if placeholder is not none -%} {{ placeholder }} {%- endif %}" value="{% if value is not none -%} {{ value }} {%- endif %}"{% if required -%} required{%- endif %}>
+</div>
+{%- endmacro %}
 <!DOCTYPE html>
 <html lang="en">
     <head>
         <meta charset="utf-8" />
         <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no" />
 
         <title>Bootstrap Budget!</title>
@@ -84,15 +92,15 @@
                         <li class="nav-item dropdown">
                             <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown">
                                 <i class="bi bi-person-fill"></i> {{ user.username }}
                             </a>
                             <ul class="dropdown-menu dropdown-menu-dark">
                                 {% if edit %}
                                 <li>
-                                    <a class="dropdown-item" href="#" data-bs-toggle="modal" data-bs-target="#editProfileModal" title="Edit Profile">
+                                    <a class="dropdown-item" href="#" data-bs-toggle="modal" data-bs-target="#updateProfileModal" title="Edit Profile">
                                         <i class="bi bi-person-fill-gear"></i> Edit Profile
                                     </a>
                                 </li>
                                 {% endif %}
                                 {% if reset %}
                                 <li>
                                     <a class="dropdown-item" href="#" data-bs-toggle="modal" data-bs-target="#resetPasswordModal" title="Reset Password">
@@ -111,15 +119,15 @@
                         </li>
                         {%- endmacro %}
                         {% block nav_items %}{% endblock %}
                     </ul>
                 </div>
             </div>
         </nav>
-        <div class="flash-alerts">
+        <div class="fixed-bottom">
         {% with messages = get_flashed_messages(with_categories=true) %}
             {% if messages %}
                 {% for category, message in messages %}
                     {% if category == 'error' %}
                     <div class="alert alert-danger alert-dismissible fade show" role="alert">
                         <i class="bi bi-exclamation-triangle-fill"></i> {{ message }}
                         <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
@@ -136,42 +144,33 @@
                     </div>
                     {% endif %}
                 {% endfor %}
             {% endif %}
         {% endwith %}
         </div>
         {% macro add_edit_profile_modal() -%}
-        <div class="modal fade" id="editProfileModal" tabindex="-1">
+        <div class="modal fade" id="updateProfileModal" tabindex="-1">
             <div class="modal-dialog modal-dialog-centered">
                 <div class="modal-content">
                     <div class="modal-header">
-                        <h5 class="modal-title">Edit Profile</h5>
+                        <h5 class="modal-title">Edit User Profile</h5>
                         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                     </div>
                     <div class="modal-body">
                         <form id="user_update" action="{{ url_for('user.update') }}" method="post">
-                            {% macro user_profile_input(id, label, value='', type='text') -%}
-                            <div class="mb-2">
-                                {% if type != 'hidden' %}
-                                <label for="{{ id }}" class="col-form-label"><strong>{{ label }}</strong></label>
-                                {% endif %}
-                                <input type="{{ type }}" class="form-control" name="{{ id }}" id="{{ id }}" value="{% if value is not none -%} {{ value }} {%- endif %}">
-                            </div>
-                            {%- endmacro %}
-
-                            {{ user_profile_input(id='first_name', label='First Name:', value=user.first_name) }}
-                            {{ user_profile_input(id='middle_name', label='Middle Name:', value=user.middle_name) }}
-                            {{ user_profile_input(id='last_name', label='Last Name:', value=user.last_name) }}
-                            {{ user_profile_input(id='address_line_1', label='Address line 1:', value=user.address_line_1) }}
-                            {{ user_profile_input(id='address_line_2', label='Address line 2:', value=user.address_line_2) }}
-                            {{ user_profile_input(id='city', label='City:', value=user.city) }}
-                            {{ user_profile_input(id='state', label='State:', value=user.state) }}
-                            {{ user_profile_input(id='zipcode', label='Zipcode:', value=user.zipcode) }}
-                            {{ user_profile_input(id='email', label='Email:', value=user.email, type='email') }}
-                            {{ user_profile_input(id='phone_number', label='Phone Number:', value=user.phone_number) }}
+                            {{ add_form_input(id='first_name', label='First Name:', value=user.first_name) }}
+                            {{ add_form_input(id='middle_name', label='Middle Name:', value=user.middle_name) }}
+                            {{ add_form_input(id='last_name', label='Last Name:', value=user.last_name) }}
+                            {{ add_form_input(id='address_line_1', label='Address line 1:', value=user.address_line_1) }}
+                            {{ add_form_input(id='address_line_2', label='Address line 2:', value=user.address_line_2) }}
+                            {{ add_form_input(id='city', label='City:', value=user.city) }}
+                            {{ add_form_input(id='state', label='State:', value=user.state) }}
+                            {{ add_form_input(id='zipcode', label='Zipcode:', value=user.zipcode) }}
+                            {{ add_form_input(id='email', label='Email:', value=user.email, type='email') }}
+                            {{ add_form_input(id='phone_number', label='Phone Number:', value=user.phone_number) }}
                         </form>
                     </div>
                     <div class="modal-footer">
                         <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancel</button>
                         <button type="submit" class="btn btn-primary" form="user_update">Save</button>
                     </div>
                 </div>
@@ -179,32 +178,22 @@
         </div>
         {%- endmacro %}
         {% macro add_reset_password_modal() -%}
         <div class="modal fade" id="resetPasswordModal" tabindex="-1">
             <div class="modal-dialog modal-dialog-centered">
                 <div class="modal-content">
                     <div class="modal-header">
-                        <h5 class="modal-title">Reset Password</h5>
+                        <h5 class="modal-title">Reset User Password</h5>
                         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                     </div>
                     <div class="modal-body">
                         <form id="reset_password" action="{{ url_for('user.reset_password') }}" method="post">
-                            {% macro user_password_input(id, label, value='', type='text') -%}
-                            <div class="mb-2">
-                                {% if type != 'hidden' %}
-                                <label for="{{ id }}" class="col-form-label"><strong>{{ label }}</strong></label>
-                                {% endif %}
-                                <input type="{{ type }}" class="form-control" name="{{ id }}" id="{{ id }}" value="{% if value is not none -%} {{ value }} {%- endif %}">
-                            </div>
-                            {%- endmacro %}
-
-                            {{ user_password_input(id='username', label='Username:', value=user.username, type='hidden') }}
-                            {{ user_password_input(id='current_password', label='Current Password:', type='password') }}
-                            {{ user_password_input(id='new_password', label='New Password:', type='password') }}
-                            {{ user_password_input(id='confirm_password', label='Confirm New Password:', type='password') }}
+                            {{ add_form_input(id='username', label='Username:', value=user.username, type='hidden') }}
+                            {{ add_form_input(id='new_password', label='New Password:', type='password', required=True) }}
+                            {{ add_form_input(id='confirm_password', label='Confirm New Password:', type='password', required=True) }}
                         </form>
                     </div>
                     <div class="modal-footer">
                         <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancel</button>
                         <button type="submit" class="btn btn-primary" form="reset_password">Save</button>
                     </div>
                 </div>
```

#### html2text {}

```diff
@@ -1,7 +1,15 @@
+{% macro add_form_input(id, label, value='', type='text', required=False,
+number_step='1', placeholder='') -%}
+{% if type != 'hidden' %} {{{{ llaabbeell }}}} {% endif %}
+% if type == 'number' -%}step="{{ number_step }}"{%- endif %} placeholder="{%
+if placeholder is not none -%} {{ placeholder }} {%- endif %}" value="{% if
+value is not none -%} {{ value }} {%- endif %}"{% if required -%} required{%-
+endif %}>
+{%- endmacro %}
 {% block view_css %}{% endblock %}
 _[_B_o_o_t_s_t_r_a_p_ _B_u_d_g_e_t_ _L_a_r_g_e_ _L_o_g_o_]
     * {% macro add_admin_console_nav(active=False) -%}
     * _A_d_m_i_n_ _C_o_n_s_o_l_e
     * {%- endmacro %} {% macro add_user_admin_nav(active=False) -%}
     * _U_s_e_r_s
     * {%- endmacro %} {% macro add_dashboard_nav(active=False) -%}
@@ -30,36 +38,30 @@
 {{ message }}
 {% elif category == 'warning' %}
 {{ message }}
 {% else %}
 {{ message }}
 {% endif %} {% endfor %} {% endif %} {% endwith %}
 {% macro add_edit_profile_modal() -%}
-**** EEddiitt PPrrooffiillee ****
-{% macro user_profile_input(id, label, value='', type='text') -%}
-{% if type != 'hidden' %} {{{{ llaabbeell }}}} {% endif %}[Unknown INPUT type]
-{%- endmacro %} {{ user_profile_input(id='first_name', label='First Name:',
-value=user.first_name) }} {{ user_profile_input(id='middle_name', label='Middle
-Name:', value=user.middle_name) }} {{ user_profile_input(id='last_name',
-label='Last Name:', value=user.last_name) }} {{ user_profile_input
-(id='address_line_1', label='Address line 1:', value=user.address_line_1) }} {
-{ user_profile_input(id='address_line_2', label='Address line 2:',
-value=user.address_line_2) }} {{ user_profile_input(id='city', label='City:',
-value=user.city) }} {{ user_profile_input(id='state', label='State:',
-value=user.state) }} {{ user_profile_input(id='zipcode', label='Zipcode:',
-value=user.zipcode) }} {{ user_profile_input(id='email', label='Email:',
-value=user.email, type='email') }} {{ user_profile_input(id='phone_number',
-label='Phone Number:', value=user.phone_number) }}
+**** EEddiitt UUsseerr PPrrooffiillee ****
+{{ add_form_input(id='first_name', label='First Name:', value=user.first_name)
+}} {{ add_form_input(id='middle_name', label='Middle Name:',
+value=user.middle_name) }} {{ add_form_input(id='last_name', label='Last Name:
+', value=user.last_name) }} {{ add_form_input(id='address_line_1',
+label='Address line 1:', value=user.address_line_1) }} {{ add_form_input
+(id='address_line_2', label='Address line 2:', value=user.address_line_2) }} {
+{ add_form_input(id='city', label='City:', value=user.city) }} {
+{ add_form_input(id='state', label='State:', value=user.state) }} {
+{ add_form_input(id='zipcode', label='Zipcode:', value=user.zipcode) }} {
+{ add_form_input(id='email', label='Email:', value=user.email, type='email') }}
+{{ add_form_input(id='phone_number', label='Phone Number:',
+value=user.phone_number) }}
 Cancel Save
 {%- endmacro %} {% macro add_reset_password_modal() -%}
-**** RReesseett PPaasssswwoorrdd ****
-{% macro user_password_input(id, label, value='', type='text') -%}
-{% if type != 'hidden' %} {{{{ llaabbeell }}}} {% endif %}[Unknown INPUT type]
-{%- endmacro %} {{ user_password_input(id='username', label='Username:',
-value=user.username, type='hidden') }} {{ user_password_input
-(id='current_password', label='Current Password:', type='password') }} {
-{ user_password_input(id='new_password', label='New Password:',
-type='password') }} {{ user_password_input(id='confirm_password',
-label='Confirm New Password:', type='password') }}
+**** RReesseett UUsseerr PPaasssswwoorrdd ****
+{{ add_form_input(id='username', label='Username:', value=user.username,
+type='hidden') }} {{ add_form_input(id='new_password', label='New Password:',
+type='password', required=True) }} {{ add_form_input(id='confirm_password',
+label='Confirm New Password:', type='password', required=True) }}
 Cancel Save
 {%- endmacro %} {% block modals %}{% endblock %} {% block main_content %}{%
 endblock %}
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/templates/login.html` & `bootstrap_budget-0.1.7/src/bootstrap_budget/templates/login.html`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget/user.py` & `bootstrap_budget-0.1.7/src/bootstrap_budget/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from flask import (
-    Blueprint, current_app, flash, g, redirect, render_template, request, Response, session, url_for
+    current_app, Blueprint, flash, g, redirect, render_template, request, Response
 )
+from werkzeug.security import generate_password_hash
 
 # Bootstrap Budget Imports
 from .auth import login_required, user_only
 from .entities import User
 
 
-# Define as a Flask blueprint: User
 bp = Blueprint('user', __name__, url_prefix='/user')
 
 
 @bp.route("/")
 @login_required
 @user_only
 def index() -> Response | str:
@@ -22,41 +22,57 @@
 @login_required
 def update() -> Response | str:
     """
     Update the current user from 'Edit Profile' modal.
 
     :return: Back to current view after update.
     """
-    user: User = g.user
-
     try:
-        user.first_name = request.form['first_name']
-        user.middle_name = request.form['middle_name']
-        user.last_name = request.form['last_name']
-        user.address_line_1 = request.form['address_line_1']
-        user.address_line_2 = request.form['address_line_2']
-        user.city = request.form['city']
-        user.state = request.form['state']
-        user.zipcode = request.form['zipcode']
-        user.email = request.form['email']
-        user.phone_number = request.form['phone_number']
+        current_app.logger.info(request.form)
+        g.user.first_name = request.form['first_name']
+        g.user.middle_name = request.form['middle_name']
+        g.user.last_name = request.form['last_name']
+        g.user.address_line_1 = request.form['address_line_1']
+        g.user.address_line_2 = request.form['address_line_2']
+        g.user.city = request.form['city']
+        g.user.state = request.form['state']
+        g.user.zipcode = request.form['zipcode']
+        g.user.email = request.form['email']
+        g.user.phone_number = request.form['phone_number']
 
         flash('User profile was successfully saved.', 'info')
     except Exception as e:
         flash(f'User profile failed to save: {e}', 'error')
 
-    g.user = user
-
     return redirect(request.referrer)
 
 
 @bp.route("/reset-password", methods=["POST"])
 @login_required
 def reset_password() -> Response | str:
     """
     Reset the password for a given user (by username) from 'Reset Password' modal.
 
     :return: Back to current view after update.
     """
-    flash('This does not do anything yet, Sorry :-/', 'warning')
+    try:
+        current_app.logger.info(request.form)
+        username: str = request.form['username']
+        user: User
+
+        if g.user.username != username:
+            user = User.get(username=request.form['username'])
+        else:
+            user = g.user
+
+        new_password = request.form['new_password']
+        confirm_password = request.form['confirm_password']
+
+        if new_password == confirm_password:
+            user.hash = generate_password_hash(new_password)
+            flash('User password was successfully changed.', 'info')
+        else:
+            flash('User password failed to change. Passwords did not match.', 'error')
+    except Exception as e:
+        flash(f'User password failed to be reset: {e}', 'error')
 
     return redirect(request.referrer)
```

### Comparing `bootstrap-budget-0.1.6/src/bootstrap_budget.egg-info/SOURCES.txt` & `bootstrap_budget-0.1.7/src/bootstrap_budget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bootstrap-budget-0.1.6/tests/test_version.py` & `bootstrap_budget-0.1.7/tests/test_version.py`

 * *Files identical despite different names*

