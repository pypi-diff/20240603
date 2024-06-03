# Comparing `tmp/django_ticketbai-1.8.tar.gz` & `tmp/django_ticketbai-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ticketbai-1.8.tar", last modified: Tue May 28 15:48:09 2024, max compression
+gzip compressed data, was "django_ticketbai-1.9.tar", last modified: Mon Jun  3 10:53:20 2024, max compression
```

## Comparing `django_ticketbai-1.8.tar` & `django_ticketbai-1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.768163 django_ticketbai-1.8/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:04.000000 django_ticketbai-1.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 15:48:04.000000 django_ticketbai-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-28 15:48:04.000000 django_ticketbai-1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 15:48:09.768163 django_ticketbai-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 15:48:04.000000 django_ticketbai-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.764163 django_ticketbai-1.8/django_ticketbai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.760163 django_ticketbai-1.8/django_ticketbai/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.760163 django_ticketbai-1.8/django_ticketbai/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.764163 django_ticketbai-1.8/django_ticketbai/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.768163 django_ticketbai-1.8/django_ticketbai/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0006_config_is_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0007_invoice_errorxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/0015_invoice_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.760163 django_ticketbai-1.8/django_ticketbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.768163 django_ticketbai-1.8/django_ticketbai/templates/PDF/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/templates/PDF/ticketbai.css
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/templates/PDF/ticketbai.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.760163 django_ticketbai-1.8/django_ticketbai/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.768163 django_ticketbai-1.8/django_ticketbai/templates/admin/django_ticketbai/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/templates/admin/django_ticketbai/app_index.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.768163 django_ticketbai-1.8/django_ticketbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/utils/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-28 15:48:04.000000 django_ticketbai-1.8/django_ticketbai/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:48:09.768163 django_ticketbai-1.8/django_ticketbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 15:48:09.000000 django_ticketbai-1.8/django_ticketbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-28 15:48:09.000000 django_ticketbai-1.8/django_ticketbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:48:09.000000 django_ticketbai-1.8/django_ticketbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 15:48:09.000000 django_ticketbai-1.8/django_ticketbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 15:48:09.000000 django_ticketbai-1.8/django_ticketbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:48:09.768163 django_ticketbai-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-28 15:48:04.000000 django_ticketbai-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.134715 django_ticketbai-1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:16.000000 django_ticketbai-1.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-06-03 10:53:16.000000 django_ticketbai-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-03 10:53:16.000000 django_ticketbai-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-06-03 10:53:20.134715 django_ticketbai-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-03 10:53:16.000000 django_ticketbai-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.130715 django_ticketbai-1.9/django_ticketbai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.126715 django_ticketbai-1.9/django_ticketbai/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.126715 django_ticketbai-1.9/django_ticketbai/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.130715 django_ticketbai-1.9/django_ticketbai/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.134715 django_ticketbai-1.9/django_ticketbai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0006_config_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0007_invoice_errorxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/0015_invoice_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.126715 django_ticketbai-1.9/django_ticketbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.134715 django_ticketbai-1.9/django_ticketbai/templates/PDF/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/templates/PDF/ticketbai.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/templates/PDF/ticketbai.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.126715 django_ticketbai-1.9/django_ticketbai/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.134715 django_ticketbai-1.9/django_ticketbai/templates/admin/django_ticketbai/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/templates/admin/django_ticketbai/app_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.134715 django_ticketbai-1.9/django_ticketbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/utils/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-03 10:53:16.000000 django_ticketbai-1.9/django_ticketbai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:53:20.134715 django_ticketbai-1.9/django_ticketbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-06-03 10:53:20.000000 django_ticketbai-1.9/django_ticketbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-06-03 10:53:20.000000 django_ticketbai-1.9/django_ticketbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:53:20.000000 django_ticketbai-1.9/django_ticketbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 10:53:20.000000 django_ticketbai-1.9/django_ticketbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 10:53:20.000000 django_ticketbai-1.9/django_ticketbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 10:53:20.134715 django_ticketbai-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-06-03 10:53:16.000000 django_ticketbai-1.9/setup.py
```

### Comparing `django_ticketbai-1.8/LICENSE` & `django_ticketbai-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/PKG-INFO` & `django_ticketbai-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.8
+Version: 1.9
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_ticketbai-1.8/django_ticketbai/admin.py` & `django_ticketbai-1.9/django_ticketbai/admin.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/locale/eu/LC_MESSAGES/django.mo` & `django_ticketbai-1.9/django_ticketbai/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/locale/eu/LC_MESSAGES/django.po` & `django_ticketbai-1.9/django_ticketbai/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0001_initial.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0010_alter_invoice_signature_value.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0010_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py` & `django_ticketbai-1.9/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/models.py` & `django_ticketbai-1.9/django_ticketbai/models.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/templates/PDF/ticketbai.html` & `django_ticketbai-1.9/django_ticketbai/templates/PDF/ticketbai.html`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     </head>
     <body>
         <center>
             {% if logo %}<img src="data:image/jpeg;base64,{{ logo }}" width="200" />{% endif %}
             <p style="font-size: 8pt;">
                 {{ subject_name }}
                 <br>
+                {{subject_address}}
+                <br>
                 IFZ: {{ entity_id }}
             </p>
         </center>
         <hr>
         <span>{{ invoice.expedition_date|date:"Y/m/d" }} - {{ invoice.expedition_time }}</span>
         <span class="right">{% trans "Simp. Invoice:" %} {{ invoice.serial_code }}/{{ invoice.num }}</span>
         <hr>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {% load i18n %}
 {% if style %}
 {% endif %}
           {% if logo %}[data:image/jpeg;base64,{{ logo }}]{% endif %}
                               {{ subject_name }}
+                             {{subject_address}}
                              IFZ: {{ entity_id }}
 ===============================================================================
 {{ invoice.expedition_date|date:"Y/m/d" }} - {{ invoice.expedition_time }} {%
 trans "Simp. Invoice:" %} {{ invoice.serial_code }}/{{ invoice.num }}
 ===============================================================================
 {{%% ttrraannss      {{%% ttrraannss          {{%% ttrraannss ""UUnniitt""        {{%% ttrraannss        {{%% ttrraannss
 ""QQuuaann.."" %%}}    ""DDeessccrriippttiioonn"" %%}}               %%}}   ""DDiissccoouunntt"" %%}}      ""TToottaall"" %%}}
```

