# Comparing `tmp/scdb_ml_app-1.0.0.tar.gz` & `tmp/SCDB_ML_app-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdb_ml_app-1.0.0.tar", last modified: Sun Jun  2 07:36:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

