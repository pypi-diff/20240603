# Comparing `tmp/pymodins-2.0.7.tar.gz` & `tmp/pymodins-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-lt5l474m\pymodins-2.0.7.tar", last modified: Sun Jun  2 19:13:05 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\Python-Module-Installer\dist\.tmp-iwdjgf77\pymodins-2.0.8.tar", last modified: Mon Jun  3 03:32:39 2024, max compression
```

## Comparing `pymodins-2.0.7.tar` & `pymodins-2.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:13:05.559224 pymodins-2.0.7/
--rw-rw-rw-   0        0        0     1133 2024-06-02 18:25:44.000000 pymodins-2.0.7/LICENSE
--rw-rw-rw-   0        0        0     4406 2024-06-02 19:13:05.554655 pymodins-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3733 2024-06-02 18:25:47.000000 pymodins-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 19:13:05.522699 pymodins-2.0.7/pymodins/
--rw-rw-rw-   0        0        0      331 2024-06-02 19:12:39.000000 pymodins-2.0.7/pymodins/__init__.py
--rw-rw-rw-   0        0        0    60371 2024-06-02 19:03:55.000000 pymodins-2.0.7/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:13:05.551723 pymodins-2.0.7/pymodins.egg-info/
--rw-rw-rw-   0        0        0     4406 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 19:13:05.000000 pymodins-2.0.7/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 19:13:05.559224 pymodins-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1377 2024-06-02 19:12:43.000000 pymodins-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:32:39.014508 pymodins-2.0.8/
+-rw-rw-rw-   0        0        0     1133 2024-06-02 20:51:09.000000 pymodins-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4447 2024-06-03 03:32:39.008666 pymodins-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3774 2024-06-02 20:51:09.000000 pymodins-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 03:32:38.981238 pymodins-2.0.8/pymodins/
+-rw-rw-rw-   0        0        0      331 2024-06-03 03:31:44.000000 pymodins-2.0.8/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    63821 2024-06-03 03:24:25.000000 pymodins-2.0.8/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:32:39.008666 pymodins-2.0.8/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     4447 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 03:32:38.000000 pymodins-2.0.8/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 03:32:39.014508 pymodins-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2024-06-03 03:31:36.000000 pymodins-2.0.8/setup.py
```

### Comparing `pymodins-2.0.7/LICENSE` & `pymodins-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.7/PKG-INFO` & `pymodins-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.7
+Version: 2.0.8
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Platform: win32
 Classifier: Programming Language :: Python :: 3
