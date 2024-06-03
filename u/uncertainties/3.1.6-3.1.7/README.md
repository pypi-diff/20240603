# Comparing `tmp/uncertainties-3.1.6.tar.gz` & `tmp/uncertainties-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainties-3.1.6.tar", last modified: Sun Jul 11 20:55:37 2021, max compression
+gzip compressed data, was "uncertainties-3.1.7.tar", last modified: Sun Jun 19 14:01:44 2022, max compression
```

## Comparing `uncertainties-3.1.6.tar` & `uncertainties-3.1.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.229312 uncertainties-3.1.6/
--rw-r--r--   0 ericlebigot   (501) staff       (20)      625 2021-07-11 20:50:02.000000 uncertainties-3.1.6/INSTALL.txt
--rw-r--r--   0 ericlebigot   (501) staff       (20)     1464 2021-01-30 14:53:55.000000 uncertainties-3.1.6/LICENSE.txt
--rw-r--r--   0 ericlebigot   (501) staff       (20)      302 2021-01-30 14:53:55.000000 uncertainties-3.1.6/MANIFEST.in
--rw-r--r--   0 ericlebigot   (501) staff       (20)    13958 2021-07-11 20:55:37.229128 uncertainties-3.1.6/PKG-INFO
--rw-r--r--   0 ericlebigot   (501) staff       (20)     2078 2021-01-30 14:53:55.000000 uncertainties-3.1.6/README.rst
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.223500 uncertainties-3.1.6/doc/
--rw-r--r--   0 ericlebigot   (501) staff       (20)     3306 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/Makefile
--rw-r--r--   0 ericlebigot   (501) staff       (20)      174 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/README.rst
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.224192 uncertainties-3.1.6/doc/_static/
--rw-r--r--   0 ericlebigot   (501) staff       (20)     8194 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/_static/default.css
--rw-r--r--   0 ericlebigot   (501) staff       (20)     4399 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/_static/eol.jpg
--rw-r--r--   0 ericlebigot   (501) staff       (20)    11294 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/_static/favicon.ico
--rw-r--r--   0 ericlebigot   (501) staff       (20)    21909 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/_static/logo.png
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.224368 uncertainties-3.1.6/doc/_templates/
--rw-r--r--   0 ericlebigot   (501) staff       (20)     3612 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/_templates/layout.html
--rw-r--r--   0 ericlebigot   (501) staff       (20)     6858 2021-07-11 20:50:02.000000 uncertainties-3.1.6/doc/conf.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)    16875 2021-07-11 20:52:17.000000 uncertainties-3.1.6/doc/index.rst
--rw-r--r--   0 ericlebigot   (501) staff       (20)      131 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/index_TOC.rst
--rw-r--r--   0 ericlebigot   (501) staff       (20)     2999 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/make.bat
--rw-r--r--   0 ericlebigot   (501) staff       (20)     7389 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/numpy_guide.rst
--rw-r--r--   0 ericlebigot   (501) staff       (20)    14178 2021-01-30 14:53:55.000000 uncertainties-3.1.6/doc/tech_guide.rst
--rw-r--r--   0 ericlebigot   (501) staff       (20)    22615 2021-07-11 20:50:02.000000 uncertainties-3.1.6/doc/user_guide.rst
--rw-r--r--   0 ericlebigot   (501) staff       (20)       38 2021-07-11 20:55:37.229349 uncertainties-3.1.6/setup.cfg
--rwxr-xr-x   0 ericlebigot   (501) staff       (20)    16132 2021-07-11 20:50:02.000000 uncertainties-3.1.6/setup.py
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.226451 uncertainties-3.1.6/uncertainties/
--rwxr-xr-x   0 ericlebigot   (501) staff       (20)      384 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/1to2.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)     9355 2021-07-11 20:50:02.000000 uncertainties-3.1.6/uncertainties/__init__.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)   127560 2021-07-11 20:50:02.000000 uncertainties-3.1.6/uncertainties/core.py
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.227297 uncertainties-3.1.6/uncertainties/lib1to2/
--rw-r--r--   0 ericlebigot   (501) staff       (20)        0 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/lib1to2/__init__.py
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.228198 uncertainties-3.1.6/uncertainties/lib1to2/fixes/
--rw-r--r--   0 ericlebigot   (501) staff       (20)        0 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/lib1to2/fixes/__init__.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)     1037 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/lib1to2/fixes/fix_std_dev.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)      490 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/lib1to2/fixes/fix_std_devs.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)     2556 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/lib1to2/fixes/fix_uarray_umatrix.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)     3041 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/lib1to2/fixes/fix_ufloat.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)     7058 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/lib1to2/test_1to2.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)    11844 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/test_umath.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)    84971 2021-07-11 20:50:02.000000 uncertainties-3.1.6/uncertainties/test_uncertainties.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)     1319 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/umath.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)    14811 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/umath_core.py
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.228858 uncertainties-3.1.6/uncertainties/unumpy/
--rw-r--r--   0 ericlebigot   (501) staff       (20)     2841 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/unumpy/__init__.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)    28256 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/unumpy/core.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)     2861 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/unumpy/test_ulinalg.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)    10702 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/unumpy/test_unumpy.py
--rw-r--r--   0 ericlebigot   (501) staff       (20)      371 2021-01-30 14:53:55.000000 uncertainties-3.1.6/uncertainties/unumpy/ulinalg.py
-drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2021-07-11 20:55:37.227108 uncertainties-3.1.6/uncertainties.egg-info/
--rw-r--r--   0 ericlebigot   (501) staff       (20)    13958 2021-07-11 20:55:37.000000 uncertainties-3.1.6/uncertainties.egg-info/PKG-INFO
--rw-r--r--   0 ericlebigot   (501) staff       (20)     1138 2021-07-11 20:55:37.000000 uncertainties-3.1.6/uncertainties.egg-info/SOURCES.txt
--rw-r--r--   0 ericlebigot   (501) staff       (20)        1 2021-07-11 20:55:37.000000 uncertainties-3.1.6/uncertainties.egg-info/dependency_links.txt
--rw-r--r--   0 ericlebigot   (501) staff       (20)       85 2021-07-11 20:55:37.000000 uncertainties-3.1.6/uncertainties.egg-info/requires.txt
--rw-r--r--   0 ericlebigot   (501) staff       (20)       14 2021-07-11 20:55:37.000000 uncertainties-3.1.6/uncertainties.egg-info/top_level.txt
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.534764 uncertainties-3.1.7/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)      625 2020-11-18 08:21:15.000000 uncertainties-3.1.7/INSTALL.txt
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     1464 2020-06-07 08:50:06.000000 uncertainties-3.1.7/LICENSE.txt
+-rw-r--r--   0 ericlebigot   (501) staff       (20)      302 2020-06-07 08:50:06.000000 uncertainties-3.1.7/MANIFEST.in
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    13939 2022-06-19 14:01:44.534547 uncertainties-3.1.7/PKG-INFO
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     2089 2022-06-19 13:58:35.000000 uncertainties-3.1.7/README.rst
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.528571 uncertainties-3.1.7/doc/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     3306 2016-07-24 17:09:02.000000 uncertainties-3.1.7/doc/Makefile
+-rw-r--r--   0 ericlebigot   (501) staff       (20)      174 2016-09-16 18:24:51.000000 uncertainties-3.1.7/doc/README.rst
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.529362 uncertainties-3.1.7/doc/_static/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     8194 2016-07-24 17:09:02.000000 uncertainties-3.1.7/doc/_static/default.css
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     4399 2013-06-06 01:54:12.000000 uncertainties-3.1.7/doc/_static/eol.jpg
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    11294 2014-01-12 19:18:44.000000 uncertainties-3.1.7/doc/_static/favicon.ico
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    21909 2013-06-06 01:54:12.000000 uncertainties-3.1.7/doc/_static/logo.png
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.529591 uncertainties-3.1.7/doc/_templates/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     3612 2018-10-28 22:09:33.000000 uncertainties-3.1.7/doc/_templates/layout.html
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     6858 2022-06-19 13:58:35.000000 uncertainties-3.1.7/doc/conf.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    16875 2022-06-19 13:58:35.000000 uncertainties-3.1.7/doc/index.rst
+-rw-r--r--   0 ericlebigot   (501) staff       (20)      131 2018-01-13 14:17:26.000000 uncertainties-3.1.7/doc/index_TOC.rst
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     2999 2013-04-13 07:35:19.000000 uncertainties-3.1.7/doc/make.bat
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     7389 2018-01-14 15:53:48.000000 uncertainties-3.1.7/doc/numpy_guide.rst
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    14178 2020-11-18 08:04:01.000000 uncertainties-3.1.7/doc/tech_guide.rst
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    22756 2022-06-19 13:58:35.000000 uncertainties-3.1.7/doc/user_guide.rst
+-rw-r--r--   0 ericlebigot   (501) staff       (20)       38 2022-06-19 14:01:44.534833 uncertainties-3.1.7/setup.cfg
+-rwxr-xr-x   0 ericlebigot   (501) staff       (20)    16132 2022-06-19 13:58:35.000000 uncertainties-3.1.7/setup.py
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.531102 uncertainties-3.1.7/uncertainties/
+-rwxr-xr-x   0 ericlebigot   (501) staff       (20)      384 2020-02-02 09:45:29.000000 uncertainties-3.1.7/uncertainties/1to2.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     9355 2022-06-19 13:58:35.000000 uncertainties-3.1.7/uncertainties/__init__.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)   127808 2022-06-19 13:58:35.000000 uncertainties-3.1.7/uncertainties/core.py
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.532331 uncertainties-3.1.7/uncertainties/lib1to2/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)        0 2016-03-18 10:27:18.000000 uncertainties-3.1.7/uncertainties/lib1to2/__init__.py
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.533256 uncertainties-3.1.7/uncertainties/lib1to2/fixes/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)        0 2016-03-18 10:27:18.000000 uncertainties-3.1.7/uncertainties/lib1to2/fixes/__init__.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     1037 2020-02-02 09:45:29.000000 uncertainties-3.1.7/uncertainties/lib1to2/fixes/fix_std_dev.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)      490 2020-02-02 09:45:29.000000 uncertainties-3.1.7/uncertainties/lib1to2/fixes/fix_std_devs.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     2556 2020-02-02 09:45:29.000000 uncertainties-3.1.7/uncertainties/lib1to2/fixes/fix_uarray_umatrix.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     3041 2020-02-02 09:45:29.000000 uncertainties-3.1.7/uncertainties/lib1to2/fixes/fix_ufloat.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     7058 2020-06-07 08:50:06.000000 uncertainties-3.1.7/uncertainties/lib1to2/test_1to2.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    11844 2020-11-18 08:04:01.000000 uncertainties-3.1.7/uncertainties/test_umath.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    84971 2022-06-19 13:58:35.000000 uncertainties-3.1.7/uncertainties/test_uncertainties.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     1319 2019-11-23 22:08:57.000000 uncertainties-3.1.7/uncertainties/umath.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    14811 2020-06-07 08:50:06.000000 uncertainties-3.1.7/uncertainties/umath_core.py
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.534230 uncertainties-3.1.7/uncertainties/unumpy/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     2841 2016-09-16 18:24:51.000000 uncertainties-3.1.7/uncertainties/unumpy/__init__.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    28256 2020-06-07 08:50:06.000000 uncertainties-3.1.7/uncertainties/unumpy/core.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     2861 2020-06-07 08:50:06.000000 uncertainties-3.1.7/uncertainties/unumpy/test_ulinalg.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    10702 2020-06-07 08:50:06.000000 uncertainties-3.1.7/uncertainties/unumpy/test_unumpy.py
+-rw-r--r--   0 ericlebigot   (501) staff       (20)      371 2020-02-02 09:45:29.000000 uncertainties-3.1.7/uncertainties/unumpy/ulinalg.py
+drwxr-xr-x   0 ericlebigot   (501) staff       (20)        0 2022-06-19 14:01:44.532007 uncertainties-3.1.7/uncertainties.egg-info/
+-rw-r--r--   0 ericlebigot   (501) staff       (20)    13939 2022-06-19 14:01:44.000000 uncertainties-3.1.7/uncertainties.egg-info/PKG-INFO
+-rw-r--r--   0 ericlebigot   (501) staff       (20)     1138 2022-06-19 14:01:44.000000 uncertainties-3.1.7/uncertainties.egg-info/SOURCES.txt
+-rw-r--r--   0 ericlebigot   (501) staff       (20)        1 2022-06-19 14:01:44.000000 uncertainties-3.1.7/uncertainties.egg-info/dependency_links.txt
+-rw-r--r--   0 ericlebigot   (501) staff       (20)       85 2022-06-19 14:01:44.000000 uncertainties-3.1.7/uncertainties.egg-info/requires.txt
+-rw-r--r--   0 ericlebigot   (501) staff       (20)       14 2022-06-19 14:01:44.000000 uncertainties-3.1.7/uncertainties.egg-info/top_level.txt
```

### Comparing `uncertainties-3.1.6/INSTALL.txt` & `uncertainties-3.1.7/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/LICENSE.txt` & `uncertainties-3.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/PKG-INFO` & `uncertainties-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: uncertainties
-Version: 3.1.6
+Version: 3.1.7
 Summary: Transparent calculations with uncertainties on the quantities involved (aka error propagation); fast calculation of derivatives
 Home-page: http://uncertainties-python-package.readthedocs.io/
 Author: Eric O. LEBIGOT (EOL)
 Author-email: eric.lebigot@normalesup.org
 License: Revised BSD License
 Project-URL: Documentation, https://uncertainties-python-package.readthedocs.io/
 Project-URL: Source, https://github.com/lebigot/uncertainties
 Keywords: error propagation,uncertainties,uncertainty calculations,standard deviation,derivatives,partial derivatives,differentiation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -143,16 +142,16 @@
 `Eric O. LEBIGOT (EOL)`_.
 
 Version history
 ===============
 
 Main changes:
 
