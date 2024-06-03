# Comparing `tmp/drf-stripe-subscription-1.2.0.tar.gz` & `tmp/drf-stripe-subscription-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-stripe-subscription-1.2.0.tar", last modified: Tue May 30 16:17:11 2023, max compression
+gzip compressed data, was "drf-stripe-subscription-1.2.1.tar", last modified: Mon Jun  3 04:59:29 2024, max compression
```

## Comparing `drf-stripe-subscription-1.2.0.tar` & `drf-stripe-subscription-1.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.115735 drf-stripe-subscription-1.2.0/
--rw-r--r--   0 oscarchen   (501) staff       (20)     1069 2023-02-26 17:26:47.000000 drf-stripe-subscription-1.2.0/LICENSE
--rw-r--r--   0 oscarchen   (501) staff       (20)       68 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/MANIFEST.in
--rw-r--r--   0 oscarchen   (501) staff       (20)    13927 2023-05-30 16:17:11.115875 drf-stripe-subscription-1.2.0/PKG-INFO
--rw-r--r--   0 oscarchen   (501) staff       (20)    10294 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/README.md
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.111434 drf-stripe-subscription-1.2.0/drf_stripe/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      158 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/admin.py
--rw-r--r--   0 oscarchen   (501) staff       (20)       94 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/apps.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.111548 drf-stripe-subscription-1.2.0/drf_stripe/management/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/__init__.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.112145 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      368 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/pull_stripe.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      592 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_customers.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      349 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_products.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      605 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_subscriptions.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.112635 drf-stripe-subscription-1.2.0/drf_stripe/migrations/
--rw-r--r--   0 oscarchen   (501) staff       (20)     5146 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/0001_initial.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2168 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      471 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/0003_price_currency.py
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     4978 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/models.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     4554 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/serializers.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2176 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/settings.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.113434 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      169 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/api.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     5764 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/checkout.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      555 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/customer_portal.py
--rw-r--r--   0 oscarchen   (501) staff       (20)    11631 2023-05-30 16:07:47.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/customers.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     3956 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/products.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     7694 2023-05-30 16:07:47.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/subscriptions.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.114409 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2233 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/currency.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1307 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/customer.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     3070 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/event.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1344 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/invoice.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1407 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/price.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1286 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/product.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2329 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/subscription.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.115018 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1654 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/customer_subscription.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2803 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/handler.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      797 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/price.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      608 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/product.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      474 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/urls.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     3045 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/views.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.115623 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/
--rw-r--r--   0 oscarchen   (501) staff       (20)    13927 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/PKG-INFO
--rw-r--r--   0 oscarchen   (501) staff       (20)     1693 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/SOURCES.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)        1 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/dependency_links.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)       64 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/requires.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)       17 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/top_level.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)     1196 2023-05-30 16:17:11.116215 drf-stripe-subscription-1.2.0/setup.cfg
--rw-r--r--   0 oscarchen   (501) staff       (20)      153 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/setup.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.517073 drf-stripe-subscription-1.2.1/
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1069 2023-02-26 17:26:47.000000 drf-stripe-subscription-1.2.1/LICENSE
+-rw-r--r--   0 oscarchen   (501) staff       (20)       68 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/MANIFEST.in
+-rw-r--r--   0 oscarchen   (501) staff       (20)    12182 2024-06-03 04:59:29.517186 drf-stripe-subscription-1.2.1/PKG-INFO
+-rw-r--r--   0 oscarchen   (501) staff       (20)    10818 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/README.md
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.511708 drf-stripe-subscription-1.2.1/drf_stripe/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      158 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/admin.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)       94 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/apps.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.511880 drf-stripe-subscription-1.2.1/drf_stripe/management/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/management/__init__.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.512503 drf-stripe-subscription-1.2.1/drf_stripe/management/commands/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/management/commands/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      368 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/management/commands/pull_stripe.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      592 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/management/commands/update_stripe_customers.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      349 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/management/commands/update_stripe_products.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      605 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/management/commands/update_stripe_subscriptions.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.513183 drf-stripe-subscription-1.2.1/drf_stripe/migrations/
+-rw-r--r--   0 oscarchen   (501) staff       (20)     5213 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/migrations/0001_initial.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2168 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      471 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/migrations/0003_price_currency.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/migrations/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     5517 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/models.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     4554 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/serializers.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2207 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/settings.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.514300 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      169 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/api.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     5791 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/checkout.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      555 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/customer_portal.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)    11658 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/customers.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     3956 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/products.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     7694 2023-05-30 16:07:47.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/subscriptions.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.515731 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2233 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/currency.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1335 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/customer.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     3090 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/event.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1344 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/invoice.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1417 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/price.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1286 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/product.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2366 2024-06-02 21:14:13.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/subscription.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.516427 drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1654 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/customer_subscription.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2803 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/handler.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      797 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/price.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      608 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/product.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      474 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/urls.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     3045 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/drf_stripe/views.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2024-06-03 04:59:29.516973 drf-stripe-subscription-1.2.1/drf_stripe_subscription.egg-info/
+-rw-r--r--   0 oscarchen   (501) staff       (20)    12182 2024-06-03 04:59:29.000000 drf-stripe-subscription-1.2.1/drf_stripe_subscription.egg-info/PKG-INFO
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1693 2024-06-03 04:59:29.000000 drf-stripe-subscription-1.2.1/drf_stripe_subscription.egg-info/SOURCES.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)        1 2024-06-03 04:59:29.000000 drf-stripe-subscription-1.2.1/drf_stripe_subscription.egg-info/dependency_links.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)       64 2024-06-03 04:59:29.000000 drf-stripe-subscription-1.2.1/drf_stripe_subscription.egg-info/requires.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)       17 2024-06-03 04:59:29.000000 drf-stripe-subscription-1.2.1/drf_stripe_subscription.egg-info/top_level.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1294 2024-06-03 04:59:29.517619 drf-stripe-subscription-1.2.1/setup.cfg
+-rw-r--r--   0 oscarchen   (501) staff       (20)      153 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.1/setup.py
```

### Comparing `drf-stripe-subscription-1.2.0/LICENSE` & `drf-stripe-subscription-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/README.md` & `drf-stripe-subscription-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -187,18 +187,20 @@
 ```
 
 ## Customizing Checkout Session Parameters
 
 Some of the checkout parameters are specified in `DRF_STRIPE` settings:
 
 `CHECKOUT_SUCCESS_URL_PATH`: The checkout session success redirect url path.
+
 `CHECKOUT_CANCEL_URL_PATH`: The checkout session cancel redirect url path.
-`PAYMENT_METHOD_TYPES`: The default
-default [payment method types](https://stripe.com/docs/api/checkout/sessions/create#create_checkout_session-payment_method_types)
+
+`PAYMENT_METHOD_TYPES`: The default [payment method types](https://stripe.com/docs/api/checkout/sessions/create#create_checkout_session-payment_method_types)
 , defaults to `["card"]`.
+
 `DEFAULT_CHECKOUT_MODE`: The default checkout mode, defaults to `"subscription"`.
 
 By default, you can create a checkout session by calling the default REST endpoint `my-site.com/stripe/checkout/`, this
 REST endpoint utilizes `drf_stripe.serializers.CheckoutRequestSerializer` to validate checkout parameters and create a
 Stripe Checkout Session. Only a `price_id` is needed, `quantity` defaults to 1.
 
 You can extend this serializer and customize Checkout behavior, such as specifying multiple `line_items`
@@ -285,15 +287,25 @@
 The following DRF_STRIPE settings can be used to customize how Django creates User instance using Stripe Customer
 attributes (default values shown):
 
 ```python
 DRF_STRIPE = {
     "DJANGO_USER_EMAIL_FIELD": "email",
     "USER_CREATE_DEFAULTS_ATTRIBUTE_MAP": {"username": "email"},
+    "DJANGO_USER_MODEL": None,
 }
 ```
 
 The `DJANGO_USER_EMAIL_FIELD` specifies name of the Django User attribute to be used to store Stripe Customer email. It
 will be used to look up existing Django User using Stripe Customer email.
 
 The `USER_CREATE_DEFAULTS_ATTRIBUTE_MAP` maps the name of Django User attribute to name of corresponding Stripe Customer
 attribute, and is used during the automated Django User instance creation.
+
+The `DJANGO_USER_MODEL` is optional in case you are not using Django's default user model (nor the model you may have configured using Django's `AUTH_USER_MODEL`) for your users you wish to associate with Stripe customers.
+In this case specify the model you wish to use using a dotted pair - the label of the Django app (which must be in your INSTALLED_APPS), and the name of the Django model that you wish to use.
+For example:
+```python
+DRF_STRIPE = {
+   "DJANGO_USER_MODEL": "myapp.MyUser"
+}
+```
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_customers.py` & `drf-stripe-subscription-1.2.1/drf_stripe/management/commands/update_stripe_customers.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_subscriptions.py` & `drf-stripe-subscription-1.2.1/drf_stripe/management/commands/update_stripe_subscriptions.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/migrations/0001_initial.py` & `drf-stripe-subscription-1.2.1/drf_stripe/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Generated by Django 4.0.1 on 2022-01-13 15:48
 
 import django.db.models.deletion
-from django.conf import settings
 from django.db import migrations, models
+from drf_stripe.models import get_drf_stripe_user_model_name
 
 
 class Migration(migrations.Migration):
     initial = True
 
+    auth_user_model = get_drf_stripe_user_model_name()
+
+
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        migrations.swappable_dependency(auth_user_model),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Feature',
             fields=[
                 ('feature_id', models.CharField(max_length=64, primary_key=True, serialize=False)),
@@ -46,15 +49,15 @@
             ],
         ),
         migrations.CreateModel(
             name='StripeUser',
             fields=[
                 ('user', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, primary_key=True,
                                               related_name='stripe_user', serialize=False,
-                                              to=settings.AUTH_USER_MODEL)),
+                                              to=auth_user_model)),
                 ('customer_id', models.CharField(max_length=128, null=True)),
             ],
         ),
         migrations.CreateModel(
             name='Subscription',
             fields=[
                 ('subscription_id', models.CharField(max_length=256, primary_key=True, serialize=False)),
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py` & `drf-stripe-subscription-1.2.1/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/models.py` & `drf-stripe-subscription-1.2.1/drf_stripe/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,33 @@
 from django.contrib.auth import get_user_model
 from django.db import models
+from django.apps import apps as django_apps
+from django.conf import settings
 
 from .stripe_models.subscription import ACCESS_GRANTING_STATUSES
+from .settings import drf_stripe_settings
+
+
+def get_drf_stripe_user_model_name():
+    if drf_stripe_settings.DJANGO_USER_MODEL:
+        return drf_stripe_settings.DJANGO_USER_MODEL
+    else:
+        return settings.AUTH_USER_MODEL
+
+
+def get_drf_stripe_user_model():
+    if drf_stripe_settings.DJANGO_USER_MODEL:
+        return django_apps.get_model(drf_stripe_settings.DJANGO_USER_MODEL, require_ready=False)
+    else:
+        return get_user_model()
 
 
 class StripeUser(models.Model):
     """A model linking Django user model with a Stripe User"""
-    user = models.OneToOneField(get_user_model(), on_delete=models.CASCADE, related_name='stripe_user',
+    user = models.OneToOneField(get_drf_stripe_user_model(), on_delete=models.CASCADE, related_name='stripe_user',
                                 primary_key=True)
     customer_id = models.CharField(max_length=128, null=True)
 
     @property
     def subscription_items(self):
         """Returns a set of SubscriptionItem instances associated with the StripeUser"""
         return SubscriptionItem.objects.filter(subscription__stripe_user=self)
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/serializers.py` & `drf-stripe-subscription-1.2.1/drf_stripe/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/settings.py` & `drf-stripe-subscription-1.2.1/drf_stripe/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "NEW_USER_FREE_TRIAL_DAYS": None,
     "CHECKOUT_SUCCESS_URL_PATH": "payment",
     "CHECKOUT_CANCEL_URL_PATH": "manage-subscription",
     "DEFAULT_PAYMENT_METHOD_TYPES": ["card"],
     "DEFAULT_CHECKOUT_MODE": "subscription",
     "DEFAULT_DISCOUNTS": None,
     "ALLOW_PROMOTION_CODES": True,
+    "DJANGO_USER_MODEL": None,
     "DJANGO_USER_EMAIL_FIELD": "email",  # used to match Stripe customer email
     "USER_CREATE_DEFAULTS_ATTRIBUTE_MAP": {  # attributes to copy from Stripe customer when creating new Django user
         "username": "email"
     }
 }
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/checkout.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import timedelta, datetime
 from functools import reduce
 from typing import overload, List, Union
 from urllib.parse import urljoin
 
-from django.contrib.auth import get_user_model
+from drf_stripe.models import get_drf_stripe_user_model as get_user_model
 from django.utils import timezone
 
 from drf_stripe.stripe_api.api import stripe_api as stripe
 from ..settings import drf_stripe_settings
 
 
 @overload
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/customer_portal.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/customer_portal.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/customers.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/customers.py`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import overload
 
