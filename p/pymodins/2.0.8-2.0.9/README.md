# Comparing `tmp/pymodins-2.0.8.tar.gz` & `tmp/pymodins-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\Python-Module-Installer\dist\.tmp-iwdjgf77\pymodins-2.0.8.tar", last modified: Mon Jun  3 03:32:39 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-yyezljxz\pymodins-2.0.9.tar", last modified: Mon Jun  3 04:14:48 2024, max compression
```

## Comparing `pymodins-2.0.8.tar` & `pymodins-2.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 03:32:39.014508 pymodins-2.0.8/
--rw-rw-rw-   0        0        0     1133 2024-06-02 20:51:09.000000 pymodins-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     4447 2024-06-03 03:32:39.008666 pymodins-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3774 2024-06-02 20:51:09.000000 pymodins-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 03:32:38.981238 pymodins-2.0.8/pymodins/
--rw-rw-rw-   0        0        0      331 2024-06-03 03:31:44.000000 pymodins-2.0.8/pymodins/__init__.py
--rw-rw-rw-   0        0        0    63821 2024-06-03 03:24:25.000000 pymodins-2.0.8/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-06-03 03:32:39.008666 pymodins-2.0.8/pymodins.egg-info/
--rw-rw-rw-   0        0        0     4447 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 03:32:39.014508 pymodins-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1377 2024-06-03 03:31:36.000000 pymodins-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:14:48.049413 pymodins-2.0.9/
+-rw-rw-rw-   0        0        0     1133 2024-06-02 20:51:09.000000 pymodins-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5030 2024-06-03 04:14:48.049413 pymodins-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4357 2024-06-03 04:10:34.000000 pymodins-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 04:14:48.023206 pymodins-2.0.9/pymodins/
+-rw-rw-rw-   0        0        0      331 2024-06-03 04:02:17.000000 pymodins-2.0.9/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    86619 2024-06-03 04:09:05.000000 pymodins-2.0.9/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:14:48.049413 pymodins-2.0.9/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     5030 2024-06-03 04:14:47.000000 pymodins-2.0.9/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-06-03 04:14:47.000000 pymodins-2.0.9/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 04:14:47.000000 pymodins-2.0.9/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-06-03 04:14:47.000000 pymodins-2.0.9/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 04:14:47.000000 pymodins-2.0.9/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 04:14:47.000000 pymodins-2.0.9/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 04:14:48.055817 pymodins-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2024-06-03 04:02:30.000000 pymodins-2.0.9/setup.py
```

### Comparing `pymodins-2.0.8/LICENSE` & `pymodins-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.8/PKG-INFO` & `pymodins-2.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.8
+Version: 2.0.9
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Platform: win32
 Classifier: Programming Language :: Python :: 3
@@ -65,14 +65,31 @@
 
 #install Build Modules
 pymodins.install_build_modules()
 
 #install Jupyter Modules
 pymodins.install_jupyter_modules()
 
+#install data visualization modules
+pymodins.install_data_visualization_modules()
+
+#install database modules
+pymodins.install_database_modules()
+
+#install CyberSecurity modules
+pymodins.install_CyberSecurity_modules()
+
+#install cloudcomputing modules
+pymodins.install_cloudcomputing_modules()
+
+#install devops modules
+pymodins.install_devops_modules()
+
+#install bigdata modules
+pymodins.install_bigdata_modules()
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
@@ -116,28 +133,34 @@
  _| |_      _|  |_    _| |_\/_| |_\  `-'  /_| |_.' /_| |_  _| |_\   |_ | \____) | 
 |_____|    |______|  |_____||_____|`.___.'|______.'|_____||_____|\____| \______.' 
 
     
 Creator: Nandhan K
 Github: @github.com/Nandhan-KA
 System Platform: win32
