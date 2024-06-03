# Comparing `tmp/airbyte-source-smartsheets-1.1.2.tar.gz` & `tmp/airbyte_source_smartsheets-1.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-smartsheets-1.1.2.tar", last modified: Thu Feb  1 13:49:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