-from django.contrib.auth import get_user_model
+from drf_stripe.models import get_drf_stripe_user_model as get_user_model
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.transaction import atomic
 
 from drf_stripe.models import StripeUser
 from drf_stripe.stripe_api.api import stripe_api as stripe
 from drf_stripe.stripe_models.customer import StripeCustomers, StripeCustomer
 from ..settings import drf_stripe_settings
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/products.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/products.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/subscriptions.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/currency.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/currency.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/customer.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/customer.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     delinquent: Optional[bool]
     discount: Optional[Dict] = None
     invoice_prefix: Optional[str]
     invoice_settings: Optional[Dict]
     livemode: Optional[bool]
     next_invoice_sequence: Optional[int]
     preferred_locales: Optional[List[str]]
-    sources: Optional[List[Dict]]
-    subscriptions: Optional[List[StripeSubscriptionItems]]
-    tax: Optional[Dict]
+    sources: Optional[List[Dict]] = None
+    subscriptions: Optional[List[StripeSubscriptionItems]] = None
+    tax: Optional[Dict] = None
     tax_exempt: Optional[str]
-    tax_ids: Optional[List[Dict]]
+    tax_ids: Optional[List[Dict]] = None
 
 
 class StripeCustomers(BaseModel):
     """Based on https://stripe.com/docs/api/customers/list"""
     data: List[StripeCustomer]
     has_more: bool = None
     url: str = None
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/event.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Union, Literal, Any
+from typing import Union, Literal, Any, Optional
 
 from pydantic import BaseModel, Field
 
 from .invoice import StripeInvoiceEventData
 from .price import StripePriceEventData
 from .product import StripeProductEventData
 from .subscription import StripeSubscriptionEventData
