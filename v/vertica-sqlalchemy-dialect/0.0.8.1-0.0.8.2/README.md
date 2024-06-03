# Comparing `tmp/vertica-sqlalchemy-dialect-0.0.8.1.tar.gz` & `tmp/vertica_sqlalchemy_dialect-0.0.8.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.8.1.tar", last modified: Fri Oct 13 09:17:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

