# Comparing `tmp/PAModelpy-0.0.3.8.tar.gz` & `tmp/PAModelpy-0.0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PAModelpy-0.0.3.8.tar", last modified: Tue Dec 19 15:47:34 2023, max compression
+gzip compressed data, was "PAModelpy-0.0.3.9.tar", last modified: Tue Dec 19 15:51:06 2023, max compression
```

## Comparing `PAModelpy-0.0.3.8.tar` & `PAModelpy-0.0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 samiralvdb  (1000) samiralvdb  (1000)        0 2023-12-19 15:47:34.278219 PAModelpy-0.0.3.8/
-drwxrwxr-x   0 samiralvdb  (1000) samiralvdb  (1000)        0 2023-12-19 15:47:34.278219 PAModelpy-0.0.3.8/PAModelpy/
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    16105 2023-12-13 13:48:31.000000 PAModelpy-0.0.3.8/PAModelpy/CatalyticEvent.py
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)     1020 2023-03-31 12:48:23.000000 PAModelpy-0.0.3.8/PAModelpy/Constraints.py
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    29567 2023-12-19 15:46:12.000000 PAModelpy-0.0.3.8/PAModelpy/Enzyme.py
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    14500 2023-11-03 11:26:47.000000 PAModelpy-0.0.3.8/PAModelpy/EnzymeSectors.py
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    23003 2023-10-10 14:21:24.000000 PAModelpy-0.0.3.8/PAModelpy/PAMValidator.py
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    78584 2023-12-19 15:46:12.000000 PAModelpy-0.0.3.8/PAModelpy/PAModel.py
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)       50 2023-12-19 15:34:28.000000 PAModelpy-0.0.3.8/PAModelpy/__init__.py
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)     2058 2023-11-06 12:02:59.000000 PAModelpy-0.0.3.8/PAModelpy/configuration.py
-drwxrwxr-x   0 samiralvdb  (1000) samiralvdb  (1000)        0 2023-12-19 15:47:34.278219 PAModelpy-0.0.3.8/PAModelpy.egg-info/
--rw-r--r--   0 samiralvdb  (1000) samiralvdb  (1000)     3759 2023-12-19 15:47:34.000000 PAModelpy-0.0.3.8/PAModelpy.egg-info/PKG-INFO
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)      384 2023-12-19 15:47:34.000000 PAModelpy-0.0.3.8/PAModelpy.egg-info/SOURCES.txt
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)        1 2023-12-19 15:47:34.000000 PAModelpy-0.0.3.8/PAModelpy.egg-info/dependency_links.txt
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)      142 2023-12-19 15:47:34.000000 PAModelpy-0.0.3.8/PAModelpy.egg-info/requires.txt
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)       10 2023-12-19 15:47:34.000000 PAModelpy-0.0.3.8/PAModelpy.egg-info/top_level.txt
--rw-r--r--   0 samiralvdb  (1000) samiralvdb  (1000)     3759 2023-12-19 15:47:34.278219 PAModelpy-0.0.3.8/PKG-INFO
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)     3062 2023-11-03 16:23:06.000000 PAModelpy-0.0.3.8/README.md
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)      740 2023-12-19 15:34:28.000000 PAModelpy-0.0.3.8/pyproject.toml
--rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)       38 2023-12-19 15:47:34.278219 PAModelpy-0.0.3.8/setup.cfg
+drwxrwxr-x   0 samiralvdb  (1000) samiralvdb  (1000)        0 2023-12-19 15:51:06.654447 PAModelpy-0.0.3.9/
+drwxrwxr-x   0 samiralvdb  (1000) samiralvdb  (1000)        0 2023-12-19 15:51:06.654447 PAModelpy-0.0.3.9/PAModelpy/
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    16105 2023-12-13 13:48:31.000000 PAModelpy-0.0.3.9/PAModelpy/CatalyticEvent.py
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)     1020 2023-03-31 12:48:23.000000 PAModelpy-0.0.3.9/PAModelpy/Constraints.py
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    29567 2023-12-19 15:46:12.000000 PAModelpy-0.0.3.9/PAModelpy/Enzyme.py
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    14500 2023-11-03 11:26:47.000000 PAModelpy-0.0.3.9/PAModelpy/EnzymeSectors.py
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    23003 2023-10-10 14:21:24.000000 PAModelpy-0.0.3.9/PAModelpy/PAMValidator.py
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)    78592 2023-12-19 15:51:00.000000 PAModelpy-0.0.3.9/PAModelpy/PAModel.py
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)       50 2023-12-19 15:51:00.000000 PAModelpy-0.0.3.9/PAModelpy/__init__.py
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)     2058 2023-11-06 12:02:59.000000 PAModelpy-0.0.3.9/PAModelpy/configuration.py
+drwxrwxr-x   0 samiralvdb  (1000) samiralvdb  (1000)        0 2023-12-19 15:51:06.654447 PAModelpy-0.0.3.9/PAModelpy.egg-info/
+-rw-r--r--   0 samiralvdb  (1000) samiralvdb  (1000)     3759 2023-12-19 15:51:06.000000 PAModelpy-0.0.3.9/PAModelpy.egg-info/PKG-INFO
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)      384 2023-12-19 15:51:06.000000 PAModelpy-0.0.3.9/PAModelpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)        1 2023-12-19 15:51:06.000000 PAModelpy-0.0.3.9/PAModelpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)      142 2023-12-19 15:51:06.000000 PAModelpy-0.0.3.9/PAModelpy.egg-info/requires.txt
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)       10 2023-12-19 15:51:06.000000 PAModelpy-0.0.3.9/PAModelpy.egg-info/top_level.txt
+-rw-r--r--   0 samiralvdb  (1000) samiralvdb  (1000)     3759 2023-12-19 15:51:06.654447 PAModelpy-0.0.3.9/PKG-INFO
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)     3062 2023-11-03 16:23:06.000000 PAModelpy-0.0.3.9/README.md
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)      740 2023-12-19 15:51:00.000000 PAModelpy-0.0.3.9/pyproject.toml
+-rw-rw-r--   0 samiralvdb  (1000) samiralvdb  (1000)       38 2023-12-19 15:51:06.654447 PAModelpy-0.0.3.9/setup.cfg
```

### Comparing `PAModelpy-0.0.3.8/PAModelpy/CatalyticEvent.py` & `PAModelpy-0.0.3.9/PAModelpy/CatalyticEvent.py`

 * *Files identical despite different names*

### Comparing `PAModelpy-0.0.3.8/PAModelpy/Constraints.py` & `PAModelpy-0.0.3.9/PAModelpy/Constraints.py`

 * *Files identical despite different names*

### Comparing `PAModelpy-0.0.3.8/PAModelpy/Enzyme.py` & `PAModelpy-0.0.3.9/PAModelpy/Enzyme.py`

 * *Files identical despite different names*

### Comparing `PAModelpy-0.0.3.8/PAModelpy/EnzymeSectors.py` & `PAModelpy-0.0.3.9/PAModelpy/EnzymeSectors.py`

 * *Files identical despite different names*

### Comparing `PAModelpy-0.0.3.8/PAModelpy/PAMValidator.py` & `PAModelpy-0.0.3.9/PAModelpy/PAMValidator.py`

 * *Files identical despite different names*

### Comparing `PAModelpy-0.0.3.8/PAModelpy/PAModel.py` & `PAModelpy-0.0.3.9/PAModelpy/PAModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1653,15 +1653,15 @@
             new._solver = copy(self.solver)  # pragma: no cover
 
         # it doesn't make sense to retain the context of a copied model so
         # assign a new empty context
         new._contexts = []
 
         # copy bounds
