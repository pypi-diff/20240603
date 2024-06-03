# Comparing `tmp/pybalmorel-0.0.8.tar.gz` & `tmp/pybalmorel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybalmorel-0.0.8.tar", last modified: Mon Mar 11 12:57:57 2024, max compression
+gzip compressed data, was "pybalmorel-0.0.9.tar", last modified: Thu Mar 14 11:29:20 2024, max compression
```

## Comparing `pybalmorel-0.0.8.tar` & `pybalmorel-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 12:57:57.525157 pybalmorel-0.0.8/
--rw-rw-rw-   0        0        0     1097 2024-03-10 17:10:52.000000 pybalmorel-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      671 2024-03-11 12:57:57.523153 pybalmorel-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       84 2024-03-10 17:04:58.000000 pybalmorel-0.0.8/README.md
--rw-rw-rw-   0        0        0      569 2024-03-11 12:57:43.000000 pybalmorel-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-11 12:57:57.529153 pybalmorel-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 12:57:57.453062 pybalmorel-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 12:57:57.480155 pybalmorel-0.0.8/src/pybalmorel/
--rw-rw-rw-   0        0        0       23 2024-03-10 17:33:54.000000 pybalmorel-0.0.8/src/pybalmorel/__init__.py
--rw-rw-rw-   0        0        0     1868 2024-03-10 16:36:45.000000 pybalmorel-0.0.8/src/pybalmorel/functions.py
-drwxrwxrwx   0        0        0        0 2024-03-11 12:57:57.520153 pybalmorel-0.0.8/src/pybalmorel.egg-info/
--rw-rw-rw-   0        0        0      671 2024-03-11 12:57:57.000000 pybalmorel-0.0.8/src/pybalmorel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-03-11 12:57:57.000000 pybalmorel-0.0.8/src/pybalmorel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 12:57:57.000000 pybalmorel-0.0.8/src/pybalmorel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-11 12:57:57.000000 pybalmorel-0.0.8/src/pybalmorel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-14 11:29:20.133063 pybalmorel-0.0.9/
+-rw-rw-rw-   0        0        0     1097 2024-03-10 17:10:52.000000 pybalmorel-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      671 2024-03-14 11:29:20.132060 pybalmorel-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2024-03-10 17:04:58.000000 pybalmorel-0.0.9/README.md
+-rw-rw-rw-   0        0        0      569 2024-03-14 11:29:11.000000 pybalmorel-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-14 11:29:20.142091 pybalmorel-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-14 11:29:20.094484 pybalmorel-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-03-14 11:29:20.107483 pybalmorel-0.0.9/src/pybalmorel/
+-rw-rw-rw-   0        0        0       23 2024-03-10 17:33:54.000000 pybalmorel-0.0.9/src/pybalmorel/__init__.py
+-rw-rw-rw-   0        0        0     2285 2024-03-14 11:28:38.000000 pybalmorel-0.0.9/src/pybalmorel/functions.py
+drwxrwxrwx   0        0        0        0 2024-03-14 11:29:20.130057 pybalmorel-0.0.9/src/pybalmorel.egg-info/
+-rw-rw-rw-   0        0        0      671 2024-03-14 11:29:20.000000 pybalmorel-0.0.9/src/pybalmorel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-03-14 11:29:20.000000 pybalmorel-0.0.9/src/pybalmorel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-14 11:29:20.000000 pybalmorel-0.0.9/src/pybalmorel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-03-14 11:29:20.000000 pybalmorel-0.0.9/src/pybalmorel.egg-info/top_level.txt
```

### Comparing `pybalmorel-0.0.8/LICENSE` & `pybalmorel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybalmorel-0.0.8/PKG-INFO` & `pybalmorel-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybalmorel
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for convenient python functions when processing Balmorel data or results
 Author-email: Mathias Berg Rosendal <mathiasros@gmail.com>
 Project-URL: Homepage, https://github.com/Mathias157
 Project-URL: Issues, https://github.com/Mathias157/balmorel-preprocessing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybalmorel-0.0.8/pyproject.toml` & `pybalmorel-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pybalmorel"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Mathias Berg Rosendal", email="mathiasros@gmail.com" },
 ]
 description = "A package for convenient python functions when processing Balmorel data or results"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pybalmorel-0.0.8/src/pybalmorel/functions.py` & `pybalmorel-0.0.9/src/pybalmorel/functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 Functions
 """
 
 import pandas as pd
 
 ### 1.0 Converting a GDX file to a pandas dataframe
-def symbol_to_df(db, symbol, cols='None'):
+def symbol_to_df(db, symbol, cols='None', parameter_or_set='parameter'):
     """
     Loads a symbol from a GDX database into a pandas dataframe
 
     Args:
         db (GamsDatabase): The loaded gdx file
         symbol (string): The wanted symbol in the gdx file
         cols (list): The columns
+        parameter_or_set (str): Choose either 'parameter' or 'set'
     """   
-    df = dict( (tuple(rec.keys), rec.value) for rec in db[symbol] )
-    df = pd.DataFrame(df, index=['Value']).T.reset_index() # Convert to dataframe
+    if parameter_or_set == 'parameter':
+        df = dict( (tuple(rec.keys), rec.value) for rec in db[symbol] )
+        df = pd.DataFrame(df, index=['Value']).T.reset_index() # Convert to dataframe
+    elif parameter_or_set == 'set':
+        df = dict( (tuple(rec.keys) ) for rec in db[symbol] )
+        df = pd.DataFrame(dict( (tuple(rec.keys)) for rec in db[symbol] ), index=['Set']).T.reset_index()
+    else:
+        print('Choose either parameter or set!')
+
     if cols != 'None':
         try:
             df.columns = cols
         except:
             pass
     return df
```

### Comparing `pybalmorel-0.0.8/src/pybalmorel.egg-info/PKG-INFO` & `pybalmorel-0.0.9/src/pybalmorel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybalmorel
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for convenient python functions when processing Balmorel data or results
 Author-email: Mathias Berg Rosendal <mathiasros@gmail.com>
 Project-URL: Homepage, https://github.com/Mathias157
 Project-URL: Issues, https://github.com/Mathias157/balmorel-preprocessing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

