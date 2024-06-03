# Comparing `tmp/moroccan_prayer_times-0.0.15.tar.gz` & `tmp/moroccan_prayer_times-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moroccan_prayer_times-0.0.15.tar", last modified: Sun Jun  2 17:17:33 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

