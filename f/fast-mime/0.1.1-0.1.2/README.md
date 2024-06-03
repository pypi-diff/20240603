# Comparing `tmp/fast_mime-0.1.1.tar.gz` & `tmp/fast_mime-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_mime-0.1.1.tar", max compression
+gzip compressed data, was "fast_mime-0.1.2.tar", max compression
```

## Comparing `fast_mime-0.1.1.tar` & `fast_mime-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1058 2024-05-18 10:51:46.909341 fast_mime-0.1.1/LICENSE
--rw-r--r--   0        0        0      660 2024-05-18 10:49:58.830749 fast_mime-0.1.1/README.md
--rw-r--r--   0        0        0    19586 2024-06-02 08:46:28.396571 fast_mime-0.1.1/fast_mime/__init__.py
--rw-r--r--   0        0        0     4337 2024-05-17 09:09:07.773517 fast_mime-0.1.1/fast_mime/data/custom.xml
--rw-r--r--   0        0        0     8920 2024-05-17 08:39:44.876303 fast_mime-0.1.1/fast_mime/data/patch.json
--rw-r--r--   0        0        0   279488 2024-05-17 09:14:27.010711 fast_mime-0.1.1/fast_mime/data/tika.xml
--rw-r--r--   0        0        0      425 2024-06-02 08:46:08.085994 fast_mime-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 fast_mime-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-18 10:51:46.909341 fast_mime-0.1.2/LICENSE
+-rw-r--r--   0        0        0      660 2024-05-18 10:49:58.830749 fast_mime-0.1.2/README.md
+-rw-r--r--   0        0        0    19715 2024-06-03 13:38:25.805507 fast_mime-0.1.2/fast_mime/__init__.py
+-rw-r--r--   0        0        0     4337 2024-05-17 09:09:07.773517 fast_mime-0.1.2/fast_mime/data/custom.xml
+-rw-r--r--   0        0        0     8920 2024-05-17 08:39:44.876303 fast_mime-0.1.2/fast_mime/data/patch.json
+-rw-r--r--   0        0        0   279488 2024-05-17 09:14:27.010711 fast_mime-0.1.2/fast_mime/data/tika.xml
+-rw-r--r--   0        0        0      425 2024-06-03 13:38:25.806477 fast_mime-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 fast_mime-0.1.2/PKG-INFO
```

### Comparing `fast_mime-0.1.1/LICENSE` & `fast_mime-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.1/README.md` & `fast_mime-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.1/fast_mime/__init__.py` & `fast_mime-0.1.2/fast_mime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,11 +598,15 @@
     def _with_io(
         self, pathname_or_io: Path | str | IO[bytes]
     ) -> Generator[IO[bytes], Any, None]:
         if isinstance(pathname_or_io, Path) or isinstance(pathname_or_io, str):
             with open(pathname_or_io, "rb") as fi:
                 yield fi
         else:
-            yield pathname_or_io
+            offset = pathname_or_io.tell()
+            try:
+                yield pathname_or_io
+            finally:
+                pathname_or_io.seek(offset)
 
 
 MIME = Mime.from_xmls()
```

### Comparing `fast_mime-0.1.1/fast_mime/data/custom.xml` & `fast_mime-0.1.2/fast_mime/data/custom.xml`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.1/fast_mime/data/patch.json` & `fast_mime-0.1.2/fast_mime/data/patch.json`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.1/fast_mime/data/tika.xml` & `fast_mime-0.1.2/fast_mime/data/tika.xml`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.1/PKG-INFO` & `fast_mime-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-mime
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Chongchen Chen
 Author-email: chenkovsky@qq.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