-- 3.1.6: the pretty-print and LaTeX format can now be customized.
-- 3.1.5: added a "p" formatting option, that makes sure that there are always
+- 3.1.6: The pretty-print and LaTeX format can now be customized.
+- 3.1.5: Added a "p" formatting option, that makes sure that there are always
   parentheses around the … ± … part of printed numbers.
 - 3.1.4: Python 2.7+ is now required.
 - 3.1.2: Fix for NumPy 1.17 and ``unumpy.ulinalg.pinv()``.
 - 3.1: Variables built through a correlation or covariance matrix, and that
   have uncertainties that span many orders of magnitude are now
   calculated more accurately (improved ``correlated_values()`` and
   ``correlated_values_norm()`` functions).
@@ -283,8 +282,7 @@
 .. _PEP 8: http://www.python.org/dev/peps/pep-0008/
 .. _error propagation theory: http://en.wikipedia.org/wiki/Propagation_of_uncertainty
 .. _Eric O. LEBIGOT (EOL): mailto:eric.lebigot@normalesup.org
 .. _PayPal: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4TK7KNDTEDT4S
 .. _main website: http://uncertainties-python-package.readthedocs.io/
 .. _code updater: http://uncertainties-python-package.readthedocs.io/en/latest/index.html#migration-from-version-1-to-version-2
 .. _formatting: http://uncertainties-python-package.readthedocs.io/en/latest/user_guide.html#printing
