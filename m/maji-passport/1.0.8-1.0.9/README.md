# Comparing `tmp/maji_passport-1.0.8.tar.gz` & `tmp/maji_passport-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maji_passport-1.0.8.tar", last modified: Thu May 30 11:21:46 2024, max compression
+gzip compressed data, was "maji_passport-1.0.9.tar", last modified: Mon Jun  3 14:09:53 2024, max compression
```

## Comparing `maji_passport-1.0.8.tar` & `maji_passport-1.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.962932 maji_passport-1.0.8/
--rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-1.0.8/LICENSE
--rw-r--r--   0 teo       (1000) teo       (1000)     3998 2024-05-30 11:21:46.962932 maji_passport-1.0.8/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     2953 2024-05-30 11:21:17.000000 maji_passport-1.0.8/README.md
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.958932 maji_passport-1.0.8/maji_passport/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      406 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/admin.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      246 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/apps.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.958932 maji_passport-1.0.8/maji_passport/authentication/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/authentication/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3046 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/authentication/backend.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.958932 maji_passport-1.0.8/maji_passport/management/
--rw-rw-r--   0 teo       (1000) teo       (1000)        0 2024-05-22 13:36:51.000000 maji_passport-1.0.8/maji_passport/management/__init__.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.958932 maji_passport-1.0.8/maji_passport/management/commands/
--rw-rw-r--   0 teo       (1000) teo       (1000)        0 2024-05-22 13:36:51.000000 maji_passport-1.0.8/maji_passport/management/commands/__init__.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      537 2024-05-22 13:36:51.000000 maji_passport-1.0.8/maji_passport/management/commands/kafka_consumer.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      861 2024-05-22 13:36:51.000000 maji_passport-1.0.8/maji_passport/management/commands/kafka_producer_test.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      236 2024-05-22 13:36:51.000000 maji_passport-1.0.8/maji_passport/management/commands/migrate_all_users_to_passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.958932 maji_passport-1.0.8/maji_passport/migrations/
--rw-rw-r--   0 teo       (1000) teo       (1000)     2234 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/0001_initial.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/0002_auto_20240418_1355.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      471 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      536 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/0004_alter_accesstoken_passport_user.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      615 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/0005_auto_20240521_1047.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     2480 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/0006_auto_20240521_1118.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      940 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/0007_auto_20240522_1304.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      640 2024-05-30 11:17:42.000000 maji_passport-1.0.8/maji_passport/migrations/0008_alter_passportuser_argo_user.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/migrations/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2078 2024-05-30 11:19:02.000000 maji_passport-1.0.8/maji_passport/models.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.962932 maji_passport-1.0.8/maji_passport/serializers/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/serializers/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/serializers/exchange.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     2105 2024-05-28 11:38:05.000000 maji_passport-1.0.8/maji_passport/serializers/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/serializers/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.962932 maji_passport-1.0.8/maji_passport/services/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/services/__init__.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     4612 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/services/auth.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     7023 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/services/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     6051 2024-05-28 11:38:05.000000 maji_passport-1.0.8/maji_passport/services/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      305 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/services/passport.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/services/passport_migrate.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.962932 maji_passport-1.0.8/maji_passport/tests/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/tests/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4010 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/tests/test_exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3026 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/tests/test_kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      940 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/urls.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     1504 2024-05-28 11:38:05.000000 maji_passport-1.0.8/maji_passport/utils.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.962932 maji_passport-1.0.8/maji_passport/views/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/views/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4932 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/views/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3753 2024-05-27 11:28:06.000000 maji_passport-1.0.8/maji_passport/views/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-30 11:21:46.958932 maji_passport-1.0.8/maji_passport.egg-info/
--rw-r--r--   0 teo       (1000) teo       (1000)     3998 2024-05-30 11:21:46.000000 maji_passport-1.0.8/maji_passport.egg-info/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     1762 2024-05-30 11:21:46.000000 maji_passport-1.0.8/maji_passport.egg-info/SOURCES.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-30 11:21:46.000000 maji_passport-1.0.8/maji_passport.egg-info/dependency_links.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      192 2024-05-30 11:21:46.000000 maji_passport-1.0.8/maji_passport.egg-info/requires.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)       14 2024-05-30 11:21:46.000000 maji_passport-1.0.8/maji_passport.egg-info/top_level.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-30 11:21:44.000000 maji_passport-1.0.8/pyproject.toml
--rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-30 11:21:46.962932 maji_passport-1.0.8/setup.cfg
--rw-rw-r--   0 teo       (1000) teo       (1000)      996 2024-05-30 11:21:44.000000 maji_passport-1.0.8/setup.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.361350 maji_passport-1.0.9/
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     1073 2024-05-27 11:51:19.000000 maji_passport-1.0.9/LICENSE
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     3625 2024-06-03 14:09:53.361012 maji_passport-1.0.9/PKG-INFO
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     2953 2024-05-27 11:51:19.000000 maji_passport-1.0.9/README.md
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.323741 maji_passport-1.0.9/maji_passport/
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/__init__.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)      406 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/admin.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)      246 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/apps.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.326533 maji_passport-1.0.9/maji_passport/authentication/
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/authentication/__init__.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     3046 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/authentication/backend.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.328019 maji_passport-1.0.9/maji_passport/management/
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/management/__init__.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.329853 maji_passport-1.0.9/maji_passport/management/commands/
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/management/commands/__init__.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      537 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/management/commands/kafka_consumer.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      861 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/management/commands/kafka_producer_test.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      236 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/management/commands/migrate_all_users_to_passport.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.335921 maji_passport-1.0.9/maji_passport/migrations/
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     2234 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      526 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/0002_auto_20240418_1355.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      471 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      536 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/0004_alter_accesstoken_passport_user.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      615 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/0005_auto_20240521_1047.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     2480 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/0006_auto_20240521_1118.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      940 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/0007_auto_20240522_1304.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      640 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/migrations/0008_alter_passportuser_argo_user.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      812 2024-06-03 14:02:26.000000 maji_passport-1.0.9/maji_passport/migrations/0009_auto_20240603_1400.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/migrations/__init__.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     2111 2024-06-03 12:25:17.000000 maji_passport-1.0.9/maji_passport/models.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.339618 maji_passport-1.0.9/maji_passport/serializers/
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/serializers/__init__.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     2397 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/serializers/exchange.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     2105 2024-06-03 10:18:28.000000 maji_passport-1.0.9/maji_passport/serializers/kafka.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)      519 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/serializers/passport.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.351260 maji_passport-1.0.9/maji_passport/services/
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/services/__init__.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     4612 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/services/auth.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     7023 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/services/exchange.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     6051 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/services/kafka.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)      305 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/services/passport.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     2880 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/services/passport_migrate.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.353562 maji_passport-1.0.9/maji_passport/tests/
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/tests/__init__.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     4010 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/tests/test_exchange.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     3026 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/tests/test_kafka.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)      940 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/urls.py
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     1504 2024-06-03 10:15:42.000000 maji_passport-1.0.9/maji_passport/utils.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.358162 maji_passport-1.0.9/maji_passport/views/
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/views/__init__.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     4932 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/views/exchange.py
+-rwxr-xr-x   0 macbookpro152015   (501) staff       (20)     3753 2024-05-27 11:51:19.000000 maji_passport-1.0.9/maji_passport/views/passport.py
+drwxr-xr-x   0 macbookpro152015   (501) staff       (20)        0 2024-06-03 14:09:53.359703 maji_passport-1.0.9/maji_passport.egg-info/
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     3625 2024-06-03 14:09:53.000000 maji_passport-1.0.9/maji_passport.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)     1778 2024-06-03 14:09:53.000000 maji_passport-1.0.9/maji_passport.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)        1 2024-06-03 14:09:53.000000 maji_passport-1.0.9/maji_passport.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)       14 2024-06-03 14:09:53.000000 maji_passport-1.0.9/maji_passport.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      668 2024-06-03 14:04:12.000000 maji_passport-1.0.9/pyproject.toml
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)       38 2024-06-03 14:09:53.362415 maji_passport-1.0.9/setup.cfg
+-rw-r--r--   0 macbookpro152015   (501) staff       (20)      996 2024-06-03 14:04:00.000000 maji_passport-1.0.9/setup.py
```

### Comparing `maji_passport-1.0.8/LICENSE` & `maji_passport-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/PKG-INFO` & `maji_passport-1.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 Metadata-Version: 2.1
 Name: maji_passport
