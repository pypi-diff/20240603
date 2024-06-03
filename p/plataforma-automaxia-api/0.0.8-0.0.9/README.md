# Comparing `tmp/plataforma-automaxia-api-0.0.8.tar.gz` & `tmp/plataforma-automaxia-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plataforma-automaxia-api-0.0.8.tar", last modified: Fri May 31 13:47:14 2024, max compression
+gzip compressed data, was "plataforma-automaxia-api-0.0.9.tar", last modified: Mon Jun  3 11:23:24 2024, max compression
```

## Comparing `plataforma-automaxia-api-0.0.8.tar` & `plataforma-automaxia-api-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 13:47:14.061403 plataforma-automaxia-api-0.0.8/
--rw-rw-rw-   0        0        0     1109 2023-02-27 17:07:43.000000 plataforma-automaxia-api-0.0.8/LICENCE
--rw-rw-rw-   0        0        0     3845 2024-05-31 13:47:14.060330 plataforma-automaxia-api-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2024-03-27 19:16:26.000000 plataforma-automaxia-api-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 13:47:14.023813 plataforma-automaxia-api-0.0.8/plataforma/
--rw-rw-rw-   0        0        0        0 2022-06-23 22:06:41.000000 plataforma-automaxia-api-0.0.8/plataforma/__init__.py
--rw-rw-rw-   0        0        0    14315 2024-05-31 13:43:11.000000 plataforma-automaxia-api-0.0.8/plataforma/automaxia_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:47:14.038560 plataforma-automaxia-api-0.0.8/plataforma_automaxia_api.egg-info/
--rw-rw-rw-   0        0        0     3845 2024-05-31 13:47:13.000000 plataforma-automaxia-api-0.0.8/plataforma_automaxia_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-05-31 13:47:13.000000 plataforma-automaxia-api-0.0.8/plataforma_automaxia_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 13:47:13.000000 plataforma-automaxia-api-0.0.8/plataforma_automaxia_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 13:47:13.000000 plataforma-automaxia-api-0.0.8/plataforma_automaxia_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-31 13:47:13.000000 plataforma-automaxia-api-0.0.8/plataforma_automaxia_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 13:47:14.061403 plataforma-automaxia-api-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-31 13:47:05.000000 plataforma-automaxia-api-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:23:24.417523 plataforma-automaxia-api-0.0.9/
+-rw-rw-rw-   0        0        0     1109 2023-02-27 17:07:43.000000 plataforma-automaxia-api-0.0.9/LICENCE
+-rw-rw-rw-   0        0        0     3845 2024-06-03 11:23:24.417523 plataforma-automaxia-api-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2024-05-31 13:48:34.000000 plataforma-automaxia-api-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:23:24.381927 plataforma-automaxia-api-0.0.9/plataforma/
+-rw-rw-rw-   0        0        0        0 2022-06-23 22:06:41.000000 plataforma-automaxia-api-0.0.9/plataforma/__init__.py
+-rw-rw-rw-   0        0        0    14526 2024-06-03 11:16:14.000000 plataforma-automaxia-api-0.0.9/plataforma/automaxia_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:23:24.414518 plataforma-automaxia-api-0.0.9/plataforma_automaxia_api.egg-info/
+-rw-rw-rw-   0        0        0     3845 2024-06-03 11:23:24.000000 plataforma-automaxia-api-0.0.9/plataforma_automaxia_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-06-03 11:23:24.000000 plataforma-automaxia-api-0.0.9/plataforma_automaxia_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:23:24.000000 plataforma-automaxia-api-0.0.9/plataforma_automaxia_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 11:23:24.000000 plataforma-automaxia-api-0.0.9/plataforma_automaxia_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-03 11:23:24.000000 plataforma-automaxia-api-0.0.9/plataforma_automaxia_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:23:24.418525 plataforma-automaxia-api-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-06-03 11:23:16.000000 plataforma-automaxia-api-0.0.9/setup.py
```

### Comparing `plataforma-automaxia-api-0.0.8/LICENCE` & `plataforma-automaxia-api-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `plataforma-automaxia-api-0.0.8/PKG-INFO` & `plataforma-automaxia-api-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plataforma-automaxia-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper oficial da Plataforma Automaxia para Python
 Home-page: UNKNOWN
 Author: Wesley Romualdo da Silva
 Author-email: wesleyromualdo@gmail.com
 License: MIT License
 Keywords: plataforma automaxia api
 Platform: UNKNOWN
@@ -121,14 +121,14 @@
 
 Ou para criar um repositÃ³rio oficial:
 
 ```plain
 python setup.py sdist
 twine upload dist/*
 user: __token__
-pass: pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8
+pass: pypi-AgEIcHlwaS5vcmcCJDhiMzljNDhmLWQ2YjUtNGY1ZS04ZWZjLTg5YjA1ZTZjMDVmZQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgmdGilNV_eODFwDGMeZpV7To11QOciChvPuZrh00DX10
 
 
-twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8 dist/*
+twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJDhiMzljNDhmLWQ2YjUtNGY1ZS04ZWZjLTg5YjA1ZTZjMDVmZQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgmdGilNV_eODFwDGMeZpV7To11QOciChvPuZrh00DX10 dist/*
 ```
 pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
```

### Comparing `plataforma-automaxia-api-0.0.8/README.md` & `plataforma-automaxia-api-0.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -108,13 +108,13 @@
 
 Ou para criar um repositório oficial:
 
 ```plain
 python setup.py sdist
 twine upload dist/*
 user: __token__
-pass: pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8
+pass: pypi-AgEIcHlwaS5vcmcCJDhiMzljNDhmLWQ2YjUtNGY1ZS04ZWZjLTg5YjA1ZTZjMDVmZQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgmdGilNV_eODFwDGMeZpV7To11QOciChvPuZrh00DX10
 
 
-twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8 dist/*
+twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJDhiMzljNDhmLWQ2YjUtNGY1ZS04ZWZjLTg5YjA1ZTZjMDVmZQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgmdGilNV_eODFwDGMeZpV7To11QOciChvPuZrh00DX10 dist/*
 ```
 pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
```

### Comparing `plataforma-automaxia-api-0.0.8/plataforma/automaxia_api.py` & `plataforma-automaxia-api-0.0.9/plataforma/automaxia_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,19 @@
         response = self.get(url)
         return response
 
     def get_logs_by_id_historico(self, historico_tarefa_id):
         url = str(self.url)+"/logs/historico-tarefa/"+str(historico_tarefa_id)
         response = self.get(url)
         return response
+    
+    def get_historico_tarefa_by_id(self, historico_tarefa_id):
+        url = str(self.url)+"/tarefa/historico-tarefa/"+str(historico_tarefa_id)
+        response = self.get(url)
+        return response
 
     def get_automacao_by_id_json(self, automacao_id):
         url = str(self.url)+"/automacao/worker/"+str(automacao_id)
         response = self.get(url)
         return response
 
     def get_automacao_by_constante_virtual_json(self, constante_virtual):
```

### Comparing `plataforma-automaxia-api-0.0.8/plataforma_automaxia_api.egg-info/PKG-INFO` & `plataforma-automaxia-api-0.0.9/plataforma_automaxia_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plataforma-automaxia-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper oficial da Plataforma Automaxia para Python
 Home-page: UNKNOWN
 Author: Wesley Romualdo da Silva
 Author-email: wesleyromualdo@gmail.com
 License: MIT License
 Keywords: plataforma automaxia api
 Platform: UNKNOWN
@@ -121,14 +121,14 @@
 
 Ou para criar um repositÃ³rio oficial:
 
 ```plain
 python setup.py sdist
 twine upload dist/*
 user: __token__
-pass: pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8
+pass: pypi-AgEIcHlwaS5vcmcCJDhiMzljNDhmLWQ2YjUtNGY1ZS04ZWZjLTg5YjA1ZTZjMDVmZQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgmdGilNV_eODFwDGMeZpV7To11QOciChvPuZrh00DX10
 
 
-twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8 dist/*
+twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJDhiMzljNDhmLWQ2YjUtNGY1ZS04ZWZjLTg5YjA1ZTZjMDVmZQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgmdGilNV_eODFwDGMeZpV7To11QOciChvPuZrh00DX10 dist/*
 ```
 pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
```

### Comparing `plataforma-automaxia-api-0.0.8/setup.py` & `plataforma-automaxia-api-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='plataforma-automaxia-api',
-    version='0.0.8',
+    version='0.0.9',
     license='MIT License',
     author='Wesley Romualdo da Silva',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='wesleyromualdo@gmail.com',
     keywords='plataforma automaxia api',
     description=u'Wrapper oficial da Plataforma Automaxia para Python',
```

