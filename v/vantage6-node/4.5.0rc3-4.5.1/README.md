# Comparing `tmp/vantage6-node-4.5.0rc3.tar.gz` & `tmp/vantage6_node-4.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-4.5.0rc3.tar", last modified: Wed May 22 15:04:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

