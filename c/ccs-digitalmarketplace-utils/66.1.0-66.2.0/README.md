# Comparing `tmp/ccs-digitalmarketplace-utils-66.1.0.tar.gz` & `tmp/ccs-digitalmarketplace-utils-66.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-utils-66.1.0.tar", last modified: Thu May 16 11:10:51 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-utils-66.2.0.tar", last modified: Mon Jun  3 09:19:57 2024, max compression
```

## Comparing `ccs-digitalmarketplace-utils-66.1.0.tar` & `ccs-digitalmarketplace-utils-66.2.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.548934 ccs-digitalmarketplace-utils-66.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:10:51.548934 ccs-digitalmarketplace-utils-66.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.540934 ccs-digitalmarketplace-utils-66.1.0/ccs_digitalmarketplace_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:10:51.000000 ccs-digitalmarketplace-utils-66.1.0/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-16 11:10:51.000000 ccs-digitalmarketplace-utils-66.1.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:10:51.000000 ccs-digitalmarketplace-utils-66.1.0/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-16 11:10:51.000000 ccs-digitalmarketplace-utils-66.1.0/ccs_digitalmarketplace_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 11:10:51.000000 ccs-digitalmarketplace-utils-66.1.0/ccs_digitalmarketplace_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.544934 ccs-digitalmarketplace-utils-66.1.0/dmutils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/asset_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/cloudfoundry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/compliance_communications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/cookie_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/csv_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/direct_plus_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/dmp_so_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.544934 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/dm_mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/dm_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/email/user_account_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/env_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.544934 ccs-digitalmarketplace-utils-66.1.0/dmutils/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/errors/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/errors/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/flask_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.548934 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/jinja2_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/ods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.548934 ccs-digitalmarketplace-utils-66.1.0/dmutils/presenters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/presenters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/presenters/compliance_communications.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/presenters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/proxy_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.548934 ccs-digitalmarketplace-utils-66.1.0/dmutils/repoutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/repoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/service_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:51.548934 ccs-digitalmarketplace-utils-66.1.0/dmutils/view_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/view_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/view_helpers/compliance_communications.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/view_helpers/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/view_helpers/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/dmutils/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:10:51.548934 ccs-digitalmarketplace-utils-66.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-16 11:10:41.000000 ccs-digitalmarketplace-utils-66.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.571134 ccs-digitalmarketplace-utils-66.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-03 09:19:57.571134 ccs-digitalmarketplace-utils-66.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.559135 ccs-digitalmarketplace-utils-66.2.0/ccs_digitalmarketplace_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-03 09:19:57.000000 ccs-digitalmarketplace-utils-66.2.0/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-06-03 09:19:57.000000 ccs-digitalmarketplace-utils-66.2.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:19:57.000000 ccs-digitalmarketplace-utils-66.2.0/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-03 09:19:57.000000 ccs-digitalmarketplace-utils-66.2.0/ccs_digitalmarketplace_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 09:19:57.000000 ccs-digitalmarketplace-utils-66.2.0/ccs_digitalmarketplace_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.567134 ccs-digitalmarketplace-utils-66.2.0/dmutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/asset_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/cloudfoundry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/compliance_communications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/cookie_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/csv_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/direct_plus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/dmp_so_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.567134 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/dm_mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/dm_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/email/user_account_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/env_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.567134 ccs-digitalmarketplace-utils-66.2.0/dmutils/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/errors/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/errors/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/flask_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.571134 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/jinja2_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/ods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.571134 ccs-digitalmarketplace-utils-66.2.0/dmutils/presenters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/presenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/presenters/compliance_communications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/presenters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/proxy_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.571134 ccs-digitalmarketplace-utils-66.2.0/dmutils/repoutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/repoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/service_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:57.571134 ccs-digitalmarketplace-utils-66.2.0/dmutils/view_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/view_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/view_helpers/compliance_communications.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/view_helpers/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/view_helpers/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/dmutils/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:19:57.571134 ccs-digitalmarketplace-utils-66.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-06-03 09:19:47.000000 ccs-digitalmarketplace-utils-66.2.0/setup.py
```

### Comparing `ccs-digitalmarketplace-utils-66.1.0/LICENCE` & `ccs-digitalmarketplace-utils-66.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/README.md` & `ccs-digitalmarketplace-utils-66.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-utils-66.2.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/access_control.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/access_control.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/asset_fingerprint.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/asset_fingerprint.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/authentication.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/authentication.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/cloudfoundry.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/compliance_communications.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/compliance_communications.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/config.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/config.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/cookie_probe.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/cookie_probe.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/csv_generator.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/csv_generator.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/dates.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/dates.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/deprecation.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/deprecation.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/direct_plus_client.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/direct_plus_client.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/documents.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/documents.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/email/dm_mailchimp.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/email/dm_mailchimp.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/email/dm_notify.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/email/dm_notify.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/email/helpers.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/email/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/email/tokens.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/email/tokens.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/email/user_account_email.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/email/user_account_email.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/env_helpers.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/env_helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/errors/api.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/errors/api.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/errors/frontend.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/errors/frontend.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/external.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/external.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/feature_flag.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/feature_flag.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/filters.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/filters.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/flask.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/flask.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/flask_init.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/flask_init.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/formats.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/formats.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/errors.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/fields.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/fields.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/helpers.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/mixins.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/validators.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/validators.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/forms/widgets.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/jinja2_environment.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/jinja2_environment.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/logging.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/logging.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/ods.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/ods.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/presenters/compliance_communications.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/presenters/compliance_communications.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/presenters/helpers.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/presenters/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/proxy_fix.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/request_id.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/request_id.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/s3.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/s3.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/service_attribute.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/service_attribute.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/session.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/session.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/status.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/status.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/timing.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/timing.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/urls.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/urls.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/user.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/user.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/view_helpers/compliance_communications.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/view_helpers/compliance_communications.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/view_helpers/pagination.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/view_helpers/pagination.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/dmutils/views.py` & `ccs-digitalmarketplace-utils-66.2.0/dmutils/views.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.1.0/setup.py` & `ccs-digitalmarketplace-utils-66.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,13 +39,13 @@
         'redis>=5.0.1',
         'fleep<1.1,>=1.0.1',
         'notifications-python-client>=8.1.0,<9.0.0',
         'odfpy>=1.4.1',
         'python-json-logger>=2.0.7,<3.0.0',
         'pytz',
         'unicodecsv>=0.14.1',
-        'urllib3<2',
+        'urllib3<3',
         'werkzeug>=2.3,<3',
         'workdays>=1.4',
     ],
     python_requires=">=3.10,<3.13",
 )
```

