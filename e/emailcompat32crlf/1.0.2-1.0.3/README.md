# Comparing `tmp/emailcompat32crlf-1.0.2.tar.gz` & `tmp/emailcompat32crlf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailcompat32crlf-1.0.2.tar", last modified: Fri May 31 22:46:13 2024, max compression
+gzip compressed data, was "emailcompat32crlf-1.0.3.tar", last modified: Mon Jun  3 08:33:47 2024, max compression
```

## Comparing `emailcompat32crlf-1.0.2.tar` & `emailcompat32crlf-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-31 22:46:13.298669 emailcompat32crlf-1.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)       57 2024-05-31 22:46:12.000000 emailcompat32crlf-1.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     2879 2024-05-31 22:46:13.298330 emailcompat32crlf-1.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2128 2024-05-31 22:46:12.000000 emailcompat32crlf-1.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-31 22:46:13.295703 emailcompat32crlf-1.0.2/emailcompat32crlf/
--rw-r--r--   0 maurits    (501) staff       (20)      517 2024-05-31 22:46:12.000000 emailcompat32crlf-1.0.2/emailcompat32crlf/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-31 22:46:13.297792 emailcompat32crlf-1.0.2/emailcompat32crlf.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     2879 2024-05-31 22:46:13.000000 emailcompat32crlf-1.0.2/emailcompat32crlf.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      265 2024-05-31 22:46:13.000000 emailcompat32crlf-1.0.2/emailcompat32crlf.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-31 22:46:13.000000 emailcompat32crlf-1.0.2/emailcompat32crlf.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-31 22:46:13.000000 emailcompat32crlf-1.0.2/emailcompat32crlf.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       18 2024-05-31 22:46:13.000000 emailcompat32crlf-1.0.2/emailcompat32crlf.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-31 22:46:13.298801 emailcompat32crlf-1.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1011 2024-05-31 22:46:12.000000 emailcompat32crlf-1.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-06-03 08:33:47.282065 emailcompat32crlf-1.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)      440 2024-06-03 08:33:46.000000 emailcompat32crlf-1.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       57 2024-06-03 08:33:46.000000 emailcompat32crlf-1.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     3424 2024-06-03 08:33:47.282177 emailcompat32crlf-1.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2231 2024-06-03 08:33:46.000000 emailcompat32crlf-1.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-06-03 08:33:47.280210 emailcompat32crlf-1.0.3/emailcompat32crlf/
+-rw-r--r--   0 maurits    (501) staff       (20)      517 2024-06-03 08:33:46.000000 emailcompat32crlf-1.0.3/emailcompat32crlf/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-06-03 08:33:47.281836 emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     3424 2024-06-03 08:33:47.000000 emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      331 2024-06-03 08:33:47.000000 emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-06-03 08:33:47.000000 emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-06-03 08:33:47.000000 emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-06-03 08:33:47.000000 emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       18 2024-06-03 08:33:47.000000 emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      102 2024-06-03 08:33:47.282551 emailcompat32crlf-1.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1290 2024-06-03 08:33:46.000000 emailcompat32crlf-1.0.3/setup.py
```

### Comparing `emailcompat32crlf-1.0.2/PKG-INFO` & `emailcompat32crlf-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailcompat32crlf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Patch stdlib email compat32 policy to default to CRLF line endings.
 Home-page: https://github.com/collective/emailcompat32crlf
 Author: Guido Stevens
 Author-email: guido.stevens@cosent.net
 License: MIT
 Keywords: email
 Classifier: Development Status :: 4 - Beta
@@ -51,7 +51,38 @@
 
 Because to fix your own code, you'd have to ensure to override the default
 policy in every single instantiation of every ``Message`` or ``MIMEText`` or any
 of the other constructors which default to the ``compat32`` policy
 without carriage returns.
 
 Instead, you now can simply add ``emailcompat32crlf`` to your project dependencies and import it. Done.
