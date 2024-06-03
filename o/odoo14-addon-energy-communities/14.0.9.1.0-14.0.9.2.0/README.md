# Comparing `tmp/odoo14-addon-energy_communities-14.0.9.1.0.tar.gz` & `tmp/odoo14-addon-energy_communities-14.0.9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_communities-14.0.9.1.0.tar", last modified: Tue May 21 13:45:35 2024, max compression
+gzip compressed data, was "odoo14-addon-energy_communities-14.0.9.2.0.tar", last modified: Mon Jun  3 13:50:08 2024, max compression
```

## Comparing `odoo14-addon-energy_communities-14.0.9.1.0.tar` & `odoo14-addon-energy_communities-14.0.9.2.0.tar`

### file list

```diff
@@ -1,134 +1,136 @@
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:35.017479 odoo14-addon-energy_communities-14.0.9.1.0/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      459 2024-05-21 13:45:35.017479 odoo14-addon-energy_communities-14.0.9.1.0/PKG-INFO
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.825465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.825465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.833465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      146 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2754 2024-05-21 13:23:58.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/__manifest__.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.833465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/client_map/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        0 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/client_map/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2749 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/client_map/config.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.833465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/client_map/resources/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    19411 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/client_map/resources/landing_cmplace.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.841466 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/controllers/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      117 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/controllers/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      188 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/controllers/controllers.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    11885 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/controllers/website_subscription_main.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    13259 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.857467 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1812 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4344 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/community_maps_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1366 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/crm_lead_tag.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      826 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/ir_cron.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    10726 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/mail_template_update_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1921 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/product_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1553 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/utm_data.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.877469 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    35736 2024-03-14 09:27:19.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/energy_selfconsumption_demo.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     7409 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/res_company_demo.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      576 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/res_lang_demo.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    16089 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/res_user_demo.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    37470 2024-03-14 09:27:19.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/subscription_request_demo.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      514 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/hooks.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.885469 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    98220 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n/ca_ES.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    85391 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n/energy_communities.pot
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    98659 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n/es.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    97508 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n/eu_ES.po
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.897470 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n_extra/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)   125993 2024-05-21 10:26:57.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n_extra/ca_ES.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)   126632 2024-05-21 10:26:57.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n_extra/es.po
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)   125034 2024-05-21 10:26:57.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n_extra/eu_ES.po
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.825465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/migrations/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.905471 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/migrations/14.0.1.1.12/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    11439 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/migrations/14.0.1.1.12/post-add-internal-user-role.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.909471 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/migrations/14.0.5.1.0/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1564 2024-03-18 08:36:03.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/migrations/14.0.5.1.0/post-setup-multicompany-partner.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.953474 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      481 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2866 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/account_move.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3613 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/auth_oauth_provider.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      255 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/cm_coordinates_mixin.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      204 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/cm_filter.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      262 2024-04-10 12:47:32.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/cm_map.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      559 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/cm_place.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      455 2023-12-15 11:40:15.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/external_id_mixin.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    17703 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/landing_page.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1978 2024-02-27 11:59:22.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/product.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    14050 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_company.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      672 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_config_settings.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3308 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_partner.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      291 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_partner_bank.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    12020 2024-03-05 11:47:38.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_users.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      216 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_users_role.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2004 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/user_current_company_mixin.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      419 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/utm_source.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.953474 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        0 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3253 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/client.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      904 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/exceptions.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.957475 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/resources/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        0 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/resources/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      546 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1588 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.961475 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/report/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      690 2024-02-27 11:59:22.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/report/report_templates.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.965475 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/security/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1654 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/security/ir.model.access.csv
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     6100 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/security/ir_rule_data.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     8756 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/security/res_users_role_data.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.973476 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      162 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5988 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_community_service.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      811 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_landing_service.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     9298 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_member_profile_service.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     6986 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_member_service.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     8674 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/schemas.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.829465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.977476 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/description/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3721 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/description/icon.png
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.829465 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/src/
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.981476 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/src/js/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      986 2024-02-27 11:59:22.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/src/js/cooperator.js
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:34.985477 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      145 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      975 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/common.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      769 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/common_service.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2820 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/helpers.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1364 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_assign_admin_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3410 2023-12-27 14:42:56.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_multicompany_easy_creation.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     6013 2024-04-22 09:35:57.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_res_company.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     6785 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_res_users.py
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:35.009478 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      572 2024-03-14 09:27:19.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/account_banking_mandate_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      537 2024-04-10 12:47:32.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/account_move_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1896 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/auth_oauth_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      359 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/ce_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      470 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/cm_place.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3282 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/landing_page_view.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     2088 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/menus.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      609 2024-02-27 11:59:22.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/product_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4580 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_company_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1020 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_config_settings.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5215 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_partner_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      635 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_users_role_view.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1161 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_users_view.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1513 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/utm_views.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      958 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/view_users_form.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    12572 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/website_formfields_template.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    18822 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/website_subscription_template.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:35.013479 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       75 2024-05-14 12:38:21.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/__init__.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     3044 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1762 2023-12-12 09:45:39.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.xml
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)    16175 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     4314 2024-05-21 13:01:28.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
-drwxrwxr-x   0 juan-pe   (1000) juan-pe   (1000)        0 2024-05-21 13:45:35.017479 odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      459 2024-05-21 13:45:34.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/PKG-INFO
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     5992 2024-05-21 13:45:34.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/SOURCES.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-05-21 13:45:34.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/dependency_links.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        1 2024-03-13 11:44:33.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/not-zip-safe
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)      897 2024-05-21 13:45:34.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/requires.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)        5 2024-05-21 13:45:34.000000 odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/top_level.txt
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)       38 2024-05-21 13:45:35.017479 odoo14-addon-energy_communities-14.0.9.1.0/setup.cfg
--rw-rw-r--   0 juan-pe   (1000) juan-pe   (1000)     1167 2024-05-21 13:17:15.000000 odoo14-addon-energy_communities-14.0.9.1.0/setup.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      459 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/PKG-INFO
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.726107 odoo14-addon-energy_communities-14.0.9.2.0/odoo/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.726107 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.729440 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      146 2024-05-16 14:34:58.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2803 2024-06-03 13:40:27.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/__manifest__.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.729440 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/client_map/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/client_map/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2749 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/client_map/config.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.729440 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/client_map/resources/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    19507 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/client_map/resources/landing_cmplace.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.729440 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/controllers/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      117 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/controllers/__init__.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      188 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/controllers/controllers.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    11885 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/controllers/website_subscription_main.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    13259 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.729440 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     1812 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4344 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/community_maps_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1366 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/crm_lead_tag.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      826 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/ir_cron.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    10726 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/mail_template_update_data.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     1921 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/product_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1553 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/utm_data.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.729440 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    35736 2024-05-31 08:02:47.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/energy_selfconsumption_demo.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     7409 2024-05-31 08:02:47.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/res_company_demo.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      576 2024-05-31 08:02:47.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/res_lang_demo.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    16089 2024-05-31 08:02:47.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/res_user_demo.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    37470 2024-05-31 08:02:47.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/subscription_request_demo.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      514 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/hooks.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.729440 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   120063 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n/ca_ES.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   106201 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n/energy_communities.pot
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   135559 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n/es.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   134013 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n/eu_ES.po
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n_extra/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   125993 2024-05-21 10:57:44.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n_extra/ca_ES.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   126632 2024-05-21 10:57:44.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n_extra/es.po
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)   125034 2024-05-21 10:57:44.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n_extra/eu_ES.po
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.726107 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/migrations/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/migrations/14.0.1.1.12/
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)    11439 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/migrations/14.0.1.1.12/post-add-internal-user-role.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/migrations/14.0.5.1.0/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1564 2024-03-26 17:49:11.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/migrations/14.0.5.1.0/post-setup-multicompany-partner.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      481 2024-05-31 15:30:46.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2866 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/account_move.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3613 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/auth_oauth_provider.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      255 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/cm_coordinates_mixin.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      204 2024-05-28 14:10:51.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/cm_filter.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      262 2024-03-26 17:49:11.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/cm_map.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      559 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/cm_place.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      455 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/external_id_mixin.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    18092 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/landing_page.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1978 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/product.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    18973 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_company.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      672 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_config_settings.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3308 2024-05-17 10:21:46.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_partner.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      291 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_partner_bank.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    12652 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_users.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      264 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_users_role.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2004 2024-05-24 15:54:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/user_current_company_mixin.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      419 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/utm_source.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3253 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/client.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      904 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/exceptions.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/resources/
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/resources/__init__.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      546 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1588 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/report/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      690 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/report/report_templates.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/security/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1764 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/security/ir.model.access.csv
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6100 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/security/ir_rule_data.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     8756 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/security/res_users_role_data.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      162 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/__init__.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     5988 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_community_service.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      811 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_landing_service.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     9298 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_member_profile_service.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     6986 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_member_service.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     8781 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/schemas.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.726107 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/description/
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     3721 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/description/icon.png
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.726107 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/src/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/src/js/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      986 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/src/js/cooperator.js
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      145 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/__init__.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      975 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/common.py
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      769 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/common_service.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2820 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/helpers.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1364 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_assign_admin_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3410 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_multicompany_easy_creation.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6013 2024-05-06 14:30:18.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_res_company.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6785 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_res_users.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      572 2024-03-26 17:49:11.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/account_banking_mandate_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      537 2024-03-26 17:49:11.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/account_move_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1896 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/auth_oauth_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      359 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/ce_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      470 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/cm_place.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3330 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/landing_page_view.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2250 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/menus.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      609 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/product_views.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5205 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_company_views.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     1020 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_config_settings.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5215 2024-05-14 15:56:16.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_partner_views.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      635 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_users_role_view.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     1161 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_users_view.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)     1513 2024-01-18 15:18:42.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/utm_views.xml
+-rwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)      958 2024-01-19 17:29:02.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/view_users_form.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    12572 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/website_formfields_template.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    18822 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/website_subscription_template.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      115 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3044 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1762 2024-03-25 16:29:39.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1296 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/change_coordinator_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1180 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/change_coordinator_wizard.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    16182 2024-06-03 13:16:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4314 2024-05-21 13:55:25.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      459 2024-06-03 13:50:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/PKG-INFO
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6129 2024-06-03 13:50:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/SOURCES.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:50:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/dependency_links.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-06-03 13:50:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/not-zip-safe
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      897 2024-06-03 13:50:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/requires.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-06-03 13:50:08.000000 odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/top_level.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-06-03 13:50:08.732773 odoo14-addon-energy_communities-14.0.9.2.0/setup.cfg
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1167 2024-06-03 13:44:10.000000 odoo14-addon-energy_communities-14.0.9.2.0/setup.py
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/__manifest__.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/__manifest__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "name": "Energy Community",
-    "version": "14.0.9.1.0",
+    "version": "14.0.9.2.0",
     "depends": [
         "account",
         "cooperator_account_banking_mandate",
         "account_lock_date_update",
         "account_multicompany_easy_creation",
         "cooperator_account_payment",
         "account_payment_order",
@@ -77,13 +77,14 @@
         "views/website_formfields_template.xml",
         "views/website_subscription_template.xml",
         "views/account_banking_mandate_views.xml",
         "data/mail_template_update_data.xml",
         "data/community_maps_data.xml",
         "wizards/multicompany_easy_creation.xml",
         "wizards/assign_admin_wizard.xml",
+        "wizards/change_coordinator_wizard.xml",
     ],
     "installable": True,
     "application": True,
     "auto_install": False,
     "post_init_hook": "post_init_hook",
 }
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/client_map/config.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/client_map/config.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/client_map/resources/landing_cmplace.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/client_map/resources/landing_cmplace.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     _name = "landing_cmplace"
 
     def __init__(self, landing):
         self.landing = landing
         self.wp_landing_data = self._get_wp_landing_data()
         button_configs = self._get_button_color_configs()
         if button_configs["errors"]:
-            raise UserError(error_msg)
+            raise UserError(button_configs["errors"])
         else:
             self.button_configs = button_configs["button_color_configs"]
 
     def create(self):
         """
         Creates a place from a landing instance.
         """
@@ -49,15 +49,15 @@
                 place = self.landing.map_place_id
                 if place:
                     place.write(validated_place_data["data"])
             if place:
                 self._place_extra_data_setup(place)
 
     def _place_extra_data_setup(self, place):
-        place.setup_slug_id()
+        # presenter metadata
         place.build_presenter_metadata_ids()
         # setup description
         self._setup_place_description(place)
         # setup external links
         self._setup_external_links(place)
         # apply translations
         self._apply_place_metadatas_translations(place)
