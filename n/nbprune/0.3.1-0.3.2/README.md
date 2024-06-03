# Comparing `tmp/nbprune-0.3.1.tar.gz` & `tmp/nbprune-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbprune-0.3.1.tar", last modified: Thu Jun 15 09:53:47 2023, max compression
+gzip compressed data, was "nbprune-0.3.2.tar", last modified: Mon Jun  3 08:52:53 2024, max compression
```

## Comparing `nbprune-0.3.1.tar` & `nbprune-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-06-15 09:53:47.126527 nbprune-0.3.1/
--rw-r--r--   0 tparment (15010) diana    (200036)     2488 2023-06-15 09:53:47.126204 nbprune-0.3.1/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)     2142 2022-06-07 10:12:58.000000 nbprune-0.3.1/README.md
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-06-15 09:53:47.123000 nbprune-0.3.1/nbprune/
--rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-06-07 12:32:54.000000 nbprune-0.3.1/nbprune/__init__.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     8734 2023-01-13 16:24:29.000000 nbprune-0.3.1/nbprune/nbprune.py
--rw-r--r--   0 tparment (15010) diana    (200036)       22 2023-01-13 16:27:45.000000 nbprune-0.3.1/nbprune/version.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-06-15 09:53:47.125769 nbprune-0.3.1/nbprune.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)     2488 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      294 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       49 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/entry_points.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-06-07 12:33:11.000000 nbprune-0.3.1/nbprune.egg-info/not-zip-safe
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/requires.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        8 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-06-15 09:53:47.126632 nbprune-0.3.1/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1534 2022-06-07 12:28:54.000000 nbprune-0.3.1/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-06-03 08:52:53.366757 nbprune-0.3.2/
+-rw-r--r--   0 tparment (15010) diana    (200036)     2686 2024-06-03 08:52:53.366035 nbprune-0.3.2/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)     2316 2024-06-03 08:19:57.000000 nbprune-0.3.2/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-06-03 08:52:53.361298 nbprune-0.3.2/nbprune/
+-rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-06-07 12:32:54.000000 nbprune-0.3.2/nbprune/__init__.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     8734 2023-01-13 16:24:29.000000 nbprune-0.3.2/nbprune/nbprune.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       22 2024-06-03 08:26:11.000000 nbprune-0.3.2/nbprune/version.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-06-03 08:52:53.365417 nbprune-0.3.2/nbprune.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)     2686 2024-06-03 08:52:53.000000 nbprune-0.3.2/nbprune.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      294 2024-06-03 08:52:53.000000 nbprune-0.3.2/nbprune.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-06-03 08:52:53.000000 nbprune-0.3.2/nbprune.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       49 2024-06-03 08:52:53.000000 nbprune-0.3.2/nbprune.egg-info/entry_points.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-06-07 12:33:11.000000 nbprune-0.3.2/nbprune.egg-info/not-zip-safe
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-06-03 08:52:53.000000 nbprune-0.3.2/nbprune.egg-info/requires.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        8 2024-06-03 08:52:53.000000 nbprune-0.3.2/nbprune.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-06-03 08:52:53.366902 nbprune-0.3.2/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1534 2022-06-07 12:28:54.000000 nbprune-0.3.2/setup.py
```

### Comparing `nbprune-0.3.1/PKG-INFO` & `nbprune-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 Metadata-Version: 2.1
 Name: nbprune
-Version: 0.3.1
+Version: 0.3.2
 Summary: With this tool, one can define pieces of a notebook that belong to teachers and should not be exposed to students.
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 Project-URL: source, https://github.com/flotpython/nbprune
 Description-Content-Type: text/markdown
+Requires-Dist: jupytext
 
 # nbprune
 
-typical use case is, a teacher writes a notebook, with solution(s) to a problem that students must solve
-
-so this means 2 versions, one for the teacher(s) with the solutions, and one for the students
-
+typical use case is, a teacher writes a notebook, with solution(s) to a problem that students must solve  
+so this means 2 versions, one for the teacher(s) with the solutions, and one for the students  
 this tool defines annotations that the teacher can use to define the parts that will be automatically removed by the tool
 
 ## keywords
 
 here are the recognized keywords
 
 | tag | meaning |
 |-|-|