-Version: 1.0.8
+Version: 1.0.9
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
-Keywords: maji passport python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: djangorestframework-jwt==1.11.0
-Requires-Dist: pyjwt==1.7.1
-Requires-Dist: djangorestframework==3.11.1
-Requires-Dist: django-countries-plus
-Requires-Dist: loguru==0.5.3
-Requires-Dist: httpx==0.18.1
-Requires-Dist: confluent-kafka==2.3.0
-Requires-Dist: Pillow>=7.2.0
-Requires-Dist: sentry_sdk
-Requires-Dist: drf-yasg[validation]
 
 # Maji Package
 Library for client side passport functionality.
 Adding new auth backend behaviour.
 Working with passport tokens.
 Adding new endpoints.
```

### Comparing `maji_passport-1.0.8/README.md` & `maji_passport-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/authentication/backend.py` & `maji_passport-1.0.9/maji_passport/authentication/backend.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/management/commands/kafka_consumer.py` & `maji_passport-1.0.9/maji_passport/management/commands/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/management/commands/kafka_producer_test.py` & `maji_passport-1.0.9/maji_passport/management/commands/kafka_producer_test.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/migrations/0001_initial.py` & `maji_passport-1.0.9/maji_passport/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/migrations/0002_auto_20240418_1355.py` & `maji_passport-1.0.9/maji_passport/migrations/0002_auto_20240418_1355.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/migrations/0004_alter_accesstoken_passport_user.py` & `maji_passport-1.0.9/maji_passport/migrations/0004_alter_accesstoken_passport_user.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/migrations/0005_auto_20240521_1047.py` & `maji_passport-1.0.9/maji_passport/migrations/0005_auto_20240521_1047.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/migrations/0006_auto_20240521_1118.py` & `maji_passport-1.0.9/maji_passport/migrations/0006_auto_20240521_1118.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/migrations/0007_auto_20240522_1304.py` & `maji_passport-1.0.9/maji_passport/migrations/0007_auto_20240522_1304.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/migrations/0008_alter_passportuser_argo_user.py` & `maji_passport-1.0.9/maji_passport/migrations/0008_alter_passportuser_argo_user.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/models.py` & `maji_passport-1.0.9/maji_passport/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 
 class PassportUser(BaseModel):
     argo_user = OneToOneField(User, null=True, on_delete=SET_NULL, related_name="passport_user")
     passport_uuid = UUIDField(null=False)
     user_auth_code = CharField(max_length=255, null=False)
     refresh_token = TextField()