@@ -67,14 +67,15 @@
         Try to generate a place data dictionary and collect errors if they're
         @returns: dictionary with 'data' key as the dict to be used for place creation or update and 'errors' key to collect errors if they're
         """
         ret_dict = {
             "data": {
                 "company_id": MapClientConfig.MAPPING__INSTANCE_ID,
                 "name": self.landing.name,
+                "slug_id": self.landing.slug_id,
                 "type": "place",
                 "status": MapClientConfig.MAPPING__LANDING_STATUS__MAP_PLACE_STATUS[
                     self.landing.status
                 ],
                 "interaction_method": "external_link",
                 "filter_mids": [(5, 0, 0)],
                 "address_txt": self._get_address_txt(),
@@ -146,14 +147,15 @@
             ret_dict["errors"].append(
                 _("Place status filter not found slug_id: {}").format(
                     place_community_status_slug
                 )
             )
         # Related coordinator
         if self.landing.hierarchy_level == "community":
+            coord_filter = False
             if self.landing.parent_landing_id:
                 if self.landing.parent_landing_id.status == "publish":
                     coord_filter = (
                         self.landing.get_map_coordinator_filter_in_related_place()
                     )
             if coord_filter:
                 ret_dict["data"]["filter_mids"].append((4, coord_filter.id))
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/controllers/website_subscription_main.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/controllers/website_subscription_main.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/community_maps_data.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/community_maps_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/crm_lead_tag.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/crm_lead_tag.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/ir_cron.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/mail_template_update_data.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/mail_template_update_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/product_data.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/product_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/data/utm_data.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/data/utm_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/energy_selfconsumption_demo.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/energy_selfconsumption_demo.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/res_company_demo.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/res_company_demo.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/res_lang_demo.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/res_lang_demo.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/res_user_demo.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/res_user_demo.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/demo/subscription_request_demo.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/demo/subscription_request_demo.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/hooks.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/hooks.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n/ca_ES.po` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n/ca_ES.po`

 * *Files 19% similar despite different names*

```diff
@@ -2,74 +2,93 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-26 12:51+0000\n"
-"PO-Revision-Date: 2024-03-26 12:51+0000\n"
+"POT-Creation-Date: 2024-05-31 09:57+0000\n"
+"PO-Revision-Date: 2024-05-31 16:15+0200\n"
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
 
 #. module: energy_communities
 #: model:mail.template,body_html:energy_communities.email_template_conditions_voluntary_share
 msgid ""
 "\n"
 "    <p>Dear ${object.name},</p>\n"
 "    <p>\n"
-"        Last week we charged your account corresponding to your voluntary contribution to the share capital of the\n"
+"        Last week we charged your account corresponding to your voluntary "
+"contribution to the share capital of the\n"
 "        <b>${object.company_id.name}</b>.\n"
 "    </p>\n"
 "    <p>\n"
-"        We attach the contract with the conditions of your investment and we remind you that for any doubt or\n"
-"        clarification in relation to the contribution made you can send an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a> or consult the website\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>.\n"
+"        We attach the contract with the conditions of your investment and "
+"we remind you that for any doubt or\n"
+"        clarification in relation to the contribution made you can send an "
+"email to\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a> or consult the website\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>.\n"
 "    </p>\n"
 "    <p>\n"
-"        We take this opportunity to thank you, once again, for your involvement with the <b>${object.company_id.name}</b>\n"
-"        objective to promote those actions or projects that contribute to an energy, economic and social transition\n"
+"        We take this opportunity to thank you, once again, for your "
+"involvement with the <b>${object.company_id.name}</b>\n"
+"        objective to promote those actions or projects that contribute to "
+"an energy, economic and social transition\n"
 "        in ${object.company_id.city}.\n"
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
+"\n"
 "    <p>Apreciat/ada ${object.firstname},</p>\n"
 "    <p>\n"
-"        Et confirmem que ja hem fet el càrrec al teu compte bancari corresponent a la teva aportació al capital voluntari de \n"
+"        Et confirmem que ja hem fet el càrrec al teu compte bancari "
+"corresponent a la teva aportació al capital voluntari de \n"
 "        <b>${object.company_id.name}</b>.\n"
 "    </p>\n"
 "    <p>\n"
-"\tRestem a la teva disposició per qualsevol dubte o aclariment en relació a la aportació realitzada a través del nostre correu electrònic \n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a> o la nostra pàgina web \n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>.\n"
+"\tRestem a la teva disposició per qualsevol dubte o aclariment en relació a "
+"la aportació realitzada a través del nostre correu electrònic \n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a> o la nostra pàgina web \n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>.\n"
 "    </p>\n"
 "    <p>\n"
-"        Aprofitem per agrair-te, un cop més, la teva implicació amb l'objectiu de <b>${object.company_id.name}</b>\n"
-"        per impulsar aquelles accions o projecte que contribueixin a una transició energètica, economia i social a ${object.company_id.city}.\n"
+"        Aprofitem per agrair-te, un cop més, la teva implicació amb "
+"l'objectiu de <b>${object.company_id.name}</b>\n"
+"        per impulsar aquelles accions o projecte que contribueixin a una "
+"transició energètica, economia i social a ${object.company_id.city}.\n"
 "    </p>\n"
 "    <p>\n"
-"Fes que corri la veu explicant el nostre projecte a familiars i amics/amigues. Com més siguem, més lluny arribarem!\n"
+"Fes que corri la veu explicant el nostre projecte a familiars i amics/"
+"amigues. Com més siguem, més lluny arribarem!\n"
 "    </p>\n"
 "    <p>\n"
 "Moltes gràcies i bona energia!\n"
 "    </p>\n"
 "    <p>\n"
 "        Atentament,\n"
 "    </p>\n"
@@ -83,23 +102,25 @@
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
 "<img src=\"/logo.png?company=${object.company_id.id}\">\n"
 "</div>\n"
 "            "
 
@@ -110,22 +131,37 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.form_field_date_past
 msgid "#{date_placeholder}"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.form.model,submission_ok_message:energy_communities.map_form_model_campanya
+msgid ""
+"<h1 class=\"text-lg font-semibold\">Formulari enviat.</h1><h2 class=\"text-"
+"lg font-medium\">Moltes gracies pel seu interès!</h2></br><div class=\"flex "
+"text-[#8a9f96]\">Quan hi hagi novetats amb la Comunitat Energètica "
+"contactarem amb tu i amb les persones que també han mostrat interès i us "
+"oferirem suport per activar-la. Som-hi!</div>"
+msgstr ""
+"<h1 class=\"text-lg font-semibold\">Formulari enviat.</h1><h2 class=\"text-"
+"lg font-medium\">Moltes gracies pel seu interès!</h2></br><div class=\"flex "
+"text-[#8a9f96]\">Quan hi hagi novetats amb la Comunitat Energètica "
+"contactarem amb tu i amb les persones que també han mostrat interès i us "
+"oferirem suport per activar-la. Som-hi!</div>"
+
+#. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser
 msgid "A super power user that is able to CRUD users on KC."
 msgstr "Un super-usuari amb permisos pper CRUD en KC."
 
 #. module: energy_communities
-#: model:ir.model,name:energy_communities.model_account_chart_template
-msgid "Account Chart Template"
-msgstr "Plantilla de gràfic de comptes"
+#: model:cm.filter.group,name:energy_communities.map_filter_group_energy_actions
+msgid "Accions energètiques"
+msgstr "Accions energètiques"
 
 #. module: energy_communities
 #: model:ir.model.constraint,message:energy_communities.constraint_account_multicompany_bank_wiz_unique_number
 #: model:ir.model.constraint,message:energy_communities.constraint_res_partner_bank_unique_number
 msgid "Account Number must be unique"
 msgstr "El número de compte ha de ser únic"
 
@@ -174,25 +210,31 @@
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_admin_provider
 msgid "Admin provider"
 msgstr "ProveÏdor AUTH  taques administratives"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_admin
 msgid "Administrator"
-msgstr "Administrador"
+msgstr "Administrator"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map__admins_to_notify
 msgid "Admins to notify"
 msgstr "Admins a notificar"
 
 #. module: energy_communities
+#: model:cm.map,proposal_form_subtitle_step_address:energy_communities.map_campanya
+msgid "Adreça"
+msgstr "Adreça"
+
+#. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_flexibility
 #: model:crm.tag,name:energy_communities.ce_tag_aggregate_demand
 msgid "Agregació i flexibilitat de la demanda"
-msgstr ""
+msgstr "Agregació i flexibilitat de la demanda"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__allow_new_members
 msgid "Allow new members"
 msgstr "Autoritza nous membres"
 
 #. module: energy_communities
@@ -228,15 +270,14 @@
 msgid "Attachment Count"
 msgstr "Número d'adjunts"
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_community_service.py:0
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #: code:addons/energy_communities/services/ce_member_service.py:0
-#: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid "Authorization token not found"
 msgstr "Token d'autorització no trobat"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.iban_template_es_ccee
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
@@ -264,15 +305,15 @@
 msgid "Become cooperator process"
 msgstr "Fer-te col·laborador"
 
 #. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
 #, python-format
 msgid "Button configs not found."
-msgstr "Configuracions de butons no trobats"
+msgstr "Configuracions de butons no trobats."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/landing_page.py:0
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__management_services
 #, python-format
 msgid "CCEE management services"
 msgstr "Serveis per la gestió de CCEE"
@@ -285,22 +326,55 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__crm_lead_id
 msgid "CRM Lead"
 msgstr "Iniciativa CRM"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_assign_admin_wizard_form
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_change_coordinator_wizard_form
 msgid "Cancelar"
 msgstr "Cancel·lar"
 
 #. module: energy_communities
+#: model:cm.map,searchbar_placeholder:energy_communities.map_campanya
+msgid "Cerca adreça o municipi"
+msgstr "Cerca adreça o municipi"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_product_product__mail_template
 #: model:ir.model.fields,field_description:energy_communities.field_product_template__mail_template
 msgid "Certificate email template"
-msgstr "Plantilla email de certificat"
+msgstr "Plantilla de email de certificat"
+
+#. module: energy_communities
+#: model:ir.actions.act_window,name:energy_communities.act_window_change_coordinator
+msgid "Change Coordinator"
+msgstr "Canvi de Coordinadora"
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_change_coordinator_wizard_form
+msgid "Change Coordinator Wizard"
+msgstr "Assistent de canvi de Coordinadora"
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/res_company.py:0
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
+#, python-format
+msgid "Change coordinator"
+msgstr "Canvi de Coordinadora"
+
+#. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__change_reason
+msgid "Change reason"
+msgstr "Motiu del canvi"
+
+#. module: energy_communities
+#: model:ir.model,name:energy_communities.model_change_coordinator_wizard
+msgid "Change the coordinator of an existing energy community"
+msgstr "Canvia la Coordinadora de una Comuntat energètica existent"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__chart_template_id
 msgid "Chart Template"
 msgstr "Plantilla plan contable"
 
 #. module: energy_communities
@@ -320,28 +394,34 @@
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "City not found"
 msgstr "Ciutat no trobada"
 
 #. module: energy_communities
+#: model:cm.place.category,name:energy_communities.map_place_category_citizen
+msgid "Ciutadania"
+msgstr "Ciutadania"
+
+#. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_utm_sources_action
 msgid "Click to define a new Source."
 msgstr "Clica per definir un nou Source."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__ce_member_status__closed
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_status__closed
 #, python-format
 msgid "Closed"
 msgstr "Tancat"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__code
+#: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line__code
 msgid "Code"
 msgstr "Codi"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__comercial_name
 msgid "Comercial name"
 msgstr "Nom comercial"
@@ -370,25 +450,25 @@
 msgid "Community company"
 msgstr "Companyia Comunitat Energètica"
 
 #. module: energy_communities
 #: code:addons/energy_communities/wizards/multicompany_easy_creation.py:0
 #, python-format
 msgid ""
-"Community created from: <a "
-"href='/web#id={id}&view_type=form&model=crm.lead&menu_id={menu_id}'>{name}</a>"
+"Community created from: <a href='/web#id={id}&view_type=form&model=crm."
+"lead&menu_id={menu_id}'>{name}</a>"
 msgstr ""
-"Communitat creada desde: <a "
-"href='/web#id={id}&view_type=form&model=crm.lead&menu_id={menu_id}'>{name}</a>"
+"Communitat creada desde: <a href='/web#id={id}&view_type=form&model=crm."
+"lead&menu_id={menu_id}'>{name}</a>"
 
 #. module: energy_communities
 #: code:addons/energy_communities/wizards/multicompany_easy_creation.py:0
 #, python-format
 msgid "Community creation process has been started."
-msgstr "El procés de creació de companyia ha començat"
+msgstr "El procés de creació de companyia ha començat."
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__community_secondary_type
 msgid "Community secondary type"
 msgstr "Tipus secundari Comunitat"
 
 #. module: energy_communities
@@ -413,14 +493,26 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__company_id
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Company"
 msgstr "Companyia"
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_res_company__logo
+msgid "Company Logo"
+msgstr "Logotip de companyia"
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/res_company.py:0
+#, python-format
+msgid ""
+"Company comercial name must be established in order to create a landing"
+msgstr "El nom comercial ha d'estar definit per poder crear una Landing"
+
+#. module: energy_communities
 #: code:addons/energy_communities/wizards/multicompany_easy_creation.py:0
 #, python-format
 msgid "Company creation successful"
 msgstr "Creació d'empresa amb èxit"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__company_hierarchy_level
@@ -432,17 +524,22 @@
 #: code:addons/energy_communities/models/landing_page.py:0
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__company_logo
 #, python-format
 msgid "Company logo"
 msgstr "Logo de la companyia"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_collective_purchases
+msgid "Compres col.lectives"
+msgstr "Compres col.lectives"
+
+#. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_collective_purchases
 msgid "Compres col·lectives"
-msgstr ""
+msgstr "Compres col·lectives"
 
 #. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_template_conditions_voluntary_share
 msgid ""
 "Conditions Share Capital to ${object.company_id.name} Ref. ACSV${object.id}"
 msgstr ""
 "Aportació voluntària a ${object.company_id.name} Ref. ACSV${object.id}: "
@@ -463,19 +560,19 @@
 msgid "Confirm Email"
 msgstr "Confirmar el correu electrònic"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_users.py:0
 #, python-format
 msgid ""
-"Conflict on user values. Please verify that all values supposed to be unique"
-" are really unique. %(detail)s"
+"Conflict on user values. Please verify that all values supposed to be "
+"unique are really unique. %(detail)s"
 msgstr ""
-"Conflicte amb les dades de usuari. Si us plau, verifica que les dades que se"
-" suposa que són úniques per a cada usuari, realment ho siguin%(detail)s"
+"Conflicte amb les dades de usuari. Si us plau, verifica que les dades que "
+"se suposa que són úniques per a cada usuari, realment ho siguin%(detail)s"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_res_partner
 msgid "Contact"
 msgstr "Contacte"
 
 #. module: energy_communities
@@ -500,20 +597,14 @@
 
 #. module: energy_communities
 #: model:product.template,name:energy_communities.share_capital_product_template
 msgid "Contribution to Share Capital"
 msgstr "Aportació al Capital Social"
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/operation_request.py:0
-#, python-format
-msgid "Converting just part of the shares is not yet implemented"
-msgstr ""
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__cooperative
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__cooperative
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__cooperative
 #, python-format
 msgid "Cooperative"
 msgstr "Cooperativa"
@@ -535,57 +626,81 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__cooperator_share_form_header_text
 msgid "Cooperator share form header text"
 msgstr "Text del formulari de participació obligatòria"
 
 #. module: energy_communities
+#: model:cm.filter.group,name:energy_communities.map_filter_group_coordinator
+msgid "Coordinadora"
+msgstr "Coordinadora"
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__hierarchy_level__coordinator
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__company_hierarchy_level__coordinator
 #, python-format
 msgid "Coordinator"
 msgstr "Coordinadora"
 
 #. module: energy_communities
 #: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
-#: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
 #: model:res.groups,name:energy_communities.role_coord_admin_res_groups
 #: model:res.users.role,name:energy_communities.role_coord_admin
 #, python-format
 msgid "Coordinator Admin"
 msgstr "Administrador de Coordinadora"
 
 #. module: energy_communities
 #: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
-#: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
 #: model:res.groups,name:energy_communities.role_coord_worker_res_groups
 #: model:res.users.role,name:energy_communities.role_coord_worker
 #, python-format
 msgid "Coordinator Worker"
 msgstr "Treballador de Coordinadora"
 
 #. module: energy_communities
+#: code:addons/energy_communities/wizards/change_coordinator_wizard.py:0
+#, python-format
+msgid "Coordinator change successful"
+msgstr "Canvi de Coordinadora executat amb èxit"
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_partner_form
 msgid "Coordinator company"
 msgstr "Companyia Coordinadora"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_res_partner_filter
 msgid "Coordinators"
 msgstr "Coordinadores"
 
 #. module: energy_communities
+#: model:cm.map,proposal_cta_title:energy_communities.map_campanya
+msgid "Crea una comunitat"
+msgstr "Crea una comunitat"
+
+#. module: energy_communities
+#: model:cm.map,proposal_form_title:energy_communities.map_campanya
+msgid "Crea una comunitat al mapa"
+msgstr "Crea una comunitat al mapa"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__create_landing
 #: model_terms:ir.ui.view,arch_db:energy_communities.wizard_multicompany_easy_creation_form_inherit
 msgid "Create Landing"
 msgstr "Crear dades públiques"
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__create_place
+msgid "Create Map Place"
+msgstr "Crear un punt de mapa"
+
+#. module: energy_communities
 #: model:ir.actions.act_window,name:energy_communities.action_open_assign_admin_wizard
 msgid "Create User"
 msgstr "Crear usuari"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
 msgid "Create landing page"
@@ -609,20 +724,22 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__create_user_in_keycloak
 msgid "Create user for keycloak"
 msgstr "Crear usuari de keyCloak/SSO desde la sòcia"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__create_uid
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__create_uid
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__create_uid
 msgid "Created by"
 msgstr "Creat per"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__create_date
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__create_date
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__create_date
 msgid "Created on"
 msgstr "Creat el"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__current_role
 msgid "Current Role"
@@ -632,39 +749,40 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
 msgid "Customize documents text"
 msgstr "Personalització de textos en documents"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_users_form_form_inherit
 msgid "DNI"
-msgstr ""
+msgstr "DNI"
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_account_move__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_cm_coordinates_mixin__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_cm_place__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__display_name
-#: model:ir.model.fields,field_description:energy_communities.field_operation_request__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_product_template__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_config_settings__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner_bank__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line__display_name
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_user_currentcompany_mixin__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source__display_name
 msgid "Display Name"
-msgstr "Nom a mostrar"
+msgstr "Mostrar Nom"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__display_footer_doc_policy_text
 msgid "Display footer doc policy text"
 msgstr "Mostrar text legal a peu de documents"
 
 #. module: energy_communities
@@ -672,14 +790,15 @@
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__status__draft
 #: model_terms:ir.ui.view,arch_db:energy_communities.landing_page_form_view
 #, python-format
 msgid "Draft"
 msgstr "Esborany"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_efficiency
 #: model:crm.tag,name:energy_communities.ce_tag_energy_efficiency
 msgid "Eficiencia energètica"
 msgstr "Eficiència Energètica"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__email
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__email
@@ -688,26 +807,27 @@
 msgstr "Correu electrònic"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Email and confirmation email addresses don't match."
-msgstr "El email i la seva confirmació no coincideixen"
+msgstr "El email i la seva confirmació no coincideixen."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Email not found"
 msgstr "Email no trobat"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_thermal_energy
 #: model:crm.tag,name:energy_communities.ce_tag_thermal_energy
 msgid "Energia tèrmica i climatització"
-msgstr ""
+msgstr "Energia tèrmica i climatització"
 
 #. module: energy_communities
 #: model:ir.module.category,name:energy_communities.energy_communities_category
 #: model:ir.ui.menu,name:energy_communities.ce_root_menu
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_res_partner_filter
 msgid "Energy Communities"
@@ -716,30 +836,28 @@
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.wizard_multicompany_easy_creation_form_inherit
 msgid "Energy Community"
 msgstr "Comunitat Energètica"
 
 #. module: energy_communities
 #: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
-#: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
 #: model:res.groups,name:energy_communities.role_ce_admin_res_groups
 #: model:res.users.role,name:energy_communities.role_ce_admin
 #, python-format
 msgid "Energy Community Administrator"
 msgstr "Administrador de la Comunitat Energètica"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.role_ce_manager_res_groups
 #: model:res.users.role,name:energy_communities.role_ce_manager
 msgid "Energy Community Manager"
 msgstr "Responsable de la Comunitat Energètica"
 
 #. module: energy_communities
 #: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
-#: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
 #: model:res.groups,name:energy_communities.role_ce_member_res_groups
 #: model:res.users.role,name:energy_communities.role_ce_member
 #, python-format
 msgid "Energy Community Member"
 msgstr "Membre de la Comunitat Energètica"
 
 #. module: energy_communities
@@ -751,22 +869,42 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__ce_status
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__ce_status
 msgid "Energy Community state"
 msgstr "Estat de la Comunitat Energètica"
 
 #. module: energy_communities
+#: model:cm.form.model,button_label:energy_communities.map_form_model_campanya
+msgid "Enviar"
+msgstr "Enviar"
+
+#. module: energy_communities
+#: model:cm.filter.group,name:energy_communities.map_filter_group_community_status
+msgid "Estat actual de la comunitat"
+msgstr "Estat actual de la comunitat"
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_change_coordinator_wizard_form
+msgid "Execute"
+msgstr "Executar"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin__external_id
 msgid "External ID"
-msgstr ""
+msgstr "ID extern"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_external_id_mixin
 msgid "External ID Mixin"
-msgstr ""
+msgstr "Mixin de ID extern"
+
+#. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__slug_id
+msgid "External slug ID"
+msgstr "Slug ID extern"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__external_website_link
 msgid "External website link"
 msgstr "Enllaç al lloc web extern"
 
 #. module: energy_communities
@@ -806,35 +944,45 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__footer_doc_policy_text
 msgid "Footer doc policy text"
 msgstr "Text legal a peu de documents"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_training
 #: model:crm.tag,name:energy_communities.ce_tag_citizen_education
 msgid "Formació ciutadana"
-msgstr ""
+msgstr "Formació ciutadana"
+
+#. module: energy_communities
+#: model:cm.map,proposal_form_subtitle_step_form:energy_communities.map_campanya
+msgid "Formulari de creació"
+msgstr "Formulari de creació"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__foundation_date
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__foundation_date
 msgid "Foundation date"
 msgstr "Data creació"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__gender
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__gender
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__gender
 msgid "Gender"
 msgstr "Gènere"
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_common_generation
 msgid "Generació renovable comunitaria"
-msgstr ""
+msgstr "Generació renovable comunitaria"
+
+#. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_generation
+msgid "Generació renovable comunitària"
+msgstr "Generació renovable comunitària"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__general_partnership
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__general_partnership
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__general_partnership
 #, python-format
@@ -849,61 +997,62 @@
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Hello,"
 msgstr "Hola,"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__hierarchy_level
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__hierarchy_level
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__hierarchy_level
 msgid "Hierarchy level"
 msgstr "Nivell jeràrquic"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.iban_template_es_ccee
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
 msgid "I accept that the entity issues direct debit receipts to this account."
 msgstr ""
 "Confirmo que la persona titular del compte bancari, sigui jo mateixa o una "
 "altra, autoritza la domiciliació dels rebuts."
 
 #. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_share
-#: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
 msgstr "Prefereixo no compartir-ho"
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__id
+#: model:ir.model.fields,field_description:energy_communities.field_account_move__id
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__id
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__id
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__id
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__id
 #: model:ir.model.fields,field_description:energy_communities.field_cm_coordinates_mixin__id
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter__id
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map__id
+#: model:ir.model.fields,field_description:energy_communities.field_cm_place__id
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin__id
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__id
-#: model:ir.model.fields,field_description:energy_communities.field_operation_request__id
 #: model:ir.model.fields,field_description:energy_communities.field_product_template__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_config_settings__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner_bank__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line__id
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__id
 #: model:ir.model.fields,field_description:energy_communities.field_user_currentcompany_mixin__id
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source__id
 msgid "ID"
-msgstr ""
+msgstr "ID"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_mailing_mailing__source_ext_id
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source__source_ext_id
 msgid "ID Ext Source"
-msgstr ""
+msgstr "Font externa"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid ""
 "INDIVIDUAL\n"
 "                PARTNER"
 msgstr "SOCI FÍSIC"
@@ -934,46 +1083,47 @@
 #: model:ir.model.fields,help:energy_communities.field_res_company__notify_to_coord_child_ccee_submissions
 #, python-format
 msgid ""
 "If it is checked, the Coordinator will receive a copy of each auto-response "
 "email that is generated in any of its CCEE when a new Member Subscription "
 "request is received."
 msgstr ""
-"Si està marcat la Coordinadora rebrà una còpia de cada correu d’autoresposta"
-" que es generi en qualsevol de les seves CCEE quan es rebi una nova "
-"socilitud de sòcia a la CE"
+"Si està marcat la Coordinadora rebrà una còpia de cada correu "
+"d’autoresposta que es generi en qualsevol de les seves CCEE quan es rebi "
+"una nova socilitud de sòcia a la CE."
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_product_product__mail_template
 #: model:ir.model.fields,help:energy_communities.field_product_template__mail_template
 msgid "If left empty, the default global mail template will be used."
 msgstr ""
-"Si es deixa buit ef fará servir la plantilla de correu global per defecte"
+"Si es deixa buit ef fará servir la plantilla de correu global per defecte."
+
+#. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__incoming_coordinator
+msgid "Incoming Coordinator"
+msgstr "Coordinadora entrant"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__individual_entrepreneur
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__individual_entrepreneur
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__individual_entrepreneur
 #, python-format
 msgid "Individual entrepreneur"
 msgstr "Empresari Individual"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:cm.place.category,name:energy_communities.map_place_category_industrial
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__landing_community_type__industrial
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_type__industrial
 #, python-format
 msgid "Industrial"
-msgstr ""
-
-#. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.ce_view_crm_case_opportunities_filter
-msgid "Info COORD"
-msgstr "Info COORD"
+msgstr "Industrial"
 
 #. module: energy_communities
 #: model:utm.source,name:energy_communities.ce_source_general_info
 msgid "Information Newsletter (general)"
 msgstr "Rebre butlletí informació general plataforma"
 
 #. module: energy_communities
@@ -1020,17 +1170,17 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__is_new_admin
 msgid "Is a new admin?"
 msgstr "És un administrador nou a la plataforma?"
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__is_voluntary
-msgid "Is voluntary contribution"
-msgstr "És una aportació voluntària"
+#: model:ir.model,name:energy_communities.model_account_move
+msgid "Journal Entry"
+msgstr "Assentament comptable"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_keycloak_provider
 msgid "Keycloak provider"
 msgstr "Proveïdor KeyCloak"
 
 #. module: energy_communities
@@ -1055,58 +1205,66 @@
 #. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
 #, python-format
 msgid "Landing lng param required for place creation"
 msgstr "La longitud és requerida per la creació d'un punt de mapa"
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter__landing_id
+msgid "Landing page"
+msgstr "Pàgina Landing"
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/cm_place.py:0
 #: model:ir.model.fields,field_description:energy_communities.field_cm_place__landing_reference
 #, python-format
 msgid "Landing reference"
 msgstr "Referència a la pàgina web"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__default_lang_id
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__lang
 msgid "Language"
 msgstr "Idioma"
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_account_chart_template____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_account_move____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_cm_coordinates_mixin____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_cm_place____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page____last_update
-#: model:ir.model.fields,field_description:energy_communities.field_operation_request____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_product_template____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_company____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_config_settings____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner_bank____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_users____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line____last_update
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_user_currentcompany_mixin____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source____last_update
 msgid "Last Modified on"
 msgstr "Última modificació el"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__write_uid
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__write_uid
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__write_uid
 msgid "Last Updated by"
 msgstr "Última actualització per"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__write_date
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__write_date
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__write_date
 msgid "Last Updated on"
 msgstr "Última actualització el"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__last_name
 msgid "Last name"
@@ -1153,15 +1311,15 @@
 msgid "Limited partnership"
 msgstr "Societat Comanditària"
 
 #. module: energy_communities
 #: model:auth.oauth.provider,body:energy_communities.keycloak_admin_provider
 #: model:auth.oauth.provider,body:energy_communities.keycloak_login_provider
 msgid "Login with Keycloak"
-msgstr "Login amb Keycloak"
+msgstr "Ligin amb Keycloak"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__landing_logo_file
 msgid "Logo Image"
 msgstr "Imatge de logo"
 
 #. module: energy_communities
@@ -1179,19 +1337,14 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__message_main_attachment_id
 msgid "Main Attachment"
 msgstr "Adjunt principal"
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
-msgid "Mandatory Shares"
-msgstr "Aportacions obligatòries"
-
-#. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
 #, python-format
 msgid "Map not found slug_id: {}"
 msgstr "Mapa no trobat per slug_id: {}"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.mass_mailing_super_user
@@ -1205,29 +1358,35 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__message_ids
 msgid "Messages"
 msgstr "Missatges"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_mobility
 #: model:crm.tag,name:energy_communities.ce_tag_sustainable_mobility
 msgid "Mobilitat sostenible"
-msgstr ""
+msgstr "Mobilitat sostenible"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__my_activity_date_deadline
 msgid "My Activity Deadline"
 msgstr "La meva deadline d'activitat"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
 msgid "My landing page"
 msgstr "La meva pàgina de destinació"
 
 #. module: energy_communities
+#: model:cm.map,external_link_cta_txt:energy_communities.map_campanya
+msgid "Més informació"
+msgstr "Més informació"
+
+#. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__company_hierarchy_level__none
 msgid "NONE"
 msgstr "Cap"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__name
 msgid "Name"
@@ -1258,17 +1417,21 @@
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__activity_type_id
 msgid "Next Activity Type"
 msgstr "Tipus de nova activitat"
 
 #. module: energy_communities
 #: model:ir.module.category,description:energy_communities.energy_communities_category
 msgid ""
-"Nivell d'Accés dels usuaris a la plataforma Odoo de les Comunitats Energètiques\n"
+"Nivell d'Accés dels usuaris a la plataforma Odoo de les Comunitats "
+"Energètiques\n"
 "        "
 msgstr ""
+"Nivell d'Accés dels usuaris a la plataforma Odoo de les Comunitats "
+"Energètiques\n"
+"        "
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_community_service.py:0
 #, python-format
 msgid "No Odoo Company found for odoo_company_id %s"
 msgstr ""
 "No s'ha trobat cap companya al Odoo pel paràmetre: odoo_company_id= %s"
@@ -1284,33 +1447,34 @@
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid "No Odoo User found for KeyCloak user id %s"
 msgstr "No s'ha trobat cap Usuari d'Odoo vinculat al Usuari de KeyCloak: %s"
 
 #. module: energy_communities
+#: model:cm.map,noresults_msg:energy_communities.map_campanya
+msgid "No hem trobats resultats. Prova a canviar la configuració de filtres."
+msgstr "No hem trobats resultats. Prova a canviar la configuració de filtres."
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__non_profit
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__non_profit
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__non_profit
 #, python-format
 msgid "Non profit association"
 msgstr "Associació sense ànim de lucre"
 
 #. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_binary
-#: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_binary
 msgid "Not binary"
 msgstr "No binari"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
-#: code:addons/energy_communities/controllers/website_subscription_main.py:0
-#: code:addons/energy_communities/controllers/website_subscription_main.py:0
-#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Not valid parameter value [odoo_company_id]"
 msgstr "El valor pel paràmetre [odoo_company_id] no és vàlid"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
@@ -1361,18 +1525,24 @@
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_auth_oauth_provider
 msgid "OAuth2 provider"
 msgstr "Proveïdor OAuth2"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_open
+msgid "Oberta"
+msgstr "Oberta"
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
-"Once you are a member you can enjoy the services available from the community and be part of a movement\n"
+"Once you are a member you can enjoy the services available from the "
+"community and be part of a movement\n"
 "                of social and energy model transformation."
 msgstr ""
 "Una vegada siguis soci/a podràs gaudir dels serveis disponibles de la "
 "comunitat energètica i, alhora, formar part d'un moviment de transformació "
 "social i de model energètic."
 
 #. module: energy_communities
@@ -1399,27 +1569,27 @@
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__ce_member_status__open
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_status__open
 #, python-format
 msgid "Open"
 msgstr "Obert"
 
 #. module: energy_communities
-#: model:ir.model,name:energy_communities.model_operation_request
-msgid "Operation request"
-msgstr "Sol·licitud d'operació"
-
-#. module: energy_communities
 #: model:crm.tag,name:energy_communities.pack_1
 msgid "Pack 1"
-msgstr ""
+msgstr "Pack 1"
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.pack_2
 msgid "Pack 2"
-msgstr ""
+msgstr "Pack 2"
+
+#. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__parent_id
+msgid "Parent Company"
+msgstr "Companyia parent"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__parent_id
 msgid "Parent Coordinator Company"
 msgstr "Empresa principal Coordinadora"
 
 #. module: energy_communities
@@ -1436,24 +1606,30 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "Parent company must be instance hierarchy level."
 msgstr "L'empresa principal ha de tenir nivell d'Instància."
 
 #. module: energy_communities
-#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
-#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
-#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
-#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__parent_landing_id
+msgid "Parent landing page"
+msgstr "Pàgina Landing parent"
+
+#. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Partner not found"
 msgstr "Soci no trobat"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_to_activate
+msgid "Per activar"
+msgstr "Per activar"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__phone
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Phone"
 msgstr "Telèfon"
 
 #. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
@@ -1470,15 +1646,14 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__map_place_id
 msgid "Place reference"
 msgstr "Referència del lloc"
 
 #. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
-#: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
 #, python-format
 msgid "Place status filter not found slug_id: {}"
 msgstr "Filtres de status de punts no trobats per slug_id: {}"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
@@ -1487,21 +1662,21 @@
 #, python-format
 msgid "Platform"
 msgstr "Plataforma"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_platform_manager
 msgid "Platform Manager"
-msgstr "Manager de la plataforma"
+msgstr "Manager de la Plataforma"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.role_platform_admin_res_groups
 #: model:res.users.role,name:energy_communities.role_platform_admin
 msgid "Platform admin role"
-msgstr "Role d'administrador de la plataforma"
+msgstr "Role d'administrador de la Plataforma"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_partner_form
 msgid "Platform company"
 msgstr "Companyia Plataforma"
 
 #. module: energy_communities
@@ -1509,15 +1684,15 @@
 msgid "Please choose an option"
 msgstr "Tria una opció"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Please upload a scan of your ID card."
-msgstr ""
+msgstr "Puja una imatge del teu document d'identitat,"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__postal_code
 msgid "Postal code"
 msgstr "Codi Postal"
 
 #. module: energy_communities
@@ -1542,15 +1717,15 @@
 msgstr "Plantilla de producte"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Provided IBAN is not valid."
-msgstr "L'IBAN no és vàlid"
+msgstr "El IBAN no és vàlid."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/landing_page.py:0
 #, python-format
 msgid "Public data update successful"
 msgstr "Actualització de dades públiques efectuat amb èxit"
 
@@ -1566,15 +1741,15 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities.landing_page_form_view
 msgid "Published"
 msgstr "Publicat"
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.print_instance
 msgid "Push user to Keycloak"
-msgstr "Publicar usuari a Keycloak"
+msgstr "Puja l'usuari a Keycloak"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__realm_name
 msgid "Realm name"
 msgstr "Nom REALM"
 
 #. module: energy_communities
@@ -1616,31 +1791,24 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__hook_cron
 msgid "Run the post hook in a cron job or not"
 msgstr "Executa, o no, una acció posterior en un cron job"
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/account_chart_template.py:0
-#, python-format
-msgid "SUBJ"
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__landing_secondary_image_file
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__secondary_image_file
 msgid "Secondary Image"
 msgstr "Imatge secundària"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Send"
 msgstr "Enviar"
 
-
 #. module: energy_communities
 #: code:addons/energy_communities/models/landing_page.py:0
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__design_services
 #, python-format
 msgid "Services for the design and implementation of CCEE"
 msgstr "Serveis pel disseny i posada en marxa de CCEE"
 
@@ -1703,21 +1871,21 @@
 #: code:addons/energy_communities/wizards/assign_admin_wizard.py:0
 #, python-format
 msgid ""
 "Since you are not a coordinator admin you are not allowed to assign "
 "coordinator admins."
 msgstr ""
 "Al no ser usuari administrador coordinador no tens permís per assignar "
-"altres administradors coordinadors"
+"altres administradors coordinadors."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Some mandatory fields have not been filled."
-msgstr "Alguns camp obligatoris no s'han emplenat"
+msgstr "Alguns camps requerits no s'han establert."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_users.py:0
 #, python-format
 msgid "Something went wrong. Mail can not be sended. More details: {}"
 msgstr "Alguna cosa ha fallat. El correu no es pot enviar. Més detalls: {}"
 
@@ -1740,14 +1908,15 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__state_id
 msgid "State"
 msgstr "Província"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__status
+#: model:ir.model.fields,field_description:energy_communities.field_res_company__landing_page_status
 msgid "Status"
 msgstr "Estat"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_res_company__activity_state
 msgid ""
 "Status based on activities\n"
@@ -1771,28 +1940,23 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__street
 msgid "Street"
 msgstr "Carrer"
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_supply
 #: model:crm.tag,name:energy_communities.ce_tag_renewable_energy
 msgid "Subministrament d'energia 100% renovable"
-msgstr ""
+msgstr "Subministrament d'energia 100% renovable"
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/account_chart_template.py:0
-#, python-format
-msgid "Subscription Journal"
-msgstr "Diari de subscripcions"
-
-#. module: energy_communities
-#: model:ir.model,name:energy_communities.model_subscription_request
-msgid "Subscription Request"
-msgstr "Sol·licitud de Subscripció"
+#: model:cm.form.model,cta_button_label:energy_communities.map_form_model_campanya
+msgid "Sumar-m'hi"
+msgstr "Sumar-m'hi"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__superuser
 msgid "Superuser"
 msgstr "Super Usuari"
 
 #. module: energy_communities
@@ -1803,46 +1967,52 @@
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid "Target Odoo Company id"
 msgstr "Companyia Odoo de destí"
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__vat
-msgid "Tax ID"
-msgstr "NIF/CIF"
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__social_telegram
 msgid "Telegram Account"
 msgstr "Compte Telegram"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__ce_telegram_url
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__telegram_link
 msgid "Telegram link"
 msgstr "Enllaç de Telegram"
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_community_service.py:0
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #: code:addons/energy_communities/services/ce_member_service.py:0
-#: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid ""
 "The received oauth KeyCloak token have not been validated by KeyCloak : {}"
 msgstr "El oauth token rebut no ha estat validat per Keycloak: {}"
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid "The role code '{}' is not a valid one"
 msgstr "El rol '{}' no és vàlid"
 
 #. module: energy_communities
+#: code:addons/energy_communities/models/res_company.py:0
+#, python-format
+msgid ""
+"There has been a coordinator change             from [OLD:{outgoing_id}] "
+"{outgoing_name} to [NEW:{incoming_id}] {incoming_name},             Change "
+"reason: {change_reason}"
+msgstr ""
+"Hi ha hagut un canvi de Coordinadora             de [OLD:{outgoing_id}] "
+"{outgoing_name} a [NEW:{incoming_id}] {incoming_name},             Motiu "
+"del canvi: {change_reason}"
+
+#. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid ""
 "There is an existing account for this vat number on this community. Please "
 "contact with the community administrators."
 msgstr ""
 "En aquesta Comunitat ja existeix un compte amb el mateix NIF/CIF. Contacta "
@@ -1850,16 +2020,22 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_account_multicompany_easy_creation_wiz__property_cooperator_account
 msgid ""
 "This account will be the default one as the receivable account for the "
 "cooperators"
 msgstr ""
-"Aquest serà el compte per defecte per al cobrament de les aportacions de les"
-" sòcies"
+"Aquest serà el compte per defecte per al cobrament de les aportacions de "
+"les sòcies"
+
+#. module: energy_communities
+#: code:addons/energy_communities/wizards/change_coordinator_wizard.py:0
+#, python-format
+msgid "This community has been moved to a new coordinator"
+msgstr "La Comunitat ha sigut moguda a una nova Coordinadora"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "This company doesn't have a voluntary product share selected."
 msgstr ""
 "Aquesta empresa no ha seleccionat cap producte de aportació voluntària."
@@ -1883,34 +2059,28 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_res_company__cooperator_journal
 msgid ""
 "This journal will be the default one as the receivable journal for the "
 "cooperators"
 msgstr ""
-"Aquest diari serà el que s'usarà per defecte per als cobraments de les altes"
-" de sòcies"
+"Aquest diari serà el que s'usarà per defecte per als cobraments de les "
+"altes de sòcies"
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #, python-format
 msgid "This language code %s is not active in Odoo. Active ones: %s"
 msgstr "Aquest codi d'idioma %s no està actiu a l'Odoo. Els actius són: %s"
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/operation_request.py:0
-#, python-format
-msgid "This operation is not yet implemented."
-msgstr ""
-
-#. module: energy_communities
-#: code:addons/energy_communities/models/operation_request.py:0
-#, python-format
-msgid "This operation must be approved before to be executed"
-msgstr ""
+#: model:cm.map,categories_filter_title:energy_communities.map_campanya
+#: model:cm.map,proposal_form_subtitle_step_category:energy_communities.map_campanya
+msgid "Tipus de comunitat"
+msgstr "Tipus de comunitat"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
 "To be a member you must fulfill this form and lateron proceed to pay the "
 "initial share of"
@@ -1922,33 +2092,33 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
 "To join, you must first fill out this form where we ask for a bank account "
 "and authorization to issue a bank receipt to collect the initial mandatory "
 "financial contribution of"
 msgstr ""
-"Per ser soci/a, primer has d'omplir aquest formulari on et demanem un compte"
-" bancari i la autorització per girar un rebut bancari per cobrar la "
+"Per ser soci/a, primer has d'omplir aquest formulari on et demanem un "
+"compte bancari i la autorització per girar un rebut bancari per cobrar la "
 "aportació obligatòria inicial de"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
 msgid "Total"
-msgstr ""
+msgstr "Total"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__ce_twitter_url
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__twitter_link
 msgid "Twitter link"
 msgstr "Enllaç a Twitter"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_res_company__activity_exception_decoration
 msgid "Type of the exception activity on record."
-msgstr "Tipus d'excepció de l'activitat en un registre"
+msgstr "Tipus d'excepció de l'activitat en un registre."
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_utm_source
 msgid "UTM Source"
 msgstr "Origen UTM"
 
 #. module: energy_communities
@@ -1973,16 +2143,16 @@
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #, python-format
 msgid ""
 "Unable to update the lang in Keycloak for the related KC user ID: {}.{}"
 msgstr ""
-"No s'ha pogut actualizar l'idioma al KeyCloak pel usuari de KeyCloak amb ID:"
-" {}.{}"
+"No s'ha pogut actualizar l'idioma al KeyCloak pel usuari de KeyCloak amb "
+"ID: {}.{}"
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #, python-format
 msgid "Unable to validate the received oauth KeyCloak token: {}"
 msgstr "No s'ha pogut validar el Oauth token rebut: {}"
 
@@ -2032,20 +2202,20 @@
 #: model_terms:ir.ui.view,arch_db:energy_communities.form_field_image
 msgid "Upload a new one to change"
 msgstr "Carregueu-ne una de nou per canviar"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__creation_partner
 msgid "Use existing partner linked to new company"
-msgstr "Fer servir contacte existent per vincular-ho a la nova companyia."
+msgstr "Fer servir contacte existent per vincular-ho a la nova companyia"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_user
 msgid "User"
-msgstr "Usuari"
+msgstr "User"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__user_current_company
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__user_current_company
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__user_current_company
 #: model:ir.model.fields,field_description:energy_communities.field_user_currentcompany_mixin__user_current_company
 msgid "User Current Company"
@@ -2117,34 +2287,28 @@
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Voluntary Share of"
 msgstr "Aportació voluntària de"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
-#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
 msgid "Voluntary Shares"
 msgstr "Aportacions voluntàries"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_form_header_text
 msgid "Voluntary share form header text"
 msgstr "Text del formulari de participació voluntària"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_id
 msgid "Voluntary share to show on website"
 msgstr "Formulari d'aportació voluntària per ensenyar a la web"
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
-msgid "vol_share_eu_es"
-msgstr " "
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__wp_landing_page_id
 msgid "WP Landing Page"
 msgstr "Pàgina de destinació WP"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__website
 msgid "Website"
@@ -2165,19 +2329,18 @@
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__why_become_cooperator
 msgid "Why become cooperator"
 msgstr "Per què fer-se soci"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_multicompany_easy_creation_wiz
 msgid "Wizard Account Multi-company Easy Creation"
-msgstr ""
+msgstr "Wizard Account Multi-company Easy Creation"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
-#: code:addons/energy_communities/models/res_company.py:0
 #: code:addons/energy_communities/models/res_config_settings.py:0
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__wordpress_base_url
 #: model:ir.model.fields,field_description:energy_communities.field_res_config_settings__wordpress_base_url
 #, python-format
 msgid "Wordpress Base URL (JWT auth)"
 msgstr "URL base de Wordpress (autenticació JWT)"
 
@@ -2211,21 +2374,21 @@
 msgstr "Landing de wordpress i punt de mapa s'han actualitzat amb èxit."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid ""
 "You can't subscribe for an amount that exceeds {amount}{currency_symbol}."
-msgstr ""
+msgstr "No pots registrar una quantitat superior a {amount}{currency_symbol}."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "You can't subscribe to two different types of share."
-msgstr ""
+msgstr "No et pots registrar a dos tipus diferents d'aportacions."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "You cannot create a instance company with a parent company."
 msgstr ""
 "Ho hi pot haver una empresa de nivell Instància que tingui una empresa "
@@ -2234,39 +2397,14 @@
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "You must check the SEPA transference."
 msgstr "Has d'acceptar la transferència per SEPA."
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/account_move.py:0
-#, python-format
-msgid ""
-"You must have a company specific sequence number for register.operation"
-msgstr ""
-"Ha d'existir una sequència numèrica per register.operation específica per "
-"aquesta companyia"
-
-#. module: energy_communities
-#: code:addons/energy_communities/models/account_move.py:0
-#, python-format
-msgid ""
-"You must have a company specific sequence number for subscription.register"
-msgstr ""
-"Ha d'existir una sequència numèrica per subscription.register específica per"
-" aquesta companyia"
-
-#. module: energy_communities
-#: code:addons/energy_communities/models/subscription_request.py:0
-#, python-format
-msgid "You must set a cooperator journal on you company."
-msgstr ""
-"Cal sel·leccionar un Diari específic per a Sòcies en aquesta companyia."
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__zip_code
 msgid "ZIP code"
 msgstr "Codi postal"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
@@ -2283,68 +2421,535 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "and"
 msgstr "i"
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
-msgid "member_ccee_eu_ES."
-msgstr " "
-
-#. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
-#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
-msgid "member_eu_ES"
-msgstr " "
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__ce_status__building
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__ce_status__building
 #, python-format
 msgid "building"
-msgstr "En construcció"
+msgstr "en construcció"
+
+#. module: energy_communities
+#: model:ir.model,name:energy_communities.model_cm_filter
+msgid "cm.filter"
+msgstr "cm.filter"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_cm_map
 msgid "cm.map"
-msgstr ""
+msgstr "cm.map"
+
+#. module: energy_communities
+#: model:ir.model,name:energy_communities.model_cm_place
+msgid "cm.place"
+msgstr "cm.place"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__community_of_property
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__community_of_property
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__community_of_property
 #, python-format
 msgid "community of property"
-msgstr "Comunitat de Bens"
+msgstr "comunitat de bens"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.form_field_date_past
 msgid "dd/mm/aaaa"
-msgstr ""
+msgstr "dd/mm/aaaa"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.form_field_date_past
 msgid "dd/mm/yyyy"
-msgstr ""
+msgstr "dd/mm/aaaa"
+
+#. module: energy_communities
+#: model:cm.map,cookies_link:energy_communities.map_campanya
+msgid "https://somcomunitats.coop/politica-de-cookies/"
+msgstr "https://somcomunitats.coop/politica-de-cookies/"
+
+#. module: energy_communities
+#: model:cm.map,privacy_link:energy_communities.map_campanya
+msgid "https://somcomunitats.coop/politica-de-privacitat/"
+msgstr "https://somcomunitats.coop/politica-de-privacitat/"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_landing_page
 msgid "landing.page"
+msgstr "landing.page"
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
+msgid "member_ccee_eu_ES."
+msgstr " "
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
+#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
+msgid "member_eu_ES"
+msgstr " "
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
+msgid "vol_share_eu_es"
+msgstr " "
+
+#. module: energy_communities
+#: model:cm.form.model,json_uischema:energy_communities.map_form_model_campanya
+msgid ""
+"{\n"
+"  \"type\": \"VerticalLayout\",\n"
+"  \"elements\": [\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"label\": \"Dades de contacte\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"VerticalLayout\",\n"
+"          \"elements\": [\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/name\",\n"
+"              \"label\": \"Nom\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/surname\",\n"
+"              \"label\": \"Cognoms\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/email\",\n"
+"              \"label\": \"Correu electrònic\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/phone\",\n"
+"              \"label\": \"Telèfon\"\n"
+"            }\n"
+"          ]\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"label\": \"Com vols participar en la Comunitat?*\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"VerticalLayout\",\n"
+"          \"elements\": [\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_member_implication\",\n"
+"              \"label\": false,\n"
+"              \"options\": {\n"
+"                \"format\": \"radio\"\n"
+"               }\n"
+"            }\n"
+"          ]\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"label\": \"De quins Serveis energètics t'agradaria participar\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"VerticalLayout\",\n"
+"          \"elements\": [\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_common_generation\",\n"
+"              \"label\": \"Generació renovable comunitaria\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_sustainable_mobility\",\n"
+"              \"label\": \"Mobilitat sostenible\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_citizen_education\",\n"
+"              \"label\": \"Formació ciutadana\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_thermal_energy\",\n"
+"              \"label\": \"Energia tèrmica i climatització\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_collective_purchases\",\n"
+"              \"label\": \"Compres col.lectives\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_aggregate_demand\",\n"
+"              \"label\": \"Agregació i flexibilitat de la demanda\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_renewable_energy\",\n"
+"              \"label\": \"Subministrament d'energia 100% renovable\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_energy_efficiency\",\n"
+"              \"label\": \"Eficiencia energètica\"\n"
+"            }\n"
+"          ]\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"VerticalLayout\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/newsletter_info\",\n"
+"          \"options\": {\n"
+"            \"html\": \"<div class='p-1 border border-transparent empty:"
+"hidden text-sm text-gray-500'>Amb l'enviament d'aquest formulari, accepteu "
+"rebre notícies d'aquesta Comunitat</div>\"\n"
+"          }\n"
+"        }\n"
+"      ]\n"
+"    }\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.form.model,json_schema:energy_communities.map_form_model_campanya
+msgid ""
+"{\n"
+"  \"type\": \"object\",\n"
+"  \"properties\": {\n"
+"    \"name\": {\n"
+"      \"type\": \"string\",\n"
+"      \"minLength\": 2\n"
+"    },\n"
+"    \"surname\": {\n"
+"      \"type\": \"string\",\n"
+"      \"minLength\": 2\n"
+"    },\n"
+"    \"email\": {\n"
+"      \"type\": \"string\",\n"
+"      \"format\": \"email\"\n"
+"    },\n"
+"    \"phone\": {\n"
+"      \"type\": \"string\",\n"
+"      \"minLength\": 2\n"
+"    },\n"
+"    \"ce_member_implication\": {\n"
+"      \"type\": \"string\",\n"
+"      \"enum\": [\n"
+"        \"low\",        \n"
+"        \"medium\",\n"
+"        \"high\",\n"
+"        \"leadership\"\n"
+"      ],\n"
+"      \"i18n\": \"ce_member_implication\",\n"
+"      \"translations\": {\n"
+"        \"low\": \"No puc participar gaire\",\n"
+"        \"medium\": \"Puc participar una mica\",\n"
+"        \"high\": \"Vull i puc participar\",\n"
+"        \"leadership\": \"M'agradaria liderar i participar\"\n"
+"      }\n"
+"    },\n"
+"    \"ce_tag_common_generation\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_energy_efficiency\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_sustainable_mobility\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_citizen_education\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_thermal_energy\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_collective_purchases\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_renewable_energy\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_aggregate_demand\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"newsletter\": {\n"
+"      \"type\": \"boolean\"\n"
+"    }\n"
+"  },\n"
+"  \"required\": [\n"
+"    \"name\",\n"
+"    \"surname\",\n"
+"    \"email\",\n"
+"    \"phone\",\n"
+"    \"ce_member_implication\"\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_uischema:energy_communities.map_presenter_model_to_activate
+msgid ""
+"{\n"
+"  \"type\":\"VerticalLayout\",\n"
+"  \"elements\": [\n"
+"    {\n"
+"      \"type\": \"HorizontalLayout\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/pd_filter_state\",\n"
+"          \"backgroundColor\": \"#8ec23a\",\n"
+"          \"textColor\": \"#fff\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/pd_category\",\n"
+"          \"backgroundColor\": \"#e8f3ec\",\n"
+"          \"textColor\": \"#153f2d\"\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/pd_title\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/pd_description\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"EnergyActions\",\n"
+"      \"scope\": \"#/properties/pd_filter_energy_actions\",\n"
+"      \"backgroundColor\": \"#51ab50\",\n"
+"      \"textColor\": \"#fff\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"#c5e2d0\",\n"
+"      \"backgroundColor\": \"#FFFFFF\",\n"
+"      \"textColor\": \"#000000\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/pd_target_objective\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"label\": \"{% if submission_number %}{{submission_number}} "
+"interessades - {% endif %}{{goalProgress}}% completada\",\n"
+"          \"scope\": \"#/properties/progress\",\n"
+"          \"options\": { \"progress\": true }\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"InteractionButtons\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/pd_secondary_description\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"center\": true,\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"transparent\",\n"
+"      \"backgroundColor\": \"#153f2d\",\n"
+"      \"textColor\": \"#FFFFFF\",\n"
+"      \"showInResult\": true,\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/pd_social_headline\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"InteractionSocial\",\n"
+"          \"IconColor\": \"#153f2d\",\n"
+"          \"IconBackgroundColor\": \"#fff\"\n"
+"        }\n"
+"      ]\n"
+"    }\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_uischema:energy_communities.map_presenter_model_open
+msgid ""
+"{\n"
+"  \"type\":\"VerticalLayout\",\n"
+"  \"elements\": [\n"
+"    {\n"
+"      \"type\": \"HorizontalLayout\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/po2_filter_state\",\n"
+"          \"backgroundColor\": \"#8ec23a\",\n"
+"          \"textColor\": \"#fff\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/po2_category\",\n"
+"          \"backgroundColor\": \"#e8f3ec\",\n"
+"          \"textColor\": \"#153f2d\"\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/po2_title\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/po2_description\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"EnergyActions\",\n"
+"      \"scope\": \"#/properties/po2_filter_energy_actions\",\n"
+"      \"backgroundColor\": \"#51ab50\",\n"
+"      \"textColor\": \"#fff\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"#c5e2d0\",\n"
+"      \"backgroundColor\": \"#FFFFFF\",\n"
+"      \"textColor\": \"#000000\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"InteractionButtons\"\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"center\": true,\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"transparent\",\n"
+"      \"backgroundColor\": \"#153f2d\",\n"
+"      \"textColor\": \"#FFFFFF\",\n"
+"      \"showInResult\": true,\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/po2_social_headline\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"InteractionSocial\",\n"
+"          \"IconColor\": \"#153f2d\",\n"
+"          \"IconBackgroundColor\": \"#fff\"\n"
+"        }\n"
+"      ]\n"
+"    }\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_dataschema:energy_communities.map_presenter_model_to_activate
+msgid ""
+"{\n"
+"\"pd_title\": \"{{name}}\",\n"
+"\"pd_filter_state\": \"{% for filter in filters_data %}{% if filter.group "
+"== 'estat-actual-de-la-comunitat' %}<div class='flex items-center w-fit "
+"font-semibold'><i class='relative z-20 fas {% if filter.icon_class == "
+"'circle' %}fa-regular fa-circle {% endif %}{% if filter.icon_class == "
+"'circle-half-stroke' %}fa-sharp fa-regular fa-circle-half-stroke {% endif %}"
+"{% if filter.icon_class == 'circle-full' %}fa-solid fa-circle {% endif %}"
+"text-base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs "
+"sm:text-sm ml-2'>{{filter.name}}</div></div>{% endif %}{% endfor %}\",\n"
+"\"pd_category\": \"<div class='flex items-center w-fit font-semibold'><i "
+"class='relative z-20 fas fa-regular fa-{{category_data.icon_class}} text-"
+"base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs sm:"
+"text-sm ml-2'>{{category_data.name}}</div></div>\",\n"
+"\"pd_filter_energy_actions\": \"<div class='flex'>{% for filter in "
+"filters_data %}{% if filter.group == 'accions-energetiques' %}<div "
+"class='px-1'><label class='w-full p-2 cursor-pointer rounded border border-"
+"transparent hover:shadow-sm hover:border-gray-300'><div class='flex md:"
+"items-center pb-2'><div class='overflow-hidden relative flex-none mt-1 sm:"
+"mt-0 rounded-full p-2 h-6 w-6 xs:h-8 xs:w-8 h-10 w-10'><div class='overflow-"
+"hidden rounded-full absolute inset-0 z-10 flex items-center justify-center "
+"border'><div class='z-0 rounded-full absolute inset-0' style='background-"
+"color: red;'></div><div style='height: 100%;' class='z-10 absolute left-0 "
+"right-0 bottom-0'></div><i class='relative z-20 fas fa-regular fa-{{filter."
+"icon_class}} text-base'></i></div></div></div></label></div>{% endif %}{% "
+"endfor %}</div>\",\n"
+"\"pd_target_objective\": \"<p class='m-2'>Objectiu: "
+"<strong>{{ goalTarget }} {% if category_slug == 'industrial' %}empreses{% "
+"else %}persones{% endif %}</strong></p>\",\n"
+"\"progress\": \"<div class='flex justify-between'><div>{% if "
+"submission_number %}<strong>{{submission_number}}</strong> interessades</"
+"div><div>{% endif %}<strong>{{goalProgress}}%</strong> completada</div></"
+"div>\",\n"
+"\"pd_secondary_description\": \"<p class='m-2 mb-4 flex flex-col justify-"
+"center align-center text-center'>Ja esteu impulsant una comunitat en aquest "
+"municipi?<br><a href='https://somcomunitats.coop/alta-nova-comunitat?"
+"map_place_ref={{slug}}' target='_parent'>Sol·licita donar-la d’alta</a></"
+"p>\",\n"
+"\"pd_social_headline\": \"<div class='flex justify-center align-center text-"
+"center'><p class='font-semibold text-white'>Comparteix i fem créixer la "
+"Comunitat Energètica</p></div>\"\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_dataschema:energy_communities.map_presenter_model_open
+msgid ""
+"{\n"
+"\"po2_title\": \"{{name}}\",\n"
+"\"po2_filter_state\": \"{% for filter in filters_data %}{% if filter.group "
+"== 'estat-actual-de-la-comunitat' %}<div class='flex items-center w-fit "
+"font-semibold'><i class='relative z-20 fas {% if filter.icon_class == "
+"'circle' %}fa-regular fa-circle {% endif %}{% if filter.icon_class == "
+"'circle-half-stroke' %}fa-sharp fa-regular fa-circle-half-stroke {% endif %}"
+"{% if filter.icon_class == 'circle-full' %}fa-solid fa-circle {% endif %}"
+"text-base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs "
+"sm:text-sm ml-2'>{{filter.name}}</div></div>{% endif %}{% endfor %}\",\n"
+"\"po2_category\": \"<div class='flex items-center w-fit font-semibold'><i "
+"class='relative z-20 fas fa-regular fa-{{category_data.icon_class}} text-"
+"base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs sm:"
+"text-sm ml-2'>{{category_data.name}}</div></div>\",\n"
+"\"po2_filter_energy_actions\": \"<div class='flex'>{% for filter in "
+"filters_data %}{% if filter.group == 'accions-energetiques' %}<div "
+"class='px-1'><label class='w-full p-2 cursor-pointer rounded border border-"
+"transparent hover:shadow-sm hover:border-gray-300'><div class='flex md:"
+"items-center pb-2'><div class='overflow-hidden relative flex-none mt-1 sm:"
+"mt-0 rounded-full p-2 h-6 w-6 xs:h-8 xs:w-8 h-10 w-10'><div class='overflow-"
+"hidden rounded-full absolute inset-0 z-10 flex items-center justify-center "
+"border'><div class='z-0 rounded-full absolute inset-0' style='background-"
+"color: red;'></div><div style='height: 100%;' class='z-10 absolute left-0 "
+"right-0 bottom-0'></div><i class='relative z-20 fas fa-regular fa-{{filter."
+"icon_class}} text-base'></i></div></div></div></label></div>{% endif %}{% "
+"endfor %}</div>\",\n"
+"\"po2_social_headline\": \"<div class='flex justify-center align-center "
+"text-center'><p class='font-semibold text-white'>Comparteix i fem créixer "
+"la Comunitat Energètica</p></div>\"\n"
+"}"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid "€ by follow the steps you will receive by email."
 msgstr ""
 "€ seguint els passos que t'indicarem per correu electrònic un cop rebem la "
 "teva petició."
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid "€_eu_ES."
 msgstr "€."
-
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n/energy_communities.pot` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n/energy_communities.pot`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-26 12:51+0000\n"
-"PO-Revision-Date: 2024-03-26 12:51+0000\n"
+"POT-Creation-Date: 2024-05-31 09:56+0000\n"
+"PO-Revision-Date: 2024-05-31 09:56+0000\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
 
@@ -58,21 +58,31 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.form_field_date_past
 msgid "#{date_placeholder}"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.form.model,submission_ok_message:energy_communities.map_form_model_campanya
+msgid ""
+"<h1 class=\"text-lg font-semibold\">Formulari enviat.</h1><h2 class=\"text-"
+"lg font-medium\">Moltes gracies pel seu interès!</h2></br><div class=\"flex "
+"text-[#8a9f96]\">Quan hi hagi novetats amb la Comunitat Energètica "
+"contactarem amb tu i amb les persones que també han mostrat interès i us "
+"oferirem suport per activar-la. Som-hi!</div>"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser
 msgid "A super power user that is able to CRUD users on KC."
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model,name:energy_communities.model_account_chart_template
-msgid "Account Chart Template"
+#: model:cm.filter.group,name:energy_communities.map_filter_group_energy_actions
+msgid "Accions energètiques"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.constraint,message:energy_communities.constraint_account_multicompany_bank_wiz_unique_number
 #: model:ir.model.constraint,message:energy_communities.constraint_res_partner_bank_unique_number
 msgid "Account Number must be unique"
 msgstr ""
@@ -130,14 +140,20 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map__admins_to_notify
 msgid "Admins to notify"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.map,proposal_form_subtitle_step_address:energy_communities.map_campanya
+msgid "Adreça"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_flexibility
 #: model:crm.tag,name:energy_communities.ce_tag_aggregate_demand
 msgid "Agregació i flexibilitat de la demanda"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__allow_new_members
 msgid "Allow new members"
@@ -233,24 +249,57 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__crm_lead_id
 msgid "CRM Lead"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_assign_admin_wizard_form
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_change_coordinator_wizard_form
 msgid "Cancelar"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.map,searchbar_placeholder:energy_communities.map_campanya
+msgid "Cerca adreça o municipi"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_product_product__mail_template
 #: model:ir.model.fields,field_description:energy_communities.field_product_template__mail_template
 msgid "Certificate email template"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.actions.act_window,name:energy_communities.act_window_change_coordinator
+msgid "Change Coordinator"
+msgstr ""
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_change_coordinator_wizard_form
+msgid "Change Coordinator Wizard"
+msgstr ""
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/res_company.py:0
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
+#, python-format
+msgid "Change coordinator"
+msgstr ""
+
+#. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__change_reason
+msgid "Change reason"
+msgstr ""
+
+#. module: energy_communities
+#: model:ir.model,name:energy_communities.model_change_coordinator_wizard
+msgid "Change the coordinator of an existing energy community"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__chart_template_id
 msgid "Chart Template"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__landing_community_type__citizen
@@ -268,28 +317,34 @@
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "City not found"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.place.category,name:energy_communities.map_place_category_citizen
+msgid "Ciutadania"
+msgstr ""
+
+#. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_utm_sources_action
 msgid "Click to define a new Source."
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__ce_member_status__closed
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_status__closed
 #, python-format
 msgid "Closed"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__code
+#: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line__code
 msgid "Code"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__comercial_name
 msgid "Comercial name"
 msgstr ""
@@ -359,14 +414,26 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__company_id
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Company"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_res_company__logo
+msgid "Company Logo"
+msgstr ""
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/res_company.py:0
+#, python-format
+msgid ""
+"Company comercial name must be established in order to create a landing"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/wizards/multicompany_easy_creation.py:0
 #, python-format
 msgid "Company creation successful"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__company_hierarchy_level
@@ -378,14 +445,19 @@
 #: code:addons/energy_communities/models/landing_page.py:0
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__company_logo
 #, python-format
 msgid "Company logo"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_collective_purchases
+msgid "Compres col.lectives"
+msgstr ""
+
+#. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_collective_purchases
 msgid "Compres col·lectives"
 msgstr ""
 
 #. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_template_conditions_voluntary_share
 msgid ""
@@ -442,20 +514,14 @@
 
 #. module: energy_communities
 #: model:product.template,name:energy_communities.share_capital_product_template
 msgid "Contribution to Share Capital"
 msgstr ""
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/operation_request.py:0
-#, python-format
-msgid "Converting just part of the shares is not yet implemented"
-msgstr ""
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__cooperative
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__cooperative
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__cooperative
 #, python-format
 msgid "Cooperative"
 msgstr ""
@@ -477,14 +543,19 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__cooperator_share_form_header_text
 msgid "Cooperator share form header text"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter.group,name:energy_communities.map_filter_group_coordinator
+msgid "Coordinadora"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__hierarchy_level__coordinator
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__company_hierarchy_level__coordinator
 #, python-format
 msgid "Coordinator"
 msgstr ""
@@ -504,30 +575,51 @@
 #: model:res.groups,name:energy_communities.role_coord_worker_res_groups
 #: model:res.users.role,name:energy_communities.role_coord_worker
 #, python-format
 msgid "Coordinator Worker"
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/wizards/change_coordinator_wizard.py:0
+#, python-format
+msgid "Coordinator change successful"
+msgstr ""
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_partner_form
 msgid "Coordinator company"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_res_partner_filter
 msgid "Coordinators"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.map,proposal_cta_title:energy_communities.map_campanya
+msgid "Crea una comunitat"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.map,proposal_form_title:energy_communities.map_campanya
+msgid "Crea una comunitat al mapa"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__create_landing
 #: model_terms:ir.ui.view,arch_db:energy_communities.wizard_multicompany_easy_creation_form_inherit
 msgid "Create Landing"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__create_place
+msgid "Create Map Place"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.actions.act_window,name:energy_communities.action_open_assign_admin_wizard
 msgid "Create User"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
 msgid "Create landing page"
@@ -551,20 +643,22 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__create_user_in_keycloak
 msgid "Create user for keycloak"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__create_uid
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__create_uid
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__create_uid
 msgid "Created by"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__create_date
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__create_date
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__create_date
 msgid "Created on"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__current_role
 msgid "Current Role"
@@ -577,32 +671,33 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_users_form_form_inherit
 msgid "DNI"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_account_move__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_cm_coordinates_mixin__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map__display_name
+#: model:ir.model.fields,field_description:energy_communities.field_cm_place__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__display_name
-#: model:ir.model.fields,field_description:energy_communities.field_operation_request__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_product_template__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_config_settings__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner_bank__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line__display_name
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_user_currentcompany_mixin__display_name
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source__display_name
 msgid "Display Name"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__display_footer_doc_policy_text
@@ -614,14 +709,15 @@
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__status__draft
 #: model_terms:ir.ui.view,arch_db:energy_communities.landing_page_form_view
 #, python-format
 msgid "Draft"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_efficiency
 #: model:crm.tag,name:energy_communities.ce_tag_energy_efficiency
 msgid "Eficiencia energètica"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__email
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__email
@@ -639,14 +735,15 @@
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Email not found"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_thermal_energy
 #: model:crm.tag,name:energy_communities.ce_tag_thermal_energy
 msgid "Energia tèrmica i climatització"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.module.category,name:energy_communities.energy_communities_category
 #: model:ir.ui.menu,name:energy_communities.ce_root_menu
@@ -693,24 +790,44 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__ce_status
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__ce_status
 msgid "Energy Community state"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.form.model,button_label:energy_communities.map_form_model_campanya
+msgid "Enviar"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.filter.group,name:energy_communities.map_filter_group_community_status
+msgid "Estat actual de la comunitat"
+msgstr ""
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_change_coordinator_wizard_form
+msgid "Execute"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin__external_id
 msgid "External ID"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_external_id_mixin
 msgid "External ID Mixin"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__slug_id
+msgid "External slug ID"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__external_website_link
 msgid "External website link"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__ce_facebook_url
 msgid "Facebook link"
@@ -748,37 +865,47 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__footer_doc_policy_text
 msgid "Footer doc policy text"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_training
 #: model:crm.tag,name:energy_communities.ce_tag_citizen_education
 msgid "Formació ciutadana"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.map,proposal_form_subtitle_step_form:energy_communities.map_campanya
+msgid "Formulari de creació"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__foundation_date
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__foundation_date
 msgid "Foundation date"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__gender
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__gender
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__gender
 msgid "Gender"
 msgstr ""
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_common_generation
 msgid "Generació renovable comunitaria"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_generation
+msgid "Generació renovable comunitària"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__general_partnership
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__general_partnership
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__general_partnership
 #, python-format
 msgid "General partnership"
 msgstr ""
@@ -791,49 +918,50 @@
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Hello,"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__hierarchy_level
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__hierarchy_level
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__hierarchy_level
 msgid "Hierarchy level"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.iban_template_es_ccee
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
 msgid "I accept that the entity issues direct debit receipts to this account."
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_share
-#: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__id
+#: model:ir.model.fields,field_description:energy_communities.field_account_move__id
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__id
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__id
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__id
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__id
 #: model:ir.model.fields,field_description:energy_communities.field_cm_coordinates_mixin__id
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter__id
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map__id
+#: model:ir.model.fields,field_description:energy_communities.field_cm_place__id
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin__id
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__id
-#: model:ir.model.fields,field_description:energy_communities.field_operation_request__id
 #: model:ir.model.fields,field_description:energy_communities.field_product_template__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_config_settings__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner_bank__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line__id
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__id
 #: model:ir.model.fields,field_description:energy_communities.field_user_currentcompany_mixin__id
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source__id
 msgid "ID"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_mailing_mailing__source_ext_id
@@ -882,36 +1010,37 @@
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_product_product__mail_template
 #: model:ir.model.fields,help:energy_communities.field_product_template__mail_template
 msgid "If left empty, the default global mail template will be used."
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__incoming_coordinator
+msgid "Incoming Coordinator"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__individual_entrepreneur
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__individual_entrepreneur
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__individual_entrepreneur
 #, python-format
 msgid "Individual entrepreneur"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:cm.place.category,name:energy_communities.map_place_category_industrial
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__landing_community_type__industrial
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_type__industrial
 #, python-format
 msgid "Industrial"
 msgstr ""
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.ce_view_crm_case_opportunities_filter
-msgid "Info COORD"
-msgstr ""
-
-#. module: energy_communities
 #: model:utm.source,name:energy_communities.ce_source_general_info
 msgid "Information Newsletter (general)"
 msgstr ""
 
 #. module: energy_communities
 #: model:utm.source,name:energy_communities.ce_source_coord_web_other
 msgid "Information about coordinators"
@@ -929,19 +1058,14 @@
 
 #. module: energy_communities
 #: model:utm.source,name:energy_communities.ce_source_future_location_ce_info
 msgid "Information about future CE by location"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_res_company__initial_subscription_share_amount
-msgid "Initial Subscription Share Amount"
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__capital_share
 msgid "Initial capital share"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__ce_instagram_url
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__instagram_link
@@ -961,16 +1085,16 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__is_new_admin
 msgid "Is a new admin?"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__is_voluntary
-msgid "Is voluntary contribution"
+#: model:ir.model,name:energy_communities.model_account_move
+msgid "Journal Entry"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_keycloak_provider
 msgid "Keycloak provider"
 msgstr ""
 
@@ -996,58 +1120,66 @@
 #. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
 #, python-format
 msgid "Landing lng param required for place creation"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter__landing_id
+msgid "Landing page"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/cm_place.py:0
 #: model:ir.model.fields,field_description:energy_communities.field_cm_place__landing_reference
 #, python-format
 msgid "Landing reference"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__default_lang_id
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__lang
 msgid "Language"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_account_chart_template____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_account_move____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_cm_coordinates_mixin____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_cm_filter____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_cm_map____last_update
+#: model:ir.model.fields,field_description:energy_communities.field_cm_place____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_external_id_mixin____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page____last_update
-#: model:ir.model.fields,field_description:energy_communities.field_operation_request____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_product_template____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_company____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_config_settings____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner_bank____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_users____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role_line____last_update
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_user_currentcompany_mixin____last_update
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source____last_update
 msgid "Last Modified on"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__write_uid
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__write_uid
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__write_uid
 msgid "Last Updated by"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__write_date
+#: model:ir.model.fields,field_description:energy_communities.field_change_coordinator_wizard__write_date
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__write_date
 msgid "Last Updated on"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_assign_admin_wizard__last_name
 msgid "Last name"
@@ -1120,19 +1252,14 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__message_main_attachment_id
 msgid "Main Attachment"
 msgstr ""
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
-msgid "Mandatory Shares"
-msgstr ""
-
-#. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
 #, python-format
 msgid "Map not found slug_id: {}"
 msgstr ""
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.mass_mailing_super_user
@@ -1146,14 +1273,15 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__message_ids
 msgid "Messages"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_mobility
 #: model:crm.tag,name:energy_communities.ce_tag_sustainable_mobility
 msgid "Mobilitat sostenible"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__my_activity_date_deadline
 msgid "My Activity Deadline"
@@ -1161,14 +1289,19 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
 msgid "My landing page"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.map,external_link_cta_txt:energy_communities.map_campanya
+msgid "Més informació"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__company_hierarchy_level__none
 msgid "NONE"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__name
 msgid "Name"
@@ -1224,25 +1357,29 @@
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid "No Odoo User found for KeyCloak user id %s"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.map,noresults_msg:energy_communities.map_campanya
+msgid "No hem trobats resultats. Prova a canviar la configuració de filtres."
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__non_profit
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__non_profit
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__non_profit
 #, python-format
 msgid "Non profit association"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_binary
-#: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_binary
 msgid "Not binary"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
@@ -1299,14 +1436,19 @@
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_auth_oauth_provider
 msgid "OAuth2 provider"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_open
+msgid "Oberta"
+msgstr ""
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
 "Once you are a member you can enjoy the services available from the community and be part of a movement\n"
 "                of social and energy model transformation."
 msgstr ""
 
@@ -1330,29 +1472,29 @@
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__ce_member_status__open
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_status__open
 #, python-format
 msgid "Open"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model,name:energy_communities.model_operation_request
-msgid "Operation request"
-msgstr ""
-
-#. module: energy_communities
 #: model:crm.tag,name:energy_communities.pack_1
 msgid "Pack 1"
 msgstr ""
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.pack_2
 msgid "Pack 2"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__parent_id
+msgid "Parent Company"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__parent_id
 msgid "Parent Coordinator Company"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__parent_id_filtered_ids
 msgid "Parent Id Filtered"
@@ -1367,24 +1509,34 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "Parent company must be instance hierarchy level."
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model.fields,field_description:energy_communities.field_landing_page__parent_landing_id
+msgid "Parent landing page"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Partner not found"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_to_activate
+msgid "Per activar"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__phone
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Phone"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/client_map/resources/landing_cmplace.py:0
@@ -1547,20 +1699,14 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__hook_cron
 msgid "Run the post hook in a cron job or not"
 msgstr ""
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/account_chart_template.py:0
-#, python-format
-msgid "SUBJ"
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__landing_secondary_image_file
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__secondary_image_file
 msgid "Secondary Image"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
@@ -1668,14 +1814,15 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__state_id
 msgid "State"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__status
+#: model:ir.model.fields,field_description:energy_communities.field_res_company__landing_page_status
 msgid "Status"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_res_company__activity_state
 msgid ""
 "Status based on activities\n"
@@ -1695,27 +1842,22 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__street
 msgid "Street"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.filter,name:energy_communities.map_filter_supply
 #: model:crm.tag,name:energy_communities.ce_tag_renewable_energy
 msgid "Subministrament d'energia 100% renovable"
 msgstr ""
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/account_chart_template.py:0
-#, python-format
-msgid "Subscription Journal"
-msgstr ""
-
-#. module: energy_communities
-#: model:ir.model,name:energy_communities.model_subscription_request
-msgid "Subscription Request"
+#: model:cm.form.model,cta_button_label:energy_communities.map_form_model_campanya
+msgid "Sumar-m'hi"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__superuser
 msgid "Superuser"
 msgstr ""
 
@@ -1727,19 +1869,14 @@
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid "Target Odoo Company id"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields,field_description:energy_communities.field_subscription_request__vat
-msgid "Tax ID"
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__social_telegram
 msgid "Telegram Account"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__ce_telegram_url
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__telegram_link
@@ -1759,14 +1896,23 @@
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid "The role code '{}' is not a valid one"
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/models/res_company.py:0
+#, python-format
+msgid ""
+"There has been a coordinator change             from [OLD:{outgoing_id}] "
+"{outgoing_name} to [NEW:{incoming_id}] {incoming_name},             Change "
+"reason: {change_reason}"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid ""
 "There is an existing account for this vat number on this community. Please "
 "contact with the community administrators."
 msgstr ""
 
@@ -1774,14 +1920,20 @@
 #: model:ir.model.fields,help:energy_communities.field_account_multicompany_easy_creation_wiz__property_cooperator_account
 msgid ""
 "This account will be the default one as the receivable account for the "
 "cooperators"
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/wizards/change_coordinator_wizard.py:0
+#, python-format
+msgid "This community has been moved to a new coordinator"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "This company doesn't have a voluntary product share selected."
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
@@ -1806,23 +1958,17 @@
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #, python-format
 msgid "This language code %s is not active in Odoo. Active ones: %s"
 msgstr ""
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/operation_request.py:0
-#, python-format
-msgid "This operation is not yet implemented."
-msgstr ""
-
-#. module: energy_communities
-#: code:addons/energy_communities/models/operation_request.py:0
-#, python-format
-msgid "This operation must be approved before to be executed"
+#: model:cm.map,categories_filter_title:energy_communities.map_campanya
+#: model:cm.map,proposal_form_subtitle_step_category:energy_communities.map_campanya
+msgid "Tipus de comunitat"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
 "To be a member you must fulfill this form and lateron proceed to pay the "
@@ -2017,34 +2163,28 @@
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Voluntary Share of"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.view_company_form_ce_inherited
-#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
 msgid "Voluntary Shares"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_form_header_text
 msgid "Voluntary share form header text"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_id
 msgid "Voluntary share to show on website"
 msgstr ""
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
-msgid "vol_share_eu_es"
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_landing_page__wp_landing_page_id
 msgid "WP Landing Page"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__website
 msgid "Website"
@@ -2132,34 +2272,14 @@
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "You must check the SEPA transference."
 msgstr ""
 
 #. module: energy_communities
-#: code:addons/energy_communities/models/account_move.py:0
-#, python-format
-msgid ""
-"You must have a company specific sequence number for register.operation"
-msgstr ""
-
-#. module: energy_communities
-#: code:addons/energy_communities/models/account_move.py:0
-#, python-format
-msgid ""
-"You must have a company specific sequence number for subscription.register"
-msgstr ""
-
-#. module: energy_communities
-#: code:addons/energy_communities/models/subscription_request.py:0
-#, python-format
-msgid "You must set a cooperator journal on you company."
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__zip_code
 msgid "ZIP code"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
@@ -2176,38 +2296,37 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "and"
 msgstr ""
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
-msgid "member_ccee_eu_ES."
-msgstr ""
-
-#. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
-#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
-msgid "member_eu_ES"
-msgstr ""
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__ce_status__building
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__ce_status__building
 #, python-format
 msgid "building"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model,name:energy_communities.model_cm_filter
+msgid "cm.filter"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model,name:energy_communities.model_cm_map
 msgid "cm.map"
 msgstr ""
 
 #. module: energy_communities
+#: model:ir.model,name:energy_communities.model_cm_place
+msgid "cm.place"
+msgstr ""
+
+#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #: model:ir.model.fields.selection,name:energy_communities.selection__account_multicompany_easy_creation_wiz__legal_form__community_of_property
 #: model:ir.model.fields.selection,name:energy_communities.selection__landing_page__community_secondary_type__community_of_property
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_company__legal_form__community_of_property
 #, python-format
 msgid "community of property"
 msgstr ""
@@ -2219,23 +2338,433 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.form_field_date_past
 msgid "dd/mm/yyyy"
 msgstr ""
 
 #. module: energy_communities
+#: model:cm.map,cookies_link:energy_communities.map_campanya
+msgid "https://somcomunitats.coop/politica-de-cookies/"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.map,privacy_link:energy_communities.map_campanya
+msgid "https://somcomunitats.coop/politica-de-privacitat/"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model,name:energy_communities.model_landing_page
 msgid "landing.page"
 msgstr ""
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
+msgid "member_ccee_eu_ES."
+msgstr ""
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
-msgid "€ by follow the steps you will receive by email."
+msgid "member_eu_ES"
+msgstr ""
+
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
+msgid "vol_share_eu_es"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.form.model,json_uischema:energy_communities.map_form_model_campanya
+msgid ""
+"{\n"
+"  \"type\": \"VerticalLayout\",\n"
+"  \"elements\": [\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"label\": \"Dades de contacte\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"VerticalLayout\",\n"
+"          \"elements\": [\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/name\",\n"
+"              \"label\": \"Nom\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/surname\",\n"
+"              \"label\": \"Cognoms\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/email\",\n"
+"              \"label\": \"Correu electrònic\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/phone\",\n"
+"              \"label\": \"Telèfon\"\n"
+"            }\n"
+"          ]\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"label\": \"Com vols participar en la Comunitat?*\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"VerticalLayout\",\n"
+"          \"elements\": [\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_member_implication\",\n"
+"              \"label\": false,\n"
+"              \"options\": {\n"
+"                \"format\": \"radio\"\n"
+"               }\n"
+"            }\n"
+"          ]\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"label\": \"De quins Serveis energètics t'agradaria participar\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"VerticalLayout\",\n"
+"          \"elements\": [\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_common_generation\",\n"
+"              \"label\": \"Generació renovable comunitaria\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_sustainable_mobility\",\n"
+"              \"label\": \"Mobilitat sostenible\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_citizen_education\",\n"
+"              \"label\": \"Formació ciutadana\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_thermal_energy\",\n"
+"              \"label\": \"Energia tèrmica i climatització\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_collective_purchases\",\n"
+"              \"label\": \"Compres col.lectives\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_aggregate_demand\",\n"
+"              \"label\": \"Agregació i flexibilitat de la demanda\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_renewable_energy\",\n"
+"              \"label\": \"Subministrament d'energia 100% renovable\"\n"
+"            },\n"
+"            {\n"
+"              \"type\": \"Control\",\n"
+"              \"scope\": \"#/properties/ce_tag_energy_efficiency\",\n"
+"              \"label\": \"Eficiencia energètica\"\n"
+"            }\n"
+"          ]\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"VerticalLayout\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/newsletter_info\",\n"
+"          \"options\": {\n"
+"            \"html\": \"<div class='p-1 border border-transparent empty:hidden text-sm text-gray-500'>Amb l'enviament d'aquest formulari, accepteu rebre notícies d'aquesta Comunitat</div>\"\n"
+"          }\n"
+"        }\n"
+"      ]\n"
+"    }\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.form.model,json_schema:energy_communities.map_form_model_campanya
+msgid ""
+"{\n"
+"  \"type\": \"object\",\n"
+"  \"properties\": {\n"
+"    \"name\": {\n"
+"      \"type\": \"string\",\n"
+"      \"minLength\": 2\n"
+"    },\n"
+"    \"surname\": {\n"
+"      \"type\": \"string\",\n"
+"      \"minLength\": 2\n"
+"    },\n"
+"    \"email\": {\n"
+"      \"type\": \"string\",\n"
+"      \"format\": \"email\"\n"
+"    },\n"
+"    \"phone\": {\n"
+"      \"type\": \"string\",\n"
+"      \"minLength\": 2\n"
+"    },\n"
+"    \"ce_member_implication\": {\n"
+"      \"type\": \"string\",\n"
+"      \"enum\": [\n"
+"        \"low\",        \n"
+"        \"medium\",\n"
+"        \"high\",\n"
+"        \"leadership\"\n"
+"      ],\n"
+"      \"i18n\": \"ce_member_implication\",\n"
+"      \"translations\": {\n"
+"        \"low\": \"No puc participar gaire\",\n"
+"        \"medium\": \"Puc participar una mica\",\n"
+"        \"high\": \"Vull i puc participar\",\n"
+"        \"leadership\": \"M'agradaria liderar i participar\"\n"
+"      }\n"
+"    },\n"
+"    \"ce_tag_common_generation\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_energy_efficiency\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_sustainable_mobility\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_citizen_education\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_thermal_energy\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_collective_purchases\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_renewable_energy\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"ce_tag_aggregate_demand\": {\n"
+"      \"type\": \"boolean\"\n"
+"    },\n"
+"    \"newsletter\": {\n"
+"      \"type\": \"boolean\"\n"
+"    }\n"
+"  },\n"
+"  \"required\": [\n"
+"    \"name\",\n"
+"    \"surname\",\n"
+"    \"email\",\n"
+"    \"phone\",\n"
+"    \"ce_member_implication\"\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_uischema:energy_communities.map_presenter_model_to_activate
+msgid ""
+"{\n"
+"  \"type\":\"VerticalLayout\",\n"
+"  \"elements\": [\n"
+"    {\n"
+"      \"type\": \"HorizontalLayout\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/pd_filter_state\",\n"
+"          \"backgroundColor\": \"#8ec23a\",\n"
+"          \"textColor\": \"#fff\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/pd_category\",\n"
+"          \"backgroundColor\": \"#e8f3ec\",\n"
+"          \"textColor\": \"#153f2d\"\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/pd_title\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/pd_description\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"EnergyActions\",\n"
+"      \"scope\": \"#/properties/pd_filter_energy_actions\",\n"
+"      \"backgroundColor\": \"#51ab50\",\n"
+"      \"textColor\": \"#fff\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"#c5e2d0\",\n"
+"      \"backgroundColor\": \"#FFFFFF\",\n"
+"      \"textColor\": \"#000000\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/pd_target_objective\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"label\": \"{% if submission_number %}{{submission_number}} interessades - {% endif %}{{goalProgress}}% completada\",\n"
+"          \"scope\": \"#/properties/progress\",\n"
+"          \"options\": { \"progress\": true }\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"InteractionButtons\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/pd_secondary_description\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"center\": true,\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"transparent\",\n"
+"      \"backgroundColor\": \"#153f2d\",\n"
+"      \"textColor\": \"#FFFFFF\",\n"
+"      \"showInResult\": true,\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/pd_social_headline\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"InteractionSocial\",\n"
+"          \"IconColor\": \"#153f2d\",\n"
+"          \"IconBackgroundColor\": \"#fff\"\n"
+"        }\n"
+"      ]\n"
+"    }\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_uischema:energy_communities.map_presenter_model_open
+msgid ""
+"{\n"
+"  \"type\":\"VerticalLayout\",\n"
+"  \"elements\": [\n"
+"    {\n"
+"      \"type\": \"HorizontalLayout\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/po2_filter_state\",\n"
+"          \"backgroundColor\": \"#8ec23a\",\n"
+"          \"textColor\": \"#fff\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"Container\",\n"
+"          \"scope\": \"#/properties/po2_category\",\n"
+"          \"backgroundColor\": \"#e8f3ec\",\n"
+"          \"textColor\": \"#153f2d\"\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/po2_title\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Display\",\n"
+"      \"scope\": \"#/properties/po2_description\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"EnergyActions\",\n"
+"      \"scope\": \"#/properties/po2_filter_energy_actions\",\n"
+"      \"backgroundColor\": \"#51ab50\",\n"
+"      \"textColor\": \"#fff\"\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"#c5e2d0\",\n"
+"      \"backgroundColor\": \"#FFFFFF\",\n"
+"      \"textColor\": \"#000000\",\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"InteractionButtons\"\n"
+"        }\n"
+"      ]\n"
+"    },\n"
+"    {\n"
+"      \"type\": \"Group\",\n"
+"      \"center\": true,\n"
+"      \"border\": true,\n"
+"      \"borderColor\": \"transparent\",\n"
+"      \"backgroundColor\": \"#153f2d\",\n"
+"      \"textColor\": \"#FFFFFF\",\n"
+"      \"showInResult\": true,\n"
+"      \"elements\": [\n"
+"        {\n"
+"          \"type\": \"Display\",\n"
+"          \"scope\": \"#/properties/po2_social_headline\"\n"
+"        },\n"
+"        {\n"
+"          \"type\": \"InteractionSocial\",\n"
+"          \"IconColor\": \"#153f2d\",\n"
+"          \"IconBackgroundColor\": \"#fff\"\n"
+"        }\n"
+"      ]\n"
+"    }\n"
+"  ]\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_dataschema:energy_communities.map_presenter_model_to_activate
+msgid ""
+"{\n"
+"\"pd_title\": \"{{name}}\",\n"
+"\"pd_filter_state\": \"{% for filter in filters_data %}{% if filter.group == 'estat-actual-de-la-comunitat' %}<div class='flex items-center w-fit font-semibold'><i class='relative z-20 fas {% if filter.icon_class == 'circle' %}fa-regular fa-circle {% endif %}{% if filter.icon_class == 'circle-half-stroke' %}fa-sharp fa-regular fa-circle-half-stroke {% endif %}{% if filter.icon_class == 'circle-full' %}fa-solid fa-circle {% endif %}text-base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs sm:text-sm ml-2'>{{filter.name}}</div></div>{% endif %}{% endfor %}\",\n"
+"\"pd_category\": \"<div class='flex items-center w-fit font-semibold'><i class='relative z-20 fas fa-regular fa-{{category_data.icon_class}} text-base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs sm:text-sm ml-2'>{{category_data.name}}</div></div>\",\n"
+"\"pd_filter_energy_actions\": \"<div class='flex'>{% for filter in filters_data %}{% if filter.group == 'accions-energetiques' %}<div class='px-1'><label class='w-full p-2 cursor-pointer rounded border border-transparent hover:shadow-sm hover:border-gray-300'><div class='flex md:items-center pb-2'><div class='overflow-hidden relative flex-none mt-1 sm:mt-0 rounded-full p-2 h-6 w-6 xs:h-8 xs:w-8 h-10 w-10'><div class='overflow-hidden rounded-full absolute inset-0 z-10 flex items-center justify-center border'><div class='z-0 rounded-full absolute inset-0' style='background-color: red;'></div><div style='height: 100%;' class='z-10 absolute left-0 right-0 bottom-0'></div><i class='relative z-20 fas fa-regular fa-{{filter.icon_class}} text-base'></i></div></div></div></label></div>{% endif %}{% endfor %}</div>\",\n"
+"\"pd_target_objective\": \"<p class='m-2'>Objectiu: <strong>{{ goalTarget }} {% if category_slug == 'industrial' %}empreses{% else %}persones{% endif %}</strong></p>\",\n"
+"\"progress\": \"<div class='flex justify-between'><div>{% if submission_number %}<strong>{{submission_number}}</strong> interessades</div><div>{% endif %}<strong>{{goalProgress}}%</strong> completada</div></div>\",\n"
+"\"pd_secondary_description\": \"<p class='m-2 mb-4 flex flex-col justify-center align-center text-center'>Ja esteu impulsant una comunitat en aquest municipi?<br><a href='https://somcomunitats.coop/alta-nova-comunitat?map_place_ref={{slug}}' target='_parent'>Sol·licita donar-la d’alta</a></p>\",\n"
+"\"pd_social_headline\": \"<div class='flex justify-center align-center text-center'><p class='font-semibold text-white'>Comparteix i fem créixer la Comunitat Energètica</p></div>\"\n"
+"}"
+msgstr ""
+
+#. module: energy_communities
+#: model:cm.presenter.model,json_dataschema:energy_communities.map_presenter_model_open
+msgid ""
+"{\n"
+"\"po2_title\": \"{{name}}\",\n"
+"\"po2_filter_state\": \"{% for filter in filters_data %}{% if filter.group == 'estat-actual-de-la-comunitat' %}<div class='flex items-center w-fit font-semibold'><i class='relative z-20 fas {% if filter.icon_class == 'circle' %}fa-regular fa-circle {% endif %}{% if filter.icon_class == 'circle-half-stroke' %}fa-sharp fa-regular fa-circle-half-stroke {% endif %}{% if filter.icon_class == 'circle-full' %}fa-solid fa-circle {% endif %}text-base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs sm:text-sm ml-2'>{{filter.name}}</div></div>{% endif %}{% endfor %}\",\n"
+"\"po2_category\": \"<div class='flex items-center w-fit font-semibold'><i class='relative z-20 fas fa-regular fa-{{category_data.icon_class}} text-base'></i><div class='text-sm cursor-pointer sm:font-semibold text-xs sm:text-sm ml-2'>{{category_data.name}}</div></div>\",\n"
+"\"po2_filter_energy_actions\": \"<div class='flex'>{% for filter in filters_data %}{% if filter.group == 'accions-energetiques' %}<div class='px-1'><label class='w-full p-2 cursor-pointer rounded border border-transparent hover:shadow-sm hover:border-gray-300'><div class='flex md:items-center pb-2'><div class='overflow-hidden relative flex-none mt-1 sm:mt-0 rounded-full p-2 h-6 w-6 xs:h-8 xs:w-8 h-10 w-10'><div class='overflow-hidden rounded-full absolute inset-0 z-10 flex items-center justify-center border'><div class='z-0 rounded-full absolute inset-0' style='background-color: red;'></div><div style='height: 100%;' class='z-10 absolute left-0 right-0 bottom-0'></div><i class='relative z-20 fas fa-regular fa-{{filter.icon_class}} text-base'></i></div></div></div></label></div>{% endif %}{% endfor %}</div>\",\n"
+"\"po2_social_headline\": \"<div class='flex justify-center align-center text-center'><p class='font-semibold text-white'>Comparteix i fem créixer la Comunitat Energètica</p></div>\"\n"
+"}"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
-msgid "€_eu_ES."
+msgid "€ by follow the steps you will receive by email."
 msgstr ""
 
+#. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
+msgid "€_eu_ES."
+msgstr ""
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n_extra/ca_ES.po` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n_extra/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n_extra/es.po` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n_extra/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/i18n_extra/eu_ES.po` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/i18n_extra/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/migrations/14.0.1.1.12/post-add-internal-user-role.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/migrations/14.0.1.1.12/post-add-internal-user-role.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/migrations/14.0.5.1.0/post-setup-multicompany-partner.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/migrations/14.0.5.1.0/post-setup-multicompany-partner.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/account_move.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/account_move.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/auth_oauth_provider.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/auth_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/cm_place.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/cm_place.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/landing_page.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/landing_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,15 @@
     )
     design_services = fields.Text(
         string=_("Services for the design and implementation of CCEE"), translate=True
     )
     management_services = fields.Text(
         string=_("CCEE management services"), translate=True
     )
-    company_logo = fields.Image(string=_("Company logo"))
-
-    slug_id = fields.Char(string="External slug ID", translate=True)
-
+    company_logo = fields.Image(string=_("Company logo"), related="company_id.logo")
     hierarchy_level = fields.Selection(
         selection=_HIERARCHY_LEVEL_VALUES,
         string="Hierarchy level",
         related="company_id.hierarchy_level",
     )
     parent_id = fields.Many2one(
         "res.company",
@@ -163,56 +160,70 @@
         self.update_translation(
             "landing.page,slug_id",
             self.slug_id,
             self.slug_id,
             "es_ES",
         )
 
-    def _get_image_attachment(self, field_name):
-        file_attachment = self.env["ir.attachment"].search(
-            [
+    def _get_image_attachment(self, field_name, query):
+        if not query:
+            query = [
                 ("res_id", "=", self.id),
                 ("res_model", "=", "landing.page"),
                 ("res_field", "=", field_name),
             ]
-        )
+        file_attachment = self.env["ir.attachment"].search(query)
         return file_attachment
 
-    def _get_image_write_date(self, field_name):
+    def _get_image_write_date(self, field_name, query=False):
         file_write_date = ""
-        file_attachment = self._get_image_attachment(field_name)
+        file_attachment = self._get_image_attachment(field_name, query)
         if file_attachment:
             file_write_date = str(file_attachment.write_date)
         return file_write_date
 
-    def _get_image_extension(self, field_name):
+    def _get_image_extension(self, field_name, query):
         file_write_date = ""
-        file_attachment = self._get_image_attachment(field_name)
+        file_attachment = self._get_image_attachment(field_name, query)
         extension = ""
         if file_attachment:
             extension = file_attachment.mimetype.split("/")[1]
         return extension
 
-    def _get_image_payload(self, field_name):
+    def _get_image_payload(self, field_name, query=False):
         base_url = self.env["ir.config_parameter"].get_param("web.base.url")
         return (
             base_url
             + "/web/image/landing.page/"
             + str(self.id)
             + "/"
             + field_name
             + "/"
             + str(self.id)
             + "-"
             + field_name
             + "."
-            + self._get_image_extension(field_name)
+            + self._get_image_extension(field_name, query)
         )
 
     def to_dict(self):
+        if self.company_logo:
+            attachment_query = [
+                ("res_id", "=", self.company_id.id),
+                ("res_model", "=", "res.company"),
+                ("res_field", "=", "logo"),
+            ]
+            company_logo = self._get_image_payload("company_logo", attachment_query)
+            company_logo_write_date = self._get_image_write_date(
+                "company_logo", attachment_query
+            )
+
+        else:
+            company_logo = ""
+            company_logo_write_date = ""
         if self.primary_image_file:
             primary_image_file = self._get_image_payload("primary_image_file")
             primary_image_file_write_date = self._get_image_write_date(
                 "primary_image_file"
             )
         else:
             primary_image_file = ""
@@ -221,20 +232,14 @@
             secondary_image_file = self._get_image_payload("secondary_image_file")
             secondary_image_file_write_date = self._get_image_write_date(
                 "secondary_image_file"
             )
         else:
             secondary_image_file = ""
             secondary_image_file_write_date = ""
-        if self.company_logo:
-            company_logo = self._get_image_payload("company_logo")
-            company_logo_write_date = self._get_image_write_date("company_logo")
-        else:
-            company_logo = ""
-            company_logo_write_date = ""
         if self.map_place_id:
             map_reference = self.map_place_id.slug_id
         else:
             map_reference = ""
         if self.why_become_cooperator == "<p><br></p>":
             self.why_become_cooperator = ""
         if self.become_cooperator_process == "<p><br></p>":
@@ -301,26 +306,26 @@
     def action_landing_page_status(self):
         for record in self:
             new_status = "draft" if record.status == "publish" else "publish"
             record.write({"status": new_status})
 
     def action_create_landing_place(self):
         for record in self:
-            record.create_landing_place()
+            record.sudo().create_landing_place()
 
     def action_update_public_data(self):
         for record in self:
             record._update_wordpress()
             if self.map_place_id:
-                record._update_landing_place()
+                record.sudo()._update_landing_place()
             if self.hierarchy_level == "coordinator":
                 if self.status == "publish":
-                    self.create_or_update_and_apply_coordinator_filter()
+                    self.sudo().create_or_update_and_apply_coordinator_filter()
                 else:
-                    self.remove_coordinator_filter_to_existing_communities()
+                    self.sudo().remove_coordinator_filter_to_existing_communities()
             self.write({"publicdata_lastupdate_datetime": datetime.now()})
             return {
                 "type": "ir.actions.client",
                 "tag": "display_notification",
                 "params": {
                     "type": "success",
                     "title": _("Public data update successful"),
@@ -357,28 +362,29 @@
 
     def company_hierarchy_level_url(self):
         if self.hierarchy_level == "coordinator":
             return "rest-ce-coord"
         else:
             return "rest-ce-landing"
 
-    def get_map_coordinator_filter_in_related_place(self, coordinator_landing=False):
-        if not coordinator_landing:
+    def get_map_coordinator_filter_in_related_place(self, coordinator=False):
+        if not coordinator:
             if self.parent_landing_id:
-                coordinator_landing = self.parent_landing_id
-        if self.hierarchy_level == "community" and coordinator_landing:
-            coordinator_filter_group = self.env.ref(
-                "energy_communities.map_filter_group_coordinator"
-            )
-            return self.env["cm.filter"].search(
-                [
-                    ("landing_id", "=", coordinator_landing.id),
-                    ("filter_group_id", "=", coordinator_filter_group.id),
-                ]
-            )
+                coordinator = self.parent_landing_id
+        if self.hierarchy_level == "community" and coordinator:
+            if coordinator.landing_page_id:
+                coordinator_filter_group = self.env.ref(
+                    "energy_communities.map_filter_group_coordinator"
+                )
+                return self.env["cm.filter"].search(
+                    [
+                        ("landing_id", "=", coordinator.landing_page_id.id),
+                        ("filter_group_id", "=", coordinator_filter_group.id),
+                    ]
+                )
         return False
 
     def create_or_update_and_apply_coordinator_filter(self):
         self.create_or_update_map_coordinator_filter()
         self.apply_coordinator_filter_to_existing_communities()
 
     def create_or_update_map_coordinator_filter(self):
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/product.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/product.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_company.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_company.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 ]
 
 
 class ResCompany(models.Model):
     _name = "res.company"
     _inherit = ["res.company", "mail.thread", "mail.activity.mixin"]
 
+    def _get_logo(self):
+        return super()._get_logo()
+
+    logo = fields.Image(default=_get_logo, string="Company Logo")
     hierarchy_level = fields.Selection(
         selection=_HIERARCHY_LEVEL_VALUES,
         required=True,
         string="Hierarchy level",
         default="community",
     )
     parent_id_filtered_ids = fields.One2many(
@@ -94,14 +98,15 @@
     )
     comercial_name = fields.Char(string="Comercial name")
     ce_status = fields.Selection(
         selection=_CE_STATUS_VALUES,
         string="Energy Community state",
     )
     landing_page_id = fields.Many2one("landing.page", string=_("Landing Page"))
+    landing_page_status = fields.Selection(related="landing_page_id.status")
     wordpress_db_username = fields.Char(string=_("Wordpress DB Admin Username"))
     wordpress_db_password = fields.Char(string=_("Wordpress DB Admin Password"))
     wordpress_base_url = fields.Char(string=_("Wordpress Base URL (JWT auth)"))
     footer_doc_policy_text = fields.Html(
         string="Footer doc policy text", translate=True
     )
     display_footer_doc_policy_text = fields.Boolean("Display footer doc policy text")
@@ -311,14 +316,20 @@
         # TODO: Get from landing page or company, for now we don't need
         return ""
 
     def get_keycloak_odoo_login_url(self):
         login_provider_id = self.env.ref("energy_communities.keycloak_login_provider")
         return login_provider_id.get_auth_link()
 
+    def company_hierarchy_level_url(self):
+        if self.hierarchy_level == "coordinator":
+            return "rest-ce-coord"
+        else:
+            return "rest-ce-landing"
+
     # LANDING
     def create_landing(self):
         if not self.comercial_name:
             raise ValidationError(
                 _(
                     "Company comercial name must be established in order to create a landing"
                 )
@@ -329,15 +340,15 @@
 
     def action_create_odoo_landing(self):
         landing_page = self.env["landing.page"]
         vals = {"company_id": self.id, "name": self.comercial_name, "status": "draft"}
         new_landing = landing_page.create(vals)
         new_landing.setup_slug_id()
         if self.hierarchy_level == "coordinator":
-            new_landing.create_or_update_and_apply_coordinator_filter()
+            new_landing.sudo().create_or_update_and_apply_coordinator_filter()
         self.write({"landing_page_id": new_landing.id})
         return new_landing
 
     def action_create_wp_landing(self, fields=None):
         instance_company = self.env["res.company"].search(
             [("hierarchy_level", "=", "instance")]
         )
@@ -359,19 +370,120 @@
             "view_type": "form",
             "view_mode": "form",
             "res_model": "landing.page",
             "res_id": self.landing_page_id.id,
             "target": "current",
         }
 
-    def company_hierarchy_level_url(self):
-        if self.hierarchy_level == "coordinator":
-            return "rest-ce-coord"
-        else:
-            return "rest-ce-landing"
+    # CHANGE COORDINATOR
+    def action_open_change_coordinator_wizard(self):
+        wizard = self.env["change.coordinator.wizard"].create({})
+        return {
+            "type": "ir.actions.act_window",
+            "name": _("Change coordinator"),
+            "res_model": "change.coordinator.wizard",
+            "view_type": "form",
+            "view_mode": "form",
+            "target": "new",
+            "res_id": wizard.id,
+        }
+
+    def change_coordinator(self, incoming_coordinator, change_reason):
+        outgoing_coordinator = self.parent_id
+        if incoming_coordinator.id != outgoing_coordinator.id:
+            # Change parent_id
+            self.write({"parent_id": incoming_coordinator.id})
+            # Add coordinator_destination visibility to company's related contact
+            self.partner_id.write({"company_ids": [(4, incoming_coordinator.id)]})
+            # Adjust related community place coordinator-filtering
+            self._adjust_related_map_place_filtering(
+                outgoing_coordinator, incoming_coordinator
+            )
+            # Sanitize related users roles
+            self._sanitize_outgoing_coordinator_users(outgoing_coordinator)
+            self._sanitize_incoming_coordinator_users(incoming_coordinator)
+            # leave message on chatter
+            self._log_change_coordinator(
+                incoming_coordinator, outgoing_coordinator, change_reason
+            )
+
+    def _log_change_coordinator(
+        self, incoming_coordinator, outgoing_coordinator, change_reason
+    ):
+        message = _(
+            "There has been a coordinator change \
+            from [OLD:{outgoing_id}] {outgoing_name} to [NEW:{incoming_id}] {incoming_name}, \
+            Change reason: {change_reason}"
+        ).format(
+            outgoing_id=outgoing_coordinator.id,
+            outgoing_name=outgoing_coordinator.name,
+            incoming_id=incoming_coordinator.id,
+            incoming_name=incoming_coordinator.name,
+            change_reason=change_reason,
+        )
+        self.message_post(
+            subject="[COORD_CHANGE]",
+            body=message,
+        )
+
+    def _adjust_related_map_place_filtering(
+        self, outgoing_coordinator, incoming_coordinator
+    ):
+        community_landing_page = self.landing_page_id
+        if community_landing_page:
+            filter_coord_arr = []
+            outgoing_coord_filter = (
+                community_landing_page.get_map_coordinator_filter_in_related_place(
+                    outgoing_coordinator
+                )
+            )
+            if outgoing_coord_filter:
+                filter_coord_arr.append((3, outgoing_coord_filter.id))
+            incoming_coord_filter = (
+                community_landing_page.get_map_coordinator_filter_in_related_place(
+                    incoming_coordinator
+                )
+            )
+            if (
+                incoming_coord_filter
+                and incoming_coordinator.landing_page_status == "publish"
+            ):
+                filter_coord_arr.append((4, incoming_coord_filter.id))
+            if community_landing_page.map_place_id and filter_coord_arr:
+                community_landing_page.map_place_id.sudo().write(
+                    {"filter_mids": filter_coord_arr}
+                )
+
+    def _sanitize_outgoing_coordinator_users(self, outgoing_coordinator):
+        coord_users = outgoing_coordinator.get_users(
+            ["role_coord_admin", "role_coord_worker"]
+        )
+        if coord_users:
+            for user in coord_users:
+                # remove community manager role for the outgoing coordinator admins/managers
+                outgoing_user_manager_roles = user.get_related_company_role(
+                    self.id, ["role_ce_manager"]
+                )
+                if outgoing_user_manager_roles:
+                    for role in outgoing_user_manager_roles:
+                        role.unlink()
+                # remove access to community for the outgoing coordinator admins/managers if needed
+                outgoing_user_roles = user.get_related_company_role(self.id)
+                if not outgoing_user_roles:
+                    user.write({"company_ids": [(3, self.id)]})
+
+    def _sanitize_incoming_coordinator_users(self, incoming_coordinator):
+        coord_users = incoming_coordinator.get_users(
+            ["role_coord_admin", "role_coord_worker"]
+        )
+        if coord_users:
+            for user in coord_users:
+                # Add community manager role for the incoming coordinator admins/workers
+                # Add access to community for the incoming coordinator admins/workers
+                user.make_ce_user(self.id, "role_ce_manager")
 
     # TODO: Unused functions. Delete if really not needed.
     def check_ce_has_admin(self):
         self.ensure_one()
         admin_roles_ids = [
             r["odoo_role_id"]
             for r in self.env["res.users"].ce_user_roles_mapping().values()
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_config_settings.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_config_settings.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_partner.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/res_users.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/res_users.py`

 * *Files 12% similar despite different names*

```diff
@@ -247,41 +247,43 @@
                             },
                         )
                     ]
                 }
             )
 
     def make_ce_user(self, company_id, role_name):
-        role = self.env["res.users.role"].search([("code", "=", role_name)])
+        related_company = self.company_ids.filtered(
+            lambda company: company.id == company_id
+        )
+        if not related_company:
+            self.write({"company_ids": [(4, company_id)]})
         current_role = self.env["res.users.role.line"].search(
             [
                 ("user_id", "=", self.id),
                 ("active", "=", True),
                 ("company_id", "=", company_id),
+                ("code", "=", role_name),
             ]
         )
-
-        if current_role:
-            current_role.write({"role_id": role})
-        else:
+        if not current_role:
+            role = self.env["res.users.role"].search([("code", "=", role_name)])
             self.write(
                 {
-                    "company_ids": [(4, company_id)],
                     "role_line_ids": [
                         (
                             0,
                             0,
                             {
                                 "user_id": self.id,
                                 "active": True,
                                 "role_id": role.id,
                                 "company_id": company_id,
                             },
                         )
-                    ],
+                    ]
                 }
             )
 
     def make_coord_user(self, company_id, role_name):
         # create ce user on this company
         self.make_ce_user(company_id, role_name)
         # apply manager role the child companies
@@ -294,14 +296,26 @@
         if role_name == "role_ce_member" or role_name == "role_ce_admin":
             self.make_ce_user(company_id, role_name)
         elif role_name == "role_coord_worker" or role_name == "role_coord_admin":
             self.make_coord_user(company_id, role_name)
         else:
             raise exceptions.UserError(_("Role not found"))
 
+    def get_related_company_role(self, company_id, role_codes=False):
+        if role_codes:
+            current_role_lines = self.role_line_ids.filtered(
+                lambda role_line: role_line.company_id.id == company_id
+                and role_line.role_id.code in role_codes
+            )
+        else:
+            current_role_lines = self.role_line_ids.filtered(
+                lambda role_line: role_line.company_id.id == company_id
+            )
+        return current_role_lines
+
     def create_energy_community_base_user(
         cls, vat, first_name, last_name, lang_code, email
     ):
         vals = {
             "login": vat,
             "firstname": first_name,
             "lastname": last_name,
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/models/user_current_company_mixin.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/models/user_current_company_mixin.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/client.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/client.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/exceptions.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/report/report_templates.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/report/report_templates.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/security/ir.model.access.csv` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/security/ir.model.access.csv`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 id,name,model_id:id,group_id:id,perm_read,perm_write,perm_create,perm_unlink
 landing_page_admin,access_landing_page_admin,model_landing_page,group_admin,1,1,1,1
 landing_page_platform_manager,access_landing_page_platform_manager,model_landing_page,group_platform_manager,1,1,1,1
 landing_page_public,access_landing_page_public,model_landing_page,base.group_public,1,0,0,0
 assign_admin_wizard,assign_admin_wizard_admin,model_assign_admin_wizard,group_admin,1,1,1,1
+change_coordinator_wizard,change_coordinator_wizard_admin,model_change_coordinator_wizard,group_admin,1,1,1,1
 multicompany_easy_creation,multicompany_easy_creation_admin,model_account_multicompany_easy_creation_wiz,group_admin,1,1,1,1
 user_role_read,user_role_read_admin,model_res_users_role,group_admin,1,0,0,0
 user_role_line_read,user_role_line_read_admin,base_user_role.model_res_users_role_line,group_admin,1,0,0,0
 ir_config_parameter_read,ir_config_parameter_read_admin,base.model_ir_config_parameter,group_admin,1,0,0,0
 ir_actions_act_window_read,ir_actions_act_window_read_admin,base.model_ir_actions_act_window,group_admin,1,0,0,0
 ir_actions_act_window_view_read,ir_actions_act_window_view_read_admin,base.model_ir_actions_act_window_view,group_admin,1,0,0,0
 res_company_modify,res_company_modify_admin,model_res_company,group_admin,1,1,1,0
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/security/ir_rule_data.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/security/ir_rule_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/security/res_users_role_data.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/security/res_users_role_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_community_service.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_community_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_landing_service.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_landing_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_member_profile_service.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_member_profile_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/ce_member_service.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/ce_member_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/services/schemas.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/services/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,16 @@
             "twitter_link": {"type": "string"},
             "instagram_link": {"type": "string"},
             "telegram_link": {"type": "string"},
             "community_active_services": {
                 "type": "list",
                 "schema": {"type": "dict", "schema": S_COMMUNITY_SERVICE},
             },
+            "company_logo": {"type": "string"},
+            "company_logo_write_date": {"type": "string"},
             "primary_image_file": {"type": "string"},
             "primary_image_file_write_date": {"type": "string"},
             "secondary_image_file": {"type": "string"},
             "secondary_image_file_write_date": {"type": "string"},
             "short_description": {"type": "string"},
             "long_description": {"type": "string"},
             "why_become_cooperator": {"type": "string"},
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/description/icon.png` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/description/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/static/src/js/cooperator.js` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/static/src/js/cooperator.js`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/common.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/common_service.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/common_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/helpers.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_assign_admin_wizard.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_assign_admin_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_multicompany_easy_creation.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_multicompany_easy_creation.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_res_company.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_res_company.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/tests/test_res_users.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/tests/test_res_users.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/account_banking_mandate_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/account_banking_mandate_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/account_move_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/account_move_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/auth_oauth_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/auth_oauth_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/landing_page_view.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/landing_page_view.xml`

 * *Files 1% similar despite different names*

#### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/landing_page_view.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/landing_page_view.xml`

```diff
@@ -37,15 +37,17 @@
           <field name="telegram_link"/>
         </group>
         <group col="4">
           <field name="primary_image_file" widget="image"/>
           <field name="secondary_image_file" widget="image"/>
         </group>
         <group>
-          <field name="company_logo"/>
+          <field name="company_logo" widget="image"/>
+        </group>
+        <group>
           <field name="short_description"/>
           <field name="long_description"/>
           <field name="why_become_cooperator" widget="html"/>
           <field name="become_cooperator_process" widget="html"/>
         </group>
         <group>
           <field name="lat" required="1"/>
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/menus.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/menus.xml`

 * *Files 8% similar despite different names*

#### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/menus.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/menus.xml`

```diff
@@ -30,8 +30,11 @@
   </record>
   <record model="ir.ui.menu" id="sale.sale_menu_root">
     <field name="groups_id" eval="[(6,0,[ref('group_platform_manager')])]"/>
   </record>
   <record model="ir.ui.menu" id="event.event_main_menu">
     <field name="groups_id" eval="[(6,0,[ref('group_platform_manager')])]"/>
   </record>
+  <record model="ir.ui.menu" id="cooperator.menu_cooperator_templates">
+    <field name="groups_id" eval="[(6,0,[ref('group_platform_manager')])]"/>
+  </record>
 </odoo>
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/product_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/product_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_company_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_company_views.xml`

 * *Files 16% similar despite different names*

#### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_company_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_company_views.xml`

```diff
@@ -1,9 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
+  <act_window id="act_window_change_coordinator" name="Change Coordinator" binding_model="res.company" res_model="change.coordinator.wizard" view_mode="form" target="new" groups="energy_communities.group_platform_manager"/>
   <record id="view_company_form_ce_inherited" model="ir.ui.view">
     <field name="name">res.company.tree.ce.inherited</field>
     <field name="model">res.company</field>
     <field name="inherit_id" ref="base.view_company_form"/>
     <field name="arch" type="xml">
       <xpath expr="//page[@name='general_info']//field[@name='parent_id']" position="attributes">
         <attribute name="invisible">True</attribute>
@@ -19,15 +20,17 @@
         <group name="voluntary_shares" string="Voluntary Shares">
           <field name="voluntary_share_form_header_text"/>
         </group>
       </group>
       <xpath expr="//sheet" position="before">
         <header>
           <field name="landing_page_id" invisible="1"/>
+          <field name="hierarchy_level" invisible="1"/>
           <button name="create_landing" type="object" string="Create landing page" attrs="{'invisible': [('landing_page_id','!=',False)]}"/>
+          <button name="action_open_change_coordinator_wizard" type="object" string="Change coordinator" groups="energy_communities.group_platform_manager" attrs="{'invisible':[('hierarchy_level', '!=','community')]}"/>
         </header>
       </xpath>
       <xpath expr="//field[@name='logo']" position="before">
         <div class="oe_button_box">
           <button name="get_landing_page_form" type="object" string="My landing page" class="oe_stat_button" icon="fa-globe" attrs="{'invisible': [('landing_page_id','=',False)]}"/>
         </div>
         <field name="admins" invisible="True"/>
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_config_settings.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_config_settings.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_partner_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_partner_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_users_role_view.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_users_role_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/res_users_view.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/res_users_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/utm_views.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/utm_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/view_users_form.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/view_users_form.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/website_formfields_template.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/website_formfields_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/views/website_subscription_template.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/views/website_subscription_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/assign_admin_wizard.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
                 "lng": self.lng,
                 "street": self.street,
                 "postal_code": self.zip_code,
                 "city": self.city,
             }
         )
         if self.create_place:
-            new_landing.create_landing_place()
+            new_landing.sudo().create_landing_place()
 
     def thread_action_accept(self):
         self.configure_community_accounting()
         self.update_taxes()
         self.update_properties()
         if self.property_cooperator_account:
             self.set_cooperative_account()
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/SOURCES.txt` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
 odoo/addons/energy_communities/views/utm_views.xml
 odoo/addons/energy_communities/views/view_users_form.xml
 odoo/addons/energy_communities/views/website_formfields_template.xml
 odoo/addons/energy_communities/views/website_subscription_template.xml
 odoo/addons/energy_communities/wizards/__init__.py
 odoo/addons/energy_communities/wizards/assign_admin_wizard.py
 odoo/addons/energy_communities/wizards/assign_admin_wizard.xml
+odoo/addons/energy_communities/wizards/change_coordinator_wizard.py
+odoo/addons/energy_communities/wizards/change_coordinator_wizard.xml
 odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
 odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
 odoo14_addon_energy_communities.egg-info/PKG-INFO
 odoo14_addon_energy_communities.egg-info/SOURCES.txt
 odoo14_addon_energy_communities.egg-info/dependency_links.txt
 odoo14_addon_energy_communities.egg-info/not-zip-safe
 odoo14_addon_energy_communities.egg-info/requires.txt
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/odoo14_addon_energy_communities.egg-info/requires.txt` & `odoo14-addon-energy_communities-14.0.9.2.0/odoo14_addon_energy_communities.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 odoo14-addon-account_payment_order
 odoo14-addon-auth_api_key
 odoo14-addon-auth_oidc
 odoo14-addon-base_rest
 odoo14-addon-base_technical_features
 odoo14-addon-base_user_role
 odoo14-addon-base_user_role_company
-odoo14-addon-community-maps==14.0.0.2.5
+odoo14-addon-community-maps==14.0.0.2.6
 odoo14-addon-cooperator-account-banking-mandate==14.0.1.1.1
 odoo14-addon-cooperator-account-payment==14.0.1.1.0
 odoo14-addon-cooperator==14.0.2.0.5
-odoo14-addon-energy-selfconsumption==14.0.4.0.3
+odoo14-addon-energy-selfconsumption==14.0.4.0.4
 odoo14-addon-l10n-es-aeat-sii-oca==14.0.2.8.1
 odoo14-addon-l10n_es_aeat
 odoo14-addon-l10n_es_cooperator
 odoo14-addon-mail-multicompany==14.0.0.1.1.dev2
 odoo14-addon-metadata==14.0.0.0.1
 odoo14-addon-partner-multi-company==14.0.1.0.1.dev4
 odoo14-addon-queue-job==14.0.3.1.5
```

### Comparing `odoo14-addon-energy_communities-14.0.9.1.0/setup.py` & `odoo14-addon-energy_communities-14.0.9.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 setuptools.setup(
     setup_requires=['setuptools-odoo'],
     odoo_addon={
         "depends_override": {
             "account_lock_date_update": "odoo14-addon-account-lock-date-update==14.0.2.0.1.dev10",
             "account_reconciliation_widget": "odoo14-addon-account-reconciliation-widget==14.0.2.0.2",
-            "community_maps": "odoo14-addon-community-maps==14.0.0.2.5",
+            "community_maps": "odoo14-addon-community-maps==14.0.0.2.6",
             "cooperator": "odoo14-addon-cooperator==14.0.2.0.5",
             "cooperator_account_payment": "odoo14-addon-cooperator-account-payment==14.0.1.1.0",
             "cooperator_account_banking_mandate": "odoo14-addon-cooperator-account-banking-mandate==14.0.1.1.1",
-            "energy_selfconsumption": "odoo14-addon-energy-selfconsumption==14.0.4.0.3",
+            "energy_selfconsumption": "odoo14-addon-energy-selfconsumption==14.0.4.0.4",
             "l10n_es_aeat_sii_oca": "odoo14-addon-l10n-es-aeat-sii-oca==14.0.2.8.1",
             "mail_multicompany": "odoo14-addon-mail-multicompany==14.0.0.1.1.dev2",
             "metadata": "odoo14-addon-metadata==14.0.0.0.1",
             "partner_multi_company": "odoo14-addon-partner-multi-company==14.0.1.0.1.dev4",
             "queue_job": "odoo14-addon-queue-job==14.0.3.1.5",
         },
     }
```