-| `prune-line` (*) | remove just that one line from the output |
 | `prune-cell` | remove this cell from the output |
 | `prune-begin` | remove this cell and the ones below from the output |
 | `prune-end` | remove this cell, but resume insertion on the next cell |
-| `prune-begin-next` (**) | keep this cell from the output, and start pruning at the next one |
-| `prune-end-previous` (**) | stop pruning, and insert the current cell |
+| `prune-begin-next` (*) | keep this cell from the output, and start pruning at the next one |
+| `prune-end-previous` (*) | stop pruning, and insert the current cell |
+| `prune-line` (*) | remove just that one line from the output |
+| `prune-line-begin` (**) | remove that line and the following ones |
+| `prune-line-end` (**) | remove that line but the following ones will show up |
 
 **NOTES**
-* (*) `prune-line` of course is not relevant, and ignored, if set in the cell's metadata tags
-* (**) because `prune-begin-next` and `prune-end-previous` appear in a cell that is visible, the whole line containing the tag is removed from the output, so it is probably best to keep these tags on a separate
+
+* (*) because `prune-begin-next` and `prune-end-previous` appear in a cell that
+  is visible, the whole line containing the tag is removed from the output, so
+  it is probably best to keep these tags on a separate line
+* (**) `prune-line` variants of course are not relevant, and are ignored, if set in the cell's metadata tags
 
 ## line format
 
 the tool will consider a tag is present in a cell if any line in the cell
 contains one of the above keywords, with the beginning of the line containing
 only `#` and spaces or tabs
 
 so for exemple
 
 | line | match |
 |:-|-|
 | prune-cell | yes |
 | # prune-cell | yes |
-| # # prune-cell | yes | 
+| # # prune-cell | yes |
 | some code prune-cell | no |
 
 ## cell metadata
 
 the tags can also be set in the cell's metadata as well (except for `prune-line`) ; something like this
 
 ```json
```

### Comparing `nbprune-0.3.1/README.md` & `nbprune-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 # nbprune
 
-typical use case is, a teacher writes a notebook, with solution(s) to a problem that students must solve
-
-so this means 2 versions, one for the teacher(s) with the solutions, and one for the students
-
+typical use case is, a teacher writes a notebook, with solution(s) to a problem that students must solve  
+so this means 2 versions, one for the teacher(s) with the solutions, and one for the students  
 this tool defines annotations that the teacher can use to define the parts that will be automatically removed by the tool
 
 ## keywords
 
 here are the recognized keywords
 
 | tag | meaning |
 |-|-|
-| `prune-line` (*) | remove just that one line from the output |
 | `prune-cell` | remove this cell from the output |
 | `prune-begin` | remove this cell and the ones below from the output |
 | `prune-end` | remove this cell, but resume insertion on the next cell |
-| `prune-begin-next` (**) | keep this cell from the output, and start pruning at the next one |
-| `prune-end-previous` (**) | stop pruning, and insert the current cell |
+| `prune-begin-next` (*) | keep this cell from the output, and start pruning at the next one |
+| `prune-end-previous` (*) | stop pruning, and insert the current cell |
+| `prune-line` (*) | remove just that one line from the output |
+| `prune-line-begin` (**) | remove that line and the following ones |
+| `prune-line-end` (**) | remove that line but the following ones will show up |
 
 **NOTES**