-        for key, var in self.variables:
+        for key, var in self.variables.items():
             new.variables[key].lb = var.lb
             new.variables[key].ub = var.ub
 
 
         for key, cons in self.constraints.items():
             new.constraints[key].lb = cons.lb
             new.constraints[key].ub = cons.ub
```

### Comparing `PAModelpy-0.0.3.8/PAModelpy/configuration.py` & `PAModelpy-0.0.3.9/PAModelpy/configuration.py`

 * *Files identical despite different names*

### Comparing `PAModelpy-0.0.3.8/PAModelpy.egg-info/PKG-INFO` & `PAModelpy-0.0.3.9/PAModelpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PAModelpy
-Version: 0.0.3.8
+Version: 0.0.3.9
 Summary: Python framework for building and analysing protein allocation models
 Author-email: Samira van den Bogaard <samira.vandenbogaard@rwth-aachen.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `PAModelpy-0.0.3.8/PKG-INFO` & `PAModelpy-0.0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PAModelpy
-Version: 0.0.3.8
+Version: 0.0.3.9
 Summary: Python framework for building and analysing protein allocation models
 Author-email: Samira van den Bogaard <samira.vandenbogaard@rwth-aachen.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `PAModelpy-0.0.3.8/README.md` & `PAModelpy-0.0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `PAModelpy-0.0.3.8/pyproject.toml` & `PAModelpy-0.0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=68"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'PAModelpy'
-version = '0.0.3.8'
+version = '0.0.3.9'
 authors = [{name='Samira van den Bogaard', email = 'samira.vandenbogaard@rwth-aachen.de'}]
 description = 'Python framework for building and analysing protein allocation models'
 readme = 'README.md'
 requires-python = '>=3.8'
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
```

