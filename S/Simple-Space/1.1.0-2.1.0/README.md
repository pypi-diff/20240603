# Comparing `tmp/simple_space-1.1.0.tar.gz` & `tmp/Simple_Space-2.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-1.1.0.tar", last modified: Sun Jun  2 18:32:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