### Comparing `django_ticketbai-1.8/django_ticketbai/utils/invoice.py` & `django_ticketbai-1.9/django_ticketbai/utils/invoice.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/utils/pdf.py` & `django_ticketbai-1.9/django_ticketbai/utils/pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 
 def get_html_string(invoice, subject, logo=None, style=None):
     t = template.loader.get_template("PDF/ticketbai.html")
     context = {
         "qr_base64": create_qr_base64(invoice, subject).decode("utf-8"),
         "subject_name": subject["name"],
+        "subject_address": subject["address"],
         "entity_id": subject["entity_id"],
         "invoice": invoice,
     }
     if style:
         context.update({"style": style})
     if logo:
         logo_path = os.path.join(settings.STATIC_ROOT, logo)
```

### Comparing `django_ticketbai-1.8/django_ticketbai/validators.py` & `django_ticketbai-1.9/django_ticketbai/validators.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai/views.py` & `django_ticketbai-1.9/django_ticketbai/views.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/django_ticketbai.egg-info/PKG-INFO` & `django_ticketbai-1.9/django_ticketbai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.8
+Version: 1.9
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_ticketbai-1.8/django_ticketbai.egg-info/SOURCES.txt` & `django_ticketbai-1.9/django_ticketbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.8/setup.py` & `django_ticketbai-1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("LICENSE") as f:
     license = f.read()
 
 
 setup(
     name="django-ticketbai",
-    version="1.8",
+    version="1.9",
     description=(
         "django-ticketbai allows to create, manage, store and send TicketBai"
         " invoices to the Basque tax authorities."
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="",
```

