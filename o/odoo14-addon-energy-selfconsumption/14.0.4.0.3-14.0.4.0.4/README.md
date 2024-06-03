# Comparing `tmp/odoo14-addon-energy_selfconsumption-14.0.4.0.3.tar.gz` & `tmp/odoo14-addon-energy_selfconsumption-14.0.4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_selfconsumption-14.0.4.0.3.tar", last modified: Tue May 21 13:48:03 2024, max compression
+gzip compressed data, was "odoo14-addon-energy_selfconsumption-14.0.4.0.4.tar", last modified: Mon Jun  3 13:55:20 2024, max compression
```

## Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3.tar` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.562801 odoo14-addon-energy_selfconsumption-14.0.4.0.3/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      419 2024-05-21 13:48:03.562801 odoo14-addon-energy_selfconsumption-14.0.4.0.3/PKG-INFO
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.458796 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.458796 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.462796 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       89 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1726 2024-05-21 13:14:47.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/__manifest__.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.466796 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/controllers/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       26 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/controllers/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      723 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/controllers/controllers.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.486797 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1342 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/contract_line_qty_formula_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      548 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/custom_paper_format_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    11100 2024-03-14 09:27:19.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/ir_attactment_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1550 2024-02-27 11:59:22.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/ir_cron.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      507 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/ir_sequence_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2690 2024-02-27 11:59:22.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/mail_template.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      247 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/project_type_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      444 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/service_available_data.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.494798 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)   122634 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/ca_ES.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)   103001 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)   115609 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/es.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)   120940 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/eu_ES.po
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.458796 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/migrations/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.494798 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/migrations/14.0.3.4.0/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      364 2024-02-27 11:59:22.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/migrations/14.0.3.4.0/post-migration.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.518799 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      272 2024-01-08 11:41:31.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      859 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/account_move.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2599 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/contract.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3291 2024-03-05 11:47:38.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/contract_line.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3704 2023-12-27 14:42:56.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/distribution_table.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1191 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/partner.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      161 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/product.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      306 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/project.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    21362 2024-03-14 09:27:19.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/selfconsumption.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5739 2024-05-21 13:01:28.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/supply_point.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3391 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.522799 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/reports/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2376 2023-12-27 14:42:56.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/reports/energy_delivered_invoice_template.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3360 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/reports/power_acquired_invoice_template.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    22768 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/reports/selfconsumption_reports.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.526799 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/security/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2768 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/security/ir.model.access.csv
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1350 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.458796 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/static/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.526799 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/static/description/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2758 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/static/description/icon.png
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.534800 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/tests/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       84 2024-04-10 14:14:59.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/tests/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5773 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/tests/test_contract_generation_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4748 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/tests/test_invoicing_reminder.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.538800 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2454 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/contract_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5795 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2488 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/res_partner_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    14049 2024-03-05 11:45:23.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1811 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     6151 2024-02-27 11:59:22.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/supply_point_views.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.554801 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      206 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5568 2024-03-14 09:27:19.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1645 2024-03-14 09:27:19.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4665 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1772 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard_view.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4507 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2096 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4429 2024-02-27 11:59:22.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2012 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    11306 2024-03-14 09:27:19.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2393 2023-12-12 09:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard_views.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:48:03.558801 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      419 2024-05-21 13:48:03.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/PKG-INFO
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3847 2024-05-21 13:48:03.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-05-21 13:48:03.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/dependency_links.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-04-18 08:53:00.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/not-zip-safe
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      286 2024-05-21 13:48:03.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/requires.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        5 2024-05-21 13:48:03.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/top_level.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       38 2024-05-21 13:48:03.562801 odoo14-addon-energy_selfconsumption-14.0.4.0.3/setup.cfg
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      453 2024-05-14 12:38:21.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.3/setup.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      419 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/PKG-INFO
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.634065 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.634065 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.634065 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       89 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1726 2024-06-03 13:42:25.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/__manifest__.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.634065 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/controllers/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       26 2023-11-02 16:23:09.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/controllers/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      723 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/controllers/controllers.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.634065 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1342 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/contract_line_qty_formula_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      548 2023-11-02 16:23:09.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/custom_paper_format_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    11100 2024-03-26 17:49:11.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/ir_attactment_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1550 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/ir_cron.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      507 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/ir_sequence_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2690 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/mail_template.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      247 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/project_type_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      444 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/service_available_data.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   122634 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/ca_ES.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   103001 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   115609 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/es.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   120940 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/eu_ES.po
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.634065 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/migrations/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/migrations/14.0.3.4.0/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      364 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/migrations/14.0.3.4.0/post-migration.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      272 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      859 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/account_move.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2599 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/contract.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3291 2024-03-26 17:49:11.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/contract_line.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3706 2024-06-03 13:16:08.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/distribution_table.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1191 2023-11-02 16:23:09.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/partner.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      161 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/product.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      306 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/project.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    21362 2024-03-26 17:49:11.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/selfconsumption.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5739 2024-05-21 13:55:25.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/supply_point.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3391 2024-06-03 13:16:08.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/reports/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2376 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/reports/energy_delivered_invoice_template.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3360 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/reports/power_acquired_invoice_template.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    22768 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/reports/selfconsumption_reports.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/security/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2768 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/security/ir.model.access.csv
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1350 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.634065 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/static/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/static/description/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2758 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/static/description/icon.png
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/tests/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       84 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/tests/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5773 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/tests/test_contract_generation_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4748 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/tests/test_invoicing_reminder.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2454 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/contract_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5795 2023-11-02 16:23:09.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2488 2023-11-02 16:23:09.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/res_partner_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    14049 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1811 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6151 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/supply_point_views.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      206 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5568 2024-03-26 17:49:11.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1645 2024-03-26 17:49:11.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4665 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1772 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard_view.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4507 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2096 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4429 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2012 2024-03-25 16:29:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    11306 2024-03-26 17:49:11.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2393 2023-11-02 09:59:24.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard_views.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      419 2024-06-03 13:55:20.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/PKG-INFO
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3847 2024-06-03 13:55:20.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:55:20.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/dependency_links.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:55:20.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/not-zip-safe
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      286 2024-06-03 13:55:20.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/requires.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-06-03 13:55:20.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/top_level.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-06-03 13:55:20.637398 odoo14-addon-energy_selfconsumption-14.0.4.0.4/setup.cfg
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      453 2024-06-03 13:45:39.000000 odoo14-addon-energy_selfconsumption-14.0.4.0.4/setup.py
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/__manifest__.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         """,
     "description": """
         Module for energetic self-consumption projects.
     """,
     "author": "Coopdevs Treball SCCL & Som Energia SCCL",
     "website": "https://coopdevs.org",
     "category": "Customizations",
-    "version": "14.0.4.0.3",
+    "version": "14.0.4.0.4",
     "depends": [
         "base",
         "mail",
         "contract",
         "contract_variable_quantity",
         "contract_queue_job",
         "contract_mandate",
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/controllers/controllers.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/controllers/controllers.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/contract_line_qty_formula_data.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/contract_line_qty_formula_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/custom_paper_format_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/custom_paper_format_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/ir_attactment_data.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/ir_attactment_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/ir_cron.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/data/mail_template.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/data/mail_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/ca_ES.po` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/es.po` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/i18n/eu_ES.po` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/i18n/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/account_move.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/account_move.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/contract.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/contract.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/contract_line.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/contract_line.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/distribution_table.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/distribution_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     _description = "Distribution Table"
 
     @api.depends("supply_point_assignation_ids.coefficient")
     def _compute_coefficient_is_valid(self):
         for record in self:
             record.coefficient_is_valid = not fields.Float.compare(
                 sum(record.supply_point_assignation_ids.mapped("coefficient")),
-                1.00000,
-                precision_rounding=0.00001,
+                1.000000,
+                precision_rounding=0.000001,
             )
 
     name = fields.Char(readonly=True)
     selfconsumption_project_id = fields.Many2one(
         "energy_selfconsumption.selfconsumption", required=True
     )
     selfconsumption_project_state = fields.Selection(
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/partner.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/partner.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/selfconsumption.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/selfconsumption.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/supply_point.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/supply_point.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         related="distribution_table_id.create_date"
     )
     supply_point_id = fields.Many2one(
         "energy_selfconsumption.supply_point", required=True
     )
     coefficient = fields.Float(
         string="Distribution coefficient",
-        digits=(1, 5),
+        digits=(7, 6),
         required=True,
         help="The sum of all the coefficients must result in 1",
     )
     owner_id = fields.Many2one("res.partner", related="supply_point_id.owner_id")
     code = fields.Char(related="supply_point_id.code")
     table_coefficient_is_valid = fields.Boolean(
         related="distribution_table_id.coefficient_is_valid"
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/reports/energy_delivered_invoice_template.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/reports/energy_delivered_invoice_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/reports/power_acquired_invoice_template.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/reports/power_acquired_invoice_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/reports/selfconsumption_reports.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/reports/selfconsumption_reports.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/security/ir.model.access.csv` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/static/description/icon.png` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/static/description/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/tests/test_contract_generation_wizard.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/tests/test_contract_generation_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/tests/test_invoicing_reminder.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/tests/test_invoicing_reminder.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/contract_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/contract_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/res_partner_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/res_partner_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/views/supply_point_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/views/supply_point_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/contract_generation_wizard_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard_view.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/define_invoicing_mode_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/distribution_table_import_wizard_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/invoicing_wizard_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard.py` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo/addons/energy_selfconsumption/wizards/selfconsumption_import_wizard_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.4.0.3/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt` & `odoo14-addon-energy_selfconsumption-14.0.4.0.4/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