@@ -34,15 +34,15 @@
     PRICE_UPDATED = 'price.updated'
     PRICE_CREATED = 'price.created'
 
 
 class StripeEventRequest(BaseModel):
     """Based on: https://stripe.com/docs/api/events/object#event_object-request"""
     id: str = None
-    idempotency_key: str = None
+    idempotency_key: Optional[str] = None
 
 
 class StripeBaseEvent(BaseModel):
     """
     Based on https://stripe.com/docs/api/events/object
     This is the base event template for more specific Stripe event classes
     """
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/invoice.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/invoice.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/price.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/price.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class PriceType(str, Enum):
     ONE_TIME = 'one_time'
     RECURRING = 'recurring'
 
 
 class StripePriceRecurring(BaseModel):
-    aggregate_usage: str = None
+    aggregate_usage: Optional[str] = None
     interval: RecurringInterval
     interval_count: Optional[int]
     usage_type: Optional[UsageType]
 
 
 class StripePrice(BaseModel):
     """A single StripePrice, see https://stripe.com/docs/api/prices/object"""
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/product.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/product.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/subscription.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_models/subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     StripeSubscriptionStatus.TRIALING
 )
 
 
 class StripeSubscriptionItemsDataItem(BaseModel):
     """Based on https://stripe.com/docs/api/subscriptions/object#subscription_object-items-data"""
     id: str
