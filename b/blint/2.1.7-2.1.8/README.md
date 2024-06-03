# Comparing `tmp/blint-2.1.7.tar.gz` & `tmp/blint-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.1.7.tar", max compression
+gzip compressed data, was "blint-2.1.8.tar", max compression
```

## Comparing `blint-2.1.7.tar` & `blint-2.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-05-28 15:15:51.594902 blint-2.1.7/LICENSE
--rw-r--r--   0        0        0     6233 2024-05-28 15:15:51.594902 blint-2.1.7/README.md
--rw-r--r--   0        0        0        0 2024-05-28 15:15:51.594902 blint-2.1.7/blint/__init__.py
--rw-r--r--   0        0        0    24648 2024-05-28 15:15:51.594902 blint-2.1.7/blint/analysis.py
--rw-r--r--   0        0        0    13915 2024-05-28 15:15:51.594902 blint-2.1.7/blint/android.py
--rw-r--r--   0        0        0    59632 2024-05-28 15:15:51.598902 blint-2.1.7/blint/binary.py
--rw-r--r--   0        0        0     2785 2024-05-28 15:15:51.598902 blint-2.1.7/blint/checks.py
--rw-r--r--   0        0        0     6447 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cli.py
--rw-r--r--   0        0        0    20192 2024-05-28 15:15:51.598902 blint-2.1.7/blint/config.py
--rw-r--r--   0        0        0      324 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-05-28 15:15:51.598902 blint-2.1.7/blint/logger.py
--rw-r--r--   0        0        0    26828 2024-05-28 15:15:51.602902 blint-2.1.7/blint/sbom.py
--rw-r--r--   0        0        0    15610 2024-05-28 15:15:51.602902 blint-2.1.7/blint/utils.py
--rw-r--r--   0        0        0     1886 2024-05-28 15:15:51.602902 blint-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     7530 1970-01-01 00:00:00.000000 blint-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-06-03 13:41:23.706437 blint-2.1.8/LICENSE
+-rw-r--r--   0        0        0     6233 2024-06-03 13:41:23.706437 blint-2.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 13:41:23.706437 blint-2.1.8/blint/__init__.py
+-rw-r--r--   0        0        0    24648 2024-06-03 13:41:23.710437 blint-2.1.8/blint/analysis.py
+-rw-r--r--   0        0        0    13915 2024-06-03 13:41:23.710437 blint-2.1.8/blint/android.py
+-rw-r--r--   0        0        0    59706 2024-06-03 13:41:23.710437 blint-2.1.8/blint/binary.py
+-rw-r--r--   0        0        0     2785 2024-06-03 13:41:23.710437 blint-2.1.8/blint/checks.py
+-rw-r--r--   0        0        0     6447 2024-06-03 13:41:23.710437 blint-2.1.8/blint/cli.py
+-rw-r--r--   0        0        0    20192 2024-06-03 13:41:23.710437 blint-2.1.8/blint/config.py
+-rw-r--r--   0        0        0      324 2024-06-03 13:41:23.710437 blint-2.1.8/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 13:41:23.710437 blint-2.1.8/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-06-03 13:41:23.710437 blint-2.1.8/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-06-03 13:41:23.710437 blint-2.1.8/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-06-03 13:41:23.710437 blint-2.1.8/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-06-03 13:41:23.714437 blint-2.1.8/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-06-03 13:41:23.714437 blint-2.1.8/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-06-03 13:41:23.714437 blint-2.1.8/blint/logger.py
+-rw-r--r--   0        0        0    26828 2024-06-03 13:41:23.714437 blint-2.1.8/blint/sbom.py
+-rw-r--r--   0        0        0    15610 2024-06-03 13:41:23.714437 blint-2.1.8/blint/utils.py
+-rw-r--r--   0        0        0     1886 2024-06-03 13:41:23.714437 blint-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7530 1970-01-01 00:00:00.000000 blint-2.1.8/PKG-INFO
```

### Comparing `blint-2.1.7/LICENSE` & `blint-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/README.md` & `blint-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/analysis.py` & `blint-2.1.8/blint/analysis.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/android.py` & `blint-2.1.8/blint/android.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/binary.py` & `blint-2.1.8/blint/binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1006,22 +1006,23 @@
             .replace("\uFFFD", "")
             .replace("\t", " ")
         ).strip()
         build_info_str = build_info_str.encode("ascii", "ignore").decode("ascii")
     elif isinstance(parsed_obj, lief.PE.Binary):
         # For PE binaries look for .data section
         s: lief.PE.Section = parsed_obj.get_section(".data")