-Python verion: 3.8.0 (tags/v3.8.0:fa919fd, Oct 14 2019, 19:37:50) [MSC v.1916 64 bit (AMD64)]
+Python version: 3.8.0 (tags/v3.8.0:fa919fd, Oct 14 2019, 19:37:50) [MSC v.1916 64 bit (AMD64)]
 pip version: pip 24.0 from c:\users\{username}\appdata\local\programs\python\python38\lib\site-packages\pip (python 3.8)
 
 Please select the type of modules you want to install:
 
 1. Basic Modules
 2. Advanced Modules
 3. Science Modules
 4. Computer Vision Modules
 5. Machine Learning Modules
 6. Deep Learning Modules
 7. Full Stack Development Modules
 8. Network Modules
 9. Build Modules
 10. Jupyter Modules
+11. Data Visualization Modules
+12. Database Modules
+13. Cybersecurity Modules
+14. Cloud Computing Modules
+15. DevOps Modules
+16. Big Data Modules
 
 Enter the number corresponding to your choice: 
 ```
 
 # Thank you for using this project!
 # Feel free to ask your queries
```

### Comparing `pymodins-2.0.8/README.md` & `pymodins-2.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -47,14 +47,31 @@
 
 #install Build Modules
 pymodins.install_build_modules()
 
 #install Jupyter Modules
 pymodins.install_jupyter_modules()
 
+#install data visualization modules
+pymodins.install_data_visualization_modules()
+
+#install database modules
+pymodins.install_database_modules()
+
+#install CyberSecurity modules
+pymodins.install_CyberSecurity_modules()
+
+#install cloudcomputing modules
+pymodins.install_cloudcomputing_modules()
+
+#install devops modules
+pymodins.install_devops_modules()
+
+#install bigdata modules
+pymodins.install_bigdata_modules()
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
@@ -98,28 +115,34 @@
  _| |_      _|  |_    _| |_\/_| |_\  `-'  /_| |_.' /_| |_  _| |_\   |_ | \____) | 
 |_____|    |______|  |_____||_____|`.___.'|______.'|_____||_____|\____| \______.' 
 
     
 Creator: Nandhan K
 Github: @github.com/Nandhan-KA
 System Platform: win32
-Python verion: 3.8.0 (tags/v3.8.0:fa919fd, Oct 14 2019, 19:37:50) [MSC v.1916 64 bit (AMD64)]
+Python version: 3.8.0 (tags/v3.8.0:fa919fd, Oct 14 2019, 19:37:50) [MSC v.1916 64 bit (AMD64)]
 pip version: pip 24.0 from c:\users\{username}\appdata\local\programs\python\python38\lib\site-packages\pip (python 3.8)
 
 Please select the type of modules you want to install:
 
 1. Basic Modules
 2. Advanced Modules
 3. Science Modules
 4. Computer Vision Modules
 5. Machine Learning Modules
 6. Deep Learning Modules
 7. Full Stack Development Modules
 8. Network Modules
 9. Build Modules
 10. Jupyter Modules
+11. Data Visualization Modules
+12. Database Modules
+13. Cybersecurity Modules
+14. Cloud Computing Modules
+15. DevOps Modules
+16. Big Data Modules
 
 Enter the number corresponding to your choice: 
 ```
 
 # Thank you for using this project!
 # Feel free to ask your queries
```

### Comparing `pymodins-2.0.8/pymodins/installer.py` & `pymodins-2.0.9/pymodins/installer.py`

 * *Files 23% similar despite different names*

