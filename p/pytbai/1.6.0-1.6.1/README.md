# Comparing `tmp/pytbai-1.6.0.tar.gz` & `tmp/pytbai-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.6.0.tar", last modified: Wed May 29 09:06:13 2024, max compression
+gzip compressed data, was "pytbai-1.6.1.tar", last modified: Mon Jun  3 11:45:38 2024, max compression
```

## Comparing `pytbai-1.6.0.tar` & `pytbai-1.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.432516 pytbai-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-29 09:06:09.000000 pytbai-1.6.0/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 09:06:09.000000 pytbai-1.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-29 09:06:09.000000 pytbai-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-29 09:06:09.000000 pytbai-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 09:06:09.000000 pytbai-1.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-29 09:06:13.432516 pytbai-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-29 09:06:09.000000 pytbai-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.428516 pytbai-1.6.0/pytbai/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.428516 pytbai-1.6.0/pytbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.428516 pytbai-1.6.0/pytbai/templates/XML/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/templates/XML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/templates/XML/tbai_structure.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.432516 pytbai-1.6.0/pytbai/templates/XSD/
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/templates/XSD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.432516 pytbai-1.6.0/pytbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-29 09:06:09.000000 pytbai-1.6.0/pytbai/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.432516 pytbai-1.6.0/pytbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-29 09:06:13.000000 pytbai-1.6.0/pytbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 09:06:13.000000 pytbai-1.6.0/pytbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:06:13.000000 pytbai-1.6.0/pytbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 09:06:13.000000 pytbai-1.6.0/pytbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 09:06:13.000000 pytbai-1.6.0/pytbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:06:13.432516 pytbai-1.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-29 09:06:09.000000 pytbai-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.432516 pytbai-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:09.000000 pytbai-1.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.432516 pytbai-1.6.0/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-29 09:06:09.000000 pytbai-1.6.0/tests/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-29 09:06:09.000000 pytbai-1.6.0/tests/certs/cert_for_tests.p12
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-29 09:06:09.000000 pytbai-1.6.0/tests/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-29 09:06:09.000000 pytbai-1.6.0/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:06:13.432516 pytbai-1.6.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-29 09:06:09.000000 pytbai-1.6.0/tests/data/tbai_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-29 09:06:09.000000 pytbai-1.6.0/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.616455 pytbai-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-03 11:45:34.000000 pytbai-1.6.1/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-03 11:45:34.000000 pytbai-1.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-06-03 11:45:34.000000 pytbai-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-06-03 11:45:34.000000 pytbai-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 11:45:34.000000 pytbai-1.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-06-03 11:45:38.616455 pytbai-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-06-03 11:45:34.000000 pytbai-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.612455 pytbai-1.6.1/pytbai/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.612455 pytbai-1.6.1/pytbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.612455 pytbai-1.6.1/pytbai/templates/XML/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/templates/XML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/templates/XML/tbai_structure.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.612455 pytbai-1.6.1/pytbai/templates/XSD/
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/templates/XSD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.616455 pytbai-1.6.1/pytbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-06-03 11:45:34.000000 pytbai-1.6.1/pytbai/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.616455 pytbai-1.6.1/pytbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-06-03 11:45:38.000000 pytbai-1.6.1/pytbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-03 11:45:38.000000 pytbai-1.6.1/pytbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:45:38.000000 pytbai-1.6.1/pytbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 11:45:38.000000 pytbai-1.6.1/pytbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 11:45:38.000000 pytbai-1.6.1/pytbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:45:38.616455 pytbai-1.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-06-03 11:45:34.000000 pytbai-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.616455 pytbai-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:34.000000 pytbai-1.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.616455 pytbai-1.6.1/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-06-03 11:45:34.000000 pytbai-1.6.1/tests/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-06-03 11:45:34.000000 pytbai-1.6.1/tests/certs/cert_for_tests.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-06-03 11:45:34.000000 pytbai-1.6.1/tests/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-03 11:45:34.000000 pytbai-1.6.1/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:38.616455 pytbai-1.6.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-06-03 11:45:34.000000 pytbai-1.6.1/tests/data/tbai_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-06-03 11:45:34.000000 pytbai-1.6.1/tests/test_basic.py
```

### Comparing `pytbai-1.6.0/CHANGELOG.txt` & `pytbai-1.6.1/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/LICENSE` & `pytbai-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/PKG-INFO` & `pytbai-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.6.0
+Version: 1.6.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.6.0/README.md` & `pytbai-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/pytbai/core.py` & `pytbai-1.6.1/pytbai/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 
 
 class Subject:
     def __init__(
         self,
         entity_id,
         name,
+        address=None,
         territory=GIPUZKOA,
         multi_recipient=N,
         external_invoice=N,
         env="DEV",
     ):
         self.entity_id = entity_id
         self.name = name
+        self.address = address
         if not territory:
             self.authority_api = GIPUZKOA[env]["invoice"]
             self.qr_api = GIPUZKOA[env]["qr"]
         elif territory in AUTHORITY_APIS:
             self.authority_api = AUTHORITY_APIS[territory][env]["invoice"]
             self.qr_api = AUTHORITY_APIS[territory][env]["qr"]
         else:
```

### Comparing `pytbai-1.6.0/pytbai/definitions.py` & `pytbai-1.6.1/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.6.1/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.6.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.6.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/pytbai/utils/xml.py` & `pytbai-1.6.1/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/pytbai.egg-info/PKG-INFO` & `pytbai-1.6.1/pytbai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.6.0
+Version: 1.6.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.6.0/pytbai.egg-info/SOURCES.txt` & `pytbai-1.6.1/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/setup.py` & `pytbai-1.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.6.0",
+    version="1.6.1",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.6.0/tests/certs/cert.pem` & `pytbai-1.6.1/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/tests/certs/cert_for_tests.p12` & `pytbai-1.6.1/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/tests/certs/key.pem` & `pytbai-1.6.1/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/tests/data/tbai_json.py` & `pytbai-1.6.1/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.6.0/tests/test_basic.py` & `pytbai-1.6.1/tests/test_basic.py`

 * *Files identical despite different names*