-    avatar_url = CharField(max_length=255, blank=True)
-    cover_url = CharField(max_length=255, blank=True)
-    display_name = CharField(max_length=255, blank=True)
+    avatar_url = CharField(max_length=255, blank=True, null=True)
+    cover_url = CharField(max_length=255, blank=True, null=True)
+    display_name = CharField(max_length=255, blank=True, null=True)
     social_networks = JSONField(default=dict, blank=True)
 
     def __str__(self):
         return (
             f"argo email - {self.argo_user.email}, passport uuid - {self.passport_uuid}"
         )
```

### Comparing `maji_passport-1.0.8/maji_passport/serializers/exchange.py` & `maji_passport-1.0.9/maji_passport/serializers/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/serializers/kafka.py` & `maji_passport-1.0.9/maji_passport/serializers/kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/serializers/passport.py` & `maji_passport-1.0.9/maji_passport/serializers/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/services/auth.py` & `maji_passport-1.0.9/maji_passport/services/auth.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/services/exchange.py` & `maji_passport-1.0.9/maji_passport/services/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/services/kafka.py` & `maji_passport-1.0.9/maji_passport/services/kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/services/passport_migrate.py` & `maji_passport-1.0.9/maji_passport/services/passport_migrate.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/tests/test_exchange.py` & `maji_passport-1.0.9/maji_passport/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/tests/test_kafka.py` & `maji_passport-1.0.9/maji_passport/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/urls.py` & `maji_passport-1.0.9/maji_passport/urls.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/utils.py` & `maji_passport-1.0.9/maji_passport/utils.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/views/exchange.py` & `maji_passport-1.0.9/maji_passport/views/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport/views/passport.py` & `maji_passport-1.0.9/maji_passport/views/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.8/maji_passport.egg-info/PKG-INFO` & `maji_passport-1.0.9/maji_passport.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 Metadata-Version: 2.1
-Name: maji-passport
-Version: 1.0.8
+Name: maji_passport
+Version: 1.0.9
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
-Keywords: maji passport python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: djangorestframework-jwt==1.11.0
-Requires-Dist: pyjwt==1.7.1
-Requires-Dist: djangorestframework==3.11.1
-Requires-Dist: django-countries-plus
-Requires-Dist: loguru==0.5.3
-Requires-Dist: httpx==0.18.1
-Requires-Dist: confluent-kafka==2.3.0
-Requires-Dist: Pillow>=7.2.0
-Requires-Dist: sentry_sdk
-Requires-Dist: drf-yasg[validation]
 
 # Maji Package
 Library for client side passport functionality.
 Adding new auth backend behaviour.
 Working with passport tokens.
 Adding new endpoints.