-
```

### Comparing `uncertainties-3.1.6/README.rst` & `uncertainties-3.1.7/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 uncertainties
 =============
 
-.. image:: https://readthedocs.org/projects/uncertainties-python-package/badge/?version=latest
-   :target: http://uncertainties-python-package.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/uncertainties/badge/?version=latest
+   :target: https://uncertainties.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
 .. image:: https://img.shields.io/pypi/v/uncertainties.svg
    :target: https://pypi.org/project/uncertainties/
 .. image:: https://pepy.tech/badge/uncertainties/week
-   :target: https://pepy.tech/badge/uncertainties/week
+   :target: https://pepy.tech/project/uncertainties
 .. image:: https://codecov.io/gh/lebigot/uncertainties/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/lebigot/uncertainties/
-.. image:: https://travis-ci.org/lebigot/uncertainties.svg?branch=master
-   :target: https://travis-ci.org/lebigot/uncertainties
+.. image:: https://travis-ci.com/lebigot/uncertainties.svg?branch=master
+   :target: https://travis-ci.com/lebigot/uncertainties
 .. image:: https://ci.appveyor.com/api/projects/status/j5238244myqx0a0r?svg=true
    :target: https://ci.appveyor.com/project/lebigot/uncertainties
 
    
 This is the ``uncertainties`` Python package, which performs **transparent
 calculations with uncertainties** (aka "error propagation"):
 