+
+If you are using Plone: we register an autoinclude entry point, so you do not even need to import it.
+
+
+Changelog
+=========
+
+1.0.3 (2024-06-03)
+------------------
+
+- Register z3c.autoinclude.plugin entry point for Plone.
+  This imports the package automatically on startup.
+  This entry point is ignored when you don't use Plone.
+
+
+1.0.2 (2024-05-31)
+------------------
+
+- Fix possible import error.
+
+
+1.0.1 (2024-05-31)
+------------------
+
+- Fix several problems in initial release.
+
+
+1.0.0 (2024-05-31)
+------------------
+
+- Initial release.
```

### Comparing `emailcompat32crlf-1.0.2/README.rst` & `emailcompat32crlf-1.0.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,7 +31,9 @@
 
 Because to fix your own code, you'd have to ensure to override the default
 policy in every single instantiation of every ``Message`` or ``MIMEText`` or any
 of the other constructors which default to the ``compat32`` policy
 without carriage returns.
 
 Instead, you now can simply add ``emailcompat32crlf`` to your project dependencies and import it. Done.
+
+If you are using Plone: we register an autoinclude entry point, so you do not even need to import it.
```

### Comparing `emailcompat32crlf-1.0.2/emailcompat32crlf/__init__.py` & `emailcompat32crlf-1.0.3/emailcompat32crlf/__init__.py`

 * *Files identical despite different names*

### Comparing `emailcompat32crlf-1.0.2/emailcompat32crlf.egg-info/PKG-INFO` & `emailcompat32crlf-1.0.3/emailcompat32crlf.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailcompat32crlf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Patch stdlib email compat32 policy to default to CRLF line endings.
 Home-page: https://github.com/collective/emailcompat32crlf
 Author: Guido Stevens
 Author-email: guido.stevens@cosent.net
 License: MIT
 Keywords: email
 Classifier: Development Status :: 4 - Beta
@@ -51,7 +51,38 @@
 
 Because to fix your own code, you'd have to ensure to override the default
 policy in every single instantiation of every ``Message`` or ``MIMEText`` or any
 of the other constructors which default to the ``compat32`` policy
 without carriage returns.
 
 Instead, you now can simply add ``emailcompat32crlf`` to your project dependencies and import it. Done.
+
+If you are using Plone: we register an autoinclude entry point, so you do not even need to import it.
+
+
+Changelog
+=========
+
+1.0.3 (2024-06-03)
+------------------
+
+- Register z3c.autoinclude.plugin entry point for Plone.
+  This imports the package automatically on startup.
+  This entry point is ignored when you don't use Plone.
+
+
+1.0.2 (2024-05-31)
+------------------
+
+- Fix possible import error.
+
+
+1.0.1 (2024-05-31)
+------------------
+
+- Fix several problems in initial release.
+
+
+1.0.0 (2024-05-31)
+------------------
+
+- Initial release.
```

### Comparing `emailcompat32crlf-1.0.2/setup.py` & `emailcompat32crlf-1.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-# -*- coding: utf-8 -*-
+from pathlib import Path
 from setuptools import setup, find_packages
 
+
+contents = []
+for filename in ("README.rst", "CHANGES.rst"):
+    path = Path(filename)
+    with path.open() as myfile:
+        contents.append(myfile.read())
+long_description = "\n\n".join(contents)
+
 setup(name='emailcompat32crlf',
-      version='1.0.2',
+      version='1.0.3',
       description='Patch stdlib email compat32 policy to default to CRLF line endings.',
-      long_description=open('README.rst').read(),
+      long_description=long_description,
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
@@ -19,8 +27,12 @@
       url='https://github.com/collective/emailcompat32crlf',
       keywords=["email"],
       author='Guido Stevens',
       author_email='guido.stevens@cosent.net',
       license='MIT',
       python_requires=">=3.8",
       packages=find_packages(),
-      zip_safe=False)
+      zip_safe=False,
+      entry_points="""
+      [z3c.autoinclude.plugin]
+      target = plone
+      """)
```

