# Comparing `tmp/odoo14-addon-energy_communities_cooperator-14.0.1.0.1.tar.gz` & `tmp/odoo14-addon-energy_communities_cooperator-14.0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_communities_cooperator-14.0.1.0.1.tar", last modified: Tue May 21 13:47:33 2024, max compression
+gzip compressed data, was "odoo14-addon-energy_communities_cooperator-14.0.1.0.2.tar", last modified: Mon Jun  3 13:51:14 2024, max compression
```

## Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1.tar` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.053110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      507 2024-05-21 13:47:33.053110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/PKG-INFO
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.029109 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.029109 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.033109 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3378 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1278 2024-05-21 13:25:20.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/__manifest__.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.037109 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/controllers/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       26 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/controllers/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1007 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/controllers/controllers.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.037109 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/data/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      363 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/data/ir_config_parameter_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    10634 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/data/mail_template_update_data.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.041110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/i18n/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    17209 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/i18n/ca_ES.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    18623 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/i18n/es.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    16311 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/i18n/eu_ES.po
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.045110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      146 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      698 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/account_move.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1466 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/cooperative_membership.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1033 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/partner.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      179 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/share_line.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     7393 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/subscription_request.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.045110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/security/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      294 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/security/ir.model.access.csv
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.049110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      450 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/account_move_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4881 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/cooperative_membership_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      585 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/operation_request_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      551 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/res_company_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2116 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/res_partner_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1991 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/subscription_request_view.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:47:33.053110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      507 2024-05-21 13:47:32.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/PKG-INFO
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1881 2024-05-21 13:47:32.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/SOURCES.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-05-21 13:47:32.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/dependency_links.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-05-07 09:00:07.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/not-zip-safe
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      121 2024-05-21 13:47:32.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/requires.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        5 2024-05-21 13:47:32.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/top_level.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       38 2024-05-21 13:47:33.053110 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/setup.cfg
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      224 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.1/setup.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.326504 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      507 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/PKG-INFO
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3378 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1278 2024-06-03 13:40:46.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/__manifest__.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/controllers/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       26 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/controllers/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1007 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/controllers/controllers.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/data/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      363 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/data/ir_config_parameter_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    10634 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/data/mail_template_update_data.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/i18n/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    19400 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/i18n/ca_ES.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    20853 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/i18n/es.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    18488 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/i18n/eu_ES.po
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      146 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      698 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/account_move.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1466 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/cooperative_membership.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1033 2024-05-17 10:23:03.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/partner.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      179 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/share_line.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     7393 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/subscription_request.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/security/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      294 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/security/ir.model.access.csv
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      450 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/account_move_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4881 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/cooperative_membership_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      585 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/operation_request_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      866 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/res_company_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2116 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/res_partner_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1991 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/subscription_request_view.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:51:14.323171 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      507 2024-06-03 13:51:14.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/PKG-INFO
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1881 2024-06-03 13:51:14.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/SOURCES.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:51:14.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/dependency_links.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:51:14.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/not-zip-safe
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      121 2024-06-03 13:51:14.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/requires.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-06-03 13:51:14.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/top_level.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-06-03 13:51:14.326504 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/setup.cfg
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      224 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_cooperator-14.0.1.0.2/setup.py
```

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/__init__.py` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/__manifest__.py` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/__manifest__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """,
     "author": "Som Comunitats SCCL",
     "website": "https://coopdevs.org",
     # Categories can be used to filter modules in modules listing
     # Check https://github.com/odoo/odoo/blob/14.0/odoo/addons/base/data/ir_module_category_data.xml
     # for the full list
     "category": "Cooperative management",
-    "version": "14.0.1.0.1",
+    "version": "14.0.1.0.2",
     "license": "AGPL-3",
     # any module necessary for this one to work correctly
     "depends": ["base", "cooperator", "l10n_es_cooperator", "energy_communities"],
     # always loaded
     "data": [
         # 'security/ir.model.access.csv',
         "views/account_move_views.xml",
```

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/controllers/controllers.py` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/controllers/controllers.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/data/mail_template_update_data.xml` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/data/mail_template_update_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/i18n/ca_ES.po` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/i18n/eu_ES.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,365 +2,436 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities_cooperator
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-18 10:44+0000\n"
-"PO-Revision-Date: 2024-04-18 10:44+0000\n"
+"POT-Creation-Date: 2024-05-31 14:23+0000\n"
+"PO-Revision-Date: 2024-05-31 16:29+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
+"Language: eu_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: \n"
-"Plural-Forms: \n"
+"Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 3.4.2\n"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,help:energy_communities_cooperator.field_subscription_request__vat
 msgid ""
 "\n"
-"        The Tax Identification Number. Complete it if the contact is subjected to\n"
+"        The Tax Identification Number. Complete it if the contact is "
+"subjected to\n"
 "        government taxes. Used in some legal statements.\"\n"
 "        "
 msgstr ""
 "\n"
-"        El NIF/CIF. Completa aquest camp si el contacte està subjecte a\n"
-"        les taxes estatals. Es fa servir en alguns  informes legals.\"\n"
+"        El NIF/CIF. Completa este campo si el contacto está subjecto a\n"
+"        las tasas estatales. Se usa en algunos informes legales.\"\n"
 "        "
 
 #. module: energy_communities_cooperator
 #: model:mail.template,body_html:energy_communities_cooperator.email_template_confirmation_voluntary_share
 msgid ""
 "\n"
 "    <p>Dear ${object.firstname},</p>\n"
 "    <p>\n"
-"        We confirm that we have correctly received your request to make a voluntary contribution to the capital\n"
-"        social of <b>${object.company_id.name}</b>, with the following data:\n"
+"        We confirm that we have correctly received your request to make a "
+"voluntary contribution to the capital\n"
+"        social of <b>${object.company_id.name}</b>, with the following "
+"data:\n"
 "    </p>\n"
 "    <ul>\n"
 "        <li>Partner VAT: <b>${object.vat}</b></li>\n"
-"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
+"li>\n"
 "        <li>Charging account: <b>${object.iban}</b></li>\n"
-"        <li>Subscription amount: <b>${object.subscription_amount}€</b></li>\n"
+"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
+"li>\n"
 "    </ul>\n"
 "    <p>\n"
-"        In the next few days you will receive the bank charge in this account, please verify that all the data\n"
-"        provided is correct and you have the money you want to invest, to avoid any incident in the\n"
+"        In the next few days you will receive the bank charge in this "
+"account, please verify that all the data\n"
+"        provided is correct and you have the money you want to invest, to "
+"avoid any incident in the\n"
 "        draft of the receipt.\n"
 "    </p>\n"
 "    <p>\n"
-"        Once the validity of the payment has been verified, you will receive a new notification confirming the\n"
+"        Once the validity of the payment has been verified, you will "
+"receive a new notification confirming the\n"
 "        contribution\n"
 "        made and detailing the particular conditions of your contribution.\n"
 "    </p>\n"
 "    <p>\n"
-"        Thank you for your involvement with the cooperative and inform you that for any doubt or clarification you can\n"
+"        Thank you for your involvement with the cooperative and inform you "
+"that for any doubt or clarification you can\n"
 "        consult\n"
 "        our website:\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
 "        or send us an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a>\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
 "    </p>\n"
 "    <p>\n"
-"        Get the word out by explaining the project to family and friends. The more we are, the further we will go!\n"
+"        Get the word out by explaining the project to family and friends. "
+"The more we are, the further we will go!\n"
 "    </p>\n"
 "    <p>\n"
 "        Thank you very much and good energy!\n"
 "    </p>\n"
 "    <p>\n"
 "        Sincerely,\n"
 "    </p>\n"
 "    <p>\n"
 "        ${object.company_id.name} team\n"
 "    </p>\n"
-"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" style=\"width: 150px;height: 80px;\"/>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
 "            "
 msgstr ""
-"    <p>Apreciat/ada ${object.firstname},</p>\n"
+"\n"
+"    <p>${object.firstname} agurgarria,</p>\n"
 "    <p>\n"
-"        Et confirmem que hem rebut correctament la teva sol·licitud per realitzar una aportació voluntària al capital social de <b>${object.company_id.name}</b>, amb les següents dades:\n"
+"Baieztatzen dizugu zuzen jaso dugula zure eskaera, <b>${object.company_id."
+"name}</b> kapital sozialera borondatezko ekarpena egiteko, datu hauekin:\n"
+"\n"
 "    </p>\n"
 "    <ul>\n"
-"        <li>Soci/sòcia NIF: <b>${object.vat}</b></li>\n"
-"        <li>Soci/sòcia: <b>${object.firstname} ${object.lastname}</b></li>\n"
-"        <li>Compte bancari: <b>${object.iban}</b></li>\n"
-"        <li>Import d'aportació: <b>${object.subscription_amount}€</b></li>\n"
+"        <li>Bazkidea DNI: <b>${object.vat}</b></li>\n"
+"        <li>Bazkidea: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Kargu-kontua: <b>${object.iban}</b></li>\n"
+"        <li>Ekarpenaren zenbatekoa: <b>${object.subscription_amount}€</b></"
+"li>\n"
 "    </ul>\n"
 "    <p>\n"
-"En els pròxims dies rebràs el càrrec bancari en aquest compte, si us plau verifica que totes les teves dades siguin correctes i disposis dels diners que vulguis invertir, per evitar qualsevol incidència en el gir del rebut.\n"
+"Datozen egunetan kontu honetan jasoko duzu bankuko kargua. Mesedez, "
+"egiaztatu emandako datu guztiak zuzenak direla eta eman nahi duzun dirua "
+"duzula, ordainagiriaren igorpenean gorabeherarik izan ez dadin.\n"
 "    </p>\n"
 "    <p>\n"
-"Una vegada verificat el pagament, rebràs una notificació confirmant l'aportació realitzada i detallant les condicions particulars de la teva aportació.\n"
+"Egindako ordainketaren balioa egiaztatu ondoren, beste jakinarazpen bat "
+"jasoko duzu, egindako ekarpena baieztatuz eta zure ekarpenaren baldintza "
+"partikularrak zehaztuz.\n"
 "    </p>\n"
 "    <p>\n"
-"Agraïm la teva implicació amb la cooperativa i t'informem que pots aclarir qualsevol dubte en la nostra pàgina web \n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>\n"
-"o enviar-nos un correu electrònic a\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a>\n"
+"Kooperatibarekin duzun inplikazioa eskertu nahi dizugu, eta, edozein "
+"zalantza argitzeko, gure web orria kontsulta dezakezu \n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"edo mezu elektroniko bat bidali \n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
+" helbidera.\n"
 "    </p>\n"
 "    <p>\n"
-"Fes que corri la veu explicant el nostre projecte a familiars i amics/amigues. Com més siguem, més lluny arribarem!\n"
+"Ahoz ahoz proiektua familiakoei, auzokideei eta lagunei azaldu. Zenbat eta "
+"gehiago izan, urrunago iritsiko gara!\n"
 "    </p>\n"
 "    <p>\n"
-"Moltes gràcies i bona energia!\n"
+"Eskerrik asko eta energia on!\n"
 "    </p>\n"
 "    <p>\n"
-"        Atentament,\n"
+"        Adeitasunez,\n"
 "    </p>\n"
-"</br>\n"
 "    <p>\n"
-"        L'equip de ${object.company_id.name}\n"
+"        ${object.company_id.name} taldea\n"
 "    </p>\n"
-"    % if object.company_id.street:\n"
-"        ${object.company_id.street}\n"
-"    % endif\n"
-"    % if object.company_id.street2:\n"
-"        ${object.company_id.street2}<br/>\n"
-"    % endif\n"
-"    % if object.company_id.city or object.company_id.zip:\n"
-"        ${object.company_id.zip} ${object.company_id.city}<br/>\n"
-"    % endif\n"
-"    % if object.company_id.country_id:\n"
-"        ${object.company_id.state_id and ('%s, ' % object.company_id.state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
-"    % endif\n"
-"    % if object.company_id.phone:\n"
-"        Teléfono:&nbsp; ${object.company_id.phone}\n"
-"    % endif\n"
-"\n"
-"    % if object.company_id.website:\n"
-"        <div>\n"
-"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object.company_id.website}</a>\n"
-"        </div>\n"
-"    %endif\n"
-"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" style=\"width: 150px;\"/>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;\"/>\n"
 "            "
 
 #. module: energy_communities_cooperator
 #: model:mail.template,body_html:energy_communities_cooperator.email_template_confirmation_company
 msgid ""
 "\n"
-"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
+"serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
+"\">\n"
 "\n"
 "    <p>Hello,</p>\n"
-"    <p>Thank you for filling out the form and request to join the Community.</p>\n"
-"    <p>In the coming weeks we will contact you to indicate the next steps</p>\n"
+"    <p>Thank you for filling out the form and request to join the Community."
+"</p>\n"
+"    <p>In the coming weeks we will contact you to indicate the next steps</"
+"p>\n"
 "    <p>Here is a copy of the data we received:</p>\n"
-"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', "
+"Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, "
+"34); background-color: #FFF; \">\n"
 "        <p> - Request to join: ${object.company_id.name}</p>\n"
 "        <p> - Company Name: ${object.company_name}</p>\n"
 "        <p> - Company Email: ${object.company_email}</p>\n"
 "        <p> - VAT: ${object.vat}</p>\n"
 "        <p> - Address: ${object.address}</p>\n"
 "        <p> - Zip code: ${object.zip_code}</p>\n"
 "        <p> - City: ${object.city}</p>\n"
 "        <p> - Country: ${object.country_id.name}</p>\n"
 "        <p> - Firstname: ${object.firstname}</p>\n"
 "        <p> - Lastname: ${object.lastname}</p>\n"
 "        <p> - Function: ${object.contact_person_function}</p>\n"
 "        <p> - Email: ${object.email}</p>\n"
 "        <p> - Phone: ${(object.phone or '')}</p>\n"
-"        <p> - Gender: ${dict(object.fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</p>\n"
+"        <p> - Gender: ${dict(object.fields_get(allfields=['gender'])"
+"['gender']['selection'])[object.gender]}</p>\n"
 "        <p> - Birthdate: ${object.birthdate}</p>\n"
-"        <p> - Language: ${dict(object.fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
+"        <p> - Language: ${dict(object.fields_get(allfields=['lang'])['lang']"
+"['selection'])[object.lang]}</p>\n"
 "        <p> - Initial share amount: ${object.subscription_amount}</p>\n"
-"    % if object.payment_mode_id.payment_method_id.code == 'sepa_direct_debit':\n"
+"    % if object.payment_mode_id.payment_method_id.code == "
+"'sepa_direct_debit':\n"
 "        <p> - Bank account: ${object.iban}</p>\n"
-"        <p> - I authorize bank receipts to be sent to this account: ${object.mandate_approved and 'SI' or 'NO'}</p>\n"
+"        <p> - I authorize bank receipts to be sent to this account: "
+"${object.mandate_approved and 'SI' or 'NO'}</p>\n"
 "    % endif\n"
 "    </div>\n"
 "    <br />\n"
 "    <p>We keep in touch for any questions.</p>\n"
 "    <p>Yours faithfully,</p>\n"
 "    <p>Somcomunitats.coop team </p>\n"
-"    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</"
+"a></p>\n"
 "</div>\n"
 "            "
 msgstr ""
-"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
+"serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
+"\">\n"
 "\n"
 "    <p>Hola,</p>\n"
-"    <p>Gràcies per omplir el formulari i sol·licitar l’adhesió a la Comunitat Energètica.</p>\n"
-"    <p>En les properes setmanes ens posarem en contacte amb tu per indicar-te les següents passes.</p>\n"
-"    <p>Aquí tens una còpia de les dades que hem rebut:</p>\n"
-"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
-"        <p> - Comunitat: ${object.company_id.name}</p>\n"
-"        <p> - Nom empresa: ${object.company_name}</p>\n"
-"        <p> - Correu empresa: ${object.company_email}</p>\n"
+"    <p>Gracias por rellenar el formulario y solicitar la adhesión a la "
+"Comunidad Energética.</p>\n"
+"    <p>En las próximas semanas nos pondremos en contacto contigo para "
+"indicarte los siguientes pasos.</p>\n"
+"    <p>Aquí tienes una copia de los datos que hemos recibido:</p>\n"
+"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', "
+"Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, "
+"34); background-color: #FFF; \">\n"
+"        <p> - Comunidad: ${object.company_id.name}</p>\n"
+"        <p> - Nombre empresa: ${object.company_name}</p>\n"
+"        <p> - Correo empresa: ${object.company_email}</p>\n"
 "        <p> - NIF/CIF empresa: ${object.vat}</p>\n"
-"        <p> - Direcció empresa: ${object.address}</p>\n"
-"        <p> - Codi postal empresa: ${object.zip_code}</p>\n"
-"        <p> - Ciutat empresa: ${object.city}</p>\n"
-"        <p> - Pais empresa: ${object.country_id.name}</p>\n"
-"        <p> - Nom persona representant: ${object.firstname}</p>\n"
-"        <p> - Cognoms persona representant: ${object.lastname}</p>\n"
-"        <p> - Càrrec representant: ${object.contact_person_function}</p>\n"
-"        <p> - Correu representant: ${object.email}</p>\n"
-"        <p> - Telèfon representant: ${(object.phone or '')}</p>\n"
-"        <p> - Gènere representant: ${dict(object.fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</p>\n"
-"        <p> - data naixement representant: ${object.birthdate}</p>\n"
-"        <p> - Idioma comunicacions: ${dict(object.fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
-"        <p> - Import aportació inicial: ${object.subscription_amount}</p>\n"
-"    % if object.payment_mode_id.payment_method_id.code == 'sepa_direct_debit': \n"
-"        <p> - Compte bancari: ${object.iban}</p>\n"
-"        <p> - Autoritzo giros bancaris a aquest compte: ${object.mandate_approved and 'SI' or 'NO'}</p> \n"
+"        <p> - Dirección empresa: ${object.address}</p>\n"
+"        <p> - Código postal empresa: ${object.zip_code}</p>\n"
+"        <p> - Ciudad empresa: ${object.city}</p>\n"
+"        <p> - País empresa: ${object.country_id.name}</p>\n"
+"        <p> - Nombre persona representante: ${object.firstname}</p>\n"
+"        <p> - Apellidos persona representante: ${object.lastname}</p>\n"
+"        <p> - Cargo representante: ${object.contact_person_function}</p>\n"
+"        <p> - Correo representante: ${object.email}</p>\n"
+"        <p> - Teléfono representante: ${(object.phone or '')}</p>\n"
+"        <p> - Género representante: ${dict(object."
+"fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</"
+"p>\n"
+"        <p> - Fecha nacimiento representante: ${object.birthdate}</p>\n"
+"        <p> - Idioma comunicaciones: ${dict(object."
+"fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
+"        <p> - Importe aportación inicial: ${object.subscription_amount}</"
+"p>\n"
+"    % if object.payment_mode_id.payment_method_id.code == "
+"'sepa_direct_debit': \n"
+"        <p> - Cuenta bancaria: ${object.iban}</p>\n"
+"        <p> - Autorizo giros bancarios a esta cuenta: ${object."
+"mandate_approved and 'SI' or 'NO'}</p> \n"
 "    % endif\n"
 "    </div>\n"
 "    <br />\n"
-"<p>Seguim en contacte per qualsevol dubte.</p>\n"
-"    <p><a href=\"https://web-prod.somcomunitats.coop/recursos/\">Recursos i FAQs</a></p>\n"
-"    <p>Atentament,</p>\n"
+"    <p>Seguimos en contacto para cualquier duda.</p>\n"
+"    <p><a href=\"https://web-prod.somcomunitats.coop/recursos/\">Recursos y "
+"FAQs</a></p>\n"
+"    <p>Atentamente,</p>\n"
 "    </br>\n"
 "    <p>${object.company_id.name}.</p>\n"
 "\n"
 "    % if object.company_id.street:\n"
 "        ${object.company_id.street}\n"
 "    % endif\n"
 "    % if object.company_id.street2:\n"
 "        ${object.company_id.street2}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.city or object.company_id.zip:\n"
 "        ${object.company_id.zip} ${object.company_id.city}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.country_id:\n"
-"        ${object.company_id.state_id and ('%s, ' % object.company_id.state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
+"        ${object.company_id.state_id and ('%s, ' % object.company_id."
+"state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.phone:\n"
 "        Teléfono:&nbsp; ${object.company_id.phone}\n"
 "    % endif\n"
 "\n"
 "    % if object.company_id.website:\n"
 "        <div>\n"
-"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object.company_id.website}</a>\n"
+"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object."
+"company_id.website}</a>\n"
 "        </div>\n"
 "    %endif\n"
 "<div>\n"
 "<img src=\"/logo.png?company=${object.company_id.id}\" width=\"150\">\n"
 "<img src=${object.env.company.logo_url}>\n"
 "</div>\n"
 "</div>\n"
-"            \n"
 "            "
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__active
 msgid "Active"
-msgstr "Actiu"
+msgstr "Activo"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__representative_of_member_company
 msgid "Company Legal Representative"
-msgstr "Representant legal de companyia"
+msgstr "Representante legal de compañía"
+
+#. module: energy_communities_cooperator
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__company_register_number
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_users__company_register_number
+msgid "Company Register Number"
+msgstr "Código de registro de la compañía"
+
+#. module: energy_communities_cooperator
+#: model:ir.model,name:energy_communities_cooperator.model_res_partner
+msgid "Contact"
+msgstr "Kontaktua"
 
 #. module: energy_communities_cooperator
 #: model:mail.template,subject:energy_communities_cooperator.email_template_confirmation_voluntary_share
 msgid "Contribute to ${object.company_id.name} Ref. ACSV${object.id}"
 msgstr ""
-"Aportació voluntària a ${object.company_id.name} Ref. ACSV${object.id}: "
-"sol·licitud rebuda"
+"${object.company_id.name} autofinantzaketan ematea Erref. ACSV${object.id}: "
+"jasotako eskaera"
 
 #. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_cooperative_membership
 msgid "Cooperative Membership"
 msgstr "Membresia"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__display_name
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__display_name
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__display_name
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__display_name
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__display_name
 msgid "Display Name"
-msgstr "Nom de visualització"
+msgstr "Nombre Mostrado"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__gender
 msgid "Gender"
-msgstr "Gènere"
+msgstr "Género"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields.selection,name:energy_communities_cooperator.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
-msgstr "Prefereixo no compartir-ho"
+msgstr "Prefiero no compartirlo"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__id
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__id
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__id
 msgid "ID"
-msgstr ""
-
-#. module: energy_communities_cooperator
-#: model:ir.actions.act_window,name:energy_communities_cooperator.action_account_move
-#: model:ir.ui.menu,name:energy_communities_cooperator.menu_account_move
-msgid "Invoices"
-msgstr "Factures"
+msgstr "Identificador"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__is_voluntary
 msgid "Is voluntary contribution"
-msgstr "És una aportació voluntària"
+msgstr "Es aportación voluntaria"
 
 #. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_account_move
 msgid "Journal Entry"
-msgstr "Assentament comptable"
+msgstr "Egunkari-sarrera"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move____last_update
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership____last_update
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner____last_update
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line____last_update
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request____last_update
 msgid "Last Modified on"
-msgstr "Última modificació el"
+msgstr "Última modificación el"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__representative
 msgid "Legal Representative"
-msgstr "Representant legal"
+msgstr "Representante legal"
+
+#. module: energy_communities_cooperator
+#: model_terms:ir.ui.view,arch_db:energy_communities_cooperator.view_subscription_request_filter_inherit
+msgid "Mandatory Shares"
+msgstr "Aportaciones obligatorias"
 
 #. module: energy_communities_cooperator
 #: model:ir.actions.act_window,name:energy_communities_cooperator.action_cooperative_membership
 #: model:ir.ui.menu,name:energy_communities_cooperator.menu_cooperative_membership
 msgid "Memberships"
-msgstr "Membresies"
+msgstr "Membresias"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields.selection,name:energy_communities_cooperator.selection__subscription_request__gender__not_binary
 msgid "Not binary"
-msgstr "No binari"
+msgstr "No binario"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__partner_id
 msgid "Partner"
-msgstr ""
+msgstr "Contacto"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_bank_statement_line__membership_id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__membership_id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_payment__membership_id
 msgid "Related membership"
 msgstr "Membresia relacionada"
 
 #. module: energy_communities_cooperator
+#: model:ir.model,name:energy_communities_cooperator.model_share_line
+msgid "Share line"
+msgstr "Línea aportación"
+
+#. module: energy_communities_cooperator
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__share_product_id
+msgid "Share type"
+msgstr "Tipo aportación"
+
+#. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_subscription_request
 msgid "Subscription Request"
-msgstr "Sol·licitud de Subscripció"
+msgstr "Sol·licitud de Suscripción"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__subscription_invoice_ids
 msgid "Subscription invoices"
-msgstr "Registres de pagament"
+msgstr "Registros de pago"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__vat
 msgid "Tax ID"
 msgstr "NIF/CIF"
 
 #. module: energy_communities_cooperator
 #: code:addons/energy_communities_cooperator/models/subscription_request.py:0
 #, python-format
+msgid "There is an existing account for this vat number on this community. "
+msgstr "Existe una cuenta para este número de identidad en la Comunidad. "
+
+#. module: energy_communities_cooperator
+#: model_terms:ir.ui.view,arch_db:energy_communities_cooperator.view_subscription_request_filter_inherit
+msgid "Voluntary Shares"
+msgstr "Aportaciones voluntarias"
+
+#. module: energy_communities_cooperator
+#: code:addons/energy_communities_cooperator/models/subscription_request.py:0
+#, python-format
 msgid "You can't create a voluntary subscription share for a new cooperator."
 msgstr ""
-"No podeu crear una quota de subscripció voluntària per a un nou cooperador."
+"Ezin duzu borondatezko harpidetza-partekaketarik sortu kooperatibatzaile "
+"berri baterako."
 
 #. module: energy_communities_cooperator
 #: model:mail.template,subject:energy_communities_cooperator.email_template_confirmation_company
 msgid "[Som Comunitats] Application to become Community membership"
-msgstr "[Som Comunitats] Sol·licitud d'adhesió a Comunitat Energètica"
+msgstr "[Somos Comunidades] Erkidegoko kide izateko eskaera"
```

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/i18n/es.po` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/i18n/ca_ES.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,366 +2,461 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities_cooperator
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-18 10:44+0000\n"
-"PO-Revision-Date: 2024-04-18 10:44+0000\n"
+"POT-Creation-Date: 2024-05-31 14:23+0000\n"
+"PO-Revision-Date: 2024-05-31 16:34+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
+"Language: ca_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: \n"
-"Plural-Forms: \n"
+"Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 3.4.2\n"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,help:energy_communities_cooperator.field_subscription_request__vat
 msgid ""
 "\n"
-"        The Tax Identification Number. Complete it if the contact is subjected to\n"
+"        The Tax Identification Number. Complete it if the contact is "
+"subjected to\n"
 "        government taxes. Used in some legal statements.\"\n"
 "        "
 msgstr ""
 "\n"
-"        El NIF/CIF. Completa este campo si el contacto está subjecto a\n"
-"        las tasas estatales. Se usa en algunos informes legales.\"\n"
+"        El NIF/CIF. Completa aquest camp si el contacte està subjecte a\n"
+"        les taxes estatals. Es fa servir en alguns  informes legals.\"\n"
 "        "
 
 #. module: energy_communities_cooperator
 #: model:mail.template,body_html:energy_communities_cooperator.email_template_confirmation_voluntary_share
 msgid ""
 "\n"
 "    <p>Dear ${object.firstname},</p>\n"
 "    <p>\n"
-"        We confirm that we have correctly received your request to make a voluntary contribution to the capital\n"
-"        social of <b>${object.company_id.name}</b>, with the following data:\n"
+"        We confirm that we have correctly received your request to make a "
+"voluntary contribution to the capital\n"
+"        social of <b>${object.company_id.name}</b>, with the following "
+"data:\n"
 "    </p>\n"
 "    <ul>\n"
 "        <li>Partner VAT: <b>${object.vat}</b></li>\n"
-"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
+"li>\n"
 "        <li>Charging account: <b>${object.iban}</b></li>\n"
-"        <li>Subscription amount: <b>${object.subscription_amount}€</b></li>\n"
+"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
+"li>\n"
 "    </ul>\n"
 "    <p>\n"
-"        In the next few days you will receive the bank charge in this account, please verify that all the data\n"
-"        provided is correct and you have the money you want to invest, to avoid any incident in the\n"
+"        In the next few days you will receive the bank charge in this "
+"account, please verify that all the data\n"
+"        provided is correct and you have the money you want to invest, to "
+"avoid any incident in the\n"
 "        draft of the receipt.\n"
 "    </p>\n"
 "    <p>\n"
-"        Once the validity of the payment has been verified, you will receive a new notification confirming the\n"
+"        Once the validity of the payment has been verified, you will "
+"receive a new notification confirming the\n"
 "        contribution\n"
-"        made and detailing the particular conditions of your contribution.\n"
+"        made and detailing the particular conditions of your "
+"contribution.\n"
 "    </p>\n"
 "    <p>\n"
-"        Thank you for your involvement with the cooperative and inform you that for any doubt or clarification you can\n"
+"        Thank you for your involvement with the cooperative and inform you "
+"that for any doubt or clarification you can\n"
 "        consult\n"
 "        our website:\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
 "        or send us an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a>\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
 "    </p>\n"
 "    <p>\n"
-"        Get the word out by explaining the project to family and friends. The more we are, the further we will go!\n"
+"        Get the word out by explaining the project to family and friends. "
+"The more we are, the further we will go!\n"
 "    </p>\n"
 "    <p>\n"
 "        Thank you very much and good energy!\n"
 "    </p>\n"
 "    <p>\n"
 "        Sincerely,\n"
 "    </p>\n"
 "    <p>\n"
 "        ${object.company_id.name} team\n"
 "    </p>\n"
-"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" style=\"width: 150px;height: 80px;\"/>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
 "            "
 msgstr ""
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Apreciado/a ${object.firstname},</p>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"Te confirmamos que hemos recibido correctamente tu solicitud para realizar una aportación voluntaria al capital social de <b style=\"font-weight:bolder;\">${object.company_id.name}</b>, con los siguientes datos:\n"
-"    </p>\n"
-"    <ul style=\"margin:0px 0 1rem 0;\">\n"
-"        <li>Socio/a NIF: <b style=\"font-weight:bolder;\">${object.vat}</b></li>\n"
-"        <li>Socio/a: <b style=\"font-weight:bolder;\">${object.firstname} ${object.lastname}</b></li>\n"
-"        <li>Cuenta de cargo: <b style=\"font-weight:bolder;\">${object.iban}</b></li>\n"
-"        <li>Importe aportación: <b style=\"font-weight:bolder;\">${object.subscription_amount}€</b></li>\n"
+"\n"
+"    <p>Apreciat/ada ${object.firstname},</p>\n"
+"    <p>\n"
+"        Et confirmem que hem rebut correctament la teva sol·licitud per "
+"realitzar una aportació voluntària al capital social de <b>${object."
+"company_id.name}</b>, amb les següents dades:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Soci/sòcia NIF: <b>${object.vat}</b></li>\n"
+"        <li>Soci/sòcia: <b>${object.firstname} ${object.lastname}</b></"
+"li>\n"
+"        <li>Compte bancari: <b>${object.iban}</b></li>\n"
+"        <li>Import d'aportació: <b>${object.subscription_amount}€</b></"
+"li>\n"
 "    </ul>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"En los próximos días recibirás el cargo bancario en esta cuenta, por favor verifica que todos los datos facilitados sean correctos y dispones del dinero que quieres invertir, para evitar cualquier incidencia en el giro del recibo.\n"
+"    <p>\n"
+"En els pròxims dies rebràs el càrrec bancari en aquest compte, si us plau "
+"verifica que totes les teves dades siguin correctes i disposis dels diners "
+"que vulguis invertir, per evitar qualsevol incidència en el gir del "
+"rebut.\n"
 "    </p>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"Una vez verificada la validez del pago realizado recibirás una nueva notificación confirmando la aportación realizada y detallando las condiciones particulares de tu aportación.\n"
+"    <p>\n"
+"Una vegada verificat el pagament, rebràs una notificació confirmant "
+"l'aportació realitzada i detallant les condicions particulars de la teva "
+"aportació.\n"
 "    </p>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"Agradecer tu implicación con la cooperativa y informarte que para cualquier duda o aclaración puedes consultar nuestra web&nbsp;\n"
-"        <a href=\"${object.company_id.website}\" style=\"text-decoration:none;background-color:transparent;color:rgb(124, 123, 173);\"> ${object.company_id.website}</a>\n"
-"        &nbsp;o enviarnos un correo electrónico \n"
-"        <a href=\"${object.company_id.email}\" style=\"text-decoration:none;background-color:transparent;color:rgb(124, 123, 173);\">${object.company_id.email}</a>\n"
+"    <p>\n"
+"Agraïm la teva implicació amb la cooperativa i t'informem que pots aclarir "
+"qualsevol dubte en la nostra pàgina web \n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"o enviar-nos un correu electrònic a\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
 "    </p>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"Haz que corra la voz explicando el proyecto a familiares y amigos/as. Cuantos más seamos, más lejos llegaremos!\n"
+"    <p>\n"
+"Fes que corri la veu explicant el nostre projecte a familiars i amics/"
+"amigues. Com més siguem, més lluny arribarem!\n"
 "    </p>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"¡Muchas gracias y buena energía!\n"
+"    <p>\n"
+"Moltes gràcies i bona energia!\n"
 "    </p>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"        Atentamente,\n"
+"    <p>\n"
+"        Atentament,\n"
 "    </p>\n"
 "</br>\n"
-"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
-"        El equipo de ${object.company_id.name}\n"
+"    <p>\n"
+"        L'equip de ${object.company_id.name}\n"
 "    </p>\n"
 "    % if object.company_id.street:\n"
 "        ${object.company_id.street}\n"
 "    % endif\n"
 "    % if object.company_id.street2:\n"
 "        ${object.company_id.street2}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.city or object.company_id.zip:\n"
 "        ${object.company_id.zip} ${object.company_id.city}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.country_id:\n"
-"        ${object.company_id.state_id and ('%s, ' % object.company_id.state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
+"        ${object.company_id.state_id and ('%s, ' % object.company_id."
+"state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.phone:\n"
 "        Teléfono:&nbsp; ${object.company_id.phone}\n"
 "    % endif\n"
 "\n"
 "    % if object.company_id.website:\n"
 "        <div>\n"
-"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object.company_id.website}</a>\n"
+"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object."
+"company_id.website}</a>\n"
 "        </div>\n"
 "    %endif\n"
-"<div>\n"
-"<img src=\"/logo.png?company=${object.company_id.id}\" width=\"150\">\n"
-"</div>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;\"/>\n"
 "            "
 
 #. module: energy_communities_cooperator
 #: model:mail.template,body_html:energy_communities_cooperator.email_template_confirmation_company
 msgid ""
 "\n"
-"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
+"serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
+"\">\n"
 "\n"
 "    <p>Hello,</p>\n"
-"    <p>Thank you for filling out the form and request to join the Community.</p>\n"
-"    <p>In the coming weeks we will contact you to indicate the next steps</p>\n"
+"    <p>Thank you for filling out the form and request to join the "
+"Community.</p>\n"
+"    <p>In the coming weeks we will contact you to indicate the next steps</"
+"p>\n"
 "    <p>Here is a copy of the data we received:</p>\n"
-"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', "
+"Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, "
+"34); background-color: #FFF; \">\n"
 "        <p> - Request to join: ${object.company_id.name}</p>\n"
 "        <p> - Company Name: ${object.company_name}</p>\n"
 "        <p> - Company Email: ${object.company_email}</p>\n"
 "        <p> - VAT: ${object.vat}</p>\n"
 "        <p> - Address: ${object.address}</p>\n"
 "        <p> - Zip code: ${object.zip_code}</p>\n"
 "        <p> - City: ${object.city}</p>\n"
 "        <p> - Country: ${object.country_id.name}</p>\n"
 "        <p> - Firstname: ${object.firstname}</p>\n"
 "        <p> - Lastname: ${object.lastname}</p>\n"
 "        <p> - Function: ${object.contact_person_function}</p>\n"
 "        <p> - Email: ${object.email}</p>\n"
 "        <p> - Phone: ${(object.phone or '')}</p>\n"
-"        <p> - Gender: ${dict(object.fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</p>\n"
+"        <p> - Gender: ${dict(object.fields_get(allfields=['gender'])"
+"['gender']['selection'])[object.gender]}</p>\n"
 "        <p> - Birthdate: ${object.birthdate}</p>\n"
-"        <p> - Language: ${dict(object.fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
+"        <p> - Language: ${dict(object.fields_get(allfields=['lang'])"
+"['lang']['selection'])[object.lang]}</p>\n"
 "        <p> - Initial share amount: ${object.subscription_amount}</p>\n"
-"    % if object.payment_mode_id.payment_method_id.code == 'sepa_direct_debit':\n"
+"    % if object.payment_mode_id.payment_method_id.code == "
+"'sepa_direct_debit':\n"
 "        <p> - Bank account: ${object.iban}</p>\n"
-"        <p> - I authorize bank receipts to be sent to this account: ${object.mandate_approved and 'SI' or 'NO'}</p>\n"
+"        <p> - I authorize bank receipts to be sent to this account: "
+"${object.mandate_approved and 'SI' or 'NO'}</p>\n"
 "    % endif\n"
 "    </div>\n"
 "    <br />\n"
 "    <p>We keep in touch for any questions.</p>\n"
 "    <p>Yours faithfully,</p>\n"
 "    <p>Somcomunitats.coop team </p>\n"
-"    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and "
+"FAQs</a></p>\n"
 "</div>\n"
 "            "
 msgstr ""
-"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
+"serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
+"\">\n"
 "\n"
 "    <p>Hola,</p>\n"
-"    <p>Gracias por rellenar el formulario y solicitar la adhesión a la Comunidad Energética.</p>\n"
-"    <p>En las próximas semanas nos pondremos en contacto contigo para indicarte los siguientes pasos.</p>\n"
-"    <p>Aquí tienes una copia de los datos que hemos recibido:</p>\n"
-"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
-"        <p> - Comunidad: ${object.company_id.name}</p>\n"
-"        <p> - Nombre empresa: ${object.company_name}</p>\n"
-"        <p> - Correo empresa: ${object.company_email}</p>\n"
+"    <p>Gràcies per omplir el formulari i sol·licitar l’adhesió a la "
+"Comunitat Energètica.</p>\n"
+"    <p>En les properes setmanes ens posarem en contacte amb tu per indicar-"
+"te les següents passes.</p>\n"
+"    <p>Aquí tens una còpia de les dades que hem rebut:</p>\n"
+"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', "
+"Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, "
+"34); background-color: #FFF; \">\n"
+"        <p> - Comunitat: ${object.company_id.name}</p>\n"
+"        <p> - Nom empresa: ${object.company_name}</p>\n"
+"        <p> - Correu empresa: ${object.company_email}</p>\n"
 "        <p> - NIF/CIF empresa: ${object.vat}</p>\n"
-"        <p> - Dirección empresa: ${object.address}</p>\n"
-"        <p> - Código postal empresa: ${object.zip_code}</p>\n"
-"        <p> - Ciudad empresa: ${object.city}</p>\n"
-"        <p> - País empresa: ${object.country_id.name}</p>\n"
-"        <p> - Nombre persona representante: ${object.firstname}</p>\n"
-"        <p> - Apellidos persona representante: ${object.lastname}</p>\n"
-"        <p> - Cargo representante: ${object.contact_person_function}</p>\n"
-"        <p> - Correo representante: ${object.email}</p>\n"
-"        <p> - Teléfono representante: ${(object.phone or '')}</p>\n"
-"        <p> - Género representante: ${dict(object.fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</p>\n"
-"        <p> - Fecha nacimiento representante: ${object.birthdate}</p>\n"
-"        <p> - Idioma comunicaciones: ${dict(object.fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
-"        <p> - Importe aportación inicial: ${object.subscription_amount}</p>\n"
-"    % if object.payment_mode_id.payment_method_id.code == 'sepa_direct_debit': \n"
-"        <p> - Cuenta bancaria: ${object.iban}</p>\n"
-"        <p> - Autorizo giros bancarios a esta cuenta: ${object.mandate_approved and 'SI' or 'NO'}</p> \n"
+"        <p> - Direcció empresa: ${object.address}</p>\n"
+"        <p> - Codi postal empresa: ${object.zip_code}</p>\n"
+"        <p> - Ciutat empresa: ${object.city}</p>\n"
+"        <p> - Pais empresa: ${object.country_id.name}</p>\n"
+"        <p> - Nom persona representant: ${object.firstname}</p>\n"
+"        <p> - Cognoms persona representant: ${object.lastname}</p>\n"
+"        <p> - Càrrec representant: ${object.contact_person_function}</p>\n"
+"        <p> - Correu representant: ${object.email}</p>\n"
+"        <p> - Telèfon representant: ${(object.phone or '')}</p>\n"
+"        <p> - Gènere representant: ${dict(object."
+"fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</"
+"p>\n"
+"        <p> - data naixement representant: ${object.birthdate}</p>\n"
+"        <p> - Idioma comunicacions: ${dict(object."
+"fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
+"        <p> - Import aportació inicial: ${object.subscription_amount}</p>\n"
+"    % if object.payment_mode_id.payment_method_id.code == "
+"'sepa_direct_debit': \n"
+"        <p> - Compte bancari: ${object.iban}</p>\n"
+"        <p> - Autoritzo giros bancaris a aquest compte: ${object."
+"mandate_approved and 'SI' or 'NO'}</p> \n"
 "    % endif\n"
 "    </div>\n"
 "    <br />\n"
-"    <p>Seguimos en contacto para cualquier duda.</p>\n"
-"    <p><a href=\"https://web-prod.somcomunitats.coop/recursos/\">Recursos y FAQs</a></p>\n"
-"    <p>Atentamente,</p>\n"
+"<p>Seguim en contacte per qualsevol dubte.</p>\n"
+"    <p><a href=\"https://web-prod.somcomunitats.coop/recursos/\">Recursos "
+"i FAQs</a></p>\n"
+"    <p>Atentament,</p>\n"
 "    </br>\n"
 "    <p>${object.company_id.name}.</p>\n"
 "\n"
 "    % if object.company_id.street:\n"
 "        ${object.company_id.street}\n"
 "    % endif\n"
 "    % if object.company_id.street2:\n"
 "        ${object.company_id.street2}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.city or object.company_id.zip:\n"
 "        ${object.company_id.zip} ${object.company_id.city}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.country_id:\n"
-"        ${object.company_id.state_id and ('%s, ' % object.company_id.state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
+"        ${object.company_id.state_id and ('%s, ' % object.company_id."
+"state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.phone:\n"
 "        Teléfono:&nbsp; ${object.company_id.phone}\n"
 "    % endif\n"
 "\n"
 "    % if object.company_id.website:\n"
 "        <div>\n"
-"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object.company_id.website}</a>\n"
+"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object."
+"company_id.website}</a>\n"
 "        </div>\n"
 "    %endif\n"
 "<div>\n"
 "<img src=\"/logo.png?company=${object.company_id.id}\" width=\"150\">\n"
 "<img src=${object.env.company.logo_url}>\n"
 "</div>\n"
 "</div>\n"
+"            \n"
 "            "
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__active
 msgid "Active"
-msgstr "Activo"
+msgstr "Actiu"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__representative_of_member_company
 msgid "Company Legal Representative"
-msgstr "Representante legal de compañía"
+msgstr "Representant legal de companyia"
+
+#. module: energy_communities_cooperator
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__company_register_number
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_users__company_register_number
+msgid "Company Register Number"
+msgstr "Codi de registre de la companyia"
+
+#. module: energy_communities_cooperator
+#: model:ir.model,name:energy_communities_cooperator.model_res_partner
+msgid "Contact"
+msgstr "Contacte"
 
 #. module: energy_communities_cooperator
 #: model:mail.template,subject:energy_communities_cooperator.email_template_confirmation_voluntary_share
 msgid "Contribute to ${object.company_id.name} Ref. ACSV${object.id}"
 msgstr ""
-"Aportación voluntaria a ${object.company_id.name} Ref. ACSV${object.id}: "
-"Solicitud recibida"
+"Aportació voluntària a ${object.company_id.name} Ref. ACSV${object.id}: "
+"sol·licitud rebuda"
 
 #. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_cooperative_membership
 msgid "Cooperative Membership"
 msgstr "Membresia"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__display_name
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__display_name
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__display_name
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__display_name
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__display_name
 msgid "Display Name"
-msgstr "Nombre Mostrado"
+msgstr "Nom de visualització"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__gender
 msgid "Gender"
-msgstr "Género"
+msgstr "Gènere"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields.selection,name:energy_communities_cooperator.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
-msgstr "Prefiero no compartirlo"
+msgstr "Prefereixo no compartir-ho"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__id
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__id
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__id
 msgid "ID"
-msgstr "Identificador"
-
-#. module: energy_communities_cooperator
-#: model:ir.actions.act_window,name:energy_communities_cooperator.action_account_move
-#: model:ir.ui.menu,name:energy_communities_cooperator.menu_account_move
-msgid "Invoices"
-msgstr "Facturas"
+msgstr "ID"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__is_voluntary
 msgid "Is voluntary contribution"
-msgstr "Es aportación voluntaria"
+msgstr "És una aportació voluntària"
 
 #. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_account_move
 msgid "Journal Entry"
-msgstr "Asiento contable"
+msgstr "Assentament comptable"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move____last_update
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership____last_update
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner____last_update
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line____last_update
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request____last_update
 msgid "Last Modified on"
-msgstr "Última modificación el"
+msgstr "Última modificació el"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__representative
 msgid "Legal Representative"
-msgstr "Representante legal"
+msgstr "Representant legal"
+
+#. module: energy_communities_cooperator
+#: model_terms:ir.ui.view,arch_db:energy_communities_cooperator.view_subscription_request_filter_inherit
+msgid "Mandatory Shares"
+msgstr "Aportacions obligatòries"
 
 #. module: energy_communities_cooperator
 #: model:ir.actions.act_window,name:energy_communities_cooperator.action_cooperative_membership
 #: model:ir.ui.menu,name:energy_communities_cooperator.menu_cooperative_membership
 msgid "Memberships"
-msgstr "Membresias"
+msgstr "Membresies"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields.selection,name:energy_communities_cooperator.selection__subscription_request__gender__not_binary
 msgid "Not binary"
-msgstr "No binario"
+msgstr "No binari"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__partner_id
 msgid "Partner"
-msgstr ""
+msgstr "Contacte"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_bank_statement_line__membership_id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__membership_id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_payment__membership_id
 msgid "Related membership"
 msgstr "Membresia relacionada"
 
 #. module: energy_communities_cooperator
+#: model:ir.model,name:energy_communities_cooperator.model_share_line
+msgid "Share line"
+msgstr "Línia aportació"
+
+#. module: energy_communities_cooperator
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__share_product_id
+msgid "Share type"
+msgstr "Tipus aportació"
+
+#. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_subscription_request
 msgid "Subscription Request"
-msgstr "Sol·licitud de Suscripción"
+msgstr "Sol·licitud de Subscripció"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__subscription_invoice_ids
 msgid "Subscription invoices"
-msgstr "Registros de pago"
+msgstr "Registres de pagament"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__vat
 msgid "Tax ID"
 msgstr "NIF/CIF"
 
 #. module: energy_communities_cooperator
 #: code:addons/energy_communities_cooperator/models/subscription_request.py:0
 #, python-format
+msgid "There is an existing account for this vat number on this community. "
+msgstr "Ja existeix un ompte per aquest número d'identitat a la Comunitat. "
+
+#. module: energy_communities_cooperator
+#: model_terms:ir.ui.view,arch_db:energy_communities_cooperator.view_subscription_request_filter_inherit
+msgid "Voluntary Shares"
+msgstr "Aportacions voluntàries"
+
+#. module: energy_communities_cooperator
+#: code:addons/energy_communities_cooperator/models/subscription_request.py:0
+#, python-format
 msgid "You can't create a voluntary subscription share for a new cooperator."
-msgstr "No puedes crear una aportación voluntaria para un miembro nuevo"
+msgstr ""
+"No podeu crear una quota de subscripció voluntària per a un nou cooperador."
 
 #. module: energy_communities_cooperator
 #: model:mail.template,subject:energy_communities_cooperator.email_template_confirmation_company
 msgid "[Som Comunitats] Application to become Community membership"
-msgstr "[Somos Comunidades] Solicitud adhesión a Comunidad Energética"
-
+msgstr "[Som Comunitats] Sol·licitud d'adhesió a Comunitat Energètica"
```

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/i18n/eu_ES.po` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/i18n/es.po`

 * *Files 18% similar despite different names*

