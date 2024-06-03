# Comparing `tmp/mzhfunc-0.1.2.tar.gz` & `tmp/MzhFunc-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzhfunc-0.1.2.tar", last modified: Mon Jun  3 01:32:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