-* (*) `prune-line` of course is not relevant, and ignored, if set in the cell's metadata tags
-* (**) because `prune-begin-next` and `prune-end-previous` appear in a cell that is visible, the whole line containing the tag is removed from the output, so it is probably best to keep these tags on a separate
+
+* (*) because `prune-begin-next` and `prune-end-previous` appear in a cell that
+  is visible, the whole line containing the tag is removed from the output, so
+  it is probably best to keep these tags on a separate line
+* (**) `prune-line` variants of course are not relevant, and are ignored, if set in the cell's metadata tags
 
 ## line format
 
 the tool will consider a tag is present in a cell if any line in the cell
 contains one of the above keywords, with the beginning of the line containing
 only `#` and spaces or tabs
 
 so for exemple
 
 | line | match |
 |:-|-|
 | prune-cell | yes |
 | # prune-cell | yes |
-| # # prune-cell | yes | 
+| # # prune-cell | yes |
 | some code prune-cell | no |
 
 ## cell metadata
 
 the tags can also be set in the cell's metadata as well (except for `prune-line`) ; something like this
 
 ```json
```

### Comparing `nbprune-0.3.1/nbprune/nbprune.py` & `nbprune-0.3.2/nbprune/nbprune.py`

 * *Files identical despite different names*

### Comparing `nbprune-0.3.1/nbprune.egg-info/PKG-INFO` & `nbprune-0.3.2/nbprune.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 Metadata-Version: 2.1
 Name: nbprune
-Version: 0.3.1
+Version: 0.3.2
 Summary: With this tool, one can define pieces of a notebook that belong to teachers and should not be exposed to students.
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 Project-URL: source, https://github.com/flotpython/nbprune
 Description-Content-Type: text/markdown
+Requires-Dist: jupytext
 
 # nbprune
 
-typical use case is, a teacher writes a notebook, with solution(s) to a problem that students must solve
-
-so this means 2 versions, one for the teacher(s) with the solutions, and one for the students
-
+typical use case is, a teacher writes a notebook, with solution(s) to a problem that students must solve  
+so this means 2 versions, one for the teacher(s) with the solutions, and one for the students  
 this tool defines annotations that the teacher can use to define the parts that will be automatically removed by the tool
 
 ## keywords
 
 here are the recognized keywords
 
 | tag | meaning |
 |-|-|
-| `prune-line` (*) | remove just that one line from the output |
 | `prune-cell` | remove this cell from the output |
 | `prune-begin` | remove this cell and the ones below from the output |
 | `prune-end` | remove this cell, but resume insertion on the next cell |
-| `prune-begin-next` (**) | keep this cell from the output, and start pruning at the next one |
-| `prune-end-previous` (**) | stop pruning, and insert the current cell |
+| `prune-begin-next` (*) | keep this cell from the output, and start pruning at the next one |
+| `prune-end-previous` (*) | stop pruning, and insert the current cell |
+| `prune-line` (*) | remove just that one line from the output |
+| `prune-line-begin` (**) | remove that line and the following ones |
+| `prune-line-end` (**) | remove that line but the following ones will show up |
 
 **NOTES**
-* (*) `prune-line` of course is not relevant, and ignored, if set in the cell's metadata tags
-* (**) because `prune-begin-next` and `prune-end-previous` appear in a cell that is visible, the whole line containing the tag is removed from the output, so it is probably best to keep these tags on a separate
+
+* (*) because `prune-begin-next` and `prune-end-previous` appear in a cell that
+  is visible, the whole line containing the tag is removed from the output, so
+  it is probably best to keep these tags on a separate line
+* (**) `prune-line` variants of course are not relevant, and are ignored, if set in the cell's metadata tags
 
 ## line format
 
 the tool will consider a tag is present in a cell if any line in the cell
 contains one of the above keywords, with the beginning of the line containing
 only `#` and spaces or tabs
 
 so for exemple
 
 | line | match |
 |:-|-|
 | prune-cell | yes |
 | # prune-cell | yes |
-| # # prune-cell | yes | 
+| # # prune-cell | yes |
 | some code prune-cell | no |
 
 ## cell metadata
 
 the tags can also be set in the cell's metadata as well (except for `prune-line`) ; something like this
 
 ```json
```

### Comparing `nbprune-0.3.1/setup.py` & `nbprune-0.3.2/setup.py`

 * *Files identical despite different names*

