# Comparing `tmp/odoo14-addon-energy_communities_crm-14.0.1.1.1.tar.gz` & `tmp/odoo14-addon-energy_communities_crm-14.0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_communities_crm-14.0.1.1.1.tar", last modified: Tue May 21 14:24:56 2024, max compression
+gzip compressed data, was "odoo14-addon-energy_communities_crm-14.0.1.1.2.tar", last modified: Mon Jun  3 13:53:08 2024, max compression
```

## Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1.tar` & `odoo14-addon-energy_communities_crm-14.0.1.1.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.067343 odoo14-addon-energy_communities_crm-14.0.1.1.1/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      485 2024-05-21 14:24:56.067343 odoo14-addon-energy_communities_crm-14.0.1.1.1/PKG-INFO
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.975334 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.975334 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.983335 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4903 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1460 2024-05-21 14:23:15.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/__manifest__.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.987335 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/controllers/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       37 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/controllers/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    25646 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/controllers/website_community_data.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.987335 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/data/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1924 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/data/crm_lead_tag.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    16616 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/data/mail_template_data.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.991335 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/i18n/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    68031 2024-05-21 10:26:57.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/i18n/ca_ES.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    67518 2024-05-21 10:26:57.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/i18n/es.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    67096 2024-05-21 10:26:57.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/i18n/eu_ES.po
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.023339 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      240 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    12235 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_lead.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      194 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_lead_metadata_line.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      820 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1953 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping_field.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2635 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_stage.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      910 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_tag.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1138 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_team.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1592 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/metadata_mapping_conf.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      174 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/utm_source.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.023339 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/security/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      558 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/security/ir.model.access.csv
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1697 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/security/ir_rule_data.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.023339 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/services/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       31 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/services/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     8701 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/services/crm_lead_service.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.975334 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/static/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:55.979334 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/static/src/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.023339 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/static/src/js/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5285 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/static/src/js/community-data-website.js
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.027339 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/tests/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       68 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/tests/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3740 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/tests/test_crm_lead.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1870 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/tests/test_crm_lead_service.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.055342 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3399 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_lead_metadata_mapping_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5900 2024-05-21 14:19:50.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_lead_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      794 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_stage_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1578 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_tag_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      959 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_team_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2340 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/energy_communities_crm_lead_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1584 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/menus.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    28028 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/website_community_data_template.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.063342 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       89 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3778 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1087 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      574 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/multicompany_easy_creation.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 14:24:56.067343 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      485 2024-05-21 14:24:55.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/PKG-INFO
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2773 2024-05-21 14:24:55.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/SOURCES.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-05-21 14:24:55.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/dependency_links.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-05-07 09:00:47.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/not-zip-safe
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      188 2024-05-21 14:24:55.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/requires.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        5 2024-05-21 14:24:55.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/top_level.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       38 2024-05-21 14:24:56.067343 odoo14-addon-energy_communities_crm-14.0.1.1.1/setup.cfg
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      449 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities_crm-14.0.1.1.1/setup.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      485 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/PKG-INFO
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.177131 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.177131 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4903 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1460 2024-06-03 13:41:17.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/__manifest__.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/controllers/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       37 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/controllers/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    25646 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/controllers/website_community_data.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/data/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1924 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/data/crm_lead_tag.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    16616 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/data/mail_template_data.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/i18n/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    73270 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/i18n/ca_ES.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    72779 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/i18n/es.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    72306 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/i18n/eu_ES.po
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      240 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    12235 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_lead.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      194 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_lead_metadata_line.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      820 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1953 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping_field.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2635 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_stage.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      910 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_tag.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1138 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_team.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1592 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/metadata_mapping_conf.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      174 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/utm_source.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/security/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      558 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/security/ir.model.access.csv
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1697 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/security/ir_rule_data.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/services/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       31 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/services/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     8701 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/services/crm_lead_service.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.177131 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/static/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.177131 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/static/src/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/static/src/js/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5285 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/static/src/js/community-data-website.js
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/tests/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       68 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/tests/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3740 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/tests/test_crm_lead.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1870 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/tests/test_crm_lead_service.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3399 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_lead_metadata_mapping_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5501 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_lead_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      794 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_stage_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1578 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_tag_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      959 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_team_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2340 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/energy_communities_crm_lead_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1584 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/menus.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    28460 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/website_community_data_template.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       89 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3778 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1087 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      574 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/multicompany_easy_creation.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      485 2024-06-03 13:53:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/PKG-INFO
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2773 2024-06-03 13:53:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/SOURCES.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:53:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/dependency_links.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:53:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/not-zip-safe
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      188 2024-06-03 13:53:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/requires.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-06-03 13:53:08.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/top_level.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-06-03 13:53:08.180464 odoo14-addon-energy_communities_crm-14.0.1.1.2/setup.cfg
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      449 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities_crm-14.0.1.1.2/setup.py
```

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/__init__.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/__manifest__.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """,
     "author": "Som Comunitats",
     "website": "https://coopdevs.org",
     # Categories can be used to filter modules in modules listing
     # Check https://github.com/odoo/odoo/blob/14.0/odoo/addons/base/data/ir_module_category_data.xml
     # for the full list
     "category": "Sales/CRM",
-    "version": "14.0.1.1.1",
+    "version": "14.0.1.1.2",
     "license": "AGPL-3",
     # any module necessary for this one to work correctly
     "depends": [
         "base",
         "crm",
         "crm_metadata",
         "crm_metadata_rest_api",
```

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/controllers/website_community_data.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/controllers/website_community_data.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/data/crm_lead_tag.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/data/crm_lead_tag.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/data/mail_template_data.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/data/mail_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/i18n/ca_ES.po` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/i18n/ca_ES.po`

 * *Files 3% similar despite different names*

```diff
@@ -2,303 +2,492 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities_crm
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-26 12:56+0000\n"
-"PO-Revision-Date: 2024-03-26 12:56+0000\n"
+"POT-Creation-Date: 2024-05-31 14:39+0000\n"
+"PO-Revision-Date: 2024-05-31 17:26+0200\n"
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
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_assigned_to_coordinator_id
 msgid ""
 "\n"
 "                \n"
-"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, "
+"Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); "
+"background-color: #FFF; \">\n"
 "                        <p>Hello,</p><br/>\n"
-"                        <p>There is a new Energy Community registration request.</p>\n"
+"                        <p>There is a new Energy Community registration "
+"request.</p>\n"
 "                        <p>Go to Odoo to track this registration.</p><br/>\n"
 "                        <p>Yours faithfully,</p>\n"
 "                        <p>Somcomunitats.coop team</p>\n"
-"                        <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                        <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                    </div>\n"
 "                \n"
 "            "
 msgstr ""
 "\n"
 "                \n"
-"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, "
+"Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); "
+"background-color: #FFF; \">\n"
 "\n"
 "                        <p>Hola,</p>\n"
 "\n"
-"                        <p>Hi ha una nova sol·licitud d’alta de Comunitat Energètica.</p>\n"
+"                        <p>Hi ha una nova sol·licitud d’alta de Comunitat "
+"Energètica.</p>\n"
 "\n"
 "                        <p>Vés al Odoo a fer seguiment d’aquesta alta.</p>\n"
 "\n"
 "                        <p>Atentament,</p>\n"
 "                        <p>Equip de somcomunitats.coop</p>\n"
-"                        <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                        <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
 "\n"
 "                    </div>\n"
 "                \n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_contact_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for contact.</p>\n"
-"                    <p>We have received your email and we have we have forwarded it to the Community so that they can contact you as soon as possible.</p>\n"
+"                    <p>We have received your email and we have we have "
+"forwarded it to the Community so that they can contact you as soon as "
+"possible.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-size:13px;font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
-"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Hola,</p>\n"
-"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Gràcies per posar-te en contacte.</p>\n"
-"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Hem rebut el teu correu electrònic i li hem fet arribar a la Comunitat Energètica perquè es posin en contacte amb tu tan aviat com els sigui possible.</p>\n"
+"\n"
+"                <div style=\"font-size:13px;font-family: 'Lucica Grande', "
+"Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, "
+"34); background-color: #FFF; \">\n"
+"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;"
+"Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Hola,</p>\n"
+"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;"
+"Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Gràcies per "
+"posar-te en contacte.</p>\n"
+"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;"
+"Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Hem rebut el "
+"teu correu electrònic i li hem fet arribar a la Comunitat Energètica perquè "
+"es posin en contacte amb tu tan aviat com els sigui possible.</p>\n"
 "                    <br>\n"
-"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Atentament,</p>\n"
-"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Equip de Som Comunitats</p>\n"
-"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\"><a href=\"https://somcomunitats.coop/recursos/\" style=\"text-decoration:none;background-color:transparent;color:rgb(124, 123, 173);\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;"
+"Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Atentament,</"
+"p>\n"
+"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;"
+"Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\">Equip de Som "
+"Comunitats</p>\n"
+"                    <p style=\"margin:0px;font-size:13px;font-family:&quot;"
+"Lucida Grande&quot;, Helvetica, Verdana, Arial, sans-serif;\"><a "
+"href=\"https://somcomunitats.coop/recursos/\" style=\"text-decoration:none;"
+"background-color:transparent;color:rgb(124, 123, 173);\">Recursos i "
+"preguntes freqüents</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_creation_receipt_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form and requesting the membership of your Energy Community on the Somcomunitats.coop platform.</p>\n"
-"                    <p>In the coming weeks we will study the application and contact you to indicate the steps and the information necessary to complete the registration process for the Community and the people who are part of it.</p>\n"
+"                    <p>Thank you for filling out the form and requesting "
+"the membership of your Energy Community on the Somcomunitats.coop platform."
+"</p>\n"
+"                    <p>In the coming weeks we will study the application "
+"and contact you to indicate the steps and the information necessary to "
+"complete the registration process for the Community and the people who are "
+"part of it.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
 "\n"
-"                    <p>Hola,</p>\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "\n"
-"                    <p>Gràcies per omplir el formulari i sol·licitar l'adhesió de la vostra Comunitat Energètica a la plataforma Som Comunitats.</p>\n"
+"                    <p>Hola,</p>\n"
 "\n"
-"                    <p>Durant els propers dies estudiarem la sol·licitud i ens posarem en contacte amb vosaltres per indicar-vos els passos i la informació necessària per acabar el procés d'alta de la Comunitat i de les persones que en formeu part.</p>\n"
+"                    <p>Gràcies per omplir el formulari i sol·licitar "
+"l'adhesió de la vostra Comunitat Energètica a la plataforma Som Comunitats."
+"</p>\n"
+"\n"
+"                    <p>Durant els propers dies estudiarem la sol·licitud i "
+"ens posarem en contacte amb vosaltres per indicar-vos els passos i la "
+"informació necessària per acabar el procés d'alta de la Comunitat i de les "
+"persones que en formeu part.</p>\n"
 "\n"
 "                    <br />\n"
 "                    <p>Seguim en contacte per qualsevol consulta.</p>\n"
 "                    <p>Atentament,</p>\n"
 "                    <p>Equip de Som Comunitats</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
 "\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_source_coord_web_other_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form to request contact regarding the Coordinators.</p>\n"
+"                    <p>Thank you for filling out the form to request "
+"contact regarding the Coordinators.</p>\n"
 "                    <p>We have successfully received your details.</p>\n"
-"                    <p>Over the next few days we will study the request and get in touch with you.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
-"                    <p>Gràcies per omplir el formulari per demanar contacte en relació a les Coordinadores.</p>\n"
+"                    <p>Gràcies per omplir el formulari per demanar contacte "
+"en relació a les Coordinadores.</p>\n"
 "                    <p>Hem rebut correctament les teves dades.</p>\n"
-"                    <p>Durant els propers dies estudiarem la sol·licitud i ens posarem en contacte amb vosaltres.</p>\n"
+"                    <p>Durant els propers dies estudiarem la sol·licitud i "
+"ens posarem en contacte amb vosaltres.</p>\n"
 "                    <br />\n"
 "                    <p>Seguim en contacte per qualsevol consulta.</p>\n"
 "                    <p>Atentament,</p>\n"
 "                    <p>Equip de Som Comunitats</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
 "\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_source_coord_web_hiring_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form to request the hiring of a Coordinator.</p>\n"
+"                    <p>Thank you for filling out the form to request the "
+"hiring of a Coordinator.</p>\n"
 "                    <p>We have successfully received your details</p>\n"
-"                    <p>Over the next few days we will study the request and get in touch with you.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
-"                    <p>Gràcies per omplir el formulari per demanar la contractació d’una Coordinadora.</p>\n"
+"                    <p>Gràcies per omplir el formulari per demanar la "
+"contractació d’una Coordinadora.</p>\n"
 "                    <p>Hem rebut correctament les teves dades.</p>\n"
-"                    <p>Durant els propers dies estudiarem la sol·licitud i ens posarem en contacte amb vosaltres.</p>\n"
+"                    <p>Durant els propers dies estudiarem la sol·licitud i "
+"ens posarem en contacte amb vosaltres.</p>\n"
 "                    <br />\n"
 "                    <p>Seguim en contacte per qualsevol consulta.</p>\n"
 "                    <p>Atentament,</p>\n"
 "                    <p>Equip de Som Comunitats</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
 "\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_advise_future_ce_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>In case an Energy Community is activated in your neighborhood or municipality, they can consult the existing requests and contact you. Without any commitment on your part beyond having shown interest in promoting a movement of social transformation and an energy model.</p>\n"
+"                    <p>In case an Energy Community is activated in your "
+"neighborhood or municipality, they can consult the existing requests and "
+"contact you. Without any commitment on your part beyond having shown "
+"interest in promoting a movement of social transformation and an energy "
+"model.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gràcies per omplir el formulari.</p>\n"
-"                    <p>En cas que s’activi una Comunitat Energètica en el teu barri o municipi, podran consultar les peticions existents i posar-se en contacte amb tu. Sense cap compromís per part teva més enllà d’haver mostrat interès en impulsar un moviment de transformació social i de model energètic.</p>\n"
+"                    <p>En cas que s’activi una Comunitat Energètica en el "
+"teu barri o municipi, podran consultar les peticions existents i posar-se "
+"en contacte amb tu. Sense cap compromís per part teva més enllà d’haver "
+"mostrat interès en impulsar un moviment de transformació social i de model "
+"energètic.</p>\n"
 "                    <br />\n"
 "                    <p>Seguim en contacte per qualsevol consulta.</p>\n"
 "                    <p>Atentament,</p>\n"
 "                    <p>Equip de Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
+"                </div>\n"
+"            "
+
+#. module: energy_communities_crm
+#: model:mail.template,body_html:energy_communities_crm.email_templ_landing_coord_newsletter
+msgid ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hello,</p>\n"
+"                    <p>Thank you for filling out the form.</p>\n"
+"                    <p>We confirm that you have successfully subscribed to "
+"the newsletter.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
+"                    <br />\n"
+"                    <p>We keep in touch for any questions.</p>\n"
+"                    <p>Yours faithfully,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</a> "
+"team </p>\n"
+"                </div>\n"
+"            "
+msgstr ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hola,</p>\n"
+"                    <p>Gràcies per emplenar el formulari.</p>\n"
+"                    <p>Et confirmem que el registre a la Newsletter s'ha "
+"efectuat amb èxit.</p>\n"
+"                    <p>En el propers dies ens posarem en contacte amb tu.</"
+"p>\n"
+"                    <br />\n"
+"                    <p>Restem en contacte per qualsevol dubte.</p>\n"
+"                    <p>Atentament,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</"
+"a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_ce_news_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>You have been subscribed correctly to the Community Newsletter.</p>\n"
-"                    <p>We will notify you if there is anything new in this community.</p>\n"
+"                    <p>You have been subscribed correctly to the Community "
+"Newsletter.</p>\n"
+"                    <p>We will notify you if there is anything new in this "
+"community.</p>\n"
 "                    <br />\n"
 "                    <p>We remain in contact for any questions.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gràcies per omplir el formulari.</p>\n"
-"                    <p>Et confirmem que t’has subscrit correctament al butlletí.</p>\n"
-"                    <p>T’avisarem en cas que hi hagi alguna novetat en aquesta comunitat.</p>\n"
+"                    <p>Et confirmem que t’has subscrit correctament al "
+"butlletí.</p>\n"
+"                    <p>T’avisarem en cas que hi hagi alguna novetat en "
+"aquesta comunitat.</p>\n"
 "                    <br/>\n"
 "                    <p>Seguim en contacte per qualsevol consulta.</p>\n"
 "                    <br/>\n"
 "                    <p>Atentament,</p>\n"
 "                    <br/>\n"
 "                    <p>Equip de Som Comunitats</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_platform_news_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>You have been subscribed correctly to the Platform Newsletter.</p>\n"
-"                    <p>We'll let you know if there's any news about the project.</p>\n"
+"                    <p>You have been subscribed correctly to the Platform "
+"Newsletter.</p>\n"
+"                    <p>We'll let you know if there's any news about the "
+"project.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gràcies per omplir el formulari.</p>\n"
-"                    <p>Et confirmem que t'has subscrit correctament al butlletí.</p>\n"
-"                    <p>T'avisarem en cas que hi hagi alguna novetat en el projecte.</p>\n"
+"                    <p>Et confirmem que t'has subscrit correctament al "
+"butlletí.</p>\n"
+"                    <p>T'avisarem en cas que hi hagi alguna novetat en el "
+"projecte.</p>\n"
 "                    <br/>\n"
 "                    <p>Seguim en contacte per qualsevol consulta.</p>\n"
 "                    <br/>\n"
 "                    <p>Atentament,</p>\n"
 "                    <p>Equip de Som Comunitats</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_contact_platform_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for getting in touch.</p>\n"
-"                    <p>We have received your email. We will contact you as soon as possible.</p>\n"
+"                    <p>We have received your email. We will contact you as "
+"soon as possible.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gràcies per posar-te en contacte.</p>\n"
-"                    <p>Hem rebut el teu correu electrònic. Ens posarem en contacte amb tu tan aviat com ens sigui possible.</p>\n"
+"                    <p>Hem rebut el teu correu electrònic. Ens posarem en "
+"contacte amb tu tan aviat com ens sigui possible.</p>\n"
 "                    <br />\n"
 "                    <p>Atentament,</p>\n"
 "                    <p>Equip de Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntes freqüents</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntes freqüents</a></p>\n"
+"                </div>\n"
+"            "
+
+#. module: energy_communities_crm
+#: model:mail.template,body_html:energy_communities_crm.email_templ_landing_coord_contact
+msgid ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hello,</p>\n"
+"                    <p>Thanks for getting in touch.</p>\n"
+"                    <p>We have received your email. We will contact you as "
+"soon as possible.</p>\n"
+"                    <br />\n"
+"                    <p>Yours faithfully,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</a> "
+"team </p>\n"
+"                </div>\n"
+"            "
+msgstr ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hola,</p>\n"
+"                    <p>Gràcies per posar-te en contacte.</p>\n"
+"                    <p>Hem rebut correctament el teu correu. Contactarem "
+"amb tu al més aviat possible.</p>\n"
+"                    <br />\n"
+"                    <p>Atentament,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</"
+"a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_close_message_template
 msgid "&amp;times;"
-msgstr ""
+msgstr "&amp;times;"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ". Additional information:"
 msgstr ". Informació addicional:"
 
 #. module: energy_communities_crm
@@ -335,16 +524,16 @@
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid ""
 "Are members charged any type of recurring fee? For what concepts? How are "
 "they charged? How often?"
 msgstr ""
-"Es cobra a les sòcies algún tipos de quota recurrent? Per a quins conceptes?"
-" Com es cobren? Amb quina periodicitat?"
+"Es cobra a les sòcies algún tipos de quota recurrent? Per a quins "
+"conceptes? Com es cobren? Amb quina periodicitat?"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.view_assign_crm_to_coordinator_wizard_form
 msgid "Assign"
 msgstr "Assignar"
 
 #. module: energy_communities_crm
@@ -520,15 +709,14 @@
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__company_id
 msgid "Company"
 msgstr "Companyia"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
-#: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Constitution date"
 msgstr "Data Constitució"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
@@ -543,14 +731,19 @@
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
 msgid "Contact CE"
 msgstr "Contacte CE"
 
 #. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
+msgid "Contact COORD"
+msgstr "Contacte COORD"
+
+#. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter_platform_admins
 msgid "Contact SomComunitats"
 msgstr "Contacte SomComunitats"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
@@ -577,34 +770,36 @@
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_mapping_field__create_date
 msgid "Created on"
 msgstr "Creat el"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_assign_crm_to_coordinator_company_wizard__crm_lead_id
 msgid "Crm Lead"
-msgstr ""
+msgstr "Crm Lead"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_mapping_field__crm_lead_metadata_mapping_id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_mailing_mailing__crm_lead_metadata_mapping_id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_utm_source__crm_lead_metadata_mapping_id
 msgid "Crm Lead Metadata Mapping"
 msgstr "Metadades mapping de CRM Lead"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/models/crm_lead.py:0
 #, python-format
 msgid "Crm Lead stage {stage_name} doesn't match it's company {company_name}"
-msgstr "La etapa {stage_name} del lead no coincideix amb la companyia {company_name}"
+msgstr ""
+"La etapa {stage_name} del lead no coincideix amb la companyia {company_name}"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/models/crm_lead.py:0
 #, python-format
 msgid "Crm Lead team {team_name} doesn't match it's company {company_name}"
-msgstr "L'equip {team_name} del lead no coincideix amb la companyia {company_name}"
+msgstr ""
+"L'equip {team_name} del lead no coincideix amb la companyia {company_name}"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__ce_child_lead_id
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_crm_lead_view_form
 msgid "Crm lead child"
 msgstr "Crm lead fill"
 
@@ -682,17 +877,17 @@
 "la comptabilitat de la Comunitat Energètica? o us ho portarà una gestoria "
 "externa?"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid ""
-"Do you plan to use the platform's Odoo (management program) to carry out tax"
-" management: generation of tax reports from the Treasury (303, 390,...) or "
-"will it be carried out by an external management company?"
+"Do you plan to use the platform's Odoo (management program) to carry out "
+"tax management: generation of tax reports from the Treasury (303, 390,...) "
+"or will it be carried out by an external management company?"
 msgstr ""
 "Teniu previst usar l'Odoo (programa de gestió) de la plataforma per portar "
 "la gestió tributària: generació d'informes tributaris d'Hisenda (303, "
 "390,...) o us ho portarà una gestoria externa?"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
@@ -707,16 +902,16 @@
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid ""
 "Do you want to comment on any other particular / important aspect of your "
 "corporate management?"
 msgstr ""
-"Vols comentar algun altre aspecte particular / important de la vostre gestió"
-" societària?"
+"Vols comentar algun altre aspecte particular / important de la vostre "
+"gestió societària?"
 
 #. module: energy_communities_crm
 #: model:ir.ui.menu,name:energy_communities_crm.ce_crm_leads_ce_contact_menu
 msgid "EC Contact"
 msgstr "Contacte CE"
 
 #. module: energy_communities_crm
@@ -752,18 +947,20 @@
 #: model:ir.model.fields.selection,name:energy_communities_crm.selection__crm_tag__tag_type__energy_service
 #, python-format
 msgid "Energy Service"
 msgstr "Serveis energètics"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
-msgid "Explain the process to become cooperator. Include payment information."
+msgid ""
+"Explain, with a maximum of 500 characters, the process to become "
+"cooperator. Include payment information."
 msgstr ""
-"Explica quin és el procés que han de fer les persones que vulguin fer-se "
-"soci o sòcies. Inclou la informació sobre quotes."
+"Explica, amb un màxim de 500 caràcters, el procés d'esdevenir soci. Inclou "
+"informació de pagament."
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__external_id
 msgid "External ID"
 msgstr "ID Externa"
 
 #. module: energy_communities_crm
@@ -793,15 +990,15 @@
 #: model:ir.ui.menu,name:energy_communities_crm.ce_crm_leads_menu
 msgid "Form submissions"
 msgstr "Entrades de formulari"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.view_crm_lead_metadata_mapping_form
 msgid "General"
-msgstr ""
+msgstr "General"
 
 #. module: energy_communities_crm
 #: model:ir.actions.act_window,name:energy_communities_crm.ce_crm_leads_general_info_action
 #: model:ir.ui.menu,name:energy_communities_crm.ce_crm_leads_general_info_menu
 msgid "General Newsletter"
 msgstr "Newsletter general"
 
@@ -830,55 +1027,60 @@
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid ""
 "IBAN 2 (bank account) used by the Energy Community (only if you use more "
 "than one)"
 msgstr ""
-"IBAN 2 (compte bancari) que usa la Comunitat Energètica (només si n'useu més"
-" d'un)"
+"IBAN 2 (compte bancari) que usa la Comunitat Energètica (només si n'useu "
+"més d'un)"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_account_multicompany_easy_creation_wiz__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_assign_crm_to_coordinator_company_wizard__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_line__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_mapping__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_mapping_field__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_stage__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_team__id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_utm_source__id
 msgid "ID"
-msgstr ""
+msgstr "ID"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__tag_ext_id
 msgid "ID Ext tag"
-msgstr ""
+msgstr "ID extern d'etiqueta"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "If possible upload a group image"
 msgstr "Preferible foto de grup"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
-"In this section you can briefly explain the advantages of joining the "
-"community"
+"In this section you can, with a maximum of 500 characters, explain the "
+"advantages of joining the community"
 msgstr ""
-"En aquesta secció pots explicar quins són els avantatges per sumar-se a la "
-"Comunitat Energètica."
+"En aquesta secció pots, amb un màxim de 500 caràcters, explicar els "
+"avantatges d'unir-te a la Comunitat"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Industrial"
-msgstr ""
+msgstr "Industrial"
+
+#. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
+msgid "Info COORD"
+msgstr "Informació COORD"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Instagram url"
 msgstr "Instagram"
 
@@ -996,15 +1198,15 @@
 #, python-format
 msgid "Name"
 msgstr "Nom"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "Necessary data for the integration of the Community:"
-msgstr "dades necessàries per a la integració de la Comunitat:"
+msgstr "Dades necessàries per a la integració de la Comunitat:"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
 msgid "Newsletter CE"
 msgstr "Butlletí CE"
 
 #. module: energy_communities_crm
@@ -1012,15 +1214,15 @@
 msgid "Newsletter SomComunitats"
 msgstr "Butlletí SomComunitats"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "No"
-msgstr ""
+msgstr "No"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
 msgid "No web form origin"
 msgstr "Sense origen de formulari web"
 
 #. module: energy_communities_crm
@@ -1050,22 +1252,22 @@
 #: code:addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py:0
 #, python-format
 msgid ""
 "Opportunity assigned to Coordinator %s (ID: %s), where %s is the id of the "
 "original instance-level record."
 msgstr ""
 "Lead assignat a la coordinadora %s (ID: %s), a on %s es el id del lead "
-"original"
+"original."
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py:0
 #, python-format
 msgid ""
-"Opportunity created from Instance opportunity with ID %s, where %s is the id"
-" of the new record generated at the Coordinator level"
+"Opportunity created from Instance opportunity with ID %s, where %s is the "
+"id of the new record generated at the Coordinator level"
 msgstr ""
 "Lead creat desde la plataforma amb ID %s, a on %s es la id del nou lead "
 "generat a la coordinadora"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_stage__original_stage_id
 msgid "Original Stage"
@@ -1118,16 +1320,16 @@
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid ""
 "Predefined language for the Community (communication will be used on this "
 "language.)"
 msgstr ""
-"Idioma predeterminat de la Comunitat Energètica (totes les comunicacions que"
-" es facin desde la CE es faran per defecte en aquest idioma)"
+"Idioma predeterminat de la Comunitat Energètica (totes les comunicacions "
+"que es facin desde la CE es faran per defecte en aquest idioma)"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Primary Image"
 msgstr "Imatge primària"
 
@@ -1137,15 +1339,15 @@
 msgstr "Política de privacitat"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Public community data changed:"
 msgstr ""
-"S'han enregistrat canvis en les dades públiques de la comunitat energètica."
+"S'han enregistrat canvis en les dades públiques de la comunitat energètica:"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.view_crm_lead_metadata_mapping_form
 msgid "Recipients"
 msgstr "Destinataris"
 
 #. module: energy_communities_crm
@@ -1162,16 +1364,16 @@
 msgstr "Lead relacionat tancat."
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Related Lead not found. The url is not correct. lead_id param invalid."
 msgstr ""
-"Lead relacionat no trobat. La url no és correcta. El paràmetre lead_id no és"
-" vàlid."
+"Lead relacionat no trobat. La url no és correcta. El paràmetre lead_id no "
+"és vàlid."
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_mapping__metadata_mapping_field_ids
 msgid "Related mapping fields"
 msgstr "Camps de mapping relacionats"
 
 #. module: energy_communities_crm
@@ -1218,15 +1420,15 @@
 #, python-format
 msgid "Surnames"
 msgstr "Cognoms"
 
 #. module: energy_communities_crm
 #: model:ir.model.constraint,message:energy_communities_crm.constraint_crm_tag_name_uniq
 msgid "Tag must be unique per company!"
-msgstr "L'etiqueta ha de ser única per companyia"
+msgstr "L'etiqueta ha de ser única per companyia!"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__tag_type
 msgid "Tag type"
 msgstr "Tipus d'etiqueta"
 
 #. module: energy_communities_crm
@@ -1254,14 +1456,28 @@
 
 #. module: energy_communities_crm
 #: model:ir.model,name:energy_communities_crm.model_utm_source
 msgid "UTM Source"
 msgstr "Origen UTM"
 
 #. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
+msgid ""
+"Use a maximum of 1000 characters to write a summary of your Energy Community"
+msgstr ""
+"Usa un màxim de 1000 caràcters per escriure un resum de la teva Comunitat "
+"Energètica"
+
+#. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
+msgid "Use a maximum of 1500 characters to explain your Energy Community"
+msgstr ""
+"Usa un màxim de 1500 caràcters per explicar la teva Comunitat Energètica"
+
+#. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__user_current_company
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__user_current_company
 msgid "User Current Company"
 msgstr "Companyia actual de l'usuari"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__user_current_role
@@ -1322,27 +1538,27 @@
 #, python-format
 msgid ""
 "Who will do the day-to-day corporate management of the Energy Community? "
 "(person/s with user access to the Odoo corporate/accounting/tax management "
 "program of the Energy Community)"
 msgstr ""
 "Quí farà la gestió societària del dia a dia de la Comunitat Energètica? "
-"(persona/es amb usuari d'accés al programa Odoo de gestió "
-"societària/comptable/tributària de la Comunitat Energètica)"
+"(persona/es amb usuari d'accés al programa Odoo de gestió societària/"
+"comptable/tributària de la Comunitat Energètica)"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Why become cooperator"
 msgstr "Per què fer-se soci"
 
 #. module: energy_communities_crm
 #: model:ir.model,name:energy_communities_crm.model_account_multicompany_easy_creation_wiz
 msgid "Wizard Account Multi-company Easy Creation"
-msgstr ""
+msgstr "Wizard Account Multi-company Easy Creation"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Yes"
 msgstr "Si"
 
@@ -1353,14 +1569,24 @@
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_successful_msg
 msgid "Your data has been successfully registered."
 msgstr "Les teves dades han sigut correctament enregistrades."
 
 #. module: energy_communities_crm
+#: model:mail.template,subject:energy_communities_crm.email_templ_landing_coord_contact
+msgid "[${object.company_id.name] Contact Form"
+msgstr "[${object.company_id.name] Formulari de contacte"
+
+#. module: energy_communities_crm
+#: model:mail.template,subject:energy_communities_crm.email_templ_landing_coord_newsletter
+msgid "[${object.company_id.name] Newsletter Subscription"
+msgstr "[${object.company_id.name] Registre a la Newsletter"
+
+#. module: energy_communities_crm
 #: code:addons/energy_communities_crm/services/crm_lead_service.py:0
 #, python-format
 msgid "[Contact CE]"
 msgstr "[Contacte CE]"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/services/crm_lead_service.py:0
@@ -1490,15 +1716,16 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "ce_manager_headline"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
-"ce_manager_headline,ce_manager_firstname,ce_manager_surname,ce_manager_email,ce_manager_phone"
+"ce_manager_headline,ce_manager_firstname,ce_manager_surname,"
+"ce_manager_email,ce_manager_phone"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model:ir.model,name:energy_communities_crm.model_crm_lead_metadata_line
 msgid "crm.lead.metadata.line"
 msgstr ""
 
@@ -1524,15 +1751,15 @@
 msgstr "lead_id a l'URL del lloc web"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "lead_id param must be defined on the url in order to use the form"
 msgstr ""
-"El paràmetre lead_id s'ha de definir a l'URL per poder utilitzar el "
+"el paràmetre lead_id s'ha de definir a l'URL per poder utilitzar el "
 "formulari"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "somenergia@delegado-datos.com"
 msgstr ""
 
@@ -1540,15 +1767,15 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "suport@somcomunitats.coop"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline
 msgid "to the <strong>public spaces</strong> of our"
-msgstr "als <strong>espais públics</strong> de la "
+msgstr "als <strong>espais públics</strong> de la"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid ""
 "to the technology platform Som Comunitats has been successfully submitted."
 msgstr ""
 "a la plataforma tecnològica de Som Comunitats ha sigut enviada amb èxit."
```

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/i18n/es.po` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/i18n/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,300 +2,479 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities_crm
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-26 12:57+0000\n"
-"PO-Revision-Date: 2024-03-26 12:57+0000\n"
+"POT-Creation-Date: 2024-05-31 14:39+0000\n"
+"PO-Revision-Date: 2024-05-31 16:56+0200\n"
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
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_assigned_to_coordinator_id
 msgid ""
 "\n"
 "                \n"
-"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, "
+"Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); "
+"background-color: #FFF; \">\n"
 "                        <p>Hello,</p><br/>\n"
-"                        <p>There is a new Energy Community registration request.</p>\n"
+"                        <p>There is a new Energy Community registration "
+"request.</p>\n"
 "                        <p>Go to Odoo to track this registration.</p><br/>\n"
 "                        <p>Yours faithfully,</p>\n"
 "                        <p>Somcomunitats.coop team</p>\n"
-"                        <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                        <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                    </div>\n"
 "                \n"
 "            "
 msgstr ""
 "\n"
 "                \n"
-"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, "
+"Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); "
+"background-color: #FFF; \">\n"
 "\n"
 "                        <p>Hola,</p>\n"
 "\n"
-"                        <p>Hay una nueva solicitud de alta de Comunidad Energética.</p>\n"
+"                        <p>Hay una nueva solicitud de alta de Comunidad "
+"Energética.</p>\n"
 "\n"
 "                        <p>Ve a Odoo a hacer seguimiento de esta alta.</p>\n"
 "\n"
 "                        <p>Atentamente,</p>\n"
 "                        <p>Equipo de Somcomunitats.coop</p>\n"
-"                        <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                        <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
 "\n"
 "                    </div>\n"
 "                \n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_contact_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for contact.</p>\n"
-"                    <p>We have received your email and we have we have forwarded it to the Community so that they can contact you as soon as possible.</p>\n"
+"                    <p>We have received your email and we have we have "
+"forwarded it to the Community so that they can contact you as soon as "
+"possible.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gracias por ponerte en contacto.</p>\n"
-"                    <p>Hemos recibido tu correo electrónico y le hemos hecho llegar a la Comunidad Energética para que se pongan en contacto contigo lo antes posible.</p>\n"
+"                    <p>Hemos recibido tu correo electrónico y le hemos "
+"hecho llegar a la Comunidad Energética para que se pongan en contacto "
+"contigo lo antes posible.</p>\n"
 "                    <br />\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somos Comunidades</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_creation_receipt_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form and requesting the membership of your Energy Community on the Somcomunitats.coop platform.</p>\n"
-"                    <p>In the coming weeks we will study the application and contact you to indicate the steps and the information necessary to complete the registration process for the Community and the people who are part of it.</p>\n"
+"                    <p>Thank you for filling out the form and requesting "
+"the membership of your Energy Community on the Somcomunitats.coop platform."
+"</p>\n"
+"                    <p>In the coming weeks we will study the application "
+"and contact you to indicate the steps and the information necessary to "
+"complete the registration process for the Community and the people who are "
+"part of it.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
 "\n"
-"                    <p>Hola,</p>\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "\n"
-"                    <p>Gracias por rellenar el formulario y solicitar la  adhesión de vuestra Comunidad Energética a la plataforma Som Comunitats.</p>\n"
+"                    <p>Hola,</p>\n"
 "\n"
-"                    <p>Durante los próximos días estudiaremos la solicitud y nos pondremos en contacto con vosotros para indicarle los pasos y la información necesaria para acabar el proceso de alta de la Comunidad y de las personas que forman parte de ella.</p>\n"
+"                    <p>Gracias por rellenar el formulario y solicitar la  "
+"adhesión de vuestra Comunidad Energética a la plataforma Som Comunitats.</"
+"p>\n"
+"\n"
+"                    <p>Durante los próximos días estudiaremos la solicitud "
+"y nos pondremos en contacto con vosotros para indicarle los pasos y la "
+"información necesaria para acabar el proceso de alta de la Comunidad y de "
+"las personas que forman parte de ella.</p>\n"
 "\n"
 "                    <br />\n"
 "                    <p>Seguimos en contacto para cualquier duda.</p>\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somos Comunidades</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
 "\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_source_coord_web_other_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form to request contact regarding the Coordinators.</p>\n"
+"                    <p>Thank you for filling out the form to request "
+"contact regarding the Coordinators.</p>\n"
 "                    <p>We have successfully received your details.</p>\n"
-"                    <p>Over the next few days we will study the request and get in touch with you.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
-"                    <p>Gracias por rellenar el formulario para pedir información en relación a las Coordinadoras.</p>\n"
+"                    <p>Gracias por rellenar el formulario para pedir "
+"información en relación a las Coordinadoras.</p>\n"
 "                    <p>Hemos recibido correctamente tus datos</p>\n"
-"                    <p>Durante los próximos días estudiaremos la solicitud y nos pondremos en contacto con usted.</p>\n"
+"                    <p>Durante los próximos días estudiaremos la solicitud "
+"y nos pondremos en contacto con usted.</p>\n"
 "                    <br />\n"
 "                    <p>Seguimos en contacto para cualquier consulta.</p>\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_source_coord_web_hiring_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form to request the hiring of a Coordinator.</p>\n"
+"                    <p>Thank you for filling out the form to request the "
+"hiring of a Coordinator.</p>\n"
 "                    <p>We have successfully received your details</p>\n"
-"                    <p>Over the next few days we will study the request and get in touch with you.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
-"                    <p>Gracias por rellenar el formulario para pedir la contratación de una Coordinadora.</p>\n"
+"                    <p>Gracias por rellenar el formulario para pedir la "
+"contratación de una Coordinadora.</p>\n"
 "                    <p>Hemos recibido correctamente tus datos</p>\n"
-"                    <p>Durante los próximos días estudiaremos la solicitud y nos pondremos en contacto con usted.</p>\n"
+"                    <p>Durante los próximos días estudiaremos la solicitud "
+"y nos pondremos en contacto con usted.</p>\n"
 "                    <br />\n"
 "                    <p>Seguimos en contacto para cualquier consulta.</p>\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_advise_future_ce_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>In case an Energy Community is activated in your neighborhood or municipality, they can consult the existing requests and contact you. Without any commitment on your part beyond having shown interest in promoting a movement of social transformation and an energy model.</p>\n"
+"                    <p>In case an Energy Community is activated in your "
+"neighborhood or municipality, they can consult the existing requests and "
+"contact you. Without any commitment on your part beyond having shown "
+"interest in promoting a movement of social transformation and an energy "
+"model.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gracias por completar el formulario.</p>\n"
-"                    <p>En caso de que se active una Comunidad Energética en tu barrio o municipio, podrán consultar las solicitudes existentes y ponerse en contacto contigo. Sin ningún compromiso por su parte más allá de haber mostrado interés en impulsar un movimiento de transformación social y un modelo energético.</p>\n"
+"                    <p>En caso de que se active una Comunidad Energética en "
+"tu barrio o municipio, podrán consultar las solicitudes existentes y "
+"ponerse en contacto contigo. Sin ningún compromiso por su parte más allá de "
+"haber mostrado interés en impulsar un movimiento de transformación social y "
+"un modelo energético.</p>\n"
 "                    <br />\n"
 "                    <p>Seguimos en contacto para cualquier consulta.</p>\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
+"                </div>\n"
+"            "
+
+#. module: energy_communities_crm
+#: model:mail.template,body_html:energy_communities_crm.email_templ_landing_coord_newsletter
+msgid ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hello,</p>\n"
+"                    <p>Thank you for filling out the form.</p>\n"
+"                    <p>We confirm that you have successfully subscribed to "
+"the newsletter.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
+"                    <br />\n"
+"                    <p>We keep in touch for any questions.</p>\n"
+"                    <p>Yours faithfully,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</a> "
+"team </p>\n"
+"                </div>\n"
+"            "
+msgstr ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hola,</p>\n"
+"                    <p>Gracias por rellenar el formulario.</p>\n"
+"                    <p>Te confirmamos que el registro a la Newsletter se ha "
+"efectuado con éxito.</p>\n"
+"\n"
+"                    <p>En los próximos dias nos pondremos en contacto.</p>\n"
+"                    <br />\n"
+"                    <p>We keep in touch for any questions.</p>\n"
+"                    <p>Restamos en contacto para cualquier consulta.</p>\n"
+"                    <p>Atentamente,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</"
+"a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_ce_news_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>You have been subscribed correctly to the Community Newsletter.</p>\n"
-"                    <p>We will notify you if there is anything new in this community.</p>\n"
+"                    <p>You have been subscribed correctly to the Community "
+"Newsletter.</p>\n"
+"                    <p>We will notify you if there is anything new in this "
+"community.</p>\n"
 "                    <br />\n"
 "                    <p>We remain in contact for any questions.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gracias por rellenar el formulario.</p>\n"
-"                    <p>Te confirmamos que te has suscrito correctamente al boletín.</p>\n"
-"                    <p>Te avisaremos en caso que haya alguna novedad en esta comunidad.</p>\n"
+"                    <p>Te confirmamos que te has suscrito correctamente al "
+"boletín.</p>\n"
+"                    <p>Te avisaremos en caso que haya alguna novedad en "
+"esta comunidad.</p>\n"
 "                    <br/>\n"
 "                    <p>Seguimos en contacto para cualquier consulta.</p>\n"
 "                    <br/>\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somos Comunidades</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_platform_news_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>You have been subscribed correctly to the Platform Newsletter.</p>\n"
-"                    <p>We'll let you know if there's any news about the project.</p>\n"
+"                    <p>You have been subscribed correctly to the Platform "
+"Newsletter.</p>\n"
+"                    <p>We'll let you know if there's any news about the "
+"project.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gracias por rellenar el formulario.</p>\n"
-"                    <p>Te confirmamos que te has suscrito correctamente en el boletín.</p>\n"
-"                    <p>Te avisaremos en caso de que haya alguna novedad en el proyecto.</p>\n"
+"                    <p>Te confirmamos que te has suscrito correctamente en "
+"el boletín.</p>\n"
+"                    <p>Te avisaremos en caso de que haya alguna novedad en "
+"el proyecto.</p>\n"
 "                    <br/>\n"
 "                    <p>Seguimos en contacto para cualquier consulta.</p>\n"
 "                    <br/>\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somos Comunidades</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos y preguntas frecuentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos y preguntas frecuentes</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_contact_platform_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for getting in touch.</p>\n"
-"                    <p>We have received your email. We will contact you as soon as possible.</p>\n"
+"                    <p>We have received your email. We will contact you as "
+"soon as possible.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hola,</p>\n"
 "                    <p>Gracias por ponerte en contacto.</p>\n"
-"                    <p>Hemos recibido tu correo electrónico. Nos pondremos en contacto contigo lo antes possible.</p>\n"
+"                    <p>Hemos recibido tu correo electrónico. Nos pondremos "
+"en contacto contigo lo antes possible.</p>\n"
 "                    <br />\n"
 "                    <p>Atentamente,</p>\n"
 "                    <p>Equipo de Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Recursos i preguntas frequentes</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Recursos i preguntas frequentes</a></p>\n"
+"                </div>\n"
+"            "
+
+#. module: energy_communities_crm
+#: model:mail.template,body_html:energy_communities_crm.email_templ_landing_coord_contact
+msgid ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hello,</p>\n"
+"                    <p>Thanks for getting in touch.</p>\n"
+"                    <p>We have received your email. We will contact you as "
+"soon as possible.</p>\n"
+"                    <br />\n"
+"                    <p>Yours faithfully,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</a> "
+"team </p>\n"
+"                </div>\n"
+"            "
+msgstr ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hola,</p>\n"
+"                    <p>Gracias por ponerte en contacto.</p>\n"
+"                    <p>Hemos recibido tu correo y nos pondremos en contacto "
+"lo antes posible.</p>\n"
+"                    <br />\n"
+"                    <p>Atentamente,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</"
+"a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_close_message_template
 msgid "&amp;times;"
-msgstr ""
+msgstr "&amp;times;"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ". Additional information:"
 msgstr ". Información adicional:"
 
 #. module: energy_communities_crm
@@ -517,15 +696,14 @@
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__company_id
 msgid "Company"
 msgstr "Compañía"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
-#: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Constitution date"
 msgstr "Fecha de constitución"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
@@ -540,14 +718,19 @@
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
 msgid "Contact CE"
 msgstr "Contacto CE"
 
 #. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
+msgid "Contact COORD"
+msgstr "Contacto COORD"
+
+#. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter_platform_admins
 msgid "Contact SomComunitats"
 msgstr "Contacto SomComunitats"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
@@ -574,34 +757,36 @@
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_mapping_field__create_date
 msgid "Created on"
 msgstr "Creado el"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_assign_crm_to_coordinator_company_wizard__crm_lead_id
 msgid "Crm Lead"
-msgstr ""
+msgstr "Crm Lead"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead_metadata_mapping_field__crm_lead_metadata_mapping_id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_mailing_mailing__crm_lead_metadata_mapping_id
 #: model:ir.model.fields,field_description:energy_communities_crm.field_utm_source__crm_lead_metadata_mapping_id
 msgid "Crm Lead Metadata Mapping"
 msgstr "Mapping de metadatos en CRM Lead"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/models/crm_lead.py:0
 #, python-format
 msgid "Crm Lead stage {stage_name} doesn't match it's company {company_name}"
-msgstr "La etapa {stage_name} del lead no coincide con la compañía {company_name}"
+msgstr ""
+"La etapa {stage_name} del lead no coincide con la compañía {company_name}"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/models/crm_lead.py:0
 #, python-format
 msgid "Crm Lead team {team_name} doesn't match it's company {company_name}"
-msgstr "EL equipo {team_name} del lead no coincide con la compañía {company_name}"
+msgstr ""
+"EL equipo {team_name} del lead no coincide con la compañía {company_name}"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__ce_child_lead_id
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_crm_lead_view_form
 msgid "Crm lead child"
 msgstr "Crm lead hijo"
 
@@ -680,17 +865,17 @@
 "llevar¿la contabilidad de la Comunidad Energética? o se lo llevará una "
 "gestoríaexterna?"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid ""
-"Do you plan to use the platform's Odoo (management program) to carry out tax"
-" management: generation of tax reports from the Treasury (303, 390,...) or "
-"will it be carried out by an external management company?"
+"Do you plan to use the platform's Odoo (management program) to carry out "
+"tax management: generation of tax reports from the Treasury (303, 390,...) "
+"or will it be carried out by an external management company?"
 msgstr ""
 "Tiene previsto usar el Odoo (programa de gestión) de la plataforma para "
 "llevarla gestión tributaria: generación de informes tributarios de Hacienda "
 "(303, 390,...) ¿o se lo llevará una gestoría externa?"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
@@ -750,18 +935,20 @@
 #: model:ir.model.fields.selection,name:energy_communities_crm.selection__crm_tag__tag_type__energy_service
 #, python-format
 msgid "Energy Service"
 msgstr "Servicios energéticos"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
-msgid "Explain the process to become cooperator. Include payment information."
+msgid ""
+"Explain, with a maximum of 500 characters, the process to become "
+"cooperator. Include payment information."
 msgstr ""
-"Explica cuál es el proceso que deben hacer las personas que quieran hacerse "
-"socio o socias. Incluye la información sobre cuotas."
+"Explica, en un màximo de 500 carácteres, el proceso de covertirse en Socio/"
+"a de la Comunidad. Incluye la información sobre el pago."
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__external_id
 msgid "External ID"
 msgstr "ID Externo"
 
 #. module: energy_communities_crm
@@ -791,15 +978,15 @@
 #: model:ir.ui.menu,name:energy_communities_crm.ce_crm_leads_menu
 msgid "Form submissions"
 msgstr "Entradas de formulario"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.view_crm_lead_metadata_mapping_form
 msgid "General"
-msgstr ""
+msgstr "General"
 
 #. module: energy_communities_crm
 #: model:ir.actions.act_window,name:energy_communities_crm.ce_crm_leads_general_info_action
 #: model:ir.ui.menu,name:energy_communities_crm.ce_crm_leads_general_info_menu
 msgid "General Newsletter"
 msgstr "Newsletter general"
 
@@ -848,35 +1035,40 @@
 #: model:ir.model.fields,field_description:energy_communities_crm.field_utm_source__id
 msgid "ID"
 msgstr "Identificador"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__tag_ext_id
 msgid "ID Ext tag"
-msgstr ""
+msgstr "ID externa de la etiqueta"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "If possible upload a group image"
 msgstr "Preferible foto de grupo"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
-"In this section you can briefly explain the advantages of joining the "
-"community"
+"In this section you can, with a maximum of 500 characters, explain the "
+"advantages of joining the community"
 msgstr ""
-"En esta sección puedes explicar cuáles son las ventajas para sumarse a la "
-"Comunidad Energética."
+"En la sección puedes, en un máximo de 500 carácteres. explicar las ventajas "
+"de unirse a la comunidad"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Industrial"
-msgstr ""
+msgstr "Industrial"
+
+#. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
+msgid "Info COORD"
+msgstr "Información COORD"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Instagram url"
 msgstr "Instagram"
 
@@ -1012,15 +1204,15 @@
 msgid "Newsletter SomComunitats"
 msgstr "Boletín SomComunitats"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "No"
-msgstr ""
+msgstr "No"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
 msgid "No web form origin"
 msgstr "Sin origen del formulario web"
 
 #. module: energy_communities_crm
@@ -1050,22 +1242,22 @@
 #: code:addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py:0
 #, python-format
 msgid ""
 "Opportunity assigned to Coordinator %s (ID: %s), where %s is the id of the "
 "original instance-level record."
 msgstr ""
 "Lead asignado a la coordinadora %s (ID: %s), donde %s es la id del lead "
-"original"
+"original."
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py:0
 #, python-format
 msgid ""
-"Opportunity created from Instance opportunity with ID %s, where %s is the id"
-" of the new record generated at the Coordinator level"
+"Opportunity created from Instance opportunity with ID %s, where %s is the "
+"id of the new record generated at the Coordinator level"
 msgstr ""
 "Lead creado desde el lead de la plataforma con ID %s, donde %s es la id del "
 "nuevo lead generado en la coordinadora"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_stage__original_stage_id
 msgid "Original Stage"
@@ -1137,15 +1329,15 @@
 msgstr "Política de privacidad"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Public community data changed:"
 msgstr ""
-"Se han registrado cambios en los datos públicos de la comunidad energética."
+"Se han registrado cambios en los datos públicos de la comunidad energética:"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.view_crm_lead_metadata_mapping_form
 msgid "Recipients"
 msgstr "Destinatarios"
 
 #. module: energy_communities_crm
@@ -1155,15 +1347,15 @@
 msgid "Regular"
 msgstr "Standard"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Related Lead closed."
-msgstr "Lead relacionado cerrado"
+msgstr "Lead relacionado cerrado."
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Related Lead not found. The url is not correct. lead_id param invalid."
 msgstr ""
 "Lead relacionado no encontrado. La url no es correcta. El parámetro lead_id "
@@ -1218,15 +1410,15 @@
 #, python-format
 msgid "Surnames"
 msgstr "Apellidos"
 
 #. module: energy_communities_crm
 #: model:ir.model.constraint,message:energy_communities_crm.constraint_crm_tag_name_uniq
 msgid "Tag must be unique per company!"
-msgstr "La etiqueta debe ser única por compañía"
+msgstr "La etiqueta debe ser única por compañía!"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__tag_type
 msgid "Tag type"
 msgstr "Tipo de etiqueta"
 
 #. module: energy_communities_crm
@@ -1255,14 +1447,28 @@
 
 #. module: energy_communities_crm
 #: model:ir.model,name:energy_communities_crm.model_utm_source
 msgid "UTM Source"
 msgstr "Origen UTM"
 
 #. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
+msgid ""
+"Use a maximum of 1000 characters to write a summary of your Energy Community"
+msgstr ""
+"Usa un màximo de 1000 carácteres para escribir un resumen de tu Comunidad "
+"Energética"
+
+#. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
+msgid "Use a maximum of 1500 characters to explain your Energy Community"
+msgstr ""
+"Usa un máximo de 1500 carácteres para explicar tu Comunidad Energética"
+
+#. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__user_current_company
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__user_current_company
 msgid "User Current Company"
 msgstr "Compañía actual del usuario"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__user_current_role
@@ -1323,16 +1529,16 @@
 #, python-format
 msgid ""
 "Who will do the day-to-day corporate management of the Energy Community? "
 "(person/s with user access to the Odoo corporate/accounting/tax management "
 "program of the Energy Community)"
 msgstr ""
 "¿Quién hará la gestión societaria del día a día de la Comunidad Energética? "
-"(persona/s con usuario de acceso al programa Odoo de gestión "
-"societaria/contable/tributaria de la Comunidad Energética)"
+"(persona/s con usuario de acceso al programa Odoo de gestión societaria/"
+"contable/tributaria de la Comunidad Energética)"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Why become cooperator"
 msgstr "Por qué hacerse socio"
 
@@ -1351,15 +1557,25 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "You can contact"
 msgstr "Puedes contactar"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_successful_msg
 msgid "Your data has been successfully registered."
-msgstr "Tus datos se han registrado con éxito"
+msgstr "Tus datos se han registrado con éxito."
+
+#. module: energy_communities_crm
+#: model:mail.template,subject:energy_communities_crm.email_templ_landing_coord_contact
+msgid "[${object.company_id.name] Contact Form"
+msgstr "[${object.company_id.name] Formulario de contacto"
+
+#. module: energy_communities_crm
+#: model:mail.template,subject:energy_communities_crm.email_templ_landing_coord_newsletter
+msgid "[${object.company_id.name] Newsletter Subscription"
+msgstr "[${object.company_id.name] Registro a la Newsletter"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/services/crm_lead_service.py:0
 #, python-format
 msgid "[Contact CE]"
 msgstr "[Contacto CE]"
 
@@ -1451,16 +1667,16 @@
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline
 msgid ""
 "and to our <strong>administrative management space</strong> (Odoo program "
 "for corporate, accounting and financial management)"
 msgstr ""
-"y en <strong>el espacio de gestión administrativa</strong> (programa Odoo de"
-" gestión societaria, contable y financiera)."
+"y en <strong>el espacio de gestión administrativa</strong> (programa Odoo "
+"de gestión societaria, contable y financiera)."
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "ce_account_management,ce_tax_management:external_management"
 msgstr ""
 
 #. module: energy_communities_crm
@@ -1492,15 +1708,16 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "ce_manager_headline"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
-"ce_manager_headline,ce_manager_firstname,ce_manager_surname,ce_manager_email,ce_manager_phone"
+"ce_manager_headline,ce_manager_firstname,ce_manager_surname,"
+"ce_manager_email,ce_manager_phone"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model:ir.model,name:energy_communities_crm.model_crm_lead_metadata_line
 msgid "crm.lead.metadata.line"
 msgstr ""
 
@@ -1513,15 +1730,15 @@
 #: model:ir.model,name:energy_communities_crm.model_crm_lead_metadata_mapping_field
 msgid "crm.lead.metadata.mapping.field"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "for further assistance."
-msgstr "si necessitas cualquier aclaración al respecto"
+msgstr "si necessitas cualquier aclaración al respecto."
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "lead_id on website url"
 msgstr "lead_id en la url web"
 
@@ -1540,15 +1757,15 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "suport@somcomunitats.coop"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline
 msgid "to the <strong>public spaces</strong> of our"
-msgstr "en los <strong>espacios públicos</strong> de la "
+msgstr "en los <strong>espacios públicos</strong> de la"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid ""
 "to the technology platform Som Comunitats has been successfully submitted."
 msgstr ""
 "a la plataforma tecnológica Som Comunitats han sido enviados con éxito."
```

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/i18n/eu_ES.po` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/i18n/eu_ES.po`

 * *Files 9% similar despite different names*

```diff
@@ -2,296 +2,476 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities_crm
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-26 12:56+0000\n"
-"PO-Revision-Date: 2024-03-26 12:56+0000\n"
+"POT-Creation-Date: 2024-05-31 14:39+0000\n"
+"PO-Revision-Date: 2024-05-31 17:14+0200\n"
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
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_assigned_to_coordinator_id
 msgid ""
 "\n"
 "                \n"
-"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, "
+"Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); "
+"background-color: #FFF; \">\n"
 "                        <p>Hello,</p><br/>\n"
-"                        <p>There is a new Energy Community registration request.</p>\n"
+"                        <p>There is a new Energy Community registration "
+"request.</p>\n"
 "                        <p>Go to Odoo to track this registration.</p><br/>\n"
 "                        <p>Yours faithfully,</p>\n"
 "                        <p>Somcomunitats.coop team</p>\n"
-"                        <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                        <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                    </div>\n"
 "                \n"
 "            "
 msgstr ""
 "\n"
 "                \n"
-"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                    <div style=\"font-family: 'Lucica Grande', Ubuntu, "
+"Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); "
+"background-color: #FFF; \">\n"
 "\n"
 "                        <p>Kaixo,</p>\n"
 "\n"
-"                        <p>Comunidad Energétican izena emateko eskaera berri bat dago.</p>\n"
+"                        <p>Comunidad Energétican izena emateko eskaera "
+"berri bat dago.</p>\n"
 "\n"
-"                        <p>Zoaz Odoo erregistro honi jarraipena emateko.</p>\n"
+"                        <p>Zoaz Odoo erregistro honi jarraipena emateko.</"
+"p>\n"
 "\n"
 "                        <p>Zinez,</p>\n"
 "                        <p>Taldea Somcomunitats.coop</p>\n"
-"                        <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                        <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
 "\n"
 "                    </div>\n"
 "                \n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_contact_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for contact.</p>\n"
-"                    <p>We have received your email and we have we have forwarded it to the Community so that they can contact you as soon as possible.</p>\n"
+"                    <p>We have received your email and we have we have "
+"forwarded it to the Community so that they can contact you as soon as "
+"possible.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Kaixo,</p>\n"
 "                    <p>Eskerrik asko harremanetan jartzeagatik.</p>\n"
-"                    <p>Zure e-posta jaso dugu eta Komunitateari birbidali diogu, ahalik eta azkarren zurekin harremanetan jartzeko.</p>\n"
+"                    <p>Zure e-posta jaso dugu eta Komunitateari birbidali "
+"diogu, ahalik eta azkarren zurekin harremanetan jartzeko.</p>\n"
 "                    <br />\n"
-"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara.</p>\n"
+"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara."
+"</p>\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_creation_receipt_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form and requesting the membership of your Energy Community on the Somcomunitats.coop platform.</p>\n"
-"                    <p>In the coming weeks we will study the application and contact you to indicate the steps and the information necessary to complete the registration process for the Community and the people who are part of it.</p>\n"
+"                    <p>Thank you for filling out the form and requesting "
+"the membership of your Energy Community on the Somcomunitats.coop platform."
+"</p>\n"
+"                    <p>In the coming weeks we will study the application "
+"and contact you to indicate the steps and the information necessary to "
+"complete the registration process for the Community and the people who are "
+"part of it.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
 "\n"
-"                    <p>Kaixo,</p>\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "\n"
-"                    <p>Eskerrik asko formularioa bete eta Somcomunitats.coop plataforman zure Energia Komunitatearen kide izatea eskatzeagatik.</p>\n"
+"                    <p>Kaixo,</p>\n"
 "\n"
-"                    <p>Datozen asteetan aplikazioa aztertuko dugu eta zurekin harremanetan jarriko gara Komunitatearen eta bertan dauden pertsonen erregistro-prozesua burutzeko beharrezkoak diren urratsak eta informazioa adierazteko.</p>\n"
+"                    <p>Eskerrik asko formularioa bete eta Somcomunitats."
+"coop plataforman zure Energia Komunitatearen kide izatea eskatzeagatik.</"
+"p>\n"
+"\n"
+"                    <p>Datozen asteetan aplikazioa aztertuko dugu eta "
+"zurekin harremanetan jarriko gara Komunitatearen eta bertan dauden "
+"pertsonen erregistro-prozesua burutzeko beharrezkoak diren urratsak eta "
+"informazioa adierazteko.</p>\n"
 "\n"
 "                    <br />\n"
-"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara.</p>\n"
+"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara."
+"</p>\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
 "\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_source_coord_web_other_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form to request contact regarding the Coordinators.</p>\n"
+"                    <p>Thank you for filling out the form to request "
+"contact regarding the Coordinators.</p>\n"
 "                    <p>We have successfully received your details.</p>\n"
-"                    <p>Over the next few days we will study the request and get in touch with you.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Kaixo,</p>\n"
-"                    <p>Eskerrik asko formularioa betetzeagatik, Koordinatzaileekin harremanetan jartzeko.</p>\n"
+"                    <p>Eskerrik asko formularioa betetzeagatik, "
+"Koordinatzaileekin harremanetan jartzeko.</p>\n"
 "                    <p>Zuzen jaso ditugu zure datuak</p>\n"
-"                    <p>Hurrengo egunetan eskaera aztertuko dugu eta zurekin harremanetan jarriko gara.</p>\n"
+"                    <p>Hurrengo egunetan eskaera aztertuko dugu eta zurekin "
+"harremanetan jarriko gara.</p>\n"
 "                    <br />\n"
-"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara.</p>\n"
+"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara."
+"</p>\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_ce_source_coord_web_hiring_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
-"                    <p>Thank you for filling out the form to request the hiring of a Coordinator.</p>\n"
+"                    <p>Thank you for filling out the form to request the "
+"hiring of a Coordinator.</p>\n"
 "                    <p>We have successfully received your details</p>\n"
-"                    <p>Over the next few days we will study the request and get in touch with you.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Kaixo,</p>\n"
-"                    <p>Eskerrik asko Koordinatzaile baten kontratazioa eskatzeko formularioa betetzeagatik.</p>\n"
+"                    <p>Eskerrik asko Koordinatzaile baten kontratazioa "
+"eskatzeko formularioa betetzeagatik.</p>\n"
 "                    <p>Zuzen jaso ditugu zure datuak</p>\n"
-"                    <p>Hurrengo egunetan eskaera aztertuko dugu eta zurekin harremanetan jarriko gara.</p>\n"
+"                    <p>Hurrengo egunetan eskaera aztertuko dugu eta zurekin "
+"harremanetan jarriko gara.</p>\n"
 "                    <br />\n"
-"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara.</p>\n"
+"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara."
+"</p>\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_advise_future_ce_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>In case an Energy Community is activated in your neighborhood or municipality, they can consult the existing requests and contact you. Without any commitment on your part beyond having shown interest in promoting a movement of social transformation and an energy model.</p>\n"
+"                    <p>In case an Energy Community is activated in your "
+"neighborhood or municipality, they can consult the existing requests and "
+"contact you. Without any commitment on your part beyond having shown "
+"interest in promoting a movement of social transformation and an energy "
+"model.</p>\n"
 "                    <br />\n"
 "                    <p>We keep in touch for any questions.</p>\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Kaixo,</p>\n"
 "                    <p>Eskerrik asko formularioa betetzeagatik.</p>\n"
-"                    <p>Zure auzoan edo udalerrian Energia Komunitate bat aktibatzen bada, dauden eskaerak kontsultatu eta zurekin harremanetan jartzeko aukera izango dute. Gizarte eraldaketarako mugimendua eta eredu energetikoa sustatzeko interesa agertu izanaz haratago euren aldetik inolako konpromisorik gabe.</p>\n"
+"                    <p>Zure auzoan edo udalerrian Energia Komunitate bat "
+"aktibatzen bada, dauden eskaerak kontsultatu eta zurekin harremanetan "
+"jartzeko aukera izango dute. Gizarte eraldaketarako mugimendua eta eredu "
+"energetikoa sustatzeko interesa agertu izanaz haratago euren aldetik "
+"inolako konpromisorik gabe.</p>\n"
 "                    <br />\n"
-"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara.</p>\n"
+"                    <p>Edozein zalantza argitzeko harremanetan jartzen gara."
+"</p>\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
+"                </div>\n"
+"            "
+
+#. module: energy_communities_crm
+#: model:mail.template,body_html:energy_communities_crm.email_templ_landing_coord_newsletter
+msgid ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hello,</p>\n"
+"                    <p>Thank you for filling out the form.</p>\n"
+"                    <p>We confirm that you have successfully subscribed to "
+"the newsletter.</p>\n"
+"                    <p>Over the next few days we will study the request and "
+"get in touch with you.</p>\n"
+"                    <br />\n"
+"                    <p>We keep in touch for any questions.</p>\n"
+"                    <p>Yours faithfully,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</a> "
+"team </p>\n"
+"                </div>\n"
+"            "
+msgstr ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hola,</p>\n"
+"                    <p>Gracias por rellenar el formulario.</p>\n"
+"                    <p>Te confirmamos que el registro a la Newsletter se ha "
+"efectuado con éxito.</p>\n"
+"                    <p>En los próximos dias nos pondremos en contacto.</p>\n"
+"                    <br />\n"
+"                    <p>Restamos en contacto para cualquier consulta.</p>\n"
+"                    <p>Atentamente,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</"
+"a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_ce_news_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>You have been subscribed correctly to the Community Newsletter.</p>\n"
-"                    <p>We will notify you if there is anything new in this community.</p>\n"
+"                    <p>You have been subscribed correctly to the Community "
+"Newsletter.</p>\n"
+"                    <p>We will notify you if there is anything new in this "
+"community.</p>\n"
 "                    <br />\n"
 "                    <p>We remain in contact for any questions.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Kaixo,</p>\n"
 "                    <p>Eskerrik asko formularioa betetzeagatik.</p>\n"
-"                    <p>Behar bezala harpidetu zara Komunitatearen buletinera.</p>\n"
+"                    <p>Behar bezala harpidetu zara Komunitatearen "
+"buletinera.</p>\n"
 "                    <br />\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_lead_request_platform_news_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for filling out the form.</p>\n"
-"                    <p>You have been subscribed correctly to the Platform Newsletter.</p>\n"
-"                    <p>We'll let you know if there's any news about the project.</p>\n"
+"                    <p>You have been subscribed correctly to the Platform "
+"Newsletter.</p>\n"
+"                    <p>We'll let you know if there's any news about the "
+"project.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Kaixo,</p>\n"
 "                    <p>Eskerrik asko formularioa betetzeagatik.</p>\n"
 "                    <p>Buletinera ondo harpidetu zara.</p>\n"
-"                    <p>Proiektuari buruzko edozein berriren berri emango dizuegu.</p>\n"
+"                    <p>Proiektuari buruzko edozein berriren berri emango "
+"dizuegu.</p>\n"
 "                    <br />\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model:mail.template,body_html:energy_communities_crm.email_templ_contact_platform_confirm_id
 msgid ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Hello,</p>\n"
 "                    <p>Thank you for getting in touch.</p>\n"
-"                    <p>We have received your email. We will contact you as soon as possible.</p>\n"
+"                    <p>We have received your email. We will contact you as "
+"soon as possible.</p>\n"
 "                    <br />\n"
 "                    <p>Yours faithfully,</p>\n"
 "                    <p>Somcomunitats.coop team </p>\n"
-"                    <p><a href=\"https://somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/recursos/"
+"\">Resources and FAQs</a></p>\n"
 "                </div>\n"
 "            "
 msgstr ""
 "\n"
-"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
 "                    <p>Kaixo,</p>\n"
 "                    <p>Eskerrik asko harremanetan jartzeagatik.</p>\n"
-"                    <p>Zure emaila jaso dugu. Ahalik eta azkarren zurekin harremanetan jarriko gara.</p>\n"
+"                    <p>Zure emaila jaso dugu. Ahalik eta azkarren zurekin "
+"harremanetan jarriko gara.</p>\n"
 "                    <br />\n"
 "                    <p>Zinez,</p>\n"
 "                    <p>Taldea Somcomunitats.coop</p>\n"
-"                    <p><a href=\"https://omcomunitats.coop/recursos/\">Baliabideak eta ohiko galderak</a></p>\n"
+"                    <p><a href=\"https://omcomunitats.coop/recursos/"
+"\">Baliabideak eta ohiko galderak</a></p>\n"
+"                </div>\n"
+"            "
+
+#. module: energy_communities_crm
+#: model:mail.template,body_html:energy_communities_crm.email_templ_landing_coord_contact
+msgid ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hello,</p>\n"
+"                    <p>Thanks for getting in touch.</p>\n"
+"                    <p>We have received your email. We will contact you as "
+"soon as possible.</p>\n"
+"                    <br />\n"
+"                    <p>Yours faithfully,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</a> "
+"team </p>\n"
+"                </div>\n"
+"            "
+msgstr ""
+"\n"
+"                <div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, "
+"Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-"
+"color: #FFF; \">\n"
+"                    <p>Hola,</p>\n"
+"                    <p>Gracias por ponerte en contacto.</p>\n"
+"                    <p>Hemos recibido tu correo electrónico. Nos pondremos "
+"en contacto contigo lo antes possible.</p>\n"
+"                    <br />\n"
+"                    <p>Atentamente,</p>\n"
+"                    <p><a href=\"https://somcomunitats.coop/landing/"
+"${object.company_id.landing_page_id.slug_id}\">${object.company_id.name</"
+"a></p>\n"
 "                </div>\n"
 "            "
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_close_message_template
 msgid "&amp;times;"
-msgstr ""
+msgstr "&amp;times;"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ". Additional information:"
 msgstr ". Información adicional:"
 
 #. module: energy_communities_crm
@@ -513,15 +693,14 @@
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__company_id
 msgid "Company"
 msgstr "Compañía"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
-#: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Constitution date"
 msgstr "Fecha de constitución"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
@@ -536,14 +715,19 @@
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
 msgid "Contact CE"
 msgstr "Kontactua CE"
 
 #. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
+msgid "Contact COORD"
+msgstr "Contacto COORD"
+
+#. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter_platform_admins
 msgid "Contact SomComunitats"
 msgstr "Kontactua SomComunitats"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
@@ -583,21 +767,23 @@
 msgid "Crm Lead Metadata Mapping"
 msgstr "Mapping de metadatos en CRM Lead"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/models/crm_lead.py:0
 #, python-format
 msgid "Crm Lead stage {stage_name} doesn't match it's company {company_name}"
-msgstr "La etapa {stage_name} del lead no coincide con la compañía {company_name}"
+msgstr ""
+"La etapa {stage_name} del lead no coincide con la compañía {company_name}"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/models/crm_lead.py:0
 #, python-format
 msgid "Crm Lead team {team_name} doesn't match it's company {company_name}"
-msgstr "EL equipo {team_name} del lead no coincide con la compañía {company_name}"
+msgstr ""
+"EL equipo {team_name} del lead no coincide con la compañía {company_name}"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__ce_child_lead_id
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_crm_lead_view_form
 msgid "Crm lead child"
 msgstr "Crm lead hijo"
 
@@ -676,17 +862,17 @@
 "llevar¿la contabilidad de la Comunidad Energética? o se lo llevará una "
 "gestoría externa?"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid ""
-"Do you plan to use the platform's Odoo (management program) to carry out tax"
-" management: generation of tax reports from the Treasury (303, 390,...) or "
-"will it be carried out by an external management company?"
+"Do you plan to use the platform's Odoo (management program) to carry out "
+"tax management: generation of tax reports from the Treasury (303, 390,...) "
+"or will it be carried out by an external management company?"
 msgstr ""
 "Tiene previsto usar el Odoo (programa de gestión) de la plataforma para "
 "llevarla gestión tributaria: generación de informes tributarios de Hacienda "
 "(303, 390,...) ¿o se lo llevará una gestoría externa?"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
@@ -746,23 +932,25 @@
 #: model:ir.model.fields.selection,name:energy_communities_crm.selection__crm_tag__tag_type__energy_service
 #, python-format
 msgid "Energy Service"
 msgstr "Servicios energéticos"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
-msgid "Explain the process to become cooperator. Include payment information."
+msgid ""
+"Explain, with a maximum of 500 characters, the process to become "
+"cooperator. Include payment information."
 msgstr ""
-"Explica cuál es el proceso que deben hacer las personas que quieran hacerse "
-"socio o socias. Incluye la información sobre cuotas."
+"Explica, en un màximo de 500 carácteres, el proceso de covertirse en Socio/"
+"a de la Comunidad. Incluye la información sobre el pago."
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__external_id
 msgid "External ID"
-msgstr ""
+msgstr "ID externo"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "External management"
 msgstr "Gestión externa"
 
@@ -787,15 +975,15 @@
 #: model:ir.ui.menu,name:energy_communities_crm.ce_crm_leads_menu
 msgid "Form submissions"
 msgstr "Entradas de formularios"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.view_crm_lead_metadata_mapping_form
 msgid "General"
-msgstr ""
+msgstr "General"
 
 #. module: energy_communities_crm
 #: model:ir.actions.act_window,name:energy_communities_crm.ce_crm_leads_general_info_action
 #: model:ir.ui.menu,name:energy_communities_crm.ce_crm_leads_general_info_menu
 msgid "General Newsletter"
 msgstr "Newsletter general"
 
@@ -844,37 +1032,42 @@
 #: model:ir.model.fields,field_description:energy_communities_crm.field_utm_source__id
 msgid "ID"
 msgstr "Identificador"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__tag_ext_id
 msgid "ID Ext tag"
-msgstr ""
+msgstr "ID externo de etiqueta"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "If possible upload a group image"
 msgstr "Preferible foto de grupo"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
-"In this section you can briefly explain the advantages of joining the "
-"community"
+"In this section you can, with a maximum of 500 characters, explain the "
+"advantages of joining the community"
 msgstr ""
-"En esta sección puedes explicar cuáles son las ventajas para sumarse a la "
-"Comunidad Energética."
+"En la sección puedes, en un máximo de 500 carácteres. explicar las ventajas "
+"de unirse a la comunidad"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Industrial"
 msgstr "Industriala"
 
 #. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
+msgid "Info COORD"
+msgstr "Información COORD"
+
+#. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Instagram url"
 msgstr "Instagram"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__finished
@@ -1008,15 +1201,15 @@
 msgid "Newsletter SomComunitats"
 msgstr "Buletinera SomComunitats"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "No"
-msgstr ""
+msgstr "No"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.ce_view_crm_case_opportunities_filter
 msgid "No web form origin"
 msgstr "Web-inprimakiaren jatorririk ez"
 
 #. module: energy_communities_crm
@@ -1046,27 +1239,26 @@
 #: code:addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py:0
 #, python-format
 msgid ""
 "Opportunity assigned to Coordinator %s (ID: %s), where %s is the id of the "
 "original instance-level record."
 msgstr ""
 "Lead asignado a la coordinadora %s (ID: %s), donde %s es la id del lead "
-"original"
+"original."
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py:0
 #, python-format
 msgid ""
-"Opportunity created from Instance opportunity with ID %s, where %s is the id"
-" of the new record generated at the Coordinator level"
+"Opportunity created from Instance opportunity with ID %s, where %s is the "
+"id of the new record generated at the Coordinator level"
 msgstr ""
 "Lead creado desde el lead de la plataforma con ID %s, donde %s es la id del "
 "nuevo lead generado en la coordinadora"
 
-
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_stage__original_stage_id
 msgid "Original Stage"
 msgstr "Etapa original"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
@@ -1134,15 +1326,15 @@
 msgstr "Política de privacidad"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Public community data changed:"
 msgstr ""
-"Se han registrado cambios en los datos públicos de la comunidad energética."
+"Se han registrado cambios en los datos públicos de la comunidad energética:"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.view_crm_lead_metadata_mapping_form
 msgid "Recipients"
 msgstr "Destinatarios"
 
 #. module: energy_communities_crm
@@ -1215,15 +1407,15 @@
 #, python-format
 msgid "Surnames"
 msgstr "Apellidos"
 
 #. module: energy_communities_crm
 #: model:ir.model.constraint,message:energy_communities_crm.constraint_crm_tag_name_uniq
 msgid "Tag must be unique per company!"
-msgstr "La etiqueta debe ser única por compañía"
+msgstr "La etiqueta debe ser única por compañía!"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__tag_type
 msgid "Tag type"
 msgstr "Tipo de etiqueta"
 
 #. module: energy_communities_crm
@@ -1252,14 +1444,28 @@
 
 #. module: energy_communities_crm
 #: model:ir.model,name:energy_communities_crm.model_utm_source
 msgid "UTM Source"
 msgstr "Origen UTM"
 
 #. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
+msgid ""
+"Use a maximum of 1000 characters to write a summary of your Energy Community"
+msgstr ""
+"Usa un màximo de 1000 carácteres para escribir un resumen de tu Comunidad "
+"Energética"
+
+#. module: energy_communities_crm
+#: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
+msgid "Use a maximum of 1500 characters to explain your Energy Community"
+msgstr ""
+"Usa un máximo de 1500 carácteres para explicar tu Comunidad Energética"
+
+#. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__user_current_company
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_tag__user_current_company
 msgid "User Current Company"
 msgstr "Compañía actual del usuario"
 
 #. module: energy_communities_crm
 #: model:ir.model.fields,field_description:energy_communities_crm.field_crm_lead__user_current_role
@@ -1320,16 +1526,16 @@
 #, python-format
 msgid ""
 "Who will do the day-to-day corporate management of the Energy Community? "
 "(person/s with user access to the Odoo corporate/accounting/tax management "
 "program of the Energy Community)"
 msgstr ""
 "¿Quién hará la gestión societaria del día a día de la Comunidad Energética? "
-"(persona/s con usuario de acceso al programa Odoo de gestión "
-"societaria/contable/tributaria de la Comunidad Energética)"
+"(persona/s con usuario de acceso al programa Odoo de gestión societaria/"
+"contable/tributaria de la Comunidad Energética)"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "Why become cooperator"
 msgstr "Zergatik bihurtu kooperante"
 
@@ -1348,15 +1554,25 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "You can contact"
 msgstr "Puedes contactar"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_successful_msg
 msgid "Your data has been successfully registered."
-msgstr "Tus datos se han registrado con éxito"
+msgstr "Tus datos se han registrado con éxito."
+
+#. module: energy_communities_crm
+#: model:mail.template,subject:energy_communities_crm.email_templ_landing_coord_contact
+msgid "[${object.company_id.name] Contact Form"
+msgstr "[${object.company_id.name] Formulario de contacto"
+
+#. module: energy_communities_crm
+#: model:mail.template,subject:energy_communities_crm.email_templ_landing_coord_newsletter
+msgid "[${object.company_id.name] Newsletter Subscription"
+msgstr "[${object.company_id.name] Registro en la Newsletter"
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/services/crm_lead_service.py:0
 #, python-format
 msgid "[Contact CE]"
 msgstr "[Kontaktua CE]"
 
@@ -1448,16 +1664,16 @@
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline
 msgid ""
 "and to our <strong>administrative management space</strong> (Odoo program "
 "for corporate, accounting and financial management)"
 msgstr ""
-"y en <strong>el espacio de gestión administrativa</strong> (programa Odoo de"
-" gestión societaria, contable y financiera)."
+"y en <strong>el espacio de gestión administrativa</strong> (programa Odoo "
+"de gestión societaria, contable y financiera)."
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "ce_account_management,ce_tax_management:external_management"
 msgstr ""
 
 #. module: energy_communities_crm
@@ -1489,15 +1705,16 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid "ce_manager_headline"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_form_fields_template
 msgid ""
-"ce_manager_headline,ce_manager_firstname,ce_manager_surname,ce_manager_email,ce_manager_phone"
+"ce_manager_headline,ce_manager_firstname,ce_manager_surname,"
+"ce_manager_email,ce_manager_phone"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model:ir.model,name:energy_communities_crm.model_crm_lead_metadata_line
 msgid "crm.lead.metadata.line"
 msgstr ""
 
@@ -1510,15 +1727,15 @@
 #: model:ir.model,name:energy_communities_crm.model_crm_lead_metadata_mapping_field
 msgid "crm.lead.metadata.mapping.field"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "for further assistance."
-msgstr "para mas información"
+msgstr "para mas información."
 
 #. module: energy_communities_crm
 #: code:addons/energy_communities_crm/controllers/website_community_data.py:0
 #, python-format
 msgid "lead_id on website url"
 msgstr "lead_id en la url web"
 
@@ -1537,15 +1754,15 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid "suport@somcomunitats.coop"
 msgstr ""
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline
 msgid "to the <strong>public spaces</strong> of our"
-msgstr "en los <strong>espacios públicos</strong> de la "
+msgstr "en los <strong>espacios públicos</strong> de la"
 
 #. module: energy_communities_crm
 #: model_terms:ir.ui.view,arch_db:energy_communities_crm.community_data_headline_message_closed
 msgid ""
 "to the technology platform Som Comunitats has been successfully submitted."
 msgstr ""
 "a la plataforma tecnológica Som Comunitats han sido enviados con éxito."
```

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_lead.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping_field.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_lead_metadata_mapping_field.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_stage.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_stage.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_tag.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_tag.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/crm_team.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/crm_team.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/models/metadata_mapping_conf.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/models/metadata_mapping_conf.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/security/ir.model.access.csv` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/security/ir_rule_data.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/security/ir_rule_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/services/crm_lead_service.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/services/crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/static/src/js/community-data-website.js` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/static/src/js/community-data-website.js`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/tests/test_crm_lead.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/tests/test_crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/tests/test_crm_lead_service.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/tests/test_crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_lead_metadata_mapping_views.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_lead_metadata_mapping_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_lead_views.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_lead_views.xml`

 * *Files 5% similar despite different names*

#### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_lead_views.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_lead_views.xml`

```diff
@@ -24,16 +24,14 @@
         <filter name="ce_source_existing_ce_info" string="Newsletter CE" domain="[('source_id','=', %(energy_communities.ce_source_existing_ce_info)d)]"/>
         <filter name="ce_source_existing_ce_contact" string="Contact CE" domain="[('source_id','=', %(energy_communities.ce_source_existing_ce_contact)d)]"/>
         <filter name="ce_source_creation_ce_proposal" string="CE creation" domain="[('source_id','=', %(energy_communities.ce_source_creation_ce_proposal)d)]"/>
         <filter name="ce_source_coord_web_hiring" string="Hire COORD" domain="[('source_id','=', %(energy_communities.ce_source_coord_web_hiring)d)]"/>
         <filter name="ce_source_coord_web_other" string="Other COORD" domain="[('source_id','=', %(energy_communities.ce_source_coord_web_other)d)]"/>
         <filter name="ce_source_existing_coord_contact" string="Contact COORD" domain="[('source_id','=', %(energy_communities.ce_source_existing_coord_contact)d)]"/>
         <filter name="ce_source_existing_coord_info" string="Info COORD" domain="[('source_id','=', %(energy_communities.ce_source_existing_coord_info)d)]"/>
-        <filter name="ce_source_existing_coord_contact" string="Contact COORD" domain="[('source_id','=', %(energy_communities.ce_source_existing_coord_contact)d)]"/>
-        <filter name="ce_source_existing_coord_info" string="Info COORD" domain="[('source_id','=', %(energy_communities.ce_source_existing_coord_info)d)]"/>
         <filter name="no_web_form_origin" string="No web form origin" domain="[('source_id','=', False)]"/>
         <separator/>
       </filter>
     </field>
   </record>
   <record id="ce_view_crm_case_opportunities_filter_platform_admins" model="ir.ui.view">
     <field name="name">ce.view.crm.opportunities.leads.filter.platform.admins</field>
```

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_stage_views.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_stage_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_tag_views.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_tag_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/crm_team_views.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/crm_team_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/energy_communities_crm_lead_views.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/energy_communities_crm_lead_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/menus.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/menus.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/website_community_data_template.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/website_community_data_template.xml`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/views/website_community_data_template.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/views/website_community_data_template.xml`

```diff
@@ -24,25 +24,29 @@
         </t>
       </div>
       <div class="col-md-12" t-if="pack_1 or pack_2">
         <t t-call="energy_communities.form_field_textarea">
           <t t-set="value" t-value="ce_description"/>
           <t t-set="key" t-value="ce_description_key"/>
           <t t-set="label" t-value="ce_description_label"/>
-          <t t-set="rows" t-value="5"/>
           <t t-set="required" t-value="True"/>
+          <t t-set="rows" t-value="10"/>
+          <t t-set="maxlength" t-value="1000"/>
+          <t t-set="description">Use a maximum of 1000 characters to write a summary of your Energy Community</t>
         </t>
       </div>
       <div class="col-md-12" t-if="pack_1 or pack_2">
         <t t-call="energy_communities.form_field_textarea">
           <t t-set="value" t-value="ce_long_description"/>
           <t t-set="key" t-value="ce_long_description_key"/>
           <t t-set="label" t-value="ce_long_description_label"/>
-          <t t-set="rows" t-value="10"/>
           <t t-set="required" t-value="True"/>
+          <t t-set="rows" t-value="10"/>
+          <t t-set="maxlength" t-value="1500"/>
+          <t t-set="description">Use a maximum of 1500 characters to explain your Energy Community</t>
         </t>
       </div>
       <div class="col-md-6" t-if="pack_1 or pack_2">
         <t t-call="energy_communities.form_field_text">
           <t t-set="value" t-value="ce_address"/>
           <t t-set="key" t-value="ce_address_key"/>
           <t t-set="label" t-value="ce_address_label"/>
@@ -127,26 +131,26 @@
       </div>
       <div class="col-md-12" t-if="pack_1 or pack_2">
         <t t-call="energy_communities.form_field_textarea">
           <t t-set="value" t-value="ce_why_become_cooperator"/>
           <t t-set="key" t-value="ce_why_become_cooperator_key"/>
           <t t-set="label" t-value="ce_why_become_cooperator_label"/>
           <t t-set="rows" t-value="5"/>
-          <t t-set="maxlength" t-value="100"/>
-          <t t-set="description">In this section you can briefly explain the advantages of joining the community</t>
+          <t t-set="maxlength" t-value="500"/>
+          <t t-set="description">In this section you can, with a maximum of 500 characters, explain the advantages of joining the community</t>
         </t>
       </div>
       <div class="col-md-12" t-if="pack_1 or pack_2">
         <t t-call="energy_communities.form_field_textarea">
           <t t-set="value" t-value="ce_become_cooperator_process"/>
           <t t-set="key" t-value="ce_become_cooperator_process_key"/>
           <t t-set="label" t-value="ce_become_cooperator_process_label"/>
           <t t-set="rows" t-value="5"/>
-          <t t-set="maxlength" t-value="100"/>
-          <t t-set="description">Explain the process to become cooperator. Include payment information.</t>
+          <t t-set="maxlength" t-value="500"/>
+          <t t-set="description">Explain, with a maximum of 500 characters, the process to become cooperator. Include payment information.</t>
         </t>
       </div>
       <div class="col-md-12" t-if="pack_1 or pack_2">
         <div class="row">
           <t t-call="energy_communities.form_field_image">
             <t t-set="value" t-value="ce_primary_image_file"/>
             <t t-set="key" t-value="ce_primary_image_file_key"/>
```

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.xml` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/assign_crm_to_coordinator_company.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo/addons/energy_communities_crm/wizards/multicompany_easy_creation.py` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo/addons/energy_communities_crm/wizards/multicompany_easy_creation.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities_crm-14.0.1.1.1/odoo14_addon_energy_communities_crm.egg-info/SOURCES.txt` & `odoo14-addon-energy_communities_crm-14.0.1.1.2/odoo14_addon_energy_communities_crm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