@@ -21,20 +21,23 @@
 [pymodins](https://github.com/Nandhan-KA/pymodins) is a Python Modules Installer for Developers and Peoples who are new to python.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pymodins.
 
 ```bash
+python setup.py install 
+        or
 pip install pymodins
 ```
 
 ## Usage
 
-```python
+```Python 
+
 import pymodins
 
 # Displays all Domains
 pymodins.run()
 
 # Install Basic Modules
 pymodins.install_basic_modules()
```

### Comparing `pymodins-2.0.7/README.md` & `pymodins-2.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 [pymodins](https://github.com/Nandhan-KA/pymodins) is a Python Modules Installer for Developers and Peoples who are new to python.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pymodins.
 
 ```bash
+python setup.py install 
+        or
 pip install pymodins
 ```
 
 ## Usage
 
-```python
+```Python 
+
 import pymodins
 
 # Displays all Domains
 pymodins.run()
 
 # Install Basic Modules
 pymodins.install_basic_modules()
```

### Comparing `pymodins-2.0.7/pymodins/installer.py` & `pymodins-2.0.8/pymodins/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,23 @@
                                                                                 
     """
     console.print(ascii_art, style="bold yellow")
     console.print("\t Creator: Nandhan K", style="bold cyan")
     console.print("\t Github: @github.com/Nandhan-KA", style="bold yellow")
     console.print(" \n \t This Project Requires Internet Connection 🌐 ", style="bold yellow")
 
-import sys
-import subprocess
-
 def sys_info():
-    print("System Platform:", sys.platform)
-    print("Python version:", sys.version)
+    console = Console()
+    console.print("System Platform:", sys.platform, style="bold white")
+    console.print("Python version:", sys.version,style="bold white")
     try:
         pip_version = subprocess.check_output(['pip', '--version']).decode().strip()
-        print("pip version:", pip_version)
+        console.print("pip version:", pip_version,style="bold white")
     except Exception as e:
-        print("Error:", e, "Reinstall Python with PIP and add PIP to the System PATH")
-
+        console.print("Error:", e, "Reinstall Python with PIP and add PIP to the System PATH",style="bold white")
 
 def upgrade_pip():
     try:
         installed_version = pip.__version__
 
         latest_pip_version_output = subprocess.check_output(['pip', 'install', '--upgrade', 'pip']).decode().strip()
         print("Latest pip version output:", latest_pip_version_output)
@@ -220,28 +217,96 @@
 ]
 
 jupyter_modules = [
     'jupyter',
     'notebook', 'jupyterlab', 'nbconvert', 'nbformat', 'ipywidgets', 'ipykernel', 'voila', 'jupyter_contrib_nbextensions', 'jupyter_dash', 'jupyter_bokeh', 'jupytext', 'jupyterhub', 'jupyter_client', 'qtconsole'
 ]
 
-# Module Types
+data_analysis_modules = [
+    'pandas', 'numpy', 'dask', 'scipy', 'statsmodels', 'vaex', 'modin', 'pyarrow', 'koalas', 'polars',
+    'datatable', 'blaze', 'turicreate', 'rapidf', 'intake', 'seaborn', 'matplotlib', 'plotly', 'ggplot', 'bokeh', 
+    'altair', 'cufflinks'
+]
+
+data_visualization_modules = [
+    'matplotlib', 'seaborn', 'plotly', 'bokeh', 'altair', 'holoviews', 'geopandas', 'folium', 'chart-studio', 'pyecharts',
+    'hvplot', 'pygal', 'missingno', 'pandas_profiling', 'pywaffle', 'yellowbrick', 'networkx', 'graphviz', 'dash', 
+    'tableau', 'vispy', 'toyplot'
+]
+
+natural_language_processing_modules = [
+    'nltk', 'spacy', 'transformers', 'flair', 'gensim', 'textblob', 'vaderSentiment', 'polyglot', 'stanfordnlp', 'allennlp',
+    'fairseq', 'fasttext', 'openai-gpt', 'bert-score', 'sentence-transformers', 'summa', 'sumy', 'pattern', 
+    'pysentimiento', 'pyphen', 'simpletransformers'
+]
+
+web_development_modules = [
+    'django', 'flask', 'fastapi', 'pyramid', 'bottle', 'cherryPy', 'tornado', 'web2py', 'falcon', 'hug', 
+    'starlette', 'responder', 'sanic', 'socketio', 'asgiref', 'webapp2', 'aiohttp', 'masonite', 'clastic', 
+    'python-decouple', 'whitenoise', 'gunicorn', 'uwsgi', 'waitress'
+]
+
+database_modules = [
+    'sqlalchemy', 'pymysql', 'psycopg2', 'sqlite3', 'mongodb', 'pymongo', 'tinydb', 'couchdb', 'cassandra-driver', 'happybase',
+    'redis', 'aioredis', 'aiomysql', 'pony', 'orm', 'orator', 'dataset', 'datasets', 'peewee', 'sqlalchemy-migrate', 'yoyo-migrations'
+]
+
+cybersecurity_modules = [
+    'cryptography', 'pycryptodome', 'paramiko', 'scapy', 'pyshark', 'dnspython', 'impacket', 'requests', 'flask-security', 
+    'django-guardian', 'mitmproxy', 'pyOpenSSL', 'certifi', 'ssl', 'keyring', 'hpack', 'brotli', 'hashlib', 'python-nmap', 
+    'jinja2', 'pyjwt', 'passlib'
+]
+
+cloud_computing_modules = [
+    'boto3', 'google-cloud', 'azure', 'awscli', 'cloudpickle', 'cloudmesh', 'apache-libcloud', 'terraform', 'pulumi', 'ansible',
+    'kubernetes', 'docker', 'docker-compose', 'pywren', 'serverless', 'salt', 'pyinfra', 'cloudinary', 'paramiko', 'cloudant', 
+    'python-openstackclient', 'troposphere'
+]
+
+devops_modules = [
+    'ansible', 'jenkins', 'travis-ci', 'git', 'docker', 'docker-compose', 'kubernetes', 'vagrant', 'puppet', 'chef', 
+    'salt', 'fabric', 'terraform', 'consul', 'nomad', 'packer', 'helm', 'spinnaker', 'circleci', 'bamboo', 'gitlab', 
+    'gitea', 'hugo', 'mkdocs', 'pre-commit', 'pyinfra'
+]
+
+big_data_modules = [
+    'pyspark', 'hadoop', 'kafka', 'dask', 'ray', 'modin', 'polars', 'koalas', 'pyarrow', 'fastparquet', 
+    'pydoop', 'pyhive', 'mrjob', 'h5py', 'tables', 'zarr', 'petastorm', 'cudf', 'datashader', 'blaze', 
+    'turicreate', 'pandas', 'pandas-profiling'
+]
+
+mobile_development_modules = [
+    'kivy', 'beeware', 'pyqt', 'tkinter', 'flutter', 'react-native', 'pyjnius', 'sl4a', 'chaquopy', 'pybee', 
+    'pyto', 'rubicon-java', 'toga', 'pylibpd', 'pyobjus', 'pgs4a', 'plyer', 'buildozer', 'briefcase', 
+    'pyinstaller', 'cx_freeze', 'nuitka', 'py2app', 'py2exe'
+]
+
 module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+    None,
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
+    'Data Analysis Modules',
+    'Data Visualization Modules',
+    'Natural Language Processing Modules',
+    'Web Development Modules',
+    'Database Modules',
+    'Cybersecurity Modules',
+    'Cloud Computing Modules',
+    'DevOps Modules',
+    'Big Data Modules',
+    'Mobile Development Modules'
+]
 
 def installer():
     if internet() and sys.platform == 'win32':
         upgrade_pip()
         clear()
         banner()
         sys_info()
@@ -394,18 +459,14 @@
         banner()
         Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
         return
     
     else:
         banner_nointernet()
 
-
-def run():
-    installer()
-
 def install_basic_modules():
     if internet() and sys.platform == 'win32':
         upgrade_pip()
         banner()
         sys_info()
         selected_option = 1
 
@@ -687,15 +748,14 @@
 def install_deeplearning_modules():
     if internet():
         upgrade_pip()
         banner()
         sys_info()
         selected_option = 6
         
-
         selected_module_type = module_types[selected_option]
 
         if selected_module_type:
             print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
                 selected_module_type.lower().replace(" ", "_")]
@@ -773,15 +833,14 @@
         banner()
         Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
         return
     
     else:
         banner_nointernet()
 
-
 def install_fullstack_modules():
     if internet():
         upgrade_pip()
         banner()
         sys_info()
         selected_option = 7
         
@@ -875,15 +934,14 @@
 def install_science_modules():
     if internet():
         upgrade_pip()
         banner()
         sys_info()
         selected_option = 3
         
-
         selected_module_type = module_types[selected_option]
 
         if selected_module_type:
             print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
                 selected_module_type.lower().replace(" ", "_")]
@@ -960,16 +1018,15 @@
     elif internet() and sys.platform == "linux":
         banner()
         Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
         return
     
     else:
         banner_nointernet()
-
-      
+    
 def install_computervision_modules():
     if internet():
         upgrade_pip()
         banner()
         sys_info()
         selected_option = 4
         
@@ -1386,8 +1443,10 @@
     elif internet() and sys.platform == "linux":
         banner()
         Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
         return
     
     else:
         banner_nointernet()
-
+        
+def run():
+    installer()
```

### Comparing `pymodins-2.0.7/pymodins.egg-info/PKG-INFO` & `pymodins-2.0.8/pymodins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.7
+Version: 2.0.8
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Platform: win32
 Classifier: Programming Language :: Python :: 3
@@ -21,20 +21,23 @@
 [pymodins](https://github.com/Nandhan-KA/pymodins) is a Python Modules Installer for Developers and Peoples who are new to python.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pymodins.
 
 ```bash
+python setup.py install 
+        or
 pip install pymodins
 ```
 
 ## Usage
 
-```python
+```Python 
+
 import pymodins
 
 # Displays all Domains
 pymodins.run()
 
 # Install Basic Modules
 pymodins.install_basic_modules()
```

### Comparing `pymodins-2.0.7/setup.py` & `pymodins-2.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import platform
 from setuptools import setup, find_packages
 
 if platform.system() == "Windows":
     setup(
         name="pymodins",
-        version="2.0.7",
+        version="2.0.8",
         packages=find_packages(),
         install_requires=[
             "rich",
             "pymsgbox"
         ],
         entry_points={
             "console_scripts": [
```

