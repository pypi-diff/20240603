# Comparing `tmp/processing_pypelines-0.0.62.tar.gz` & `tmp/processing_pypelines-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing_pypelines-0.0.62.tar", last modified: Fri May 31 16:21:09 2024, max compression
+gzip compressed data, was "processing_pypelines-0.0.63.tar", last modified: Mon Jun  3 12:00:55 2024, max compression
```

## Comparing `processing_pypelines-0.0.62.tar` & `processing_pypelines-0.0.63.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2024-05-31 16:21:00.614107 processing_pypelines-0.0.62/LICENSE
--rw-r--r--   0        0        0      118 2024-05-31 16:21:00.614107 processing_pypelines-0.0.62/README.md
--rw-r--r--   0        0        0     1152 2024-05-31 16:21:09.805964 processing_pypelines-0.0.62/pyproject.toml
--rw-r--r--   0        0        0      367 2024-05-31 16:21:00.618106 processing_pypelines-0.0.62/src/pypelines/__init__.py
--rw-r--r--   0        0        0     4483 2024-05-31 16:21:00.618106 processing_pypelines-0.0.62/src/pypelines/accessors.py
--rw-r--r--   0        0        0     4671 2024-05-31 16:21:00.618106 processing_pypelines-0.0.62/src/pypelines/arguments.py
--rw-r--r--   0        0        0    34304 2024-05-31 16:21:00.618106 processing_pypelines-0.0.62/src/pypelines/celery_tasks.py
--rw-r--r--   0        0        0    11851 2024-05-31 16:21:00.618106 processing_pypelines-0.0.62/src/pypelines/disk.py
--rw-r--r--   0        0        0     6647 2024-05-31 16:21:00.618106 processing_pypelines-0.0.62/src/pypelines/examples.py
--rw-r--r--   0        0        0   352259 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/feature_test.ipynb
--rw-r--r--   0        0        0     7880 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/graphs.py
--rw-r--r--   0        0        0    17630 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/loggs.py
--rw-r--r--   0        0        0     5985 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/multisession.py
--rw-r--r--   0        0        0    18914 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/pickle_backend.py
--rw-r--r--   0        0        0     6559 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/pipelines.py
--rw-r--r--   0        0        0     9547 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/pipes.py
--rw-r--r--   0        0        0     3084 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/sessions.py
--rw-r--r--   0        0        0    36861 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/steps.py
--rw-r--r--   0        0        0     3915 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/tasks.py
--rw-r--r--   0        0        0     7360 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/src/pypelines/versions.py
--rw-r--r--   0        0        0        0 2024-05-31 16:21:00.698105 processing_pypelines-0.0.62/tests/__init__.py
--rw-r--r--   0        0        0      962 2024-05-31 16:21:00.622106 processing_pypelines-0.0.62/tests/tests.py
--rw-r--r--   0        0        0     1230 2024-05-31 16:21:00.626106 processing_pypelines-0.0.62/tests/versions_example.json
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.62/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-06-03 12:00:45.684462 processing_pypelines-0.0.63/LICENSE
+-rw-r--r--   0        0        0      118 2024-06-03 12:00:45.684462 processing_pypelines-0.0.63/README.md
+-rw-r--r--   0        0        0     1152 2024-06-03 12:00:55.020318 processing_pypelines-0.0.63/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-06-03 12:00:45.684462 processing_pypelines-0.0.63/src/pypelines/__init__.py
+-rw-r--r--   0        0        0     4483 2024-06-03 12:00:45.684462 processing_pypelines-0.0.63/src/pypelines/accessors.py
+-rw-r--r--   0        0        0     4671 2024-06-03 12:00:45.684462 processing_pypelines-0.0.63/src/pypelines/arguments.py
+-rw-r--r--   0        0        0    34304 2024-06-03 12:00:45.688462 processing_pypelines-0.0.63/src/pypelines/celery_tasks.py
+-rw-r--r--   0        0        0    11851 2024-06-03 12:00:45.688462 processing_pypelines-0.0.63/src/pypelines/disk.py
+-rw-r--r--   0        0        0     6647 2024-06-03 12:00:45.688462 processing_pypelines-0.0.63/src/pypelines/examples.py
+-rw-r--r--   0        0        0   352259 2024-06-03 12:00:45.688462 processing_pypelines-0.0.63/src/pypelines/feature_test.ipynb
+-rw-r--r--   0        0        0     7880 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/graphs.py
+-rw-r--r--   0        0        0    17630 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/loggs.py
+-rw-r--r--   0        0        0     5985 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/multisession.py
+-rw-r--r--   0        0        0    18914 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/pickle_backend.py
+-rw-r--r--   0        0        0     6559 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/pipelines.py
+-rw-r--r--   0        0        0     9547 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/pipes.py
+-rw-r--r--   0        0        0     3084 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/sessions.py
+-rw-r--r--   0        0        0    37059 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/steps.py
+-rw-r--r--   0        0        0     3915 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/tasks.py
+-rw-r--r--   0        0        0     7360 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/src/pypelines/versions.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:00:45.740461 processing_pypelines-0.0.63/tests/__init__.py
+-rw-r--r--   0        0        0      962 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/tests/tests.py
+-rw-r--r--   0        0        0     1230 2024-06-03 12:00:45.692462 processing_pypelines-0.0.63/tests/versions_example.json
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.63/PKG-INFO
```

### Comparing `processing_pypelines-0.0.62/LICENSE` & `processing_pypelines-0.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/pyproject.toml` & `processing_pypelines-0.0.63/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 maintainers = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 description = "Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = []
-version = "0.0.62"
+version = "0.0.63"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 celery = [
     "celery>=5.3.5",
```

### Comparing `processing_pypelines-0.0.62/src/pypelines/accessors.py` & `processing_pypelines-0.0.63/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/arguments.py` & `processing_pypelines-0.0.63/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/celery_tasks.py` & `processing_pypelines-0.0.63/src/pypelines/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/disk.py` & `processing_pypelines-0.0.63/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/examples.py` & `processing_pypelines-0.0.63/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/feature_test.ipynb` & `processing_pypelines-0.0.63/src/pypelines/feature_test.ipynb`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/graphs.py` & `processing_pypelines-0.0.63/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/loggs.py` & `processing_pypelines-0.0.63/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/multisession.py` & `processing_pypelines-0.0.63/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/pickle_backend.py` & `processing_pypelines-0.0.63/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/pipelines.py` & `processing_pypelines-0.0.63/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/pipes.py` & `processing_pypelines-0.0.63/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/sessions.py` & `processing_pypelines-0.0.63/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/steps.py` & `processing_pypelines-0.0.63/src/pypelines/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,18 +184,17 @@
         return self.get_save_wrapped()
 
     @property
     def generate(self):
         """Return the result of calling the get_generate_wrapped method."""
         return self.get_generate_wrapped()
 
-    # def make_wrapped_functions(self):
-    #     self.save = self.make_wrapped_save()
-    #     self.load = self.make_wrapped_load()
-    #     self.generate = self.make_wrapped_generate()
+    @property
+    def run_callbacks(self):
+        return self.get_run_callbacks()
 
     def get_save_wrapped(self):
         """Returns a wrapped function that saves data using the disk class.
 
         This function wraps the save method of the disk class with additional functionality.
 
         Args:
@@ -284,14 +283,41 @@
         if self.do_dispatch:
             return autoload_arguments(
                 self.pipe.dispatcher(loggedmethod(self.generation_mechanism), "generator"),
                 self,
             )
         return autoload_arguments(loggedmethod(self.generation_mechanism), self)
 
+    def get_run_callbacks(self):
+        def wrapper(session, extra="", show_plots=True):
+            logger = logging.getLogger("callback_runner")
+            for callback_data in self.callbacks:
+                arguments = {"session": session, "extra": extra, "pipeline": self.pipeline}
+                if isinstance(callback_data, tuple):
+                    callback = callback_data[0]
+                    overriding_arguments = callback_data[1]
+                else:
+                    callback = callback_data
+                    overriding_arguments = {}
+                arguments.update(overriding_arguments)
+                on_what = f"{session.alias}.{extra}" if extra else session.alias
+                try:
+                    logger.info(f"Running the callback {callback.__name__} on {on_what}")
+                    callback(**arguments)
+                except Exception as e:
+                    import traceback
+
+                    traceback_msg = traceback.format_exc()
+                    logger.error(f"The callback {callback} failed with error : {e}")
+                    logger.error(f"Full traceback below :\n{traceback_msg}")
+
+        if self.do_dispatch:
+            return self.pipe.dispatcher(wrapper, "callbacks")
+        return wrapper
+
     def get_level(self, selfish=False) -> int:
         """Get the level of the step.
 
         Args:
             selfish (bool): Whether to calculate the level selfishly. Defaults to False.
 
         Returns:
@@ -517,15 +543,15 @@
             if self.is_refresh_in_kwargs():
                 kwargs.update({"refresh": refresh})
             result = self.pipe.pre_run_wrapper(self.worker(session, *args, **kwargs))
 
             if save_output:
                 logger.save(f"Saving the generated {self.relative_name}{'.' + extra if extra else ''} output.")
                 disk_object.save(result)
-                self.run_callbacks(session, extra, show_plots=False)
+                self.run_callbacks(session, extra=extra, show_plots=False)
 
             return result
 
         original_signature = inspect.signature(self.worker)
         original_params = list(original_signature.parameters.values())
 
         kwarg_position = len(original_params)
@@ -551,35 +577,14 @@
 
         # Replace the wrapper function's signature with the new one
         wrapper.__signature__ = original_signature.replace(parameters=original_params)
         wrapper.__doc__ = self.generate_doc()
 
         return wrapper
 
-    def run_callbacks(self, session, extra="", show_plots=True) -> None:
-        logger = logging.getLogger("callback_runner")
-        for callback_data in self.callbacks:
-            arguments = {"session": session, "extra": extra, "pipeline": self.pipeline}
-            if isinstance(callback_data, tuple):
-                callback = callback_data[0]
-                overriding_arguments = callback_data[1]
-            else:
-                callback = callback_data
-                overriding_arguments = {}
-            arguments.update(overriding_arguments)
-            try:
-                logger.info(f"Running the callback {callback.__name__}")
-                callback(**arguments)
-            except Exception as e:
-                import traceback
-
-                traceback_msg = traceback.format_exc()
-                logger.error(f"The callback {callback} failed with error : {e}")
-                logger.error("Full traceback below :\n" + traceback_msg)
-
     def generate_doc(self) -> str:
         """Generate a new docstring by inserting a chapter about Pipeline Args before the existing
         docstring of the function.
         If the existing docstring contains 'Raises' or 'Returns', the new chapter will be inserted before that.
         If not, it will be inserted at the end of the existing docstring.
         """
```

### Comparing `processing_pypelines-0.0.62/src/pypelines/tasks.py` & `processing_pypelines-0.0.63/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/src/pypelines/versions.py` & `processing_pypelines-0.0.63/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/tests/tests.py` & `processing_pypelines-0.0.63/tests/tests.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/tests/versions_example.json` & `processing_pypelines-0.0.63/tests/versions_example.json`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.62/PKG-INFO` & `processing_pypelines-0.0.63/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.62
+Version: 0.0.63
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Home-page: https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Author-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 Maintainer-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: Repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

