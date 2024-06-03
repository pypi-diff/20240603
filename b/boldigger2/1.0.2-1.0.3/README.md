# Comparing `tmp/boldigger2-1.0.2.tar.gz` & `tmp/boldigger2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boldigger2-1.0.2.tar", last modified: Thu May 30 05:22:29 2024, max compression
+gzip compressed data, was "boldigger2-1.0.3.tar", last modified: Sun Jun  2 14:13:49 2024, max compression
```

## Comparing `boldigger2-1.0.2.tar` & `boldigger2-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 05:22:29.610154 boldigger2-1.0.2/
--rw-rw-rw-   0        0        0     1093 2024-05-29 03:47:00.000000 boldigger2-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0    10834 2024-05-30 05:22:29.609158 boldigger2-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9928 2024-05-29 18:51:46.000000 boldigger2-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 05:22:29.591991 boldigger2-1.0.2/boldigger2/
--rw-rw-rw-   0        0        0        0 2024-05-29 03:44:28.000000 boldigger2-1.0.2/boldigger2/__init__.py
--rw-rw-rw-   0        0        0     1602 2024-05-21 05:50:28.000000 boldigger2-1.0.2/boldigger2/__main__.py
--rw-rw-rw-   0        0        0    12036 2024-05-29 03:46:11.000000 boldigger2-1.0.2/boldigger2/additional_data_download.py
--rw-rw-rw-   0        0        0    10838 2024-05-29 03:51:42.000000 boldigger2-1.0.2/boldigger2/digger_hit.py
--rw-rw-rw-   0        0        0    21740 2024-05-29 03:46:11.000000 boldigger2-1.0.2/boldigger2/id_engine_coi.py
--rw-rw-rw-   0        0        0     2516 2024-05-29 03:46:11.000000 boldigger2-1.0.2/boldigger2/login.py
-drwxrwxrwx   0        0        0        0 2024-05-30 05:22:29.608161 boldigger2-1.0.2/boldigger2.egg-info/
--rw-rw-rw-   0        0        0    10834 2024-05-30 05:22:29.000000 boldigger2-1.0.2/boldigger2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-05-30 05:22:29.000000 boldigger2-1.0.2/boldigger2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 05:22:29.000000 boldigger2-1.0.2/boldigger2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-30 05:22:29.000000 boldigger2-1.0.2/boldigger2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      192 2024-05-30 05:22:29.000000 boldigger2-1.0.2/boldigger2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-30 05:22:29.000000 boldigger2-1.0.2/boldigger2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2024-05-29 03:59:19.000000 boldigger2-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 05:22:29.610154 boldigger2-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1270 2024-05-30 05:21:59.000000 boldigger2-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:13:49.755512 boldigger2-1.0.3/
+-rw-rw-rw-   0        0        0     1093 2024-05-29 03:47:00.000000 boldigger2-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    10954 2024-06-02 14:13:49.754500 boldigger2-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9929 2024-06-02 14:11:07.000000 boldigger2-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 14:13:49.738553 boldigger2-1.0.3/boldigger2/
+-rw-rw-rw-   0        0        0        0 2024-05-29 03:44:28.000000 boldigger2-1.0.3/boldigger2/__init__.py
+-rw-rw-rw-   0        0        0     1602 2024-05-21 05:50:28.000000 boldigger2-1.0.3/boldigger2/__main__.py
+-rw-rw-rw-   0        0        0    12036 2024-05-29 03:46:11.000000 boldigger2-1.0.3/boldigger2/additional_data_download.py
+-rw-rw-rw-   0        0        0    10838 2024-05-29 03:51:42.000000 boldigger2-1.0.3/boldigger2/digger_hit.py
+-rw-rw-rw-   0        0        0    21740 2024-05-29 03:46:11.000000 boldigger2-1.0.3/boldigger2/id_engine_coi.py
+-rw-rw-rw-   0        0        0     2516 2024-05-29 03:46:11.000000 boldigger2-1.0.3/boldigger2/login.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:13:49.754500 boldigger2-1.0.3/boldigger2.egg-info/
+-rw-rw-rw-   0        0        0    10954 2024-06-02 14:13:49.000000 boldigger2-1.0.3/boldigger2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-06-02 14:13:49.000000 boldigger2-1.0.3/boldigger2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 14:13:49.000000 boldigger2-1.0.3/boldigger2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-06-02 14:13:49.000000 boldigger2-1.0.3/boldigger2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      247 2024-06-02 14:13:49.000000 boldigger2-1.0.3/boldigger2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-02 14:13:49.000000 boldigger2-1.0.3/boldigger2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2024-05-29 03:59:19.000000 boldigger2-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 14:13:49.755512 boldigger2-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2024-06-02 14:13:16.000000 boldigger2-1.0.3/setup.py
```

### Comparing `boldigger2-1.0.2/LICENSE.txt` & `boldigger2-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.2/PKG-INFO` & `boldigger2-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boldigger2
-Version: 1.0.2
+Version: 1.0.3
 Summary: An even better python package to query different databases of boldsystems.org
 Home-page: https://github.com/DominikBuchner/BOLDigger
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,18 @@
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: requests_html>=0.10.0
 Requires-Dist: tqdm>=4.66.4
 Requires-Dist: tqdm_joblib>=0.0.4
 Requires-Dist: urllib3>=1.26.12