```diff
@@ -2,220 +2,314 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities_cooperator
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-18 10:43+0000\n"
-"PO-Revision-Date: 2024-04-18 10:43+0000\n"
+"POT-Creation-Date: 2024-05-31 14:23+0000\n"
+"PO-Revision-Date: 2024-05-31 16:26+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: \n"
-"Plural-Forms: \n"
+"Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 3.4.2\n"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,help:energy_communities_cooperator.field_subscription_request__vat
 msgid ""
 "\n"
-"        The Tax Identification Number. Complete it if the contact is subjected to\n"
+"        The Tax Identification Number. Complete it if the contact is "
+"subjected to\n"
 "        government taxes. Used in some legal statements.\"\n"
 "        "
 msgstr ""
 "\n"
 "        El NIF/CIF. Completa este campo si el contacto está subjecto a\n"
 "        las tasas estatales. Se usa en algunos informes legales.\"\n"
 "        "
 
 #. module: energy_communities_cooperator
 #: model:mail.template,body_html:energy_communities_cooperator.email_template_confirmation_voluntary_share
 msgid ""
 "\n"
 "    <p>Dear ${object.firstname},</p>\n"
 "    <p>\n"
-"        We confirm that we have correctly received your request to make a voluntary contribution to the capital\n"
-"        social of <b>${object.company_id.name}</b>, with the following data:\n"
+"        We confirm that we have correctly received your request to make a "
+"voluntary contribution to the capital\n"
+"        social of <b>${object.company_id.name}</b>, with the following "
+"data:\n"
 "    </p>\n"
 "    <ul>\n"
 "        <li>Partner VAT: <b>${object.vat}</b></li>\n"
-"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
+"li>\n"
 "        <li>Charging account: <b>${object.iban}</b></li>\n"
-"        <li>Subscription amount: <b>${object.subscription_amount}€</b></li>\n"
+"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
+"li>\n"
 "    </ul>\n"
 "    <p>\n"
-"        In the next few days you will receive the bank charge in this account, please verify that all the data\n"
-"        provided is correct and you have the money you want to invest, to avoid any incident in the\n"
+"        In the next few days you will receive the bank charge in this "
+"account, please verify that all the data\n"
+"        provided is correct and you have the money you want to invest, to "
+"avoid any incident in the\n"
 "        draft of the receipt.\n"
 "    </p>\n"
 "    <p>\n"
-"        Once the validity of the payment has been verified, you will receive a new notification confirming the\n"
+"        Once the validity of the payment has been verified, you will "
+"receive a new notification confirming the\n"
 "        contribution\n"
-"        made and detailing the particular conditions of your contribution.\n"
+"        made and detailing the particular conditions of your "
+"contribution.\n"
 "    </p>\n"
 "    <p>\n"
-"        Thank you for your involvement with the cooperative and inform you that for any doubt or clarification you can\n"
+"        Thank you for your involvement with the cooperative and inform you "
+"that for any doubt or clarification you can\n"
 "        consult\n"
 "        our website:\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
 "        or send us an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a>\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
 "    </p>\n"
 "    <p>\n"
-"        Get the word out by explaining the project to family and friends. The more we are, the further we will go!\n"
+"        Get the word out by explaining the project to family and friends. "
+"The more we are, the further we will go!\n"
 "    </p>\n"
 "    <p>\n"
 "        Thank you very much and good energy!\n"
 "    </p>\n"
 "    <p>\n"
 "        Sincerely,\n"
 "    </p>\n"
 "    <p>\n"
 "        ${object.company_id.name} team\n"
 "    </p>\n"
-"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" style=\"width: 150px;height: 80px;\"/>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
 "            "
 msgstr ""
-"    <p>${object.firstname} agurgarria,</p>\n"
-"    <p>\n"
-"Baieztatzen dizugu zuzen jaso dugula zure eskaera, <b>${object.company_id.name}</b> kapital sozialera borondatezko ekarpena egiteko, datu hauekin:\n"
 "\n"
-"    </p>\n"
-"    <ul>\n"
-"        <li>Bazkidea DNI: <b>${object.vat}</b></li>\n"
-"        <li>Bazkidea: <b>${object.firstname} ${object.lastname}</b></li>\n"
-"        <li>Kargu-kontua: <b>${object.iban}</b></li>\n"
-"        <li>Ekarpenaren zenbatekoa: <b>${object.subscription_amount}€</b></li>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Apreciado/a "
+"${object.firstname},</p>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"Te confirmamos que hemos recibido correctamente tu solicitud para realizar "
+"una aportación voluntaria al capital social de <b style=\"font-weight:"
+"bolder;\">${object.company_id.name}</b>, con los siguientes datos:\n"
+"    </p>\n"
+"    <ul style=\"margin:0px 0 1rem 0;\">\n"
+"        <li>Socio/a NIF: <b style=\"font-weight:bolder;\">${object.vat}</"
+"b></li>\n"
+"        <li>Socio/a: <b style=\"font-weight:bolder;\">${object.firstname} "
+"${object.lastname}</b></li>\n"
+"        <li>Cuenta de cargo: <b style=\"font-weight:bolder;\">${object."
+"iban}</b></li>\n"
+"        <li>Importe aportación: <b style=\"font-weight:bolder;\">${object."
+"subscription_amount}€</b></li>\n"
 "    </ul>\n"
-"    <p>\n"
-"Datozen egunetan kontu honetan jasoko duzu bankuko kargua. Mesedez, egiaztatu emandako datu guztiak zuzenak direla eta eman nahi duzun dirua duzula, ordainagiriaren igorpenean gorabeherarik izan ez dadin.\n"
-"    </p>\n"
-"    <p>\n"
-"Egindako ordainketaren balioa egiaztatu ondoren, beste jakinarazpen bat jasoko duzu, egindako ekarpena baieztatuz eta zure ekarpenaren baldintza partikularrak zehaztuz.\n"
-"    </p>\n"
-"    <p>\n"
-"Kooperatibarekin duzun inplikazioa eskertu nahi dizugu, eta, edozein zalantza argitzeko, gure web orria kontsulta dezakezu \n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>\n"
-"edo mezu elektroniko bat bidali \n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a>\n"
-" helbidera.\n"
-"    </p>\n"
-"    <p>\n"
-"Ahoz ahoz proiektua familiakoei, auzokideei eta lagunei azaldu. Zenbat eta gehiago izan, urrunago iritsiko gara!\n"
-"    </p>\n"
-"    <p>\n"
-"Eskerrik asko eta energia on!\n"
-"    </p>\n"
-"    <p>\n"
-"        Adeitasunez,\n"
-"    </p>\n"
-"    <p>\n"
-"        ${object.company_id.name} taldea\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"En los próximos días recibirás el cargo bancario en esta cuenta, por favor "
+"verifica que todos los datos facilitados sean correctos y dispones del "
+"dinero que quieres invertir, para evitar cualquier incidencia en el giro "
+"del recibo.\n"
+"    </p>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"Una vez verificada la validez del pago realizado recibirás una nueva "
+"notificación confirmando la aportación realizada y detallando las "
+"condiciones particulares de tu aportación.\n"
+"    </p>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"Agradecer tu implicación con la cooperativa y informarte que para "
+"cualquier duda o aclaración puedes consultar nuestra web&nbsp;\n"
+"        <a href=\"${object.company_id.website}\" style=\"text-decoration:"
+"none;background-color:transparent;color:rgb(124, 123, 173);\"> ${object."
+"company_id.website}</a>\n"
+"        &nbsp;o enviarnos un correo electrónico \n"
+"        <a href=\"${object.company_id.email}\" style=\"text-decoration:"
+"none;background-color:transparent;color:rgb(124, 123, 173);\">${object."
+"company_id.email}</a>\n"
+"    </p>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"Haz que corra la voz explicando el proyecto a familiares y amigos/as. "
+"Cuantos más seamos, más lejos llegaremos!\n"
+"    </p>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"¡Muchas gracias y buena energía!\n"
+"    </p>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"        Atentamente,\n"
+"    </p>\n"
+"</br>\n"
+"    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida "
+"Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">\n"
+"        El equipo de ${object.company_id.name}\n"
 "    </p>\n"
-"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" style=\"width: 150px;\"/>\n"
+"    % if object.company_id.street:\n"
+"        ${object.company_id.street}\n"
+"    % endif\n"
+"    % if object.company_id.street2:\n"
+"        ${object.company_id.street2}<br/>\n"
+"    % endif\n"
+"    % if object.company_id.city or object.company_id.zip:\n"
+"        ${object.company_id.zip} ${object.company_id.city}<br/>\n"
+"    % endif\n"
+"    % if object.company_id.country_id:\n"
+"        ${object.company_id.state_id and ('%s, ' % object.company_id."
+"state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
+"    % endif\n"
+"    % if object.company_id.phone:\n"
+"        Teléfono:&nbsp; ${object.company_id.phone}\n"
+"    % endif\n"
+"\n"
+"    % if object.company_id.website:\n"
+"        <div>\n"
+"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object."
+"company_id.website}</a>\n"
+"        </div>\n"
+"    %endif\n"
+"<div>\n"
+"<img src=\"/logo.png?company=${object.company_id.id}\" width=\"150\">\n"
+"</div>\n"
 "            "
 
-
 #. module: energy_communities_cooperator
 #: model:mail.template,body_html:energy_communities_cooperator.email_template_confirmation_company
 msgid ""
 "\n"
-"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
+"serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
+"\">\n"
 "\n"
 "    <p>Hello,</p>\n"
-"    <p>Thank you for filling out the form and request to join the Community.</p>\n"
-"    <p>In the coming weeks we will contact you to indicate the next steps</p>\n"
+"    <p>Thank you for filling out the form and request to join the "
+"Community.</p>\n"
+"    <p>In the coming weeks we will contact you to indicate the next steps</"
+"p>\n"
 "    <p>Here is a copy of the data we received:</p>\n"
-"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', "
+"Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, "
+"34); background-color: #FFF; \">\n"
 "        <p> - Request to join: ${object.company_id.name}</p>\n"
 "        <p> - Company Name: ${object.company_name}</p>\n"
 "        <p> - Company Email: ${object.company_email}</p>\n"
 "        <p> - VAT: ${object.vat}</p>\n"
 "        <p> - Address: ${object.address}</p>\n"
 "        <p> - Zip code: ${object.zip_code}</p>\n"
 "        <p> - City: ${object.city}</p>\n"
 "        <p> - Country: ${object.country_id.name}</p>\n"
 "        <p> - Firstname: ${object.firstname}</p>\n"
 "        <p> - Lastname: ${object.lastname}</p>\n"
 "        <p> - Function: ${object.contact_person_function}</p>\n"
 "        <p> - Email: ${object.email}</p>\n"
 "        <p> - Phone: ${(object.phone or '')}</p>\n"
-"        <p> - Gender: ${dict(object.fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</p>\n"
+"        <p> - Gender: ${dict(object.fields_get(allfields=['gender'])"
+"['gender']['selection'])[object.gender]}</p>\n"
 "        <p> - Birthdate: ${object.birthdate}</p>\n"
-"        <p> - Language: ${dict(object.fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
+"        <p> - Language: ${dict(object.fields_get(allfields=['lang'])"
+"['lang']['selection'])[object.lang]}</p>\n"
 "        <p> - Initial share amount: ${object.subscription_amount}</p>\n"
-"    % if object.payment_mode_id.payment_method_id.code == 'sepa_direct_debit':\n"
+"    % if object.payment_mode_id.payment_method_id.code == "
+"'sepa_direct_debit':\n"
 "        <p> - Bank account: ${object.iban}</p>\n"
-"        <p> - I authorize bank receipts to be sent to this account: ${object.mandate_approved and 'SI' or 'NO'}</p>\n"
+"        <p> - I authorize bank receipts to be sent to this account: "
+"${object.mandate_approved and 'SI' or 'NO'}</p>\n"
 "    % endif\n"
 "    </div>\n"
 "    <br />\n"
 "    <p>We keep in touch for any questions.</p>\n"
 "    <p>Yours faithfully,</p>\n"
 "    <p>Somcomunitats.coop team </p>\n"
-"    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and "
+"FAQs</a></p>\n"
 "</div>\n"
 "            "
 msgstr ""
-"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
+"serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
+"\">\n"
 "\n"
 "    <p>Hola,</p>\n"
-"    <p>Gracias por rellenar el formulario y solicitar la adhesión a la Comunidad Energética.</p>\n"
-"    <p>En las próximas semanas nos pondremos en contacto contigo para indicarte los siguientes pasos.</p>\n"
+"    <p>Gracias por rellenar el formulario y solicitar la adhesión a la "
+"Comunidad Energética.</p>\n"
+"    <p>En las próximas semanas nos pondremos en contacto contigo para "
+"indicarte los siguientes pasos.</p>\n"
 "    <p>Aquí tienes una copia de los datos que hemos recibido:</p>\n"
-"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"    <div id=\"field_list_div\" style=\"font-family: 'Lucica Grande', "
+"Ubuntu, Arial, Verdana, sans-serif; font-size: 10px; color: rgb(34, 34, "
+"34); background-color: #FFF; \">\n"
 "        <p> - Comunidad: ${object.company_id.name}</p>\n"
 "        <p> - Nombre empresa: ${object.company_name}</p>\n"
 "        <p> - Correo empresa: ${object.company_email}</p>\n"
 "        <p> - NIF/CIF empresa: ${object.vat}</p>\n"
 "        <p> - Dirección empresa: ${object.address}</p>\n"
 "        <p> - Código postal empresa: ${object.zip_code}</p>\n"
 "        <p> - Ciudad empresa: ${object.city}</p>\n"
 "        <p> - País empresa: ${object.country_id.name}</p>\n"
 "        <p> - Nombre persona representante: ${object.firstname}</p>\n"
 "        <p> - Apellidos persona representante: ${object.lastname}</p>\n"
 "        <p> - Cargo representante: ${object.contact_person_function}</p>\n"
 "        <p> - Correo representante: ${object.email}</p>\n"
 "        <p> - Teléfono representante: ${(object.phone or '')}</p>\n"
-"        <p> - Género representante: ${dict(object.fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</p>\n"
+"        <p> - Género representante: ${dict(object."
+"fields_get(allfields=['gender'])['gender']['selection'])[object.gender]}</"
+"p>\n"
 "        <p> - Fecha nacimiento representante: ${object.birthdate}</p>\n"
-"        <p> - Idioma comunicaciones: ${dict(object.fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
-"        <p> - Importe aportación inicial: ${object.subscription_amount}</p>\n"
-"    % if object.payment_mode_id.payment_method_id.code == 'sepa_direct_debit': \n"
+"        <p> - Idioma comunicaciones: ${dict(object."
+"fields_get(allfields=['lang'])['lang']['selection'])[object.lang]}</p>\n"
+"        <p> - Importe aportación inicial: ${object.subscription_amount}</"
+"p>\n"
+"    % if object.payment_mode_id.payment_method_id.code == "
+"'sepa_direct_debit': \n"
 "        <p> - Cuenta bancaria: ${object.iban}</p>\n"
-"        <p> - Autorizo giros bancarios a esta cuenta: ${object.mandate_approved and 'SI' or 'NO'}</p> \n"
+"        <p> - Autorizo giros bancarios a esta cuenta: ${object."
+"mandate_approved and 'SI' or 'NO'}</p> \n"
 "    % endif\n"
 "    </div>\n"
 "    <br />\n"
 "    <p>Seguimos en contacto para cualquier duda.</p>\n"
-"    <p><a href=\"https://web-prod.somcomunitats.coop/recursos/\">Recursos y FAQs</a></p>\n"
+"    <p><a href=\"https://web-prod.somcomunitats.coop/recursos/\">Recursos "
+"y FAQs</a></p>\n"
 "    <p>Atentamente,</p>\n"
 "    </br>\n"
 "    <p>${object.company_id.name}.</p>\n"
 "\n"
 "    % if object.company_id.street:\n"
 "        ${object.company_id.street}\n"
 "    % endif\n"
 "    % if object.company_id.street2:\n"
 "        ${object.company_id.street2}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.city or object.company_id.zip:\n"
 "        ${object.company_id.zip} ${object.company_id.city}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.country_id:\n"
-"        ${object.company_id.state_id and ('%s, ' % object.company_id.state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
+"        ${object.company_id.state_id and ('%s, ' % object.company_id."
+"state_id.name) or ''} ${object.company_id.country_id.name or ''}<br/>\n"
 "    % endif\n"
 "    % if object.company_id.phone:\n"
 "        Teléfono:&nbsp; ${object.company_id.phone}\n"
 "    % endif\n"
 "\n"
 "    % if object.company_id.website:\n"
 "        <div>\n"
-"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object.company_id.website}</a>\n"
+"            Web :&nbsp;<a href=\"${object.company_id.website}\">${object."
+"company_id.website}</a>\n"
 "        </div>\n"
 "    %endif\n"
 "<div>\n"
 "<img src=\"/logo.png?company=${object.company_id.id}\" width=\"150\">\n"
 "<img src=${object.env.company.logo_url}>\n"
 "</div>\n"
 "</div>\n"
@@ -228,28 +322,41 @@
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__representative_of_member_company
 msgid "Company Legal Representative"
 msgstr "Representante legal de compañía"
 
 #. module: energy_communities_cooperator
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__company_register_number
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_users__company_register_number
+msgid "Company Register Number"
+msgstr "Código de registro de la compañía"
+
+#. module: energy_communities_cooperator
+#: model:ir.model,name:energy_communities_cooperator.model_res_partner
+msgid "Contact"
+msgstr "Contacte"
+
+#. module: energy_communities_cooperator
 #: model:mail.template,subject:energy_communities_cooperator.email_template_confirmation_voluntary_share
 msgid "Contribute to ${object.company_id.name} Ref. ACSV${object.id}"
 msgstr ""
-"${object.company_id.name} autofinantzaketan ematea Erref. ACSV${object.id}: "
-"jasotako eskaera"
+"Aportación voluntaria a ${object.company_id.name} Ref. ACSV${object.id}: "
+"Solicitud recibida"
 
 #. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_cooperative_membership
 msgid "Cooperative Membership"
 msgstr "Membresia"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__display_name
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__display_name
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__display_name
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__display_name
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__display_name
 msgid "Display Name"
 msgstr "Nombre Mostrado"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__gender
 msgid "Gender"
@@ -259,70 +366,83 @@
 #: model:ir.model.fields.selection,name:energy_communities_cooperator.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
 msgstr "Prefiero no compartirlo"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__id
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner__id
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__id
 msgid "ID"
 msgstr "Identificador"
 
 #. module: energy_communities_cooperator
-#: model:ir.actions.act_window,name:energy_communities_cooperator.action_account_move
-#: model:ir.ui.menu,name:energy_communities_cooperator.menu_account_move
-msgid "Invoices"
-msgstr "Facturas"
-
-#. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__is_voluntary
 msgid "Is voluntary contribution"
 msgstr "Es aportación voluntaria"
 
 #. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_account_move
 msgid "Journal Entry"
-msgstr "Egunkari-sarrera"
+msgstr "Asiento contable"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move____last_update
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership____last_update
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_res_partner____last_update
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line____last_update
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request____last_update
 msgid "Last Modified on"
 msgstr "Última modificación el"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__representative
 msgid "Legal Representative"
 msgstr "Representante legal"
 
 #. module: energy_communities_cooperator
+#: model_terms:ir.ui.view,arch_db:energy_communities_cooperator.view_subscription_request_filter_inherit
+msgid "Mandatory Shares"
+msgstr "Aportaciones obligatorias"
+
+#. module: energy_communities_cooperator
 #: model:ir.actions.act_window,name:energy_communities_cooperator.action_cooperative_membership
 #: model:ir.ui.menu,name:energy_communities_cooperator.menu_cooperative_membership
 msgid "Memberships"
 msgstr "Membresias"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields.selection,name:energy_communities_cooperator.selection__subscription_request__gender__not_binary
 msgid "Not binary"
 msgstr "No binario"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__partner_id
 msgid "Partner"
-msgstr ""
+msgstr "Contacto"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_bank_statement_line__membership_id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_move__membership_id
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_account_payment__membership_id
 msgid "Related membership"
 msgstr "Membresia relacionada"
 
 #. module: energy_communities_cooperator
+#: model:ir.model,name:energy_communities_cooperator.model_share_line
+msgid "Share line"
+msgstr "Línea aportación"
+
+#. module: energy_communities_cooperator
+#: model:ir.model.fields,field_description:energy_communities_cooperator.field_share_line__share_product_id
+msgid "Share type"
+msgstr "Tipo aportación"
+
+#. module: energy_communities_cooperator
 #: model:ir.model,name:energy_communities_cooperator.model_subscription_request
 msgid "Subscription Request"
 msgstr "Sol·licitud de Suscripción"
 
 #. module: energy_communities_cooperator
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_cooperative_membership__subscription_invoice_ids
 msgid "Subscription invoices"
@@ -332,16 +452,25 @@
 #: model:ir.model.fields,field_description:energy_communities_cooperator.field_subscription_request__vat
 msgid "Tax ID"
 msgstr "NIF/CIF"
 
 #. module: energy_communities_cooperator
 #: code:addons/energy_communities_cooperator/models/subscription_request.py:0
 #, python-format
+msgid "There is an existing account for this vat number on this community. "
+msgstr "Existe una cuenta para este número de identidad en la Comunidad."
+
+#. module: energy_communities_cooperator
+#: model_terms:ir.ui.view,arch_db:energy_communities_cooperator.view_subscription_request_filter_inherit
+msgid "Voluntary Shares"
+msgstr "Aportaciones voluntarias"
+
+#. module: energy_communities_cooperator
+#: code:addons/energy_communities_cooperator/models/subscription_request.py:0
+#, python-format
 msgid "You can't create a voluntary subscription share for a new cooperator."
-msgstr ""
-"Ezin duzu borondatezko harpidetza-partekaketarik sortu kooperatibatzaile "
-"berri baterako."
+msgstr "No puedes crear una aportación voluntaria para un miembro nuevo."
 
 #. module: energy_communities_cooperator
 #: model:mail.template,subject:energy_communities_cooperator.email_template_confirmation_company
 msgid "[Som Comunitats] Application to become Community membership"
-msgstr "[Somos Comunidades] Erkidegoko kide izateko eskaera"
+msgstr "[Somos Comunidades] Solicitud adhesión a Comunidad Energética"
```

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/account_move.py` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/account_move.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/cooperative_membership.py` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/cooperative_membership.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/partner.py` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/partner.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/models/subscription_request.py` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/cooperative_membership_views.xml` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/cooperative_membership_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/operation_request_views.xml` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/operation_request_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/res_company_views.xml` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/res_company_views.xml`

 * *Files 24% similar despite different names*

#### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/res_company_views.xml` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/res_company_views.xml`

```diff
@@ -4,13 +4,19 @@
     <field name="name">res.company.form.easymy.coop.inherit</field>
     <field name="model">res.company</field>
     <field name="inherit_id" ref="cooperator.view_company_form"/>
     <field name="arch" type="xml">
       <field name="property_cooperator_account" position="after">
         <field name="subscription_journal_id"/>
       </field>
-      <group name="coop_grp" position="inside">
+      <field name="cooperator_share_update_mail_template" position="before">
         <field name="send_share_update_email"/>
-      </group>
+      </field>
+      <field name="cooperator_share_transfer_mail_template" position="before">
+        <field name="send_share_transfer_email"/>
+      </field>
+      <field name="cooperator_waiting_list_mail_template" position="before">
+        <field name="send_waiting_list_email"/>
+      </field>
     </field>
   </record>
 </odoo>
```

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/res_partner_views.xml` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/res_partner_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo/addons/energy_communities_cooperator/views/subscription_request_view.xml` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo/addons/energy_communities_cooperator/views/subscription_request_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_cooperator-14.0.1.0.1/odoo14_addon_energy_communities_cooperator.egg-info/SOURCES.txt` & `odoo14-addon-energy_communities_cooperator-14.0.1.0.2/odoo14_addon_energy_communities_cooperator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

