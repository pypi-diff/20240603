# Comparing `tmp/bd_sig_filter-1.1.tar.gz` & `tmp/bd_sig_filter-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bd_sig_filter-1.1.tar", last modified: Sun Jun  2 12:44:51 2024, max compression
+gzip compressed data, was "bd_sig_filter-1.2.tar", last modified: Mon Jun  3 10:12:14 2024, max compression
```

## Comparing `bd_sig_filter-1.1.tar` & `bd_sig_filter-1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:51.169963 bd_sig_filter-1.1/bd_sig_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/BOMClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/ComponentClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/ComponentListClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/SigEntryClass.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2742 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/bd_data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1416 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/bd_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5395 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/global_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/bd_sig_filter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/bd_sig_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 12:44:51.000000 bd_sig_filter-1.1/bd_sig_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-02 12:44:41.000000 bd_sig_filter-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:44:51.173963 bd_sig_filter-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:12:14.173906 bd_sig_filter-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-06-03 10:12:14.173906 bd_sig_filter-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:12:14.169906 bd_sig_filter-1.2/bd_sig_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/BOMClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/ComponentClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/ComponentListClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/SigEntryClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2742 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/bd_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1416 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/bd_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5395 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/global_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/bd_sig_filter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:12:14.173906 bd_sig_filter-1.2/bd_sig_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-06-03 10:12:14.000000 bd_sig_filter-1.2/bd_sig_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-03 10:12:14.000000 bd_sig_filter-1.2/bd_sig_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:12:14.000000 bd_sig_filter-1.2/bd_sig_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 10:12:14.000000 bd_sig_filter-1.2/bd_sig_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-03 10:12:14.000000 bd_sig_filter-1.2/bd_sig_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 10:12:14.000000 bd_sig_filter-1.2/bd_sig_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-03 10:12:08.000000 bd_sig_filter-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 10:12:14.173906 bd_sig_filter-1.2/setup.cfg
```

### Comparing `bd_sig_filter-1.1/LICENSE` & `bd_sig_filter-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.1/bd_sig_filter/BOMClass.py` & `bd_sig_filter-1.2/bd_sig_filter/BOMClass.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.1/bd_sig_filter/ComponentClass.py` & `bd_sig_filter-1.2/bd_sig_filter/ComponentClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.ignore = False
         self.mark_reviewed = False
         self.filter_name = self.filter_name_string(name)
         self.filter_version = self.filter_version_string(version)
         self.sig_match_result = -1
         self.compname_found = False
         self.compver_found = False
-        self.reason = 'No Action'
+        self.reason = 'No Action - compname or version not found in Sig paths'
         self.best_sigpath = ''
 
     def get_compverid(self):
         try:
             return self.data['componentVersion'].split('/')[-1]
         except KeyError:
             return ''
@@ -136,17 +136,27 @@
 
     @staticmethod
     def filter_name_string(name):
         # Remove common words
         # - for, with, in, on,
         # Remove strings in brackets
         # Replace / with space
-        ret_name = re.sub(r" for | with | in | on | a |apache ", r" ", name, flags=re.IGNORECASE)
-        ret_name = re.sub(r"\(.*\)", r"", ret_name)
-        ret_name = re.sub(r"/", r" ", ret_name)
+        ret_name = re.sub(r"\(.*\)", r"", name)
+        for rep in [r" for ", r" with ", r" in ", r" on ", r" a ", r" the ", r" by ",
+                    r" and ", r"^apache | apache | apache$", r" bundle ", r" only | only$", r" from ",
+                    r" to ", r" - "]:
+            ret_name = re.sub(rep, " ", ret_name, flags=re.IGNORECASE)
+        ret_name = re.sub(r"[/@#:]", " ", ret_name)
+        ret_name = re.sub(r" \w$| \w |^\w ", r" ", ret_name)
+        ret_name = ret_name.replace("::", " ")
+        ret_name = re.sub(r"  *", r" ", ret_name)
+        ret_name = re.sub(r"^ ", r"", ret_name)
+        ret_name = re.sub(r" $", r"", ret_name)
+
+        logging.debug(f"filter_name_string(): Compname '{name}' replaced with '{ret_name}'")
         return ret_name
 
     @staticmethod
     def filter_version_string(version):
         # Remove +git*
         # Remove -snapshot*
         # Replace / with space
