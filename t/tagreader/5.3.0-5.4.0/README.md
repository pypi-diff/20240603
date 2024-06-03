# Comparing `tmp/tagreader-5.3.0.tar.gz` & `tmp/tagreader-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-5.3.0.tar", max compression
+gzip compressed data, was "tagreader-5.4.0.tar", max compression
```

## Comparing `tagreader-5.3.0.tar` & `tagreader-5.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1085 2024-04-19 11:41:44.416766 tagreader-5.3.0/LICENSE
--rw-r--r--   0        0        0     1804 2024-04-19 11:41:44.416766 tagreader-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     2303 2024-04-19 11:41:44.416766 tagreader-5.3.0/README.md
--rw-r--r--   0        0        0      318 2024-04-19 11:41:44.416766 tagreader-5.3.0/tagreader/__init__.py
--rw-r--r--   0        0        0      289 2024-04-19 11:41:44.416766 tagreader-5.3.0/tagreader/__version__.py
--rw-r--r--   0        0        0    12149 2024-04-19 11:41:44.416766 tagreader-5.3.0/tagreader/cache.py
--rw-r--r--   0        0        0    22781 2024-04-19 11:41:44.416766 tagreader-5.3.0/tagreader/clients.py
--rw-r--r--   0        0        0      208 2024-04-19 11:41:44.416766 tagreader-5.3.0/tagreader/logger.py
--rw-r--r--   0        0        0     9217 2024-04-19 11:41:44.416766 tagreader-5.3.0/tagreader/utils.py
--rw-r--r--   0        0        0    36782 2024-04-19 11:41:44.432390 tagreader-5.3.0/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 tagreader-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-06-03 12:18:35.500216 tagreader-5.4.0/LICENSE
+-rw-r--r--   0        0        0     1816 2024-06-03 12:18:35.515841 tagreader-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2303 2024-06-03 12:18:35.500216 tagreader-5.4.0/README.md
+-rw-r--r--   0        0        0      318 2024-06-03 12:18:35.515841 tagreader-5.4.0/tagreader/__init__.py
+-rw-r--r--   0        0        0      289 2024-06-03 12:18:35.515841 tagreader-5.4.0/tagreader/__version__.py
+-rw-r--r--   0        0        0    12149 2024-06-03 12:18:35.515841 tagreader-5.4.0/tagreader/cache.py
+-rw-r--r--   0        0        0    22781 2024-06-03 12:18:35.515841 tagreader-5.4.0/tagreader/clients.py
+-rw-r--r--   0        0        0      208 2024-06-03 12:18:35.515841 tagreader-5.4.0/tagreader/logger.py
+-rw-r--r--   0        0        0     8743 2024-06-03 12:18:35.515841 tagreader-5.4.0/tagreader/utils.py
+-rw-r--r--   0        0        0    36842 2024-06-03 12:18:35.515841 tagreader-5.4.0/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 tagreader-5.4.0/PKG-INFO
```

### Comparing `tagreader-5.3.0/LICENSE` & `tagreader-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tagreader-5.3.0/pyproject.toml` & `tagreader-5.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tagreader"
-version = "5.3.0"
+version = "5.4.0"
 description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
 authors = ["Einar S. Idsø <eiids@equinor.com>", "Morten Dæhli Aslesen <masl@equinor.com"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tagreader"}]
 keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
 homepage = "https://github.com/equinor/tagreader-python"
@@ -29,25 +29,25 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = ">=1"
 certifi = "^2023.7.22"
 requests = "^2"
 requests-kerberos = "^0"
-msal-bearer = "^0.2.1"
+msal-bearer = ">=0.2.1,<1.1.0"
 notebook = { version = "^7.0.3", optional = true }
 matplotlib = { version = "^3", optional = true }
 diskcache = "^5.6.1"
 pycryptodome = "^3.20.0"
 requests-ntlm = ">=1.1,<=2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3"
-pytest = "^7"
+pytest = ">=7,<9"
 
 [tool.poetry.extras]
 notebooks = ["notebook", "matplotlib"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tagreader-5.3.0/README.md` & `tagreader-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tagreader-5.3.0/tagreader/cache.py` & `tagreader-5.4.0/tagreader/cache.py`

 * *Files identical despite different names*

### Comparing `tagreader-5.3.0/tagreader/clients.py` & `tagreader-5.4.0/tagreader/clients.py`

 * *Files identical despite different names*

### Comparing `tagreader-5.3.0/tagreader/utils.py` & `tagreader-5.4.0/tagreader/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,19 +125,15 @@
     GOOD = enum.auto()  # Number of good data points
     BAD = NOTGOOD = enum.auto()  # Number of not good data points
     TOTAL = enum.auto()  # Number of total data
     SUM = enum.auto()  # Sum of data
     SNAPSHOT = FINAL = LAST = enum.auto()  # Last sampled value
 
 
-def add_statoil_root_certificate() -> bool:
-    return add_equinor_root_certificate(True) and add_equinor_root_certificate(False)
-
-
-def add_equinor_root_certificate(get_equinor: bool = True) -> bool:
+def add_equinor_root_certificate() -> bool:
     """
     This is a utility function for Equinor employees on Equinor managed machines.
 
     The function searches for the Equinor Root certificate in the
     cert store and imports it to the cacert bundle. Does nothing if not
     running on Equinor host.
 
@@ -148,49 +144,42 @@
         bool: True if function completes successfully
     """
     import hashlib
     import ssl
 
     import certifi
 
-    STATOIL_ROOT_PEM_HASH = "ce7bb185ab908d2fea28c7d097841d9d5bbf2c76"
     EQUINOR_root_PEM_HASH = "5A206332CE73CED1D44C8A99C4C43B7CEE03DF5F"
-
-    if get_equinor:
-        used_hash = EQUINOR_root_PEM_HASH.upper()
-        ca_search = "Equinor Root CA"
-    else:
-        used_hash = STATOIL_ROOT_PEM_HASH.upper()
-        ca_search = "Statoil Root CA"
+    ca_search = "Equinor Root CA"
 
     found = False
     der = None
 
     if is_linux():
         return True
     elif is_windows():
         logger.debug("Scanning CA certificate in Windows cert store", end="")
         for cert in ssl.enum_certificates("CA"):
             der = cert[0]
             # deepcode ignore InsecureHash: <Only hashes to compare with known hash>
-            if hashlib.sha1(der).hexdigest().upper() == used_hash:
+            if hashlib.sha1(der).hexdigest().upper() == EQUINOR_root_PEM_HASH:
                 found = True
                 logger.debug("CA certificate found!")
                 break
     elif is_mac():
         macos_ca_certs = subprocess.run(
             ["security", "find-certificate", "-a", "-c", ca_search, "-Z"],
             stdout=subprocess.PIPE,
         ).stdout
 
-        if used_hash in str(macos_ca_certs).upper():
+        if EQUINOR_root_PEM_HASH in str(macos_ca_certs).upper():
             c = get_macos_equinor_certificates()
             for cert in c:
                 # deepcode ignore InsecureHash: <Only hashes to compare with known hash>
-                if hashlib.sha1(cert).hexdigest().upper() == used_hash:
+                if hashlib.sha1(cert).hexdigest().upper() == EQUINOR_root_PEM_HASH:
                     der = cert
                     found = True
                     break
 
     if found and der:
         pem = ssl.DER_cert_to_PEM_cert(der)
         if pem in certifi.contents():
@@ -205,22 +194,19 @@
             logger.debug("Completed")
     else:
         warnings.warn("Unable to locate root certificate on this host.")
 
     return found
 
 
-def get_macos_equinor_certificates(get_equinor: bool = True):
+def get_macos_equinor_certificates():
     import ssl
     import tempfile
 
-    if get_equinor:
-        ca_search = "Equinor Root CA"
-    else:
-        ca_search = "Statoil Root CA"
+    ca_search = "Equinor Root CA"
 
     ctx = ssl.create_default_context()
     macos_ca_certs = subprocess.run(
         ["security", "find-certificate", "-a", "-c", ca_search, "-p"],
         stdout=subprocess.PIPE,
     ).stdout
     with tempfile.NamedTemporaryFile("w+b", delete=False) as tmp_file:
```

### Comparing `tagreader-5.3.0/tagreader/web_handlers.py` & `tagreader-5.4.0/tagreader/web_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,19 +519,21 @@
             "</Q>",
         ]
         return "".join(parts)
 
     def _get_tag_description(self, tag: str):
         query = self.generate_get_description_query(tag)
         url = urljoin(self.base_url, "TagInfo")
-        data = self.fetch(url, params=query)
         try:
+            data = self.fetch(url, params=query)
             desc = data["data"]["tags"][0]["attrData"][0]["samples"][0]["v"]
         except KeyError:
             desc = ""
+        except JSONDecodeError:
+            desc = ""
         return desc
 
     def read_tag(
         self,
         tag: str,
         start: Optional[datetime],
         end: Optional[datetime],
```

### Comparing `tagreader-5.3.0/PKG-INFO` & `tagreader-5.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 5.3.0
+Version: 5.4.0
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
 Home-page: https://github.com/equinor/tagreader-python
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
@@ -25,15 +25,15 @@
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: notebooks
 Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: matplotlib (>=3,<4) ; extra == "notebooks"
-Requires-Dist: msal-bearer (>=0.2.1,<0.3.0)
+Requires-Dist: msal-bearer (>=0.2.1,<1.1.0)
 Requires-Dist: notebook (>=7.0.3,<8.0.0) ; extra == "notebooks"
 Requires-Dist: pandas (>=1)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: requests-kerberos (>=0,<1)
 Requires-Dist: requests-ntlm (>=1.1,<=2.0)
 Project-URL: Repository, https://github.com/equinor/tagreader-python
```