@@ -22,21 +23,21 @@
     >>> from uncertainties.umath import *  # sin(), etc.
     >>> x = ufloat(1, 0.1)  # x = 1+/-0.1
     >>> print 2*x
     2.00+/-0.20
     >>> sin(2*x)  # In a Python shell, "print" is optional
     0.9092974268256817+/-0.08322936730942848
 
-This package also automatically calculates derivatives:
+This package also **automatically calculates derivatives of arbitrary functions**:
 
     >>> (2*x+1000).derivatives[x]
     2.0
 
 The main documentation is available at
-http://uncertainties-python-package.readthedocs.io/.
+https://uncertainties.readthedocs.io/.
 
 Git branches
 ------------
 
 The ``release`` branch is the latest stable release. It should pass the tests.
```

### Comparing `uncertainties-3.1.6/doc/Makefile` & `uncertainties-3.1.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/_static/default.css` & `uncertainties-3.1.7/doc/_static/default.css`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/_static/eol.jpg` & `uncertainties-3.1.7/doc/_static/eol.jpg`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/_static/favicon.ico` & `uncertainties-3.1.7/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/_static/logo.png` & `uncertainties-3.1.7/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/_templates/layout.html` & `uncertainties-3.1.7/doc/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/conf.py` & `uncertainties-3.1.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/index.rst` & `uncertainties-3.1.7/doc/index.rst`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/make.bat` & `uncertainties-3.1.7/doc/make.bat`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/numpy_guide.rst` & `uncertainties-3.1.7/doc/numpy_guide.rst`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/tech_guide.rst` & `uncertainties-3.1.7/doc/tech_guide.rst`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/doc/user_guide.rst` & `uncertainties-3.1.7/doc/user_guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -588,16 +588,16 @@
    frmtr = ShorthandFormatter()
 
    print frmtr.format("Result = {0:.1u}", x)  # 1-digit uncertainty
 
 prints with the shorthand notation: ``Result = 0.20(1)``.
 
 