-        build_info_str = (
-            codecs.decode(
-                s.content.tobytes()[: int(s.size / 32)], encoding="ascii", errors="replace"
+        if s and not isinstance(s, lief.lief_errors):
+            build_info_str = (
+                codecs.decode(
+                    s.content.tobytes()[: int(s.size / 32)], encoding="ascii", errors="replace"
+                )
+                .replace("\0", "")
+                .replace("\uFFFD", "")
+                .replace("\t", " ")
             )
-            .replace("\0", "")
-            .replace("\uFFFD", "")
-            .replace("\t", " ")
-        )
     lines = build_info_str.split("\n")
     for line in lines:
         if line.startswith("Go buildinf:"):
             tmp_a = line.split("Go buildinf:")
             formulation["go_version"] = tmp_a[-1].split("\x19")[0].split(" ")[-1]
         if "path " in line:
             tmp_a = line.split("path ")
@@ -1040,15 +1041,15 @@
             formulation[tmp_a[0].replace("-", "")] = tmp_a[1]
 
     return deps, formulation
 
 
 def parse_rust_buildinfo(parsed_obj: lief.Binary) -> list:
     """
-    Parse the rust build info section of binaries that are cargo-auditable to extract rust dependencies
+    Parse the rust build info section that are cargo-auditable to extract rust dependencies
     Args:
         parsed_obj (lief.Binary): The parsed object representing the binary.
 
     Returns:
         list: List representing the dependencies.
     """
     deps = []
```

### Comparing `blint-2.1.7/blint/checks.py` & `blint-2.1.8/blint/checks.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/cli.py` & `blint-2.1.8/blint/cli.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/config.py` & `blint-2.1.8/blint/config.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/cyclonedx/spdx.py` & `blint-2.1.8/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/cyclonedx/spec.py` & `blint-2.1.8/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_entries_generic.yml` & `blint-2.1.8/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_entries_pe.yml` & `blint-2.1.8/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_exe_go.yml` & `blint-2.1.8/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_imports_pe.yml` & `blint-2.1.8/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_methods_generic.yml` & `blint-2.1.8/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_methods_mips.yml` & `blint-2.1.8/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_monero_generic.yml` & `blint-2.1.8/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_monero_go.yml` & `blint-2.1.8/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_monero_rust` & `blint-2.1.8/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_monero_rust.yml` & `blint-2.1.8/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_rootkits_win.yml` & `blint-2.1.8/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.1.8/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_symbols_generic.yml` & `blint-2.1.8/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.1.8/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_symbols_macho.yml` & `blint-2.1.8/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/annotations/review_symbols_rust.yml` & `blint-2.1.8/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/data/rules.yml` & `blint-2.1.8/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/logger.py` & `blint-2.1.8/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/sbom.py` & `blint-2.1.8/blint/sbom.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/blint/utils.py` & `blint-2.1.8/blint/utils.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.7/pyproject.toml` & `blint-2.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.1.7"
+version = "2.1.8"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
@@ -25,20 +25,20 @@
 "CI" = "https://github.com/AppThreat/blint/actions"
 
 [tool.poetry.scripts]
 blint = 'blint.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
-lief = "^0.14.0"
-rich = "^13.7.0"
+lief = "^0.14.1"
+rich = "^13.7.1"
 PyYAML = "^6.0.1"
 defusedxml = "^0.7.1"
 pydantic = {version = "^2.6.0", extras = ["email"]}
-orjson = "^3.10.1"
+orjson = "^3.10.3"
 symbolic = "10.2.1"
 ar = "^0.9.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 black = "^24.0.0"
 flake8 = "^7.0.0"
```

### Comparing `blint-2.1.7/PKG-INFO` & `blint-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.1.7
+Version: 2.1.8
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
@@ -18,18 +18,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: ar (>=0.9.1,<0.10.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: lief (>=0.14.0,<0.15.0)
-Requires-Dist: orjson (>=3.10.1,<4.0.0)
+Requires-Dist: lief (>=0.14.1,<0.15.0)
+Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: pydantic[email] (>=2.6.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: symbolic (==10.2.1)
 Project-URL: CI, https://github.com/AppThreat/blint/actions
 Project-URL: Repository, https://github.com/OWASP-dep-scan/blint
 Description-Content-Type: text/markdown
 
 # BLint
```

