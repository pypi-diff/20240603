# Comparing `tmp/pycnite-2023.9.8.tar.gz` & `tmp/pycnite-2024.5.27-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycnite-2023.9.8.tar", last modified: Mon Sep 11 23:53:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

