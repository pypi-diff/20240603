# Comparing `tmp/gardener_cicd_cli-1.2410.0.tar.gz` & `tmp/gardener_cicd_cli-1.2411.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_cli-1.2410.0.tar", last modified: Fri May 31 11:11:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

