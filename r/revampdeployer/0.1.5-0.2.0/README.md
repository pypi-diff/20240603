# Comparing `tmp/revampdeployer-0.1.5.tar.gz` & `tmp/revampdeployer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revampdeployer-0.1.5.tar", last modified: Tue May 21 13:36:07 2024, max compression
+gzip compressed data, was "revampdeployer-0.2.0.tar", last modified: Sun Jun  2 14:39:18 2024, max compression
```

## Comparing `revampdeployer-0.1.5.tar` & `revampdeployer-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 13:36:07.969186 revampdeployer-0.1.5/
--rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.1.5/LICENSE
--rw-r--r--   0 evsi       (501) staff       (20)     1943 2024-05-21 13:36:07.968869 revampdeployer-0.1.5/PKG-INFO
--rw-r--r--   0 evsi       (501) staff       (20)     1821 2024-05-21 13:35:32.000000 revampdeployer-0.1.5/README.md
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 13:36:07.967629 revampdeployer-0.1.5/revampdeployer/
--rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.1.5/revampdeployer/__init__.py
--rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.1.5/revampdeployer/__main__.py
--rw-r--r--   0 evsi       (501) staff       (20)     7178 2024-05-21 13:26:49.000000 revampdeployer-0.1.5/revampdeployer/deployer.py
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 13:36:07.968589 revampdeployer-0.1.5/revampdeployer.egg-info/
--rw-r--r--   0 evsi       (501) staff       (20)     1943 2024-05-21 13:36:07.000000 revampdeployer-0.1.5/revampdeployer.egg-info/PKG-INFO
--rw-r--r--   0 evsi       (501) staff       (20)      300 2024-05-21 13:36:07.000000 revampdeployer-0.1.5/revampdeployer.egg-info/SOURCES.txt
--rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-21 13:36:07.000000 revampdeployer-0.1.5/revampdeployer.egg-info/dependency_links.txt
--rw-r--r--   0 evsi       (501) staff       (20)       64 2024-05-21 13:36:07.000000 revampdeployer-0.1.5/revampdeployer.egg-info/entry_points.txt
--rw-r--r--   0 evsi       (501) staff       (20)       15 2024-05-21 13:36:07.000000 revampdeployer-0.1.5/revampdeployer.egg-info/top_level.txt
--rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-21 13:36:07.969236 revampdeployer-0.1.5/setup.cfg
--rw-r--r--   0 evsi       (501) staff       (20)      558 2024-05-21 13:35:44.000000 revampdeployer-0.1.5/setup.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-06-02 14:39:18.035564 revampdeployer-0.2.0/
+-rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.2.0/LICENSE
+-rw-r--r--   0 evsi       (501) staff       (20)     1934 2024-06-02 14:39:18.035246 revampdeployer-0.2.0/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)     1812 2024-06-02 14:33:52.000000 revampdeployer-0.2.0/README.md
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-06-02 14:39:18.034134 revampdeployer-0.2.0/revampdeployer/
+-rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.2.0/revampdeployer/__init__.py
+-rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.2.0/revampdeployer/__main__.py
+-rw-r--r--   0 evsi       (501) staff       (20)     7715 2024-06-02 14:36:16.000000 revampdeployer-0.2.0/revampdeployer/deployer.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-06-02 14:39:18.034989 revampdeployer-0.2.0/revampdeployer.egg-info/
+-rw-r--r--   0 evsi       (501) staff       (20)     1934 2024-06-02 14:39:17.000000 revampdeployer-0.2.0/revampdeployer.egg-info/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)      300 2024-06-02 14:39:18.000000 revampdeployer-0.2.0/revampdeployer.egg-info/SOURCES.txt
+-rw-r--r--   0 evsi       (501) staff       (20)        1 2024-06-02 14:39:17.000000 revampdeployer-0.2.0/revampdeployer.egg-info/dependency_links.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       64 2024-06-02 14:39:17.000000 revampdeployer-0.2.0/revampdeployer.egg-info/entry_points.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       15 2024-06-02 14:39:17.000000 revampdeployer-0.2.0/revampdeployer.egg-info/top_level.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       38 2024-06-02 14:39:18.035664 revampdeployer-0.2.0/setup.cfg
+-rw-r--r--   0 evsi       (501) staff       (20)      558 2024-06-02 14:38:56.000000 revampdeployer-0.2.0/setup.py
```

### Comparing `revampdeployer-0.1.5/LICENSE` & `revampdeployer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revampdeployer-0.1.5/PKG-INFO` & `revampdeployer-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revampdeployer
-Version: 0.1.5
+Version: 0.2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RevampDeployer
 
 RevampDeployer is a tool for managing and automating the deployment process of applications to remote servers.
 
@@ -43,19 +43,19 @@
         "address": "192.168.1.2",
         "username": "admin",
         "password": "password2"
     },
     # Other servers...
 }
 
