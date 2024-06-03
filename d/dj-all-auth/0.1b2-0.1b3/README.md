# Comparing `tmp/dj_all_auth-0.1b2.tar.gz` & `tmp/dj_all_auth-0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_all_auth-0.1b2.tar", last modified: Mon Jun  3 10:04:20 2024, max compression
+gzip compressed data, was "dj_all_auth-0.1b3.tar", last modified: Mon Jun  3 10:56:40 2024, max compression
```

## Comparing `dj_all_auth-0.1b2.tar` & `dj_all_auth-0.1b3.tar`

### file list

```diff
@@ -1,111 +1,123 @@
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-06-03 05:39:14.000000 dj_all_auth-0.1b2/LICENSE
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      140 2024-06-03 10:01:27.000000 dj_all_auth-0.1b2/MANIFEST.in
--rw-r--r--   0 deviser   (1000) deviser   (1000)     1922 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/PKG-INFO
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      916 2024-06-03 10:02:34.000000 dj_all_auth-0.1b2/README.rst
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.349715 dj_all_auth-0.1b2/dj_all_auth/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      559 2024-06-03 09:58:34.000000 dj_all_auth-0.1b2/dj_all_auth/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     2992 2024-06-02 20:07:47.000000 dj_all_auth-0.1b2/dj_all_auth/admin.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      152 2024-06-03 09:58:34.000000 dj_all_auth-0.1b2/dj_all_auth/apps.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      554 2024-03-30 22:46:44.000000 dj_all_auth-0.1b2/dj_all_auth/base_models.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      557 2024-06-02 21:50:53.000000 dj_all_auth-0.1b2/dj_all_auth/context_processors.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.349715 dj_all_auth-0.1b2/dj_all_auth/lib/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1287 2024-06-02 21:21:20.000000 dj_all_auth-0.1b2/dj_all_auth/lib/Mail.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-01-14 01:50:51.000000 dj_all_auth-0.1b2/dj_all_auth/lib/__init__.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/migrations/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     4576 2024-06-03 05:06:59.000000 dj_all_auth-0.1b2/dj_all_auth/migrations/0001_initial.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-06-03 04:45:15.000000 dj_all_auth-0.1b2/dj_all_auth/migrations/__init__.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/models/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      272 2024-03-31 02:13:04.000000 dj_all_auth-0.1b2/dj_all_auth/models/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       57 2024-06-03 04:45:15.000000 dj_all_auth-0.1b2/dj_all_auth/models.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-03-04 17:09:21.000000 dj_all_auth-0.1b2/dj_all_auth/services/__init__.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/auth/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-03-09 22:30:18.000000 dj_all_auth-0.1b2/dj_all_auth/services/auth/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     4977 2024-06-02 21:24:59.000000 dj_all_auth-0.1b2/dj_all_auth/services/auth/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/connections/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-03-30 22:34:37.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/__init__.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     5733 2024-06-02 21:26:59.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/Discord.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      236 2024-06-02 21:27:09.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      629 2024-06-02 21:27:26.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/models.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      374 2024-03-30 23:17:39.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/urls.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1900 2024-04-15 09:07:04.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/connections/google/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     5123 2024-03-31 02:48:39.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/google/Google.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      228 2024-03-24 10:17:00.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/google/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      660 2024-03-30 22:40:50.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/google/models.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      370 2024-03-24 10:17:00.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/google/urls.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1912 2024-03-30 22:55:38.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/google/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     3306 2024-03-31 02:49:04.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/Steam.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       88 2024-03-30 22:55:55.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      455 2024-03-30 22:43:31.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/models.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      366 2024-03-24 10:17:00.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/urls.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1520 2024-03-30 22:52:49.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     6017 2024-03-31 02:49:48.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/Twitch.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      228 2024-03-24 10:17:00.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      626 2024-03-30 22:43:50.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/models.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      370 2024-03-24 10:17:00.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/urls.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1880 2024-03-30 22:52:57.000000 dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/profile/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       77 2024-03-20 11:53:53.000000 dj_all_auth-0.1b2/dj_all_auth/services/profile/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      800 2024-05-21 07:26:13.000000 dj_all_auth-0.1b2/dj_all_auth/services/profile/models.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      224 2024-03-24 08:11:07.000000 dj_all_auth-0.1b2/dj_all_auth/services/profile/urls.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     2363 2024-06-02 21:32:21.000000 dj_all_auth-0.1b2/dj_all_auth/services/profile/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/services/security/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       78 2024-03-21 07:36:00.000000 dj_all_auth-0.1b2/dj_all_auth/services/security/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      147 2024-03-21 07:36:52.000000 dj_all_auth-0.1b2/dj_all_auth/services/security/urls.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      331 2024-03-20 11:00:57.000000 dj_all_auth-0.1b2/dj_all_auth/services/security/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.349715 dj_all_auth-0.1b2/dj_all_auth/templates/
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.353715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1353 2024-06-02 21:51:32.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/base.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1933 2024-04-15 09:04:30.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/login.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      420 2024-06-02 21:52:19.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/logout.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1531 2024-04-15 09:04:41.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      882 2024-04-15 09:04:47.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset_complete.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1637 2024-04-15 09:04:51.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset_confirm.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      766 2024-04-15 09:04:55.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset_done.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     3075 2024-04-15 09:03:38.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/register.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1414 2024-04-15 09:04:59.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/request_account_activation.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1761 2024-05-23 10:06:44.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/index.html
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      912 2024-03-24 11:34:38.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/base.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1439 2024-05-09 20:22:18.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/css_section.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      252 2024-01-14 02:51:52.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/flash_messages.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      400 2024-03-17 21:46:15.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/head_section.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1204 2024-04-15 09:24:26.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/js_section.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      717 2024-03-24 11:52:16.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/navbar.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     5476 2024-01-14 01:50:51.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/page-loader.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1464 2024-05-09 20:21:57.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/sidebar.html
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.349715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/activate_request/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      110 2024-04-29 18:21:11.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/activate_request/mail.text
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/password_reset/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      612 2024-01-14 01:50:51.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/password_reset/mail.text
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/register/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      110 2024-04-29 18:21:53.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/register/mail.text
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/profile/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)    11978 2024-05-23 10:03:43.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/profile/index.html
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/security/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1017 2024-05-01 11:46:23.000000 dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/security/index.html
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       60 2024-06-03 04:45:15.000000 dj_all_auth-0.1b2/dj_all_auth/tests.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     2142 2024-03-31 01:05:33.000000 dj_all_auth-0.1b2/dj_all_auth/urls.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth/utils/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1051 2024-06-02 21:34:57.000000 dj_all_auth-0.1b2/dj_all_auth/utils/TokenGenerator.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-01-14 01:50:51.000000 dj_all_auth-0.1b2/dj_all_auth/utils/__init__.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      785 2024-06-02 21:34:34.000000 dj_all_auth-0.1b2/dj_all_auth/utils/forms.py
--rw-rw-r--   0 deviser   (1000) deviser   (1000)      325 2024-03-24 10:21:56.000000 dj_all_auth-0.1b2/dj_all_auth/views.py
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/dj_all_auth.egg-info/
--rw-r--r--   0 deviser   (1000) deviser   (1000)     1922 2024-06-03 10:04:20.000000 dj_all_auth-0.1b2/dj_all_auth.egg-info/PKG-INFO
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     3466 2024-06-03 10:04:20.000000 dj_all_auth-0.1b2/dj_all_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        1 2024-06-03 10:04:20.000000 dj_all_auth-0.1b2/dj_all_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       14 2024-06-03 10:04:20.000000 dj_all_auth-0.1b2/dj_all_auth.egg-info/requires.txt
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       12 2024-06-03 10:04:20.000000 dj_all_auth-0.1b2/dj_all_auth.egg-info/top_level.txt
-drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/docs/
--rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-06-03 05:45:25.000000 dj_all_auth-0.1b2/docs/.gitignore
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       88 2024-06-02 18:58:47.000000 dj_all_auth-0.1b2/pyproject.toml
--rw-rw-r--   0 deviser   (1000) deviser   (1000)     1025 2024-06-03 10:04:20.357715 dj_all_auth-0.1b2/setup.cfg
--rw-rw-r--   0 deviser   (1000) deviser   (1000)       38 2024-06-02 19:00:44.000000 dj_all_auth-0.1b2/setup.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-06-03 05:39:14.000000 dj_all_auth-0.1b3/LICENSE
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      140 2024-06-03 10:01:27.000000 dj_all_auth-0.1b3/MANIFEST.in
+-rw-r--r--   0 deviser   (1000) deviser   (1000)     2081 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/PKG-INFO
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1074 2024-06-03 10:34:27.000000 dj_all_auth-0.1b3/README.rst
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      559 2024-06-03 09:58:34.000000 dj_all_auth-0.1b3/dj_all_auth/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     2992 2024-06-02 20:07:47.000000 dj_all_auth-0.1b3/dj_all_auth/admin.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      152 2024-06-03 09:58:34.000000 dj_all_auth-0.1b3/dj_all_auth/apps.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      554 2024-03-30 22:46:44.000000 dj_all_auth-0.1b3/dj_all_auth/base_models.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      557 2024-06-02 21:50:53.000000 dj_all_auth-0.1b3/dj_all_auth/context_processors.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/lib/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1287 2024-06-02 21:21:20.000000 dj_all_auth-0.1b3/dj_all_auth/lib/Mail.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-01-14 01:50:51.000000 dj_all_auth-0.1b3/dj_all_auth/lib/__init__.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/migrations/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     4576 2024-06-03 05:06:59.000000 dj_all_auth-0.1b3/dj_all_auth/migrations/0001_initial.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-06-03 04:45:15.000000 dj_all_auth-0.1b3/dj_all_auth/migrations/__init__.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/models/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      272 2024-03-31 02:13:04.000000 dj_all_auth-0.1b3/dj_all_auth/models/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       57 2024-06-03 04:45:15.000000 dj_all_auth-0.1b3/dj_all_auth/models.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-03-04 17:09:21.000000 dj_all_auth-0.1b3/dj_all_auth/services/__init__.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/auth/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-03-09 22:30:18.000000 dj_all_auth-0.1b3/dj_all_auth/services/auth/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     4977 2024-06-02 21:24:59.000000 dj_all_auth-0.1b3/dj_all_auth/services/auth/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/connections/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-03-30 22:34:37.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/__init__.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     5733 2024-06-02 21:26:59.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/Discord.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      236 2024-06-02 21:27:09.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      629 2024-06-02 21:27:26.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/models.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      374 2024-03-30 23:17:39.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/urls.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1900 2024-04-15 09:07:04.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/connections/google/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     5123 2024-03-31 02:48:39.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/google/Google.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      228 2024-03-24 10:17:00.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/google/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      660 2024-03-30 22:40:50.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/google/models.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      370 2024-03-24 10:17:00.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/google/urls.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1912 2024-03-30 22:55:38.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/google/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     3306 2024-03-31 02:49:04.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/Steam.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       88 2024-03-30 22:55:55.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      455 2024-03-30 22:43:31.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/models.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      366 2024-03-24 10:17:00.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/urls.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1520 2024-03-30 22:52:49.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     6017 2024-03-31 02:49:48.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/Twitch.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      228 2024-03-24 10:17:00.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      626 2024-03-30 22:43:50.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/models.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      370 2024-03-24 10:17:00.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/urls.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1880 2024-03-30 22:52:57.000000 dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/profile/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       77 2024-03-20 11:53:53.000000 dj_all_auth-0.1b3/dj_all_auth/services/profile/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      800 2024-05-21 07:26:13.000000 dj_all_auth-0.1b3/dj_all_auth/services/profile/models.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      224 2024-03-24 08:11:07.000000 dj_all_auth-0.1b3/dj_all_auth/services/profile/urls.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     2363 2024-06-02 21:32:21.000000 dj_all_auth-0.1b3/dj_all_auth/services/profile/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.746355 dj_all_auth-0.1b3/dj_all_auth/services/security/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       78 2024-03-21 07:36:00.000000 dj_all_auth-0.1b3/dj_all_auth/services/security/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      147 2024-03-21 07:36:52.000000 dj_all_auth-0.1b3/dj_all_auth/services/security/urls.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      331 2024-03-20 11:00:57.000000 dj_all_auth-0.1b3/dj_all_auth/services/security/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/static/
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/static/images/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)    17974 2024-02-17 22:48:33.000000 dj_all_auth-0.1b3/dj_all_auth/static/images/default.webp
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)   343102 2024-01-14 01:50:51.000000 dj_all_auth-0.1b3/dj_all_auth/static/images/loginRegister.webp
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     5802 2024-05-23 09:21:42.000000 dj_all_auth-0.1b3/dj_all_auth/static/images/logo.webp
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/static/justify/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)    14522 2024-01-14 01:50:51.000000 dj_all_auth-0.1b3/dj_all_auth/static/justify/justify.js
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/static/notify/
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/static/notify/css/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     2931 2024-02-17 23:02:28.000000 dj_all_auth-0.1b3/dj_all_auth/static/notify/css/notify.css
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/static/notify/js/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     5847 2024-02-17 23:02:16.000000 dj_all_auth-0.1b3/dj_all_auth/static/notify/js/notify.js
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/templates/
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1353 2024-06-02 21:51:32.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/base.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1933 2024-04-15 09:04:30.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/login.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      420 2024-06-02 21:52:19.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/logout.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1531 2024-04-15 09:04:41.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      882 2024-04-15 09:04:47.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset_complete.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1637 2024-04-15 09:04:51.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset_confirm.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      766 2024-04-15 09:04:55.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset_done.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     3075 2024-04-15 09:03:38.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/register.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1414 2024-04-15 09:04:59.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/request_account_activation.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1761 2024-05-23 10:06:44.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/index.html
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      912 2024-03-24 11:34:38.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/base.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1439 2024-05-09 20:22:18.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/css_section.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      252 2024-01-14 02:51:52.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/flash_messages.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      400 2024-03-17 21:46:15.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/head_section.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1204 2024-04-15 09:24:26.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/js_section.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      717 2024-03-24 11:52:16.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/navbar.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     5476 2024-01-14 01:50:51.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/page-loader.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1464 2024-05-09 20:21:57.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/sidebar.html
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.742355 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/activate_request/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      110 2024-04-29 18:21:11.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/activate_request/mail.text
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/password_reset/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      612 2024-01-14 01:50:51.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/password_reset/mail.text
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/register/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      110 2024-04-29 18:21:53.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/register/mail.text
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/profile/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)    11978 2024-05-23 10:03:43.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/profile/index.html
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/security/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1017 2024-05-01 11:46:23.000000 dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/security/index.html
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       60 2024-06-03 04:45:15.000000 dj_all_auth-0.1b3/dj_all_auth/tests.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     2142 2024-03-31 01:05:33.000000 dj_all_auth-0.1b3/dj_all_auth/urls.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth/utils/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1051 2024-06-02 21:34:57.000000 dj_all_auth-0.1b3/dj_all_auth/utils/TokenGenerator.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-01-14 01:50:51.000000 dj_all_auth-0.1b3/dj_all_auth/utils/__init__.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      785 2024-06-02 21:34:34.000000 dj_all_auth-0.1b3/dj_all_auth/utils/forms.py
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)      325 2024-03-24 10:21:56.000000 dj_all_auth-0.1b3/dj_all_auth/views.py
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/dj_all_auth.egg-info/
+-rw-r--r--   0 deviser   (1000) deviser   (1000)     2081 2024-06-03 10:56:40.000000 dj_all_auth-0.1b3/dj_all_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     3704 2024-06-03 10:56:40.000000 dj_all_auth-0.1b3/dj_all_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        1 2024-06-03 10:56:40.000000 dj_all_auth-0.1b3/dj_all_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       14 2024-06-03 10:56:40.000000 dj_all_auth-0.1b3/dj_all_auth.egg-info/requires.txt
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       12 2024-06-03 10:56:40.000000 dj_all_auth-0.1b3/dj_all_auth.egg-info/top_level.txt
+drwxrwxr-x   0 deviser   (1000) deviser   (1000)        0 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/docs/
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)        0 2024-06-03 05:45:25.000000 dj_all_auth-0.1b3/docs/.gitignore
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       88 2024-06-02 18:58:47.000000 dj_all_auth-0.1b3/pyproject.toml
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)     1025 2024-06-03 10:56:40.750356 dj_all_auth-0.1b3/setup.cfg
+-rw-rw-r--   0 deviser   (1000) deviser   (1000)       38 2024-06-02 19:00:44.000000 dj_all_auth-0.1b3/setup.py
```

### Comparing `dj_all_auth-0.1b2/PKG-INFO` & `dj_all_auth-0.1b3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-all-auth
-Version: 0.1b2
+Version: 0.1b3
 Summary: Django all auth includes all account, including django default, OAuth (Google, Discord, Twitch), openId (Steam).
 Home-page: https://www.example.com/
 Author: Deviser
 Author-email: deviserops+pypi@gmail.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -58,7 +58,15 @@
     python manage.py migrate
 
 5. If you are using multilanguage then to create language file run::
 
     python manage.py makemessages -i venv --all
 
 6. Visit the ``/accounts/`` URL to access user account.
