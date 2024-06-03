# Comparing `tmp/tmp_box-0.0.6.tar.gz` & `tmp/tmp_box-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmp_box-0.0.6.tar", last modified: Mon Jun  3 11:53:53 2024, max compression
+gzip compressed data, was "tmp_box-0.0.7.tar", last modified: Mon Jun  3 12:16:14 2024, max compression
```

## Comparing `tmp_box-0.0.6.tar` & `tmp_box-0.0.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.210680 tmp_box-0.0.6/
--rw-rw-rw-   0        0        0       40 2024-06-02 13:45:44.000000 tmp_box-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      116 2024-06-03 11:53:53.209678 tmp_box-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        5 2024-06-02 13:27:59.000000 tmp_box-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.074172 tmp_box-0.0.6/app/
--rw-rw-rw-   0        0        0       21 2024-06-02 13:23:31.000000 tmp_box-0.0.6/app/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.077173 tmp_box-0.0.6/app/base/
--rw-rw-rw-   0        0        0        0 2024-06-02 05:39:47.000000 tmp_box-0.0.6/app/base/__init__.py
--rw-rw-rw-   0        0        0     1905 2024-06-02 09:59:51.000000 tmp_box-0.0.6/app/base/abstract.py
--rw-rw-rw-   0        0        0      824 2024-05-30 15:12:39.000000 tmp_box-0.0.6/app/context.py
--rw-rw-rw-   0        0        0     2585 2024-06-02 16:01:15.000000 tmp_box-0.0.6/app/main.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.096181 tmp_box-0.0.6/app/models/
--rw-rw-rw-   0        0        0        0 2024-05-30 06:13:56.000000 tmp_box-0.0.6/app/models/__init__.py
--rw-rw-rw-   0        0        0      356 2024-05-30 09:42:34.000000 tmp_box-0.0.6/app/models/path_models.py
--rw-rw-rw-   0        0        0      189 2024-05-30 10:34:46.000000 tmp_box-0.0.6/app/models/settings_model.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.100173 tmp_box-0.0.6/app/repositories/
--rw-rw-rw-   0        0        0        0 2024-05-30 06:13:23.000000 tmp_box-0.0.6/app/repositories/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.117179 tmp_box-0.0.6/app/repositories/json_dir/
--rw-rw-rw-   0        0        0       62 2024-06-02 10:00:23.000000 tmp_box-0.0.6/app/repositories/json_dir/last_template.json
--rw-rw-rw-   0        0        0      172 2024-06-02 15:27:08.000000 tmp_box-0.0.6/app/repositories/json_dir/saved_templates.json
--rw-rw-rw-   0        0        0     1716 2024-06-02 16:01:15.000000 tmp_box-0.0.6/app/repositories/json_repositories.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.120174 tmp_box-0.0.6/app/routers/
--rw-rw-rw-   0        0        0        0 2024-05-31 08:25:26.000000 tmp_box-0.0.6/app/routers/__init__.py
--rw-rw-rw-   0        0        0     3042 2024-06-02 16:01:15.000000 tmp_box-0.0.6/app/routers/view.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.155008 tmp_box-0.0.6/app/services/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:29:44.000000 tmp_box-0.0.6/app/services/__init__.py
--rw-rw-rw-   0        0        0     1200 2024-06-02 09:59:50.000000 tmp_box-0.0.6/app/services/from_alias.py
--rw-rw-rw-   0        0        0     1273 2024-06-02 09:59:50.000000 tmp_box-0.0.6/app/services/from_last.py
--rw-rw-rw-   0        0        0      887 2024-06-02 09:59:50.000000 tmp_box-0.0.6/app/services/from_path.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.163972 tmp_box-0.0.6/app/utils/
--rw-rw-rw-   0        0        0        0 2024-05-30 06:14:54.000000 tmp_box-0.0.6/app/utils/__init__.py
--rw-rw-rw-   0        0        0      588 2024-05-30 08:57:58.000000 tmp_box-0.0.6/app/utils/models_utils.py
--rw-rw-rw-   0        0        0     2609 2024-06-02 07:04:20.000000 tmp_box-0.0.6/app/utils/path_utils.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.187709 tmp_box-0.0.6/app/visualize/
--rw-rw-rw-   0        0        0        0 2024-06-01 09:01:24.000000 tmp_box-0.0.6/app/visualize/__init__.py
--rw-rw-rw-   0        0        0      795 2024-06-01 09:36:54.000000 tmp_box-0.0.6/app/visualize/facade.py
--rw-rw-rw-   0        0        0      376 2024-06-01 09:32:22.000000 tmp_box-0.0.6/app/visualize/readers.py
--rw-rw-rw-   0        0        0      869 2024-06-01 09:36:54.000000 tmp_box-0.0.6/app/visualize/visualizers.py
--rw-rw-rw-   0        0        0       42 2024-06-03 11:53:53.210680 tmp_box-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      485 2024-06-03 11:53:50.000000 tmp_box-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 11:53:53.208679 tmp_box-0.0.6/tmp_box.egg-info/
--rw-rw-rw-   0        0        0      116 2024-06-03 11:53:53.000000 tmp_box-0.0.6/tmp_box.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2024-06-03 11:53:53.000000 tmp_box-0.0.6/tmp_box.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 11:53:53.000000 tmp_box-0.0.6/tmp_box.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-06-03 11:53:53.000000 tmp_box-0.0.6/tmp_box.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-06-03 11:53:53.000000 tmp_box-0.0.6/tmp_box.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-06-03 11:53:53.000000 tmp_box-0.0.6/tmp_box.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.676437 tmp_box-0.0.7/
+-rw-rw-rw-   0        0        0       40 2024-06-02 13:45:44.000000 tmp_box-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      116 2024-06-03 12:16:14.675435 tmp_box-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2024-06-02 13:27:59.000000 tmp_box-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.634437 tmp_box-0.0.7/app/
+-rw-rw-rw-   0        0        0       21 2024-06-02 13:23:31.000000 tmp_box-0.0.7/app/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.635441 tmp_box-0.0.7/app/base/
+-rw-rw-rw-   0        0        0        0 2024-06-02 05:39:47.000000 tmp_box-0.0.7/app/base/__init__.py
+-rw-rw-rw-   0        0        0     1905 2024-06-02 09:59:51.000000 tmp_box-0.0.7/app/base/abstract.py
+-rw-rw-rw-   0        0        0      824 2024-05-30 15:12:39.000000 tmp_box-0.0.7/app/context.py
+-rw-rw-rw-   0        0        0     2585 2024-06-02 16:01:15.000000 tmp_box-0.0.7/app/main.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.638435 tmp_box-0.0.7/app/models/
+-rw-rw-rw-   0        0        0        0 2024-05-30 06:13:56.000000 tmp_box-0.0.7/app/models/__init__.py
+-rw-rw-rw-   0        0        0      356 2024-05-30 09:42:34.000000 tmp_box-0.0.7/app/models/path_models.py
+-rw-rw-rw-   0        0        0      189 2024-05-30 10:34:46.000000 tmp_box-0.0.7/app/models/settings_model.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.640437 tmp_box-0.0.7/app/repositories/
+-rw-rw-rw-   0        0        0        0 2024-05-30 06:13:23.000000 tmp_box-0.0.7/app/repositories/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.642442 tmp_box-0.0.7/app/repositories/json_dir/
+-rw-rw-rw-   0        0        0       62 2024-06-02 10:00:23.000000 tmp_box-0.0.7/app/repositories/json_dir/last_template.json
+-rw-rw-rw-   0        0        0      172 2024-06-02 15:27:08.000000 tmp_box-0.0.7/app/repositories/json_dir/saved_templates.json
+-rw-rw-rw-   0        0        0     1716 2024-06-02 16:01:15.000000 tmp_box-0.0.7/app/repositories/json_repositories.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.644437 tmp_box-0.0.7/app/routers/
+-rw-rw-rw-   0        0        0        0 2024-05-31 08:25:26.000000 tmp_box-0.0.7/app/routers/__init__.py
+-rw-rw-rw-   0        0        0     3042 2024-06-02 16:01:15.000000 tmp_box-0.0.7/app/routers/view.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.648435 tmp_box-0.0.7/app/services/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:29:44.000000 tmp_box-0.0.7/app/services/__init__.py
+-rw-rw-rw-   0        0        0     1200 2024-06-02 09:59:50.000000 tmp_box-0.0.7/app/services/from_alias.py
+-rw-rw-rw-   0        0        0     1273 2024-06-02 09:59:50.000000 tmp_box-0.0.7/app/services/from_last.py
+-rw-rw-rw-   0        0        0      887 2024-06-02 09:59:50.000000 tmp_box-0.0.7/app/services/from_path.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.651435 tmp_box-0.0.7/app/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-30 06:14:54.000000 tmp_box-0.0.7/app/utils/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-05-30 08:57:58.000000 tmp_box-0.0.7/app/utils/models_utils.py
+-rw-rw-rw-   0        0        0     2609 2024-06-02 07:04:20.000000 tmp_box-0.0.7/app/utils/path_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.654435 tmp_box-0.0.7/app/visualize/
+-rw-rw-rw-   0        0        0        0 2024-06-01 09:01:24.000000 tmp_box-0.0.7/app/visualize/__init__.py
+-rw-rw-rw-   0        0        0      942 2024-06-03 12:16:07.000000 tmp_box-0.0.7/app/visualize/facade.py
+-rw-rw-rw-   0        0        0      376 2024-06-01 09:32:22.000000 tmp_box-0.0.7/app/visualize/readers.py
+-rw-rw-rw-   0        0        0      869 2024-06-01 09:36:54.000000 tmp_box-0.0.7/app/visualize/visualizers.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 12:16:14.677436 tmp_box-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      487 2024-06-03 12:16:07.000000 tmp_box-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 12:16:14.674436 tmp_box-0.0.7/tmp_box.egg-info/
+-rw-rw-rw-   0        0        0      116 2024-06-03 12:16:14.000000 tmp_box-0.0.7/tmp_box.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2024-06-03 12:16:14.000000 tmp_box-0.0.7/tmp_box.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 12:16:14.000000 tmp_box-0.0.7/tmp_box.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-06-03 12:16:14.000000 tmp_box-0.0.7/tmp_box.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-06-03 12:16:14.000000 tmp_box-0.0.7/tmp_box.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-06-03 12:16:14.000000 tmp_box-0.0.7/tmp_box.egg-info/top_level.txt
```

### Comparing `tmp_box-0.0.6/app/base/abstract.py` & `tmp_box-0.0.7/app/base/abstract.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/context.py` & `tmp_box-0.0.7/app/context.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/main.py` & `tmp_box-0.0.7/app/main.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/repositories/json_repositories.py` & `tmp_box-0.0.7/app/repositories/json_repositories.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/routers/view.py` & `tmp_box-0.0.7/app/routers/view.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/services/from_alias.py` & `tmp_box-0.0.7/app/services/from_alias.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/services/from_last.py` & `tmp_box-0.0.7/app/services/from_last.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/services/from_path.py` & `tmp_box-0.0.7/app/services/from_path.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/utils/models_utils.py` & `tmp_box-0.0.7/app/utils/models_utils.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/utils/path_utils.py` & `tmp_box-0.0.7/app/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/app/visualize/facade.py` & `tmp_box-0.0.7/app/visualize/facade.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,7 +17,11 @@
 
 	def execute(self, path: Path):
 		suffix = path.suffix
 		if suffix in self.__dict_suffix__:
 			visualizer, reader = self.__dict_suffix__[suffix]
 			renderable = visualizer(reader=reader()).visualize(path)
 			self.console.print(renderable)
+		else:
+			visualizer = TextualVisualizer(reader=TextualReader())
+			renderable = visualizer.visualize(path)
+			self.console.print(renderable)
```

### Comparing `tmp_box-0.0.6/app/visualize/visualizers.py` & `tmp_box-0.0.7/app/visualize/visualizers.py`

 * *Files identical despite different names*

### Comparing `tmp_box-0.0.6/tmp_box.egg-info/SOURCES.txt` & `tmp_box-0.0.7/tmp_box.egg-info/SOURCES.txt`

 * *Files identical despite different names*

