# Comparing `tmp/pydivar-1.0.2.tar.gz` & `tmp/pydivar-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivar-1.0.2.tar", last modified: Sun Nov 26 05:02:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