+Requires-Dist: tables>=3.9.2
+Requires-Dist: html5lib>=1.1
+Requires-Dist: lxml>=4.9.1
+Requires-Dist: soupsieve>=2.5
 
 # BOLDigger2
 ![boldigger_logo](https://github.com/DominikBuchner/BOLDigger2/assets/38790188/0cb8ac93-139d-47df-9d78-380d76dd0033)
 
 [![Downloads](https://pepy.tech/badge/boldigger2)](https://pepy.tech/project/boldigger2)
 
 An even better Python program to query .fasta files against the COI database of www.boldsystems.org
@@ -55,15 +59,15 @@
 - **Adjusted Species-Level Threshold**: BOLDigger2 accepts hits with a similarity of >= 97% as species-level records. This decision aligns with the 3% OTU clustering threshold commonly used in DNA metabarcoding.
 - **Increased process safety**: BOLDigger2 can be stopped at any point in the processing and will simply continue where it was stopped. BOLDigger2 will no longer alter the provided FASTA file. BOLDigger2 accepts both common FASTA formats.
 - **Dynamic downloads**: BOLDigger2 will automatically adjust the number of sequences per query to the BOLD database. If the connection times out the query size will be reduced, if the request is successful, the query size will be increased.
 - **Improved error handling**: Broken records in the BOLD database are now detected and directly reported as a "BrokenRecord" in addition to "NoMatches". If the BOLD website is not accessible, BOLDigger2 will simply wait until it is up again.
 
 ## Installation and Usage
 
-BOLDigger2 requires Python version 3.9 or higher and can be easily installed using pip in any command line:
+BOLDigger2 requires Python version 3.10 or higher and can be easily installed using pip in any command line:
 
 `pip install boldigger2`
 
 This command will install BOLDigger2 along with all its dependencies.
 
 To run the identify function, use the following command:
```

### Comparing `boldigger2-1.0.2/README.md` & `boldigger2-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 - **Adjusted Species-Level Threshold**: BOLDigger2 accepts hits with a similarity of >= 97% as species-level records. This decision aligns with the 3% OTU clustering threshold commonly used in DNA metabarcoding.
 - **Increased process safety**: BOLDigger2 can be stopped at any point in the processing and will simply continue where it was stopped. BOLDigger2 will no longer alter the provided FASTA file. BOLDigger2 accepts both common FASTA formats.
 - **Dynamic downloads**: BOLDigger2 will automatically adjust the number of sequences per query to the BOLD database. If the connection times out the query size will be reduced, if the request is successful, the query size will be increased.
 - **Improved error handling**: Broken records in the BOLD database are now detected and directly reported as a "BrokenRecord" in addition to "NoMatches". If the BOLD website is not accessible, BOLDigger2 will simply wait until it is up again.
 
 ## Installation and Usage
 
-BOLDigger2 requires Python version 3.9 or higher and can be easily installed using pip in any command line:
+BOLDigger2 requires Python version 3.10 or higher and can be easily installed using pip in any command line:
 
 `pip install boldigger2`
 
 This command will install BOLDigger2 along with all its dependencies.
 
 To run the identify function, use the following command:
```

### Comparing `boldigger2-1.0.2/boldigger2/__main__.py` & `boldigger2-1.0.3/boldigger2/__main__.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.2/boldigger2/additional_data_download.py` & `boldigger2-1.0.3/boldigger2/additional_data_download.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.2/boldigger2/digger_hit.py` & `boldigger2-1.0.3/boldigger2/digger_hit.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.2/boldigger2/id_engine_coi.py` & `boldigger2-1.0.3/boldigger2/id_engine_coi.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.2/boldigger2/login.py` & `boldigger2-1.0.3/boldigger2/login.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.2/boldigger2.egg-info/PKG-INFO` & `boldigger2-1.0.3/boldigger2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boldigger2
-Version: 1.0.2
+Version: 1.0.3
 Summary: An even better python package to query different databases of boldsystems.org
 Home-page: https://github.com/DominikBuchner/BOLDigger
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,18 @@
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: requests_html>=0.10.0
 Requires-Dist: tqdm>=4.66.4
 Requires-Dist: tqdm_joblib>=0.0.4
 Requires-Dist: urllib3>=1.26.12
+Requires-Dist: tables>=3.9.2
+Requires-Dist: html5lib>=1.1
+Requires-Dist: lxml>=4.9.1
+Requires-Dist: soupsieve>=2.5
 
 # BOLDigger2
 ![boldigger_logo](https://github.com/DominikBuchner/BOLDigger2/assets/38790188/0cb8ac93-139d-47df-9d78-380d76dd0033)
 
 [![Downloads](https://pepy.tech/badge/boldigger2)](https://pepy.tech/project/boldigger2)
 
 An even better Python program to query .fasta files against the COI database of www.boldsystems.org
@@ -55,15 +59,15 @@
 - **Adjusted Species-Level Threshold**: BOLDigger2 accepts hits with a similarity of >= 97% as species-level records. This decision aligns with the 3% OTU clustering threshold commonly used in DNA metabarcoding.
 - **Increased process safety**: BOLDigger2 can be stopped at any point in the processing and will simply continue where it was stopped. BOLDigger2 will no longer alter the provided FASTA file. BOLDigger2 accepts both common FASTA formats.
 - **Dynamic downloads**: BOLDigger2 will automatically adjust the number of sequences per query to the BOLD database. If the connection times out the query size will be reduced, if the request is successful, the query size will be increased.
 - **Improved error handling**: Broken records in the BOLD database are now detected and directly reported as a "BrokenRecord" in addition to "NoMatches". If the BOLD website is not accessible, BOLDigger2 will simply wait until it is up again.
 
 ## Installation and Usage
 
-BOLDigger2 requires Python version 3.9 or higher and can be easily installed using pip in any command line:
+BOLDigger2 requires Python version 3.10 or higher and can be easily installed using pip in any command line:
 
 `pip install boldigger2`
 
 This command will install BOLDigger2 along with all its dependencies.
 
 To run the identify function, use the following command:
```

### Comparing `boldigger2-1.0.2/setup.py` & `boldigger2-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="boldigger2",
-    version="1.0.2",
+    version="1.0.3",
     author="Dominik Buchner",
     author_email="dominik.buchner524@googlemail.com",
     description="An even better python package to query different databases of boldsystems.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DominikBuchner/BOLDigger",
     packages=setuptools.find_packages(),
@@ -22,14 +22,18 @@
         "numpy>=1.26.4",
         "pandas>=2.2.2",
         "Requests>=2.32.2",
         "requests_html>=0.10.0",
         "tqdm>=4.66.4",
         "tqdm_joblib>=0.0.4",
         "urllib3>=1.26.12",
+        "tables>=3.9.2",
+        "html5lib>=1.1",
+        "lxml>=4.9.1",
+        "soupsieve>=2.5",
     ],
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