-Customization of the pretty print and LaTeX outputs
----------------------------------------------------
+Customizing the pretty-print and LaTeX outputs
+----------------------------------------------
 
 The pretty print and LaTeX outputs themselves can be customized.
 
 For example, the pretty-print representation of numbers with uncertainty can
 display multiplication with a centered dot (⋅) instead of the default symbol
 (×), like in ``(2.00±0.10)⋅10⁻¹``; this is easily done through the global
 setting ``uncertainties.core.MULT_SYMBOLS["pretty-print"] = "⋅"``.
@@ -619,16 +619,19 @@
 
 It is thus possible to take a function :func:`f` *that returns a
 single float*, and to automatically generalize it so that it also
 works with numbers with uncertainties:
 
 >>> wrapped_f = uncertainties.wrap(f)
 
-The new function :func:`wrapped_f` *accepts numbers with uncertainties*
-as arguments *wherever a Python float is used* for :func:`f`.
+The new function :func:`wrapped_f` (optionally) *accepts a number
+with uncertainty* in place of any float *argument* of :func:`f` (note
+that floats contained instead *inside* arguments of :func:`f`, like
+in a list or a NumPy array, *cannot* be replaced by numbers with
+uncertainties).
 :func:`wrapped_f` returns the same values as :func:`f`, but with
 uncertainties.
 
 With a simple wrapping call like above, uncertainties in the function
 result are automatically calculated numerically. **Analytical
 uncertainty calculations can be performed** if derivatives are
 provided to :func:`wrap`.