-    billing_thresholds: Dict = None
+    billing_thresholds: Optional[Dict] = None
     created: datetime
     metadata: Dict
     price: StripePrice
     quantity: int
     subscription: str
     tax_rates: List
 
@@ -52,27 +52,27 @@
     cancel_at: Optional[datetime] = None
     ended_at: Optional[datetime] = None
     trial_end: Optional[datetime] = None
     trial_start: Optional[datetime] = None
     current_period_end: Optional[datetime]
     current_period_start: Optional[datetime]
     customer: Optional[str]
-    default_payment_method: str = None
+    default_payment_method: Optional[str] = None
     items: Optional[StripeSubscriptionItems]
     latest_invoice: Optional[str]
     metadata: Optional[Dict]
-    pending_setup_intent: str = None
+    pending_setup_intent: Optional[str] = None
     pending_update: Any = None
     status: Optional[StripeSubscriptionStatus]
 
 
 class StripeSubscriptions(BaseModel):
     """Based on https://stripe.com/docs/api/subscriptions/list"""
     data: List[StripeSubscription]
     has_more: bool = None
     url: str = None
 
 
 class StripeSubscriptionEventData(BaseModel):
     """Based on https://stripe.com/docs/api/events/object#event_object-data"""
     object: StripeSubscription
-    previous_attributes: Optional[StripeSubscription]
+    previous_attributes: Optional[StripeSubscription] = None
```

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/customer_subscription.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/customer_subscription.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/handler.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/handler.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/price.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/price.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/product.py` & `drf-stripe-subscription-1.2.1/drf_stripe/stripe_webhooks/product.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe/views.py` & `drf-stripe-subscription-1.2.1/drf_stripe/views.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/SOURCES.txt` & `drf-stripe-subscription-1.2.1/drf_stripe_subscription.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.2.0/setup.cfg` & `drf-stripe-subscription-1.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 [metadata]
 name = drf-stripe-subscription
-version = 1.2.0
+version = 1.2.1
 description = A Django app that provides subscription features with Stripe and REST endpoints.
 long_description = file: README.md
 url = https://github.com/oscarychen/drf-stripe-subscription
 author = Oscar Chen
 author_email = quacky@duck.com
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
+	Framework :: Django :: 5.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	Django >= 3.0
 	djangorestframework >= 3.0
 	pydantic >= 1.8
 	stripe >= 2.63
 
 [egg_info]
```

