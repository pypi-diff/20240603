# Comparing `tmp/django-locality-two-2.2.tar.gz` & `tmp/django_locality_two-3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-locality-two-2.2.tar", last modified: Thu Oct  5 15:22:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