```

### Comparing `uncertainties-3.1.6/setup.py` & `uncertainties-3.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         sys.exit(error_msg)
 except AttributeError:  # sys.version_info was introduced in Python 2.0
     sys.exit(error_msg)
 
 # Common options for distutils/setuptools's setup():
 setup_options = dict(
     name='uncertainties',
-    version='3.1.6',
+    version='3.1.7',
     author='Eric O. LEBIGOT (EOL)',
     author_email='eric.lebigot@normalesup.org',
     url='http://uncertainties-python-package.readthedocs.io/',
     license='Revised BSD License',
     description=('Transparent calculations with uncertainties on the'
                  ' quantities involved (aka error propagation);'
                  ' fast calculation of derivatives'),
@@ -127,16 +127,16 @@
 `Eric O. LEBIGOT (EOL)`_.
 
 Version history
 ===============
 
 Main changes:
 
-- 3.1.6: the pretty-print and LaTeX format can now be customized.
-- 3.1.5: added a "p" formatting option, that makes sure that there are always
+- 3.1.6: The pretty-print and LaTeX format can now be customized.
+- 3.1.5: Added a "p" formatting option, that makes sure that there are always
   parentheses around the … ± … part of printed numbers.
 - 3.1.4: Python 2.7+ is now required.
 - 3.1.2: Fix for NumPy 1.17 and ``unumpy.ulinalg.pinv()``.
 - 3.1: Variables built through a correlation or covariance matrix, and that
   have uncertainties that span many orders of magnitude are now
   calculated more accurately (improved ``correlated_values()`` and
   ``correlated_values_norm()`` functions).
```

### Comparing `uncertainties-3.1.6/uncertainties/__init__.py` & `uncertainties-3.1.7/uncertainties/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,11 +222,11 @@
 author.'''
 
 from builtins import map
 from .core import *
 from .core import __all__  # For a correct help(uncertainties)
 
 # Numerical version:
-__version_info__ = (3, 1, 6)
+__version_info__ = (3, 1, 7)
 __version__ = '.'.join(map(str, __version_info__))
 
 __author__ = 'Eric O. LEBIGOT (EOL) <eric.lebigot@normalesup.org>'
```

### Comparing `uncertainties-3.1.6/uncertainties/core.py` & `uncertainties-3.1.7/uncertainties/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 # (AffineScalarFunc object) whose nominal value is sin(0.2) and
 # whose variations are given by sin(0.2+delta) = 0.98...*delta.
 # Uncertainties can then be calculated by using this local linear
 # approximation of the original function.
 
 from __future__ import division  # Many analytical derivatives depend on this
 
-from builtins import str
-from builtins import next
-from builtins import map
-from builtins import zip
-from builtins import range
-from past.builtins import basestring
-from builtins import object
+from builtins import str, next, map, zip, range, object
 import math
 from math import sqrt, log, isnan, isinf  # Optimization: no attribute look-up
 import re
 import sys
+if sys.version_info < (3,):
+     from past.builtins import basestring
+else:
+     # Avoid importing from past in Python 3 since it utilizes the builtin
+     # 'imp' module, which is deprecated as of Python 3.4, see
+     # https://docs.python.org/3/library/imp.html. The 2to3 tool replaces
+     # basestring with str, so that's what we effectively do here as well:
+     basestring = str
 
 try:
     from math import isinfinite  # !! Python 3.2+
 except ImportError:
     def isinfinite(x):
         return isinf(x) or isnan(x)
```

### Comparing `uncertainties-3.1.6/uncertainties/lib1to2/fixes/fix_std_dev.py` & `uncertainties-3.1.7/uncertainties/lib1to2/fixes/fix_std_dev.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/lib1to2/fixes/fix_uarray_umatrix.py` & `uncertainties-3.1.7/uncertainties/lib1to2/fixes/fix_uarray_umatrix.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/lib1to2/fixes/fix_ufloat.py` & `uncertainties-3.1.7/uncertainties/lib1to2/fixes/fix_ufloat.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/lib1to2/test_1to2.py` & `uncertainties-3.1.7/uncertainties/lib1to2/test_1to2.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/test_umath.py` & `uncertainties-3.1.7/uncertainties/test_umath.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/test_uncertainties.py` & `uncertainties-3.1.7/uncertainties/test_uncertainties.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/umath.py` & `uncertainties-3.1.7/uncertainties/umath.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/umath_core.py` & `uncertainties-3.1.7/uncertainties/umath_core.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/unumpy/__init__.py` & `uncertainties-3.1.7/uncertainties/unumpy/__init__.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/unumpy/core.py` & `uncertainties-3.1.7/uncertainties/unumpy/core.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/unumpy/test_ulinalg.py` & `uncertainties-3.1.7/uncertainties/unumpy/test_ulinalg.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties/unumpy/test_unumpy.py` & `uncertainties-3.1.7/uncertainties/unumpy/test_unumpy.py`

 * *Files identical despite different names*

### Comparing `uncertainties-3.1.6/uncertainties.egg-info/PKG-INFO` & `uncertainties-3.1.7/uncertainties.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: uncertainties
-Version: 3.1.6
+Version: 3.1.7
 Summary: Transparent calculations with uncertainties on the quantities involved (aka error propagation); fast calculation of derivatives
 Home-page: http://uncertainties-python-package.readthedocs.io/
 Author: Eric O. LEBIGOT (EOL)
 Author-email: eric.lebigot@normalesup.org
 License: Revised BSD License
 Project-URL: Documentation, https://uncertainties-python-package.readthedocs.io/
 Project-URL: Source, https://github.com/lebigot/uncertainties
 Keywords: error propagation,uncertainties,uncertainty calculations,standard deviation,derivatives,partial derivatives,differentiation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -143,16 +142,16 @@
 `Eric O. LEBIGOT (EOL)`_.
 
 Version history
 ===============
 
 Main changes:
 
-- 3.1.6: the pretty-print and LaTeX format can now be customized.
-- 3.1.5: added a "p" formatting option, that makes sure that there are always
+- 3.1.6: The pretty-print and LaTeX format can now be customized.
+- 3.1.5: Added a "p" formatting option, that makes sure that there are always
   parentheses around the … ± … part of printed numbers.
 - 3.1.4: Python 2.7+ is now required.
 - 3.1.2: Fix for NumPy 1.17 and ``unumpy.ulinalg.pinv()``.
 - 3.1: Variables built through a correlation or covariance matrix, and that
   have uncertainties that span many orders of magnitude are now
   calculated more accurately (improved ``correlated_values()`` and
   ``correlated_values_norm()`` functions).
@@ -283,8 +282,7 @@
 .. _PEP 8: http://www.python.org/dev/peps/pep-0008/
 .. _error propagation theory: http://en.wikipedia.org/wiki/Propagation_of_uncertainty
 .. _Eric O. LEBIGOT (EOL): mailto:eric.lebigot@normalesup.org
 .. _PayPal: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4TK7KNDTEDT4S
 .. _main website: http://uncertainties-python-package.readthedocs.io/
 .. _code updater: http://uncertainties-python-package.readthedocs.io/en/latest/index.html#migration-from-version-1-to-version-2
 .. _formatting: http://uncertainties-python-package.readthedocs.io/en/latest/user_guide.html#printing
-
```

### Comparing `uncertainties-3.1.6/uncertainties.egg-info/SOURCES.txt` & `uncertainties-3.1.7/uncertainties.egg-info/SOURCES.txt`

 * *Files identical despite different names*

