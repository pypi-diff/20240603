# Comparing `tmp/document_merge_service-6.5.0.tar.gz` & `tmp/document_merge_service-6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.5.0.tar", max compression
+gzip compressed data, was "document_merge_service-6.5.1.tar", max compression
```

## Comparing `document_merge_service-6.5.0.tar` & `document_merge_service-6.5.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    14122 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/LICENSE
--rw-r--r--   0        0        0     2522 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3232 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0     5490 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/2023.test.test.docx-template.docx
--rw-r--r--   0        0        0      580 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     7335 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx
--rw-r--r--   0        0        0     6087 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0     4750 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/invalid-template.xlsx
--rw-r--r--   0        0        0  1127936 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0    10589 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/odt-template.odt
--rw-r--r--   0        0        0       22 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0    10586 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/factories.py
--rw-r--r--   0        0        0      815 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/file_converter.py
--rw-r--r--   0        0        0     3013 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1628 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     2252 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/commands/upload_local_templates.py
--rw-r--r--   0        0        0     1248 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      374 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1004 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      932 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1845 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4995 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0    30689 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/__snapshots__/test_template.ambr
--rw-r--r--   0        0        0     2357 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1446 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_convert.py
--rw-r--r--   0        0        0     1963 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25891 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0     1712 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_upload_local_templates.py
--rw-r--r--   0        0        0     6947 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      460 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3797 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2909 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/extensions/__init__.py
--rw-r--r--   0        0        0       52 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/extensions/permissions.py
--rw-r--r--   0        0        0       52 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/extensions/visibilities.py
--rw-r--r--   0        0        0      789 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/sentry.py
--rw-r--r--   0        0        0     9066 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      197 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     4007 2024-05-30 12:01:47.376634 document_merge_service-6.5.0/pyproject.toml
--rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 document_merge_service-6.5.0/PKG-INFO
+-rw-r--r--   0        0        0    14466 2024-06-03 11:55:36.020717 document_merge_service-6.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-06-03 11:55:36.020717 document_merge_service-6.5.1/LICENSE
+-rw-r--r--   0        0        0     2522 2024-06-03 11:55:36.020717 document_merge_service-6.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.020717 document_merge_service-6.5.1/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.020717 document_merge_service-6.5.1/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2024-06-03 11:55:36.020717 document_merge_service-6.5.1/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3232 2024-06-03 11:55:36.020717 document_merge_service-6.5.1/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0     5490 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/2023.test.test.docx-template.docx
+-rw-r--r--   0        0        0      580 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     7335 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx
+-rw-r--r--   0        0        0     6087 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0     4750 2024-06-03 11:55:36.024717 document_merge_service-6.5.1/document_merge_service/api/data/invalid-template.xlsx
+-rw-r--r--   0        0        0  1127936 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0    10589 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/odt-template.odt
+-rw-r--r--   0        0        0       22 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0    10586 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0      815 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/file_converter.py
+-rw-r--r--   0        0        0     3013 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     2252 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      932 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2024-06-03 11:55:36.028717 document_merge_service-6.5.1/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4995 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0    30689 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/__snapshots__/test_template.ambr
+-rw-r--r--   0        0        0     2357 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1446 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_convert.py
+-rw-r--r--   0        0        0     1963 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25891 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0     1712 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      460 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3797 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     9191 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      197 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     4107 2024-06-03 11:55:36.032717 document_merge_service-6.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 document_merge_service-6.5.1/PKG-INFO
```

### Comparing `document_merge_service-6.5.0/CHANGELOG.md` & `document_merge_service-6.5.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 6.5.1 (3 June 2024)
+### Fix
+
+* **deps:** Allow caching with memcache ([`2f7c2bc`](https://github.com/adfinis/document-merge-service/commit/2f7c2bc196f56dd5488101c8ad1e639671002005))
+* **deps:** Fix usage with postgres database ([`f29c763`](https://github.com/adfinis/document-merge-service/commit/f29c7635d3fa7759c9c9e98bc6e437da650ebb26))
+
 ## 6.5.0 (30 May 2024)
 ### Feature
 
 * **docker:** Update python to v3.12 ([`14c4d7f`](https://github.com/adfinis/document-merge-service/commit/14c4d7f97005ce9651be6dc37eae904125614e29))
 * **deps:** Update dependencies ([`5773d5c`](https://github.com/adfinis/document-merge-service/commit/5773d5c5283543c843c4986daf8b71cc1cafa611))
 * **deps:** Update django to v4.2 LTS ([`5287a3e`](https://github.com/adfinis/document-merge-service/commit/5287a3e4a6b26c12e122026f789e80d2c70f892b))
```

### Comparing `document_merge_service-6.5.0/LICENSE` & `document_merge_service-6.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/README.md` & `document_merge_service-6.5.1/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/authentication.py` & `document_merge_service-6.5.1/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/2023.test.test.docx-template.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/2023.test.test.docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/__init__.py` & `document_merge_service-6.5.1/document_merge_service/api/data/__init__.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/black.png` & `document_merge_service-6.5.1/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/invalid-template.xlsx` & `document_merge_service-6.5.1/document_merge_service/api/data/invalid-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.5.1/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.5.1/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/odt-template.odt` & `document_merge_service-6.5.1/document_merge_service/api/data/odt-template.odt`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.5.1/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.5.1/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.5.1/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/engines.py` & `document_merge_service-6.5.1/document_merge_service/api/engines.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/file_converter.py` & `document_merge_service-6.5.1/document_merge_service/api/file_converter.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/filters.py` & `document_merge_service-6.5.1/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/jinja.py` & `document_merge_service-6.5.1/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.5.1/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/management/commands/upload_local_templates.py` & `document_merge_service-6.5.1/document_merge_service/api/management/commands/upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.5.1/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.5.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/migrations/0006_remove_template_group.py` & `document_merge_service-6.5.1/document_merge_service/api/migrations/0006_remove_template_group.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/models.py` & `document_merge_service-6.5.1/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/serializers.py` & `document_merge_service-6.5.1/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/__snapshots__/test_template.ambr` & `document_merge_service-6.5.1/document_merge_service/api/tests/__snapshots__/test_template.ambr`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_convert.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/tests/test_upload_local_templates.py` & `document_merge_service-6.5.1/document_merge_service/api/tests/test_upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/unoconv.py` & `document_merge_service-6.5.1/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/api/views.py` & `document_merge_service-6.5.1/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/conftest.py` & `document_merge_service-6.5.1/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/sentry.py` & `document_merge_service-6.5.1/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/document_merge_service/settings.py` & `document_merge_service-6.5.1/document_merge_service/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,17 @@
     "rest_framework",
     "django_filters",
     "document_merge_service.api.apps.DefaultConfig",
     "corsheaders",
     "generic_permissions.apps.GenericPermissionsConfig",
 ]
 
+if "postgresql" in DATABASES["default"]["ENGINE"]:  # pragma: no cover
+    INSTALLED_APPS.append("django.contrib.postgres")
+
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "corsheaders.middleware.CorsMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.locale.LocaleMiddleware",
 ]
```

### Comparing `document_merge_service-6.5.0/document_merge_service/tests/test_settings.py` & `document_merge_service-6.5.1/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.5.0/pyproject.toml` & `document_merge_service-6.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.5.0"
+version = "6.5.1"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
@@ -36,15 +36,16 @@
 django-generic-api-permissions = "^0.4.6"
 django-storages = "^1.14.3"
 djangorestframework = "^3.15.1"
 docx-mailmerge = "^0.5.0"
 docxtpl = "^0.17.0"
 Jinja2 = "^3.1.4"
 mysqlclient = { version = "^2.2.4", optional = true }
-psycopg = { version = "^3.1.19", optional = true }
+psycopg = { version = "^3.1.19", optional = true, extras = ["binary"] }
+pymemcache = { version = "^4.0.0", optional = true }
 python-dateutil = "^2.9.0"
 python-memcached = "^1.59"
 requests = "^2.32.3"
 sentry-sdk = "^2.3.1"
 urllib3 = "^2.2.1"
 uWSGI = "^2.0.21"
 xltpl = "~0.19"
@@ -80,14 +81,15 @@
 types-setuptools = "70.0.0.20240524"
 types-toml = "0.10.8.20240310"
 
 [tool.poetry.extras]
 mysql = ["mysqlclient"]
 pgsql = ["psycopg"]
 databases = ["mysqlclient", "psycopg"]
+memcache = ["pymemcache"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 skip = "migrations"
```

### Comparing `document_merge_service-6.5.0/PKG-INFO` & `document_merge_service-6.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.5.0
+Version: 6.5.1
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,29 +15,31 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: databases
+Provides-Extra: memcache
 Provides-Extra: mysql
 Provides-Extra: pgsql
 Requires-Dist: Babel (>=2.15.0,<3.0.0)
 Requires-Dist: Django (>=4.2.13,<4.3.0)
 Requires-Dist: Jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: django-cors-headers (>=4.3.1,<5.0.0)
 Requires-Dist: django-environ (>=0.11.2,<0.12.0)
 Requires-Dist: django-filter (>=24.2,<25.0)
 Requires-Dist: django-generic-api-permissions (>=0.4.6,<0.5.0)
 Requires-Dist: django-storages (>=1.14.3,<2.0.0)
 Requires-Dist: djangorestframework (>=3.15.1,<4.0.0)
 Requires-Dist: docx-mailmerge (>=0.5.0,<0.6.0)
 Requires-Dist: docxtpl (>=0.17.0,<0.18.0)
 Requires-Dist: mysqlclient (>=2.2.4,<3.0.0) ; extra == "mysql" or extra == "databases"
-Requires-Dist: psycopg (>=3.1.19,<4.0.0) ; extra == "pgsql" or extra == "databases"
+Requires-Dist: psycopg[binary] (>=3.1.19,<4.0.0) ; extra == "pgsql" or extra == "databases"
+Requires-Dist: pymemcache (>=4.0.0,<5.0.0) ; extra == "memcache"
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: python-memcached (>=1.59,<2.0)
 Requires-Dist: requests (>=2.32.3,<3.0.0)
 Requires-Dist: sentry-sdk (>=2.3.1,<3.0.0)
 Requires-Dist: uWSGI (>=2.0.21,<3.0.0)
 Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
 Requires-Dist: xltpl (>=0.19,<0.20)
```