```diff
@@ -217,38 +217,20 @@
 ]
 
 jupyter_modules = [
     'jupyter',
     'notebook', 'jupyterlab', 'nbconvert', 'nbformat', 'ipywidgets', 'ipykernel', 'voila', 'jupyter_contrib_nbextensions', 'jupyter_dash', 'jupyter_bokeh', 'jupytext', 'jupyterhub', 'jupyter_client', 'qtconsole'
 ]
 
-data_analysis_modules = [
-    'pandas', 'numpy', 'dask', 'scipy', 'statsmodels', 'vaex', 'modin', 'pyarrow', 'koalas', 'polars',
-    'datatable', 'blaze', 'turicreate', 'rapidf', 'intake', 'seaborn', 'matplotlib', 'plotly', 'ggplot', 'bokeh', 
-    'altair', 'cufflinks'
-]
-
 data_visualization_modules = [
     'matplotlib', 'seaborn', 'plotly', 'bokeh', 'altair', 'holoviews', 'geopandas', 'folium', 'chart-studio', 'pyecharts',
     'hvplot', 'pygal', 'missingno', 'pandas_profiling', 'pywaffle', 'yellowbrick', 'networkx', 'graphviz', 'dash', 
     'tableau', 'vispy', 'toyplot'
 ]
 
-natural_language_processing_modules = [
-    'nltk', 'spacy', 'transformers', 'flair', 'gensim', 'textblob', 'vaderSentiment', 'polyglot', 'stanfordnlp', 'allennlp',
-    'fairseq', 'fasttext', 'openai-gpt', 'bert-score', 'sentence-transformers', 'summa', 'sumy', 'pattern', 
-    'pysentimiento', 'pyphen', 'simpletransformers'
-]
-
-web_development_modules = [
-    'django', 'flask', 'fastapi', 'pyramid', 'bottle', 'cherryPy', 'tornado', 'web2py', 'falcon', 'hug', 
-    'starlette', 'responder', 'sanic', 'socketio', 'asgiref', 'webapp2', 'aiohttp', 'masonite', 'clastic', 
-    'python-decouple', 'whitenoise', 'gunicorn', 'uwsgi', 'waitress'
-]
-
 database_modules = [
     'sqlalchemy', 'pymysql', 'psycopg2', 'sqlite3', 'mongodb', 'pymongo', 'tinydb', 'couchdb', 'cassandra-driver', 'happybase',
     'redis', 'aioredis', 'aiomysql', 'pony', 'orm', 'orator', 'dataset', 'datasets', 'peewee', 'sqlalchemy-migrate', 'yoyo-migrations'
 ]
 
 cybersecurity_modules = [
     'cryptography', 'pycryptodome', 'paramiko', 'scapy', 'pyshark', 'dnspython', 'impacket', 'requests', 'flask-security', 
@@ -270,56 +252,60 @@
 
 big_data_modules = [
     'pyspark', 'hadoop', 'kafka', 'dask', 'ray', 'modin', 'polars', 'koalas', 'pyarrow', 'fastparquet', 
     'pydoop', 'pyhive', 'mrjob', 'h5py', 'tables', 'zarr', 'petastorm', 'cudf', 'datashader', 'blaze', 
     'turicreate', 'pandas', 'pandas-profiling'
 ]
 
-mobile_development_modules = [
-    'kivy', 'beeware', 'pyqt', 'tkinter', 'flutter', 'react-native', 'pyjnius', 'sl4a', 'chaquopy', 'pybee', 
-    'pyto', 'rubicon-java', 'toga', 'pylibpd', 'pyobjus', 'pgs4a', 'plyer', 'buildozer', 'briefcase', 
-    'pyinstaller', 'cx_freeze', 'nuitka', 'py2app', 'py2exe'
-]
+
 
 module_types = [
     None,
     'Basic Modules',
     'Advanced Modules',
     'Science Modules',
     'Computer Vision Modules',
     'Machine Learning Modules',
     'Deep Learning Modules',
     'Full Stack Development Modules',
     'Network Modules',
     'Build Modules',
     'Jupyter Modules',
-    'Data Analysis Modules',
     'Data Visualization Modules',
-    'Natural Language Processing Modules',
-    'Web Development Modules',
     'Database Modules',
     'Cybersecurity Modules',
     'Cloud Computing Modules',
     'DevOps Modules',
     'Big Data Modules',
-    'Mobile Development Modules'
 ]
 
 def installer():
     if internet() and sys.platform == 'win32':
         upgrade_pip()
         clear()
         banner()
         sys_info()
-        
         module_types = [
-            'Basic Modules', 'Advanced Modules', 'Science Modules', 'Computer Vision Modules',
-            'Machine Learning Modules', 'Deep Learning Modules', 'Full Stack Development Modules',
-            'Network Modules', 'Build Modules', 'Jupyter Modules'
-        ]
+    'Basic Modules',
+    'Advanced Modules',
+    'Science Modules',
+    'Computer Vision Modules',
+    'Machine Learning Modules',
+    'Deep Learning Modules',
+    'Full Stack Development Modules',
+    'Network Modules',
+    'Build Modules',
+    'Jupyter Modules',
+    'Data Visualization Modules',
+    'Database Modules',
+    'Cybersecurity Modules',
+    'Cloud Computing Modules',
+    'DevOps Modules',
+    'Big Data Modules',
+]
 
         print("\nPlease select the type of modules you want to install:\n")
         for i, module_type in enumerate(module_types, 1):
             print(f"{i}. {module_type}")
 
         try:
             selected_module_type = int(
@@ -453,15 +439,16 @@
 
         except Exception as e:
             print("Error:", e, "\nPlease try again.")
             installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
         return
     
     else:
         banner_nointernet()
 
 def install_basic_modules():
     if internet() and sys.platform == 'win32':
@@ -546,17 +533,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
                     
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
     else:
         banner_nointernet()
 
 def install_advanced_modules():
     if internet():
         upgrade_pip()
         banner()
@@ -640,17 +627,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
     else:
         banner_nointernet()
 
 
 def install_machinelearning_modules():
     if internet():
         upgrade_pip()
@@ -734,17 +721,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
     else:
         banner_nointernet()
 
 
 def install_deeplearning_modules():
     if internet():
         upgrade_pip()
@@ -827,17 +814,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+            
     else:
         banner_nointernet()
 
 def install_fullstack_modules():
     if internet():
         upgrade_pip()
         banner()
@@ -920,17 +907,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+            
     else:
         banner_nointernet()
 
 
 def install_science_modules():
     if internet():
         upgrade_pip()
@@ -1013,17 +1000,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
     else:
         banner_nointernet()
     
 def install_computervision_modules():
     if internet():
         upgrade_pip()
         banner()
@@ -1129,17 +1116,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
     else:
         banner_nointernet()
 
        
 def install_network_modules():
     if internet():
         upgrade_pip()
@@ -1223,16 +1210,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
     
     else:
         banner_nointernet()
 
 
 def install_build_modules():
     if internet():
@@ -1347,17 +1335,17 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
-    
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
     else:
         banner_nointernet()
 
 def install_jupyter_modules():
     if internet():
         upgrade_pip()
         banner()
@@ -1438,15 +1426,584 @@
                     print(f"{user} Thank you for using.")
                     sys.exit()
                 elif more.lower() in ["yes", "y"]:
                     installer()
             
     elif internet() and sys.platform == "linux":
         banner()
-        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
-        return
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
     
     else:
         banner_nointernet()
-        
+   
+   
+
+def install_data_visualization_modules():
+    if internet() and sys.platform == 'win32':
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 11
+
+        selected_module_type = module_types[selected_option]
+
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
+
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
+
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
+
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+                    
+    elif internet() and sys.platform == "linux":
+        banner()
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
+    else:
+        banner_nointernet()
+
+
+def install_database_modules():
+    if internet() and sys.platform == 'win32':
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 12
+
+        selected_module_type = module_types[selected_option]
+
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
+
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
+
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
+
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+                    
+    elif internet() and sys.platform == "linux":
+        banner()
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
+    else:
+        banner_nointernet()
+
+
+
+def install_CyberSecurity_modules():
+    if internet() and sys.platform == 'win32':
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 13
+
+        selected_module_type = module_types[selected_option]
+
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
+
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
+
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
+
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+                    
+    elif internet() and sys.platform == "linux":
+        banner()
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
+    else:
+        banner_nointernet()
+
+
+def install_cloudcomputing_modules():
+    if internet() and sys.platform == 'win32':
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 14
+
+        selected_module_type = module_types[selected_option]
+
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
+
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
+
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
+
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+                    
+    elif internet() and sys.platform == "linux":
+        banner()
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
+    else:
+        banner_nointernet()
+
+
+def install_devops_modules():
+    if internet() and sys.platform == 'win32':
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 15
+
+        selected_module_type = module_types[selected_option]
+
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
+
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
+
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
+
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+                    
+    elif internet() and sys.platform == "linux":
+        banner()
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
+    else:
+        banner_nointernet()
+
+
+def install_bigdata_modules():
+    if internet() and sys.platform == 'win32':
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 16
+
+        selected_module_type = module_types[selected_option]
+
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
+
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
+
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
+
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+                    
+    elif internet() and sys.platform == "linux":
+        banner()
+        console = Console()
+        console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+          
+    else:
+        banner_nointernet()
+
+
 def run():
-    installer()
+    installer()
+    
+run()
```