-local_scripts_dir = "local_scripts/"  # Директория локальных скриптов
-scripts_dir = "scripts/"  # Директория скриптов для выполнения на сервере
-input_dir = "input/"  # Директория с файлами для отправки на сервер
-output_dir = "output/"  # Директория для размещения файлов на сервере
-scripts_dir_deploy = "deploy_scripts/"  # Директория скриптов для пост-деплой конфигурации
+local_scripts = "local_scripts/"  # Директория локальных скриптов
+predeploy_scripts = "scripts/"  # Директория скриптов для выполнения на сервере
+dist = "input/"  # Директория с файлами для отправки на сервер
+dest = "output/"  # Директория для размещения файлов на сервере
+postdeploy_scripts = "deploy_scripts/"  # Директория скриптов для пост-деплой конфигурации
 ```
 
 This file should contain a list of servers, script directories, input and output directories, etc. Make sure all parameters are correct and match your environment.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for additional information.
```

### Comparing `revampdeployer-0.1.5/README.md` & `revampdeployer-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,19 +37,19 @@
         "address": "192.168.1.2",
         "username": "admin",
         "password": "password2"
     },
     # Other servers...
 }
 
-local_scripts_dir = "local_scripts/"  # Директория локальных скриптов
-scripts_dir = "scripts/"  # Директория скриптов для выполнения на сервере
-input_dir = "input/"  # Директория с файлами для отправки на сервер
-output_dir = "output/"  # Директория для размещения файлов на сервере
-scripts_dir_deploy = "deploy_scripts/"  # Директория скриптов для пост-деплой конфигурации
+local_scripts = "local_scripts/"  # Директория локальных скриптов
+predeploy_scripts = "scripts/"  # Директория скриптов для выполнения на сервере
+dist = "input/"  # Директория с файлами для отправки на сервер
+dest = "output/"  # Директория для размещения файлов на сервере
+postdeploy_scripts = "deploy_scripts/"  # Директория скриптов для пост-деплой конфигурации
 ```
 
 This file should contain a list of servers, script directories, input and output directories, etc. Make sure all parameters are correct and match your environment.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for additional information.
```

### Comparing `revampdeployer-0.1.5/revampdeployer/deployer.py` & `revampdeployer-0.2.0/revampdeployer/deployer.py`

 * *Files 13% similar despite different names*

```diff
@@ -166,19 +166,31 @@
     if len(sys.argv) != 2:
         logger.error("Usage: deployer.py <server_name>")
         sys.exit(1)
 
     server_name = sys.argv[1]
 
     # Получаем конфигурации из config.py
-    scripts_dir = config.scripts_dir
-    input_dir = config.input_dir
-    output_dir = config.output_dir
-    local_dir = config.local_scripts_dir
-    scripts_dir_deploy = config.scripts_dir_deploy
+    scripts_dir = config.predeploy_scripts
+    input_dir = config.dist
+    output_dir = config.dest
+    local_dir = config.local_scripts
+    scripts_dir_deploy = config.postdeploy_scripts
+
+    if not os.path.isdir(scripts_dir):
+        logger.error(f"The directory {scripts_dir} does not exist.")
+    if not os.path.isdir(input_dir):
+        logger.error(f"The directory {input_dir} does not exist.")
+    if not os.path.isdir(output_dir):
+        logger.error(f"The directory {output_dir} does not exist.")
+    if not os.path.isdir(local_dir):
+        logger.error(f"The directory {local_dir} does not exist.")
+    if not os.path.isdir(scripts_dir_deploy):
+        logger.error(f"The directory {scripts_dir_deploy} does not exist.")
+
 
     # Запуск развертывания на сервере
     asyncio.run(deploy_to_server(server_name, scripts_dir, input_dir, output_dir, scripts_dir_deploy, local_dir))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `revampdeployer-0.1.5/revampdeployer.egg-info/PKG-INFO` & `revampdeployer-0.2.0/revampdeployer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revampdeployer
-Version: 0.1.5
+Version: 0.2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RevampDeployer
 
 RevampDeployer is a tool for managing and automating the deployment process of applications to remote servers.
 
@@ -43,19 +43,19 @@
         "address": "192.168.1.2",
         "username": "admin",
         "password": "password2"
     },
     # Other servers...
 }
 
-local_scripts_dir = "local_scripts/"  # Директория локальных скриптов
-scripts_dir = "scripts/"  # Директория скриптов для выполнения на сервере
-input_dir = "input/"  # Директория с файлами для отправки на сервер
-output_dir = "output/"  # Директория для размещения файлов на сервере
-scripts_dir_deploy = "deploy_scripts/"  # Директория скриптов для пост-деплой конфигурации
+local_scripts = "local_scripts/"  # Директория локальных скриптов
+predeploy_scripts = "scripts/"  # Директория скриптов для выполнения на сервере
+dist = "input/"  # Директория с файлами для отправки на сервер
+dest = "output/"  # Директория для размещения файлов на сервере
+postdeploy_scripts = "deploy_scripts/"  # Директория скриптов для пост-деплой конфигурации
 ```
 
 This file should contain a list of servers, script directories, input and output directories, etc. Make sure all parameters are correct and match your environment.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for additional information.
```

### Comparing `revampdeployer-0.1.5/setup.py` & `revampdeployer-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Читаем содержимое файла README.md
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="revampdeployer",
-    version="0.1.5",
+    version="0.2.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "revampdeployer = revampdeployer.__main__:main"
         ]
     },
     # Добавляем описание пакета из README.md
```

