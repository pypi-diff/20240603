# Comparing `tmp/postcode_to_timezone-2024.6.1.tar.gz` & `tmp/postcode_to_timezone-2024.6.2.tar.gz`

## Comparing `postcode_to_timezone-2024.6.1.tar` & `postcode_to_timezone-2024.6.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.1/postcode_to_timezone.py
--rw-r--r--   0        0        0    71623 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.1/postcode_to_timezone_lookup.csv
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.1/LICENSE
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.1/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.1/pyproject.toml
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.2/postcode_to_timezone.py
+-rw-r--r--   0        0        0    71623 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.2/postcode_to_timezone_lookup.csv
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.2/LICENSE
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.2/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 postcode_to_timezone-2024.6.2/PKG-INFO
```

### Comparing `postcode_to_timezone-2024.6.1/postcode_to_timezone.py` & `postcode_to_timezone-2024.6.2/postcode_to_timezone.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 return None
 
     return "".join(filter(str.isalnum, postcode))
 
 
 @functools.cache
 def _postcodes_lookup():
-    with open('postcodes-lookup.csv', 'rt') as f:
+    with open('postcode_to_timezone_lookup.csv', 'rt') as f:
         return [tuple(line.split(',')) for line in f]
 
 
 def get_tz(country_code: str, postcode: str) -> str | None:
     country_code = country_code.lower()
     postcode = normalize_postcode(country_code, postcode)
```

### Comparing `postcode_to_timezone-2024.6.1/postcode_to_timezone_lookup.csv` & `postcode_to_timezone-2024.6.2/postcode_to_timezone_lookup.csv`

 * *Files identical despite different names*

### Comparing `postcode_to_timezone-2024.6.1/LICENSE` & `postcode_to_timezone-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postcode_to_timezone-2024.6.1/README.md` & `postcode_to_timezone-2024.6.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# Postcode to Timezone
+
+Example:
+
+```python
+from postcode_to_timezone import postcode_to_timezone
+
+postcode_to_timezone('NL', '1234 AB')
+```
+
+return `'Europe/Amsterdam'`
+
 ## Sources
 
 ### `location_postcode.csv.xz`
 
 A dump of the location_postcode table in a Nominatim database. Nominatim creates this database from OpenStreetMap data using the following query:
 
 ```sql
```

### Comparing `postcode_to_timezone-2024.6.1/pyproject.toml` & `postcode_to_timezone-2024.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "postcode-to-timezone"
-version = "2024.6.1"
+version = "2024.6.2"
 dependencies = []
 
 authors = [{ name = "Koert van der Veer", email = "pypi@ondergetekende.nl" }]
 
 maintainers = [
   { name = "Koert van der Veer", email = "pypi@ondergetekende.nl" },
 ]
```

### Comparing `postcode_to_timezone-2024.6.1/PKG-INFO` & `postcode_to_timezone-2024.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.3
 Name: postcode-to-timezone
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: Converts postcodes to timezones
 Author-email: Koert van der Veer <pypi@ondergetekende.nl>
 Maintainer-email: Koert van der Veer <pypi@ondergetekende.nl>
 License: Copyright 2024 Koert van der Veer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE
 Description-Content-Type: text/markdown
 
+# Postcode to Timezone
+
+Example:
+
+```python
+from postcode_to_timezone import postcode_to_timezone
+
+postcode_to_timezone('NL', '1234 AB')
+```
+
+return `'Europe/Amsterdam'`
+
 ## Sources
 
 ### `location_postcode.csv.xz`
 
 A dump of the location_postcode table in a Nominatim database. Nominatim creates this database from OpenStreetMap data using the following query:
 
 ```sql
```