### Comparing `pymodins-2.0.8/pymodins.egg-info/PKG-INFO` & `pymodins-2.0.9/pymodins.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.8
+Version: 2.0.9
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Platform: win32
 Classifier: Programming Language :: Python :: 3
@@ -65,14 +65,31 @@
 
 #install Build Modules
 pymodins.install_build_modules()
 
 #install Jupyter Modules
 pymodins.install_jupyter_modules()
 
+#install data visualization modules
+pymodins.install_data_visualization_modules()
+
+#install database modules
+pymodins.install_database_modules()
+
+#install CyberSecurity modules
+pymodins.install_CyberSecurity_modules()
+
+#install cloudcomputing modules
+pymodins.install_cloudcomputing_modules()
+
+#install devops modules
+pymodins.install_devops_modules()
+
+#install bigdata modules
+pymodins.install_bigdata_modules()
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
@@ -116,28 +133,34 @@
  _| |_      _|  |_    _| |_\/_| |_\  `-'  /_| |_.' /_| |_  _| |_\   |_ | \____) | 
 |_____|    |______|  |_____||_____|`.___.'|______.'|_____||_____|\____| \______.' 
 
     
 Creator: Nandhan K
 Github: @github.com/Nandhan-KA
 System Platform: win32
-Python verion: 3.8.0 (tags/v3.8.0:fa919fd, Oct 14 2019, 19:37:50) [MSC v.1916 64 bit (AMD64)]
+Python version: 3.8.0 (tags/v3.8.0:fa919fd, Oct 14 2019, 19:37:50) [MSC v.1916 64 bit (AMD64)]
 pip version: pip 24.0 from c:\users\{username}\appdata\local\programs\python\python38\lib\site-packages\pip (python 3.8)
 
 Please select the type of modules you want to install:
 
 1. Basic Modules
 2. Advanced Modules
 3. Science Modules
 4. Computer Vision Modules
 5. Machine Learning Modules
 6. Deep Learning Modules
 7. Full Stack Development Modules
 8. Network Modules
 9. Build Modules
 10. Jupyter Modules
+11. Data Visualization Modules
+12. Database Modules
+13. Cybersecurity Modules
+14. Cloud Computing Modules
+15. DevOps Modules
+16. Big Data Modules
 
 Enter the number corresponding to your choice: 
 ```
 
 # Thank you for using this project!
 # Feel free to ask your queries
```

### Comparing `pymodins-2.0.8/setup.py` & `pymodins-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import platform
 from setuptools import setup, find_packages
 
 if platform.system() == "Windows":
     setup(
         name="pymodins",
-        version="2.0.8",
+        version="2.0.9",
         packages=find_packages(),
         install_requires=[
             "rich",
             "pymsgbox"
         ],
         entry_points={
             "console_scripts": [
```