+
+
+Notes:
+--------
+
+- static/notify :: Ref: https://github.com/deviserops/notify
+- static/justify :: Ref: https://github.com/deviserops/justify
+- static/images
```

### Comparing `dj_all_auth-0.1b2/README.rst` & `dj_all_auth-0.1b3/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -33,7 +33,15 @@
     python manage.py migrate
 
 5. If you are using multilanguage then to create language file run::
 
     python manage.py makemessages -i venv --all
 
 6. Visit the ``/accounts/`` URL to access user account.
+
+
+Notes:
+--------
+
+- static/notify :: Ref: https://github.com/deviserops/notify
+- static/justify :: Ref: https://github.com/deviserops/justify
+- static/images
```

### Comparing `dj_all_auth-0.1b2/dj_all_auth/__init__.py` & `dj_all_auth-0.1b3/dj_all_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/admin.py` & `dj_all_auth-0.1b3/dj_all_auth/admin.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/base_models.py` & `dj_all_auth-0.1b3/dj_all_auth/base_models.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/context_processors.py` & `dj_all_auth-0.1b3/dj_all_auth/context_processors.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/lib/Mail.py` & `dj_all_auth-0.1b3/dj_all_auth/lib/Mail.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/migrations/0001_initial.py` & `dj_all_auth-0.1b3/dj_all_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/auth/views.py` & `dj_all_auth-0.1b3/dj_all_auth/services/auth/views.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/Discord.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/Discord.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/models.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/models.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/discord/views.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/discord/views.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/google/Google.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/google/Google.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/google/models.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/google/models.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/google/views.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/google/views.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/Steam.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/Steam.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/steam/views.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/steam/views.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/Twitch.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/Twitch.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/models.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/models.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/connections/twitch/views.py` & `dj_all_auth-0.1b3/dj_all_auth/services/connections/twitch/views.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/profile/models.py` & `dj_all_auth-0.1b3/dj_all_auth/services/profile/models.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/services/profile/views.py` & `dj_all_auth-0.1b3/dj_all_auth/services/profile/views.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/base.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/base.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/login.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/login.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset_complete.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset_confirm.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/password_reset_done.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/register.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/register.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/auth/request_account_activation.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/auth/request_account_activation.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/index.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/index.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/base.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/base.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/css_section.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/css_section.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/js_section.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/js_section.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/navbar.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/navbar.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/page-loader.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/page-loader.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/layouts/sidebar.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/layouts/sidebar.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/mail/password_reset/mail.text` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/mail/password_reset/mail.text`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/profile/index.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/profile/index.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/templates/dj_all_auth/security/index.html` & `dj_all_auth-0.1b3/dj_all_auth/templates/dj_all_auth/security/index.html`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/urls.py` & `dj_all_auth-0.1b3/dj_all_auth/urls.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/utils/TokenGenerator.py` & `dj_all_auth-0.1b3/dj_all_auth/utils/TokenGenerator.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth/utils/forms.py` & `dj_all_auth-0.1b3/dj_all_auth/utils/forms.py`

 * *Files identical despite different names*