```

### Comparing `maji_passport-1.0.8/maji_passport.egg-info/SOURCES.txt` & `maji_passport-1.0.9/maji_passport.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 maji_passport/apps.py
 maji_passport/models.py
 maji_passport/urls.py
 maji_passport/utils.py
 maji_passport.egg-info/PKG-INFO
 maji_passport.egg-info/SOURCES.txt
 maji_passport.egg-info/dependency_links.txt
-maji_passport.egg-info/requires.txt
 maji_passport.egg-info/top_level.txt
 maji_passport/authentication/__init__.py
 maji_passport/authentication/backend.py
 maji_passport/management/__init__.py
 maji_passport/management/commands/__init__.py
 maji_passport/management/commands/kafka_consumer.py
 maji_passport/management/commands/kafka_producer_test.py
@@ -25,14 +24,15 @@
 maji_passport/migrations/0002_auto_20240418_1355.py
 maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
 maji_passport/migrations/0004_alter_accesstoken_passport_user.py
 maji_passport/migrations/0005_auto_20240521_1047.py
 maji_passport/migrations/0006_auto_20240521_1118.py
 maji_passport/migrations/0007_auto_20240522_1304.py
 maji_passport/migrations/0008_alter_passportuser_argo_user.py
+maji_passport/migrations/0009_auto_20240603_1400.py
 maji_passport/migrations/__init__.py
 maji_passport/serializers/__init__.py
 maji_passport/serializers/exchange.py
 maji_passport/serializers/kafka.py
 maji_passport/serializers/passport.py
 maji_passport/services/__init__.py
 maji_passport/services/auth.py
```

### Comparing `maji_passport-1.0.8/pyproject.toml` & `maji_passport-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maji_passport"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Viktor Ivanov", email="viktorteodorihivanov@gmail.com" },
 ]
 description = "Maji Passport With custom authorisation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `maji_passport-1.0.8/setup.py` & `maji_passport-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='maji_passport',
-  version='1.0.8',
+  version='1.0.9',
   author='ViktorTeodorih',
   author_email='viktorteodorihivanov@gmail.com',
   description='Maji Passport With custom authorisation',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://passport.maji.la/',
   packages=find_packages(),
```

