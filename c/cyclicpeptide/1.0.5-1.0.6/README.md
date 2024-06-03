# Comparing `tmp/cyclicpeptide-1.0.5.tar.gz` & `tmp/cyclicpeptide-1.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclicpeptide-1.0.5.tar", last modified: Fri May 31 07:10:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