### Comparing `dj_all_auth-0.1b2/dj_all_auth.egg-info/PKG-INFO` & `dj_all_auth-0.1b3/dj_all_auth.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-all-auth
-Version: 0.1b2
+Version: 0.1b3
 Summary: Django all auth includes all account, including django default, OAuth (Google, Discord, Twitch), openId (Steam).
 Home-page: https://www.example.com/
 Author: Deviser
 Author-email: deviserops+pypi@gmail.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -58,7 +58,15 @@
     python manage.py migrate
 
 5. If you are using multilanguage then to create language file run::
 
     python manage.py makemessages -i venv --all
 
 6. Visit the ``/accounts/`` URL to access user account.
+
+
+Notes:
+--------
+
+- static/notify :: Ref: https://github.com/deviserops/notify
+- static/justify :: Ref: https://github.com/deviserops/justify
+- static/images
```

### Comparing `dj_all_auth-0.1b2/dj_all_auth.egg-info/SOURCES.txt` & `dj_all_auth-0.1b3/dj_all_auth.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,20 @@
 dj_all_auth/services/profile/__init__.py
 dj_all_auth/services/profile/models.py
 dj_all_auth/services/profile/urls.py
 dj_all_auth/services/profile/views.py
 dj_all_auth/services/security/__init__.py
 dj_all_auth/services/security/urls.py
 dj_all_auth/services/security/views.py
+dj_all_auth/static/images/default.webp
+dj_all_auth/static/images/loginRegister.webp
+dj_all_auth/static/images/logo.webp
+dj_all_auth/static/justify/justify.js
+dj_all_auth/static/notify/css/notify.css
+dj_all_auth/static/notify/js/notify.js
 dj_all_auth/templates/dj_all_auth/index.html
 dj_all_auth/templates/dj_all_auth/auth/base.html
 dj_all_auth/templates/dj_all_auth/auth/login.html
 dj_all_auth/templates/dj_all_auth/auth/logout.html
 dj_all_auth/templates/dj_all_auth/auth/password_reset.html
 dj_all_auth/templates/dj_all_auth/auth/password_reset_complete.html
 dj_all_auth/templates/dj_all_auth/auth/password_reset_confirm.html
```

### Comparing `dj_all_auth-0.1b2/setup.cfg` & `dj_all_auth-0.1b3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-all-auth
-version = 0.1-beta2
+version = 0.1-beta3
 description = Django all auth includes all account, including django default, OAuth (Google, Discord, Twitch), openId (Steam).
 long_description = file: README.rst
 url = https://www.example.com/
 author = Deviser
 author_email = deviserops+pypi@gmail.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

