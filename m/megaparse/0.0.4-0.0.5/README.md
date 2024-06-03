# Comparing `tmp/megaparse-0.0.4.tar.gz` & `tmp/megaparse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaparse-0.0.4.tar", last modified: Sun Jun  2 10:23:19 2024, max compression
+gzip compressed data, was "megaparse-0.0.5.tar", last modified: Sun Jun  2 10:36:26 2024, max compression
```

## Comparing `megaparse-0.0.4.tar` & `megaparse-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:19.574667 megaparse-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 10:23:11.000000 megaparse-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-06-02 10:23:19.574667 megaparse-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-06-02 10:23:11.000000 megaparse-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:19.574667 megaparse-0.0.4/megaparse/
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/Converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/markdown_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:19.574667 megaparse-0.0.4/megaparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:23:19.574667 megaparse-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-06-02 10:23:11.000000 megaparse-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:26.671664 megaparse-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 10:36:22.000000 megaparse-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-06-02 10:36:26.667664 megaparse-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-02 10:36:22.000000 megaparse-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:26.667664 megaparse-0.0.5/megaparse/
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-06-02 10:36:22.000000 megaparse-0.0.5/megaparse/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:22.000000 megaparse-0.0.5/megaparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-06-02 10:36:22.000000 megaparse-0.0.5/megaparse/markdown_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-02 10:36:22.000000 megaparse-0.0.5/megaparse/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-06-02 10:36:22.000000 megaparse-0.0.5/megaparse/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-02 10:36:22.000000 megaparse-0.0.5/megaparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:26.667664 megaparse-0.0.5/megaparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-06-02 10:36:26.000000 megaparse-0.0.5/megaparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 10:36:26.000000 megaparse-0.0.5/megaparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:36:26.000000 megaparse-0.0.5/megaparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 10:36:26.000000 megaparse-0.0.5/megaparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 10:36:26.000000 megaparse-0.0.5/megaparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:36:26.671664 megaparse-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-06-02 10:36:22.000000 megaparse-0.0.5/setup.py
```

### Comparing `megaparse-0.0.4/LICENSE` & `megaparse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.4/PKG-INFO` & `megaparse-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaparse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Parse complex files (PDF,Docx,PPTX) for LLM consumption
 Author: Quivr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-docx
 Requires-Dist: mammoth
 Requires-Dist: python-pptx
@@ -41,15 +41,19 @@
 
 ```bash
 pip install megaparse
 ```
 
 ## Usage
 
-Add your OpenAI API key to the .env file
+1. Add your OpenAI API key to the .env file
+
+2. Install poppler on your computer (images and PDFs)
+3. 
+4. Install tesseract on your computer (images and PDFs)
 
 ```python
 from megaparse import MegaParse
 
 megaparse = MegaParse(file_path="./test.pdf")
 content = megaparse.convert()
 print(content)
```

### Comparing `megaparse-0.0.4/README.md` & `megaparse-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
 ```bash
 pip install megaparse
 ```
 
 ## Usage
 
-Add your OpenAI API key to the .env file
+1. Add your OpenAI API key to the .env file
+
+2. Install poppler on your computer (images and PDFs)
+3. 
+4. Install tesseract on your computer (images and PDFs)
 
 ```python
 from megaparse import MegaParse
 
 megaparse = MegaParse(file_path="./test.pdf")
 content = megaparse.convert()
 print(content)
```

### Comparing `megaparse-0.0.4/megaparse/Converter.py` & `megaparse-0.0.5/megaparse/Converter.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.4/megaparse/markdown_processor.py` & `megaparse-0.0.5/megaparse/markdown_processor.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.4/megaparse/unstructured.py` & `megaparse-0.0.5/megaparse/unstructured.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.4/megaparse/utils.py` & `megaparse-0.0.5/megaparse/utils.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.4/megaparse.egg-info/PKG-INFO` & `megaparse-0.0.5/megaparse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaparse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Parse complex files (PDF,Docx,PPTX) for LLM consumption
 Author: Quivr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-docx
 Requires-Dist: mammoth
 Requires-Dist: python-pptx
@@ -41,15 +41,19 @@
 
 ```bash
 pip install megaparse
 ```
 
 ## Usage
 
-Add your OpenAI API key to the .env file
+1. Add your OpenAI API key to the .env file
+
+2. Install poppler on your computer (images and PDFs)
+3. 
+4. Install tesseract on your computer (images and PDFs)
 
 ```python
 from megaparse import MegaParse
 
 megaparse = MegaParse(file_path="./test.pdf")
 content = megaparse.convert()
 print(content)
```