```

### Comparing `bd_sig_filter-1.1/bd_sig_filter/ComponentListClass.py` & `bd_sig_filter-1.2/bd_sig_filter/ComponentListClass.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.1/bd_sig_filter/SigEntryClass.py` & `bd_sig_filter-1.2/bd_sig_filter/SigEntryClass.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
             # self.elements = self.path.replace("!", os.sep).replace("#", os.sep).split(os.sep)
             self.elements = list(filter(None, elements))
 
         except KeyError:
             return
 
     def search_component(self, compname, compver):
+        logging.debug("")
         logging.debug(f"search_component() Checking Comp '{compname}/{compver}' - {self.path}:")
         # If component_version_reqd:
         # - folder matches compname and compver
         # - folder1 matches compname and folder2 matches compver
         # Else:
         # - folder matches compname
         # Returns:
@@ -29,16 +30,18 @@
         # Match_value - search result against both
 
         compstring = f"{compname} {compver}"
         element_in_compname = 0
         compver_in_element = 0
 
         # test of path search
-        comp_in_path = fuzz.token_set_ratio(compstring, self.path)
-        logging.debug(f"search_component(): comp_in_path is {comp_in_path}: path='{self.path}")
+        newpath = self.path.replace(os.sep, " ")
+        newpath = re.sub(r"([a-zA-Z-]*)[0-9] ", "\1 ", newpath)
+        comp_in_path = fuzz.token_set_ratio(compstring, newpath)
+        logging.debug(f"search_component(): TEST comp_in_path is {comp_in_path}: path='{self.path}")
 
         found_compname_only = False
         for element in self.elements:
             pos = re.search(r"\.dll|\.obj|\.o|\.a|\.lib|\.iso|\.qcow2|\.vmdk|\.vdi|\.ova|\.nbi|\.vib|\.exe|\.img|"
                             "\.bin|\.apk|\.aac|\.ipa|\.msi|\.zip|\.gz|\.tar|\.xz|\.lz|\.bz2|\.7z|\.rar|"
                             "\.cpio|\.Z|\.lz4|\.lha|\.arj|\.jar|\.ear|\.war|\.rpm|\.deb|\.dmg|\.pki", element)
             if pos is not None:
@@ -58,14 +61,16 @@
                 elif element_in_compname > 50 and len(element) > 2:
                     found_compname_only = True
                     logging.debug(f"search_component() - FOUND component name ONLY ({compname}) in '{element}'")
             elif found_compname_only:
                 if compver_in_element > 50:
                     logging.debug(f"search_component() - MATCHED component version ({compver}) in '{element}'")
                     return True, True, element_in_compname + compver_in_element
+                else:
+                    test = 1
 
         if found_compname_only:
             logging.debug("search_component() - MATCHED Compname only")
             return True, False, element_in_compname + compver_in_element
 
         logging.debug(f"search_component() - NOT MATCHED")
         return False, False, 0
@@ -85,13 +90,15 @@
             def_folders = ['.cache', '.m2', '.local', '.cache','.config', '.docker', '.npm', '.npmrc', '.pyenv',
                            '.Trash', '.git', 'node_modules']
             for e in self.elements:
                 if e in def_folders:
                     return True, f"Found '{e}' in Signature match path '{self.path}'"
 
         if not global_values.no_ignore_test:
-            test_folders = ['test', 'tests']
+            test_folders = r"^test$|^tests$|^testsuite$"
             for e in self.elements:
-                if e in test_folders:
+                if re.search(test_folders, e, flags=re.IGNORECASE) is not None:
                     return True, f"Found '{e}' in Signature match path '{self.path}'"
+                # if e in test_folders:
+                #     return True, f"Found '{e}' in Signature match path '{self.path}'"
 
         return False, ''
```

### Comparing `bd_sig_filter-1.1/bd_sig_filter/bd_data.py` & `bd_sig_filter-1.2/bd_sig_filter/bd_data.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.1/bd_sig_filter/bd_project.py` & `bd_sig_filter-1.2/bd_sig_filter/bd_project.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.1/bd_sig_filter/config.py` & `bd_sig_filter-1.2/bd_sig_filter/config.py`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.1/bd_sig_filter.egg-info/SOURCES.txt` & `bd_sig_filter-1.2/bd_sig_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bd_sig_filter-1.1/pyproject.toml` & `bd_sig_filter-1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bd_sig_filter"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="Matthew Brady", email="mbrad@synopsys.com" },
 ]
 description = "BD_sig_filter - BD Script to ignore components matched from Signature scan likely to be partial or invalid matches."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

