# Comparing `tmp/django_simple_deploy-0.6.5.tar.gz` & `tmp/django_simple_deploy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_deploy-0.6.5.tar", last modified: Fri May 31 14:51:38 2024, max compression
+gzip compressed data, was "django_simple_deploy-0.7.0.tar", last modified: Mon Jun  3 00:26:26 2024, max compression
```

## Comparing `django_simple_deploy-0.6.5.tar` & `django_simple_deploy-0.7.0.tar`

### file list

```diff
@@ -1,89 +1,117 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:38.000249 django_simple_deploy-0.6.5/
--rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-31 14:51:38.000186 django_simple_deploy-0.6.5/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.999957 django_simple_deploy-0.6.5/django_simple_deploy.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-31 14:51:37.000000 django_simple_deploy-0.6.5/django_simple_deploy.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2804 2024-05-31 14:51:37.000000 django_simple_deploy-0.6.5/django_simple_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-31 14:51:37.000000 django_simple_deploy-0.6.5/django_simple_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       42 2024-05-31 14:51:37.000000 django_simple_deploy-0.6.5/django_simple_deploy.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       14 2024-05-31 14:51:37.000000 django_simple_deploy-0.6.5/django_simple_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.990117 django_simple_deploy-0.6.5/docs/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.992090 django_simple_deploy-0.6.5/docs/contributing/
--rw-r--r--   0 eric       (501) staff       (20)     2239 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.5/docs/contributing/architecture_notes.md
--rw-r--r--   0 eric       (501) staff       (20)      836 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.5/docs/contributing/coding_guide.md
--rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.5/docs/contributing/development_environment.md
--rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/contributing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/contributing/own_account.md
--rw-r--r--   0 eric       (501) staff       (20)     5344 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/docs/contributing/parking_lot.md
--rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.5/docs/contributing/test_run.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.992727 django_simple_deploy-0.6.5/docs/design_docs/
--rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/design_docs/rationale.md
--rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/design_docs/strengths_limitations.md
--rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/design_docs/use_cases.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.993143 django_simple_deploy-0.6.5/docs/general_documentation/
--rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.5/docs/general_documentation/choosing_platform.md
--rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/general_documentation/cli_reference.md
--rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/index.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.994260 django_simple_deploy-0.6.5/docs/maintaining/
--rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/maintaining/adr.md
--rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/maintaining/index.md
--rw-r--r--   0 eric       (501) staff       (20)     1859 2024-05-27 16:42:26.000000 django_simple_deploy-0.6.5/docs/maintaining/managing_releases.md
--rw-r--r--   0 eric       (501) staff       (20)     1666 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.5/docs/maintaining/merging_prs.md
--rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/maintaining/updating_docs.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.994953 django_simple_deploy-0.6.5/docs/quick_starts/
--rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/quick_starts/index.md
--rw-r--r--   0 eric       (501) staff       (20)     3937 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/docs/quick_starts/quick_start_flyio.md
--rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.5/docs/quick_starts/quick_start_heroku.md
--rw-r--r--   0 eric       (501) staff       (20)     3359 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/docs/quick_starts/quick_start_platformsh.md
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/requirements.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.995224 django_simple_deploy-0.6.5/docs/roadmap/
--rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/docs/roadmap/index.md
--rw-r--r--   0 eric       (501) staff       (20)     6143 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/docs/roadmap/reaching_one_point_o.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.996047 django_simple_deploy-0.6.5/docs/testing/
--rw-r--r--   0 eric       (501) staff       (20)     4740 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.5/docs/testing/e2e_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      665 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.5/docs/testing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     5142 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.5/docs/testing/integration_tests.md
--rw-r--r--   0 eric       (501) staff       (20)     1251 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.5/docs/testing/unit_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django_simple_deploy-0.6.5/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)     1355 2024-05-31 14:51:38.000923 django_simple_deploy-0.6.5/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.996291 django_simple_deploy-0.6.5/simple_deploy/
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      157 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.5/simple_deploy/apps.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.987626 django_simple_deploy-0.6.5/simple_deploy/management/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.996941 django_simple_deploy-0.6.5/simple_deploy/management/commands/
--rw-r--r--   0 eric       (501) staff       (20)     3902 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/cli.py
--rw-r--r--   0 eric       (501) staff       (20)     3342 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.997200 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/
--rw-r--r--   0 eric       (501) staff       (20)    29285 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     7830 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.997821 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/
--rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/dockerfile
--rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
--rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
--rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/fly.toml
--rw-r--r--   0 eric       (501) staff       (20)     1416 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.998089 django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/
--rw-r--r--   0 eric       (501) staff       (20)    19163 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     4650 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.998280 django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/templates/
--rw-r--r--   0 eric       (501) staff       (20)     1285 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.998744 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/
--rw-r--r--   0 eric       (501) staff       (20)    16681 2024-05-31 14:28:44.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     6986 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.999525 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/
--rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/services.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1072 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.988157 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/tests/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.999651 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/tests/unit_tests/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-31 14:51:37.999783 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/
--rw-r--r--   0 eric       (501) staff       (20)      640 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
--rw-r--r--   0 eric       (501) staff       (20)     1256 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
--rw-r--r--   0 eric       (501) staff       (20)     1010 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/utils.py
--rw-r--r--   0 eric       (501) staff       (20)    27314 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/simple_deploy.py
--rw-r--r--   0 eric       (501) staff       (20)    12349 2024-05-25 22:52:28.000000 django_simple_deploy-0.6.5/simple_deploy/management/commands/utils.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.763133 django_simple_deploy-0.7.0/
+-rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)     2834 2024-06-03 00:26:26.763076 django_simple_deploy-0.7.0/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.762869 django_simple_deploy-0.7.0/django_simple_deploy.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     2834 2024-06-03 00:26:26.000000 django_simple_deploy-0.7.0/django_simple_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     4780 2024-06-03 00:26:26.000000 django_simple_deploy-0.7.0/django_simple_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2024-06-03 00:26:26.000000 django_simple_deploy-0.7.0/django_simple_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       56 2024-06-03 00:26:26.000000 django_simple_deploy-0.7.0/django_simple_deploy.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       14 2024-06-03 00:26:26.000000 django_simple_deploy-0.7.0/django_simple_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.750208 django_simple_deploy-0.7.0/docs/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.751094 django_simple_deploy-0.7.0/docs/contributing/
+-rw-r--r--   0 eric       (501) staff       (20)     2239 2024-05-26 21:53:10.000000 django_simple_deploy-0.7.0/docs/contributing/architecture_notes.md
+-rw-r--r--   0 eric       (501) staff       (20)     1157 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/docs/contributing/coding_guide.md
+-rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django_simple_deploy-0.7.0/docs/contributing/development_environment.md
+-rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/contributing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/contributing/own_account.md
+-rw-r--r--   0 eric       (501) staff       (20)     7011 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/docs/contributing/parking_lot.md
+-rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django_simple_deploy-0.7.0/docs/contributing/test_run.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.751475 django_simple_deploy-0.7.0/docs/design_docs/
+-rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/design_docs/rationale.md
+-rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/design_docs/strengths_limitations.md
+-rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/design_docs/use_cases.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.751724 django_simple_deploy-0.7.0/docs/general_documentation/
+-rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django_simple_deploy-0.7.0/docs/general_documentation/choosing_platform.md
+-rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/general_documentation/cli_reference.md
+-rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/index.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.752361 django_simple_deploy-0.7.0/docs/maintaining/
+-rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/maintaining/adr.md
+-rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/maintaining/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     1859 2024-05-27 16:42:26.000000 django_simple_deploy-0.7.0/docs/maintaining/managing_releases.md
+-rw-r--r--   0 eric       (501) staff       (20)     1666 2024-05-28 19:42:57.000000 django_simple_deploy-0.7.0/docs/maintaining/merging_prs.md
+-rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/maintaining/updating_docs.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.752868 django_simple_deploy-0.7.0/docs/quick_starts/
+-rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/quick_starts/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3937 2024-05-30 16:43:25.000000 django_simple_deploy-0.7.0/docs/quick_starts/quick_start_flyio.md
+-rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django_simple_deploy-0.7.0/docs/quick_starts/quick_start_heroku.md
+-rw-r--r--   0 eric       (501) staff       (20)     3359 2024-05-30 16:43:25.000000 django_simple_deploy-0.7.0/docs/quick_starts/quick_start_platformsh.md
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/requirements.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.753142 django_simple_deploy-0.7.0/docs/roadmap/
+-rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/docs/roadmap/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     6143 2024-05-30 16:43:25.000000 django_simple_deploy-0.7.0/docs/roadmap/reaching_one_point_o.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.753626 django_simple_deploy-0.7.0/docs/testing/
+-rw-r--r--   0 eric       (501) staff       (20)     4740 2024-04-22 20:08:42.000000 django_simple_deploy-0.7.0/docs/testing/e2e_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      665 2024-04-22 20:08:42.000000 django_simple_deploy-0.7.0/docs/testing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     5142 2024-04-22 20:08:42.000000 django_simple_deploy-0.7.0/docs/testing/integration_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)     1251 2024-04-22 20:08:42.000000 django_simple_deploy-0.7.0/docs/testing/unit_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django_simple_deploy-0.7.0/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1372 2024-06-03 00:26:26.763788 django_simple_deploy-0.7.0/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.754381 django_simple_deploy-0.7.0/simple_deploy/
+-rw-r--r--   0 eric       (501) staff       (20)       64 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      157 2024-05-23 22:47:20.000000 django_simple_deploy-0.7.0/simple_deploy/apps.py
+-rw-r--r--   0 eric       (501) staff       (20)      441 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/hookspecs.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.747379 django_simple_deploy-0.7.0/simple_deploy/management/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.755432 django_simple_deploy-0.7.0/simple_deploy/management/commands/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     3902 2024-04-22 20:08:42.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/cli.py
+-rw-r--r--   0 eric       (501) staff       (20)     3342 2024-05-23 22:47:20.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.755957 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/
+-rw-r--r--   0 eric       (501) staff       (20)     1079 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     7830 2024-05-30 16:43:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.757039 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/developer_resources/
+-rw-r--r--   0 eric       (501) staff       (20)      692 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/developer_resources/README.md
+-rw-r--r--   0 eric       (501) staff       (20)     4431 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/developer_resources/fly_apps_create.json
+-rw-r--r--   0 eric       (501) staff       (20)    11569 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/developer_resources/fly_apps_list_one_app_deployed.json
+-rw-r--r--   0 eric       (501) staff       (20)     3673 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/developer_resources/fly_apps_list_one_app_not_deployed.json
+-rw-r--r--   0 eric       (501) staff       (20)      157 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/developer_resources/fly_postgres_users.txt
+-rw-r--r--   0 eric       (501) staff       (20)      943 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/developer_resources/platform_notes.md
+-rw-r--r--   0 eric       (501) staff       (20)    29450 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/platform_deployer.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.757918 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/
+-rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/dockerfile
+-rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
+-rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
+-rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/fly.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1416 2024-05-28 19:42:57.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.758494 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/
+-rw-r--r--   0 eric       (501) staff       (20)      731 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     4650 2024-05-26 21:53:10.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.759081 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/developer_resources/
+-rw-r--r--   0 eric       (501) staff       (20)      692 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/developer_resources/README.md
+-rw-r--r--   0 eric       (501) staff       (20)      931 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/developer_resources/heroku_apps_create.json
+-rw-r--r--   0 eric       (501) staff       (20)     1557 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/developer_resources/heroku_apps_info_no_db.json
+-rw-r--r--   0 eric       (501) staff       (20)     3200 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/developer_resources/heroku_apps_info_with_db.json
+-rw-r--r--   0 eric       (501) staff       (20)    19258 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/platform_deployer.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.759228 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1285 2024-05-28 19:42:57.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.760001 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/
+-rw-r--r--   0 eric       (501) staff       (20)      909 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     6986 2024-05-30 16:43:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.760223 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/
+-rw-r--r--   0 eric       (501) staff       (20)      692 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.761625 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/
+-rw-r--r--   0 eric       (501) staff       (20)      896 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/README.md
+-rw-r--r--   0 eric       (501) staff       (20)     2740 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/platform_create_help.txt
+-rw-r--r--   0 eric       (501) staff       (20)     2443 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/platform_create_output.txt
+-rw-r--r--   0 eric       (501) staff       (20)     1440 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/platform_organization_info_output.txt
+-rw-r--r--   0 eric       (501) staff       (20)      398 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/platform_organization_list_output.txt
+-rw-r--r--   0 eric       (501) staff       (20)     4497 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/platform_project_info_output.txt
+-rw-r--r--   0 eric       (501) staff       (20)     2456 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/developer_resources/output_samples/platform_push_help.txt
+-rw-r--r--   0 eric       (501) staff       (20)    16804 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/platform_deployer.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.762408 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/services.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1072 2024-05-23 23:04:10.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.748462 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.762528 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/tests/unit_tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-06-03 00:26:26.762694 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/
+-rw-r--r--   0 eric       (501) staff       (20)      640 2024-05-23 00:41:20.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
+-rw-r--r--   0 eric       (501) staff       (20)     1256 2024-05-30 16:43:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
+-rw-r--r--   0 eric       (501) staff       (20)     1010 2024-05-30 16:43:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/utils.py
+-rw-r--r--   0 eric       (501) staff       (20)    28928 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/simple_deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)    11707 2024-06-03 00:15:25.000000 django_simple_deploy-0.7.0/simple_deploy/management/commands/utils.py
+-rw-r--r--   0 eric       (501) staff       (20)      110 2024-06-01 20:21:00.000000 django_simple_deploy-0.7.0/simple_deploy/plugins.py
```

### Comparing `django_simple_deploy-0.6.5/LICENSE` & `django_simple_deploy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/PKG-INFO` & `django_simple_deploy-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.5
+Version: 0.7.0
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.2
+Requires-Dist: pluggy>=1.5.0
 Requires-Dist: toml>=0.10.2
 Requires-Dist: requests>=2.28.0
 
 # django-simple-deploy
 
 Initial Django deployments made easy.
```

### Comparing `django_simple_deploy-0.6.5/README.md` & `django_simple_deploy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/django_simple_deploy.egg-info/PKG-INFO` & `django_simple_deploy-0.7.0/django_simple_deploy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.5
+Version: 0.7.0
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.2
+Requires-Dist: pluggy>=1.5.0
 Requires-Dist: toml>=0.10.2
 Requires-Dist: requests>=2.28.0
 
 # django-simple-deploy
 
 Initial Django deployments made easy.
```

### Comparing `django_simple_deploy-0.6.5/docs/contributing/architecture_notes.md` & `django_simple_deploy-0.7.0/docs/contributing/architecture_notes.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/contributing/coding_guide.md` & `django_simple_deploy-0.7.0/docs/contributing/coding_guide.md`

 * *Files 17% similar despite different names*

```diff
@@ -22,7 +22,17 @@
 
 ## Python usage
 
 ### Use `path.read_text()` when possible.
 
 We are passing paths around most of the time. Use `path.read_text()`, rather than `with open(filename)`.
 
+
+## Working with plugins
+
+### Return values
+
+When you call out to a function implemented by a plugin that returns a value, that value is packed into a list. Often we're just dealing with one plugin, so you'll see code that looks like this:
+
+```python
+automate_all_msg = pm.hook.simple_deploy_get_automate_all_msg()[0]
+```
```

### Comparing `django_simple_deploy-0.6.5/docs/contributing/development_environment.md` & `django_simple_deploy-0.7.0/docs/contributing/development_environment.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/contributing/index.md` & `django_simple_deploy-0.7.0/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/contributing/own_account.md` & `django_simple_deploy-0.7.0/docs/contributing/own_account.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/contributing/test_run.md` & `django_simple_deploy-0.7.0/docs/contributing/test_run.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/design_docs/rationale.md` & `django_simple_deploy-0.7.0/docs/design_docs/rationale.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/design_docs/strengths_limitations.md` & `django_simple_deploy-0.7.0/docs/design_docs/strengths_limitations.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/design_docs/use_cases.md` & `django_simple_deploy-0.7.0/docs/design_docs/use_cases.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/general_documentation/choosing_platform.md` & `django_simple_deploy-0.7.0/docs/general_documentation/choosing_platform.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/general_documentation/cli_reference.md` & `django_simple_deploy-0.7.0/docs/general_documentation/cli_reference.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/index.md` & `django_simple_deploy-0.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/maintaining/adr.md` & `django_simple_deploy-0.7.0/docs/maintaining/adr.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/maintaining/index.md` & `django_simple_deploy-0.7.0/docs/maintaining/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/maintaining/managing_releases.md` & `django_simple_deploy-0.7.0/docs/maintaining/managing_releases.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/maintaining/merging_prs.md` & `django_simple_deploy-0.7.0/docs/maintaining/merging_prs.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/maintaining/updating_docs.md` & `django_simple_deploy-0.7.0/docs/maintaining/updating_docs.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/quick_starts/quick_start_flyio.md` & `django_simple_deploy-0.7.0/docs/quick_starts/quick_start_flyio.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/quick_starts/quick_start_heroku.md` & `django_simple_deploy-0.7.0/docs/quick_starts/quick_start_heroku.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/quick_starts/quick_start_platformsh.md` & `django_simple_deploy-0.7.0/docs/quick_starts/quick_start_platformsh.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/roadmap/reaching_one_point_o.md` & `django_simple_deploy-0.7.0/docs/roadmap/reaching_one_point_o.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/testing/e2e_tests.md` & `django_simple_deploy-0.7.0/docs/testing/e2e_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/testing/index.md` & `django_simple_deploy-0.7.0/docs/testing/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/testing/integration_tests.md` & `django_simple_deploy-0.7.0/docs/testing/integration_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/docs/testing/unit_tests.md` & `django_simple_deploy-0.7.0/docs/testing/unit_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/setup.cfg` & `django_simple_deploy-0.7.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-simple-deploy
-version = 0.6.5
+version = 0.7.0
 description = A management command that auto-configures a Django project for deployment.
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Documentation = https://django-simple-deploy.readthedocs.io/en/latest/
 	GitHub = https://github.com/ehmatthes/django-simple-deploy
 	Changelog = https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
@@ -32,14 +32,15 @@
 
 [options]
 include_package_data = true
 packages = simple_deploy
 python_requires = >=3.8
 install_requires = 
 	Django >=  4.2
+	pluggy >= 1.5.0
 	toml >= 0.10.2
 	requests >= 2.28.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/cli.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/cli.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/deploy_messages.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/deploy.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/platform_deployer.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,34 +11,31 @@
 import sys, os, re, json
 from pathlib import Path
 
 from django.utils.safestring import mark_safe
 
 import requests
 
-from simple_deploy.management.commands import deploy_messages as d_msgs
-from simple_deploy.management.commands.fly_io import deploy_messages as flyio_msgs
-
-from simple_deploy.management.commands.utils import SimpleDeployCommandError
-from simple_deploy.management.commands import utils as sd_utils
+from . import deploy_messages as platform_msgs
 
 
 class PlatformDeployer:
     """Perform the initial deployment to Fly.io
 
     If --automate-all is used, carry out an actual deployment.
     If not, do all configuration work so the user only has to commit changes, and call
     `fly deploy`.
     """
 
     def __init__(self, command):
         """Establishes connection to existing simple_deploy command object."""
         self.sd = command
         self.stdout = self.sd.stdout
-        self.messages = flyio_msgs
+        self.messages = platform_msgs
+        self.templates_path = Path(__file__).parent / "templates"
 
     # --- Public methods ---
 
     def deploy(self, *args, **options):
         """Coordinate the overall configuration and deployment."""
         self.sd.write_output("\nConfiguring project for deployment to Fly.io...")
 
@@ -144,15 +141,17 @@
 
         if self.sd.pkg_manager == "poetry":
             dockerfile_template = "dockerfile_poetry"
         elif self.sd.pkg_manager == "pipenv":
             dockerfile_template = "dockerfile_pipenv"
         else:
             dockerfile_template = "dockerfile"
-        sd_utils.write_file_from_template(path, dockerfile_template, context)
+        template_path = self.templates_path / dockerfile_template
+
+        self.sd.utils.write_file_from_template(path, template_path, context)
 
         msg = f"\n    Generated Dockerfile: {path}"
         self.sd.write_output(msg)
 
     def _add_dockerignore(self):
         """Add a dockerignore file, based on user's local project environmnet.
         Ignore virtual environment dir, system-specific cruft, and IDE cruft.
@@ -181,30 +180,34 @@
             self.sd.write_output("    Found existing fly.toml file.")
         else:
             # Generate file from template.
             context = {
                 "deployed_project_name": self.deployed_project_name,
                 "using_pipenv": (self.sd.pkg_manager == "pipenv"),
             }
-            sd_utils.write_file_from_template(path, "fly.toml", context)
+            template_path = self.templates_path / "fly.toml"
+
+            self.sd.utils.write_file_from_template(path, template_path, context)
 
             msg = f"\n    Generated fly.toml: {path}"
             self.sd.write_output(msg)
 
     def _modify_settings(self):
         """Add platformsh-specific settings."""
         self.sd.write_output("\n  Adding a Fly.io-specific settings block...")
 
         settings_string = self.sd.settings_path.read_text()
         safe_settings_string = mark_safe(settings_string)
         context = {
             "current_settings": safe_settings_string,
             "deployed_project_name": self.deployed_project_name,
         }
-        sd_utils.write_file_from_template(self.sd.settings_path, "settings.py", context)
+        template_path = self.templates_path / "settings.py"
+
+        self.sd.utils.write_file_from_template(self.sd.settings_path, template_path, context)
 
         msg = f"    Modified settings.py file: {self.sd.settings_path}"
         self.sd.write_output(msg)
 
     def _add_requirements(self):
         """Add requirements for deploying to Fly.io."""
         requirements = ["gunicorn", "psycopg2-binary", "dj-database-url", "whitenoise"]
@@ -323,29 +326,29 @@
         """Make sure the Fly.io CLI is installed, and user is authenticated."""
         cmd = "fly version"
 
         # This generates a FileNotFoundError on Ubuntu if the CLI is not installed.
         try:
             output_obj = self.sd.run_quick_command(cmd)
         except FileNotFoundError:
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
 
         self.sd.log_info(output_obj)
 
         # DEV: Note which OS this block runs on; I believe it's macOS.
         if output_obj.returncode:
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
 
         # Check that user is authenticated.
         cmd = "fly auth whoami --json"
         output_obj = self.sd.run_quick_command(cmd)
 
         error_msg = "Error: No access token available."
         if error_msg in output_obj.stderr.decode():
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_logged_out)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_logged_out)
 
         # Show current authenticated fly user.
         whoami_json = json.loads(output_obj.stdout.decode())
         user_email = whoami_json["email"]
         msg = f"  Logged in to Fly.io CLI as: {user_email}"
         self.sd.write_output(msg)
 
@@ -413,28 +416,28 @@
         """Select the correct project to deploy to."""
 
         if not project_names:
             # No app name found.
             if self.sd.automate_all:
                 self.app_name = self._create_flyio_app()
             else:
-                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
+                raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.no_project_name)
         elif len(project_names) == 1:
             # Only one app name found. Confirm we can deploy to this app.
             project_name = project_names[0]
             msg = f"\n*** Found one undeployed app on Fly.io: {project_name} ***"
             self.sd.write_output(msg)
 
             prompt = "Is this the app you want to deploy to?"
             if self.sd.get_confirmation(prompt):
                 self.app_name = project_name
             elif self.sd.automate_all:
                 self.app_name = self._create_flyio_app()
             else:
-                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
+                raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.no_project_name)
         else:
             # More than one undeployed app found. `apps list` doesn't show
             # much specific information for undeployed apps. For exmaple we
             # don't know the creation date, so we can't identify the most
             # recently created app.
 
             # Rather than a bunch of conditional logic about automate-all runs, just add
@@ -450,15 +453,15 @@
 
             valid_choices = [i for i in range(len(project_names))]
 
             # Confirm selection, because we do *not* want to deploy
             # against the wrong app.
             confirmed = False
             while not confirmed:
-                selection = sd_utils.get_numbered_choice(
+                selection = self.sd.utils.get_numbered_choice(
                     self.sd, prompt, valid_choices, self.messages.no_project_name
                 )
                 selected_name = project_names[selection]
 
                 confirm_prompt = f"You have selected {selected_name}."
                 confirm_prompt += " Is that correct?"
                 confirmed = self.sd.get_confirmation(confirm_prompt)
@@ -493,15 +496,15 @@
         self.sd.write_output(output_str)
 
         # Get app name.
         app_dict = json.loads(output_str)
         try:
             self.app_name = app_dict["Name"]
         except KeyError:
-            raise SimpleDeployCommandError(self.sd, self.messages.create_app_failed)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.create_app_failed)
         else:
             msg = f"  Created new app: {self.app_name}"
             self.sd.write_output(msg)
             return self.app_name
 
     def _create_db(self):
         """Create a remote database.
@@ -687,15 +690,15 @@
         else:
             # This db has more than the default users, and not just the current app.
             # Let's not touch it. If anyone hits this situation and we should proceed,
             # we'll revisit this block.
             # Note: This path has only been tested once, by manually adding
             # "dummy-user" to the list of db users."
             msg = self.messages.cant_use_db(self.db_name, self.db_users)
-            raise SimpleDeployCommandError(self.sd, msg)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, msg)
 
     def _confirm_use_attached_db(self):
         """Confirm it's okay to use db that's already attached to this app.
 
         Returns:
             None: If confirmation granted.
 
@@ -705,15 +708,15 @@
         msg = self.messages.use_attached_db(self.db_name, self.db_users)
         self.sd.write_output(msg)
 
         msg = f"Okay to use {self.db_name} and proceed?"
         if not self.sd.get_confirmation(msg):
             # Permission to use this db denied. Can't simply create a new db,
             # because the name we'd use is already taken.
-            raise SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
 
     def _confirm_use_unattached_db(self):
         """Confirm it's okay to use db whose name matches this app, but hasn't
         been attached to this app.
 
         If confirmation given, calls _attach_db().
 
@@ -733,15 +736,15 @@
         if self.sd.get_confirmation(msg):
             self._attach_db(self.db_name)
             return
         else:
             # Permission to use this db denied.
             # Can't simply create a new db, because the name we'd use is
             # already taken.
-            raise SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
 
     def _confirm_create_db(self, db_cmd):
         """Confirm the user wants a database created on their behalf.
 
         Returns:
             None
 
@@ -754,15 +757,15 @@
 
         # Show the command that will be run on the user's behalf.
         self.stdout.write(self.messages.confirm_create_db(db_cmd))
         if self.sd.get_confirmation():
             self.stdout.write("  Creating database...")
         else:
             # Quit and invite the user to create a database manually.
-            raise SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
 
     def _attach_db(self):
         """Attach the database to the app."""
         msg = "  Attaching database to Fly.io app..."
         self.sd.write_output(msg)
         cmd = f"fly postgres attach --app {self.deployed_project_name} {self.db_name}"
 
@@ -775,8 +778,8 @@
         output_scrubbed = [
             l for l in output_str.splitlines() if "DATABASE_URL" not in l
         ]
         output_scrubbed = "\n".join(output_scrubbed)
         self.sd.log_info(output_scrubbed)
 
         msg = "  Attached database to app."
-        self.sd.write_output(msg)
+        self.sd.write_output(msg)
```

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/deploy_messages.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/fly.toml` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/fly.toml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/fly_io/templates/settings.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/fly_io/templates/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/deploy.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/platform_deployer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """Manages all Heroku-specific aspects of the deployment process."""
 
 import sys, os, re, json, subprocess
+from pathlib import Path
 from itertools import takewhile
 
 from django.conf import settings
 from django.core.management.base import CommandError
 from django.core.management.utils import get_random_secret_key
 from django.utils.crypto import get_random_string
 from django.utils.safestring import mark_safe
 
-from simple_deploy.management.commands import deploy_messages as d_msgs
-from simple_deploy.management.commands.heroku import deploy_messages as heroku_msgs
-
-from simple_deploy.management.commands.utils import SimpleDeployCommandError
-from simple_deploy.management.commands import utils as sd_utils
+from . import deploy_messages as platform_msgs
 
 
 class PlatformDeployer:
     """Perform the initial deployment to Heroku.
 
     If --automate-all is used, carry out an actual deployment.
     If not, do all configuration work so the user only has to commit changes, and run
     `git push heroku main`.
     """
 
     def __init__(self, command):
         """Establishes connection to existing simple_deploy command object."""
         self.sd = command
         self.stdout = self.sd.stdout
-        self.messages = heroku_msgs
+        self.messages = platform_msgs
+        self.templates_path = Path(__file__).parent / "templates"
 
     # --- Public methods ---
 
     def deploy(self, *args, **options):
         self.sd.write_output("\nConfiguring project for deployment to Heroku...")
 
         self._validate_platform()
@@ -209,15 +207,15 @@
         path = self.sd.project_root / "Procfile"
         self.sd.write_output(f"\n  Looking for {path.as_posix()}...")
 
         if path.exists():
             self.sd.write_output("    Found existing Procfile.")
             proceed = self.sd.get_confirmation(self.messages.procfile_found)
             if not proceed:
-                raise SimpleDeployCommandError(self.messages.cant_overwrite_procfile)
+                raise self.sd.utils.SimpleDeployCommandError(self.messages.cant_overwrite_procfile)
 
         # No Procfile exists, or we're free to write over existing one.
         self.sd.write_output("    Generating Procfile...")
 
         wsgi_path = f"{self.sd.local_project_name}.wsgi"
         if self.sd.nested_project:
             wsgi_path = f"{self.sd.local_project_name}.{wsgi_path}"
@@ -258,15 +256,17 @@
         setting should be customized.
         """
         self.sd.write_output("\n  Adding a Heroku-specific settings block...")
 
         settings_string = self.sd.settings_path.read_text()
         safe_settings_string = mark_safe(settings_string)
         context = {"current_settings": safe_settings_string}
-        sd_utils.write_file_from_template(self.sd.settings_path, "settings.py", context)
+
+        template_path = self.templates_path / "settings.py"
+        self.sd.utils.write_file_from_template(self.sd.settings_path, template_path, context)
 
         msg = f"    Modified settings.py file: {self.sd.settings_path}"
         self.sd.write_output(msg)
 
     def _conclude_automate_all(self):
         """Finish automating the push to Heroku."""
         if not self.sd.automate_all:
@@ -367,22 +367,22 @@
             return
 
         cmd = "heroku --version"
         try:
             output_obj = self.sd.run_quick_command(cmd)
         except FileNotFoundError:
             # This generates a FileNotFoundError on Linux (Ubuntu) if CLI not installed.
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
 
         self.sd.log_info(output_obj)
 
         # The returncode for a successful command is 0, so anything truthy means the
         # command errored out.
         if output_obj.returncode:
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
 
     def _check_cli_authenticated(self):
         """Verify the user has authenticated with the CLI.
 
         Returns:
             None
 
@@ -393,16 +393,17 @@
             return
 
         cmd = "heroku auth:whoami"
         output_obj = self.sd.run_quick_command(cmd)
         self.sd.log_info(output_obj)
 
         output_str = output_obj.stderr.decode()
-        if "Error: Invalid credentials provided" in output_str:
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_authenticated)
+        # I believe I've seen both of these messages when not logged in.
+        if ("Error: Invalid credentials provided" in output_str) or ("Error: not logged in" in output_str):
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_not_authenticated)
 
     def _check_heroku_project_available(self):
         """Verify that a Heroku project is available to push to.
 
         Assume the user has already run `heroku create.`
 
         Returns:
@@ -428,15 +429,15 @@
         output_obj = self.sd.run_quick_command(cmd)
         self.sd.write_output(output_obj)
 
         output_str = output_obj.stdout.decode()
 
         # If output_str is emtpy, there is no heroku app.
         if not output_str:
-            raise SimpleDeployCommandError(
+            raise self.sd.utils.SimpleDeployCommandError(
                 self.sd, self.messages.no_heroku_app_detected
             )
 
         # Parse output for app_name.
         self.apps_list = json.loads(output_str)
         app_dict = self.apps_list["app"]
         self.heroku_app_name = app_dict["name"]
```

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/deploy_messages.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/heroku/templates/settings.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/heroku/templates/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/deploy.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/platform_deployer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,33 @@
 from pathlib import Path
 
 from django.conf import settings
 from django.core.management.utils import get_random_secret_key
 from django.utils.crypto import get_random_string
 from django.utils.safestring import mark_safe
 
-from simple_deploy.management.commands import deploy_messages as d_msgs
-from simple_deploy.management.commands.platform_sh import deploy_messages as plsh_msgs
+from . import deploy_messages as platform_msgs
 
-from simple_deploy.management.commands.utils import SimpleDeployCommandError
-from simple_deploy.management.commands import utils as sd_utils
-from simple_deploy.management.commands.platform_sh import utils as plsh_utils
+from . import utils as plsh_utils
 
 
 class PlatformDeployer:
     """Perform the initial deployment to Platform.sh.
 
     If --automate-all is used, carry out an actual deployment.
     If not, do all configuration work so the user only has to commit changes, and call
     `platform push`.
     """
 
     def __init__(self, command):
         """Establishes connection to existing simple_deploy command object."""
         self.sd = command
         self.stdout = self.sd.stdout
-        self.messages = plsh_msgs
+        self.messages = platform_msgs
+        self.templates_path = Path(__file__).parent / "templates"
 
     # --- Public methods ---
 
     def deploy(self, *args, **options):
         """Coordinate the overall configuration and deployment."""
 
         self.sd.write_output("\nConfiguring project for deployment to Platform.sh...")
@@ -109,28 +107,30 @@
             #   This may affect whether a CompletedProcess is returned, or an Exception
             # is raised.
             # Also, create command outputs project id to stdout if known, all other
             # output goes to stderr.
             self.sd.run_slow_command(cmd)
         except subprocess.CalledProcessError as e:
             error_msg = self.messages.unknown_create_error(e)
-            raise SimpleDeployCommandError(self.sd, error_msg)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, error_msg)
 
     def _modify_settings(self):
         """Add platformsh-specific settings.
 
         This settings block is currently the same for all users. The ALLOWED_HOSTS
         setting should be customized.
         """
         self.sd.write_output("\n  Adding a Platform.sh-specific settings block...")
 
         settings_string = self.sd.settings_path.read_text()
         safe_settings_string = mark_safe(settings_string)
         context = {"current_settings": safe_settings_string}
-        sd_utils.write_file_from_template(self.sd.settings_path, "settings.py", context)
+
+        template_path = self.templates_path / "settings.py"
+        self.sd.utils.write_file_from_template(self.sd.settings_path, template_path, context)
 
         msg = f"    Modified settings.py file: {self.sd.settings_path}"
         self.sd.write_output(msg)
 
     def _generate_platform_app_yaml(self):
         """Create .platform.app.yaml file, if not present."""
 
@@ -152,15 +152,17 @@
 
             if self.sd.pkg_manager == "poetry":
                 template_path = "poetry.platform.app.yaml"
             elif self.sd.pkg_manager == "pipenv":
                 template_path = "pipenv.platform.app.yaml"
             else:
                 template_path = "platform.app.yaml"
-            sd_utils.write_file_from_template(path, template_path, context)
+            template_path = self.templates_path / template_path
+
+            self.sd.utils.write_file_from_template(path, template_path, context)
 
             msg = f"\n    Generated {path.as_posix()}"
             self.sd.write_output(msg)
             return path
 
     def _add_requirements(self):
         """Add requirements for Platform.sh."""
@@ -185,15 +187,16 @@
         path = self.platform_dir_path / "services.yaml"
         self.sd.write_output(f"\n  Looking for {path.as_posix()}...")
 
         if path.exists():
             self.sd.write_output("    Found existing services.yaml file.")
         else:
             self.sd.write_output("    No services.yaml file found. Generating file...")
-            sd_utils.write_file_from_template(path, "services.yaml")
+            template_path = self.templates_path / "services.yaml"
+            self.sd.utils.write_file_from_template(path, template_path)
 
             msg = f"\n    Generated {path.as_posix()}"
             self.sd.write_output(msg)
             return path
 
     def _conclude_automate_all(self):
         """Finish automating the push to Platform.sh.
@@ -267,24 +270,24 @@
         """Make sure the Platform.sh CLI is installed, and user is authenticated."""
         cmd = "platform --version"
 
         # This generates a FileNotFoundError on Ubuntu if the CLI is not installed.
         try:
             output_obj = self.sd.run_quick_command(cmd)
         except FileNotFoundError:
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
 
         self.sd.log_info(output_obj)
 
         # Check that the user is authenticated.
         cmd = "platform auth:info --no-interaction"
         output_obj = self.sd.run_quick_command(cmd)
 
         if "Authentication is required." in output_obj.stderr.decode():
-            raise SimpleDeployCommandError(self.sd, self.messages.cli_logged_out)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.cli_logged_out)
 
     def _get_platformsh_project_name(self):
         """Get the deployed project name.
 
         If using automate_all, we'll set this. Otherwise, we're looking for the name
         that was given in the `platform create` command.
         - Try to get this from `project:info`.
@@ -318,23 +321,23 @@
         # If there's no stdout, the user is probably logged out, hasn't called
         #   create, or doesn't have the CLI installed.
         # Also, I've seen both ProjectNotFoundException and RootNotFoundException
         #   raised when no project has been created.
         if not output_str:
             output_str = output_obj.stderr.decode()
             if "LoginRequiredException" in output_str:
-                raise SimpleDeployCommandError(self.sd, self.messages.login_required)
+                raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.login_required)
             elif "ProjectNotFoundException" in output_str:
-                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
+                raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.no_project_name)
             elif "RootNotFoundException" in output_str:
-                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
+                raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.no_project_name)
             else:
                 error_msg = self.messages.unknown_error
                 error_msg += self.messages.cli_not_installed
-                raise SimpleDeployCommandError(self.sd, error_msg)
+                raise self.sd.utils.SimpleDeployCommandError(self.sd, error_msg)
 
         # Pull deployed project name from output.
         lines = output_str.splitlines()
         title_line = [line for line in lines if "title," in line][0]
         # Assume first project is one to use.
         project_name = title_line.split(",")[1].strip()
         project_name = plsh_utils.get_project_name(output_str)
@@ -343,15 +346,15 @@
         # See: https://github.com/ehmatthes/django-simple-deploy/issues/323
         if " " in project_name:
             project_name = project_name.replace(" ", "_").lower()
         if project_name:
             return project_name
 
         # Couldn't find a project name. Warn user, and tell them about override flag.
-        raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
+        raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.no_project_name)
 
     def _get_org_name(self):
         """Get the organization name associated with the user's Platform.sh account.
 
         This is needed for creating a project using automate_all.
         Confirm that it's okay to use this org.
 
@@ -369,15 +372,15 @@
         cmd = "platform organization:list --yes --format csv"
         output_obj = self.sd.run_quick_command(cmd)
         output_str = output_obj.stdout.decode()
         self.sd.log_info(output_str)
 
         org_names = plsh_utils.get_org_names(output_str)
         if not org_names:
-            raise SimpleDeployCommandError(self.sd, self.messages.org_not_found)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, self.messages.org_not_found)
 
         if len(org_names) == 1:
             # Get permission to use this org.
             org_name = org_names[0]
             if self._confirm_use_org(org_name):
                 return org_name
 
@@ -388,15 +391,15 @@
         prompt += "\nWhich org would you like to use? "
 
         valid_choices = [i for i in range(len(org_names))]
 
         # Confirm selection, because we do *not* want to deploy using the wrong org.
         confirmed = False
         while not confirmed:
-            selection = sd_utils.get_numbered_choice(
+            selection = self.sd.utils.get_numbered_choice(
                 self.sd, prompt, valid_choices, self.messages.no_org_available
             )
             selected_org = org_names[selection]
 
             confirm_prompt = f"You have selected {selected_org}."
             confirm_prompt += " Is that correct?"
             confirmed = self.sd.get_confirmation(confirm_prompt)
@@ -417,8 +420,8 @@
         if confirmed:
             self.stdout.write("  Okay, continuing with deployment.")
             return True
         else:
             # Exit, with a message that configuration is still an option.
             msg = self.messages.cancel_plsh
             msg += self.messages.may_configure
-            raise SimpleDeployCommandError(self.sd, msg)
+            raise self.sd.utils.SimpleDeployCommandError(self.sd, msg)
```

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/deploy_messages.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/templates/settings.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/templates/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/platform_sh/utils.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/platform_sh/utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/simple_deploy.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/simple_deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,30 +31,32 @@
 from importlib import import_module
 
 from django.core.management.base import BaseCommand
 from django.conf import settings
 
 import toml
 
-from . import deploy_messages as d_msgs
-from . import utils as sd_utils
+from . import deploy_messages
+from . import utils
 from . import cli
 
+from simple_deploy.plugins import pm
+
 
 class Command(BaseCommand):
     """Configure a project for deployment to a specific platform.
 
     If using --automate-all, carry out the actual deployment as well.
     """
 
     # Show a summary of simple_deploy in the help text.
     help = "Configures your project for deployment to the specified platform."
 
     def __init__(self):
-        """Customize help output."""
+        """Customize help output, assign attributes."""
 
         # Keep default BaseCommand args out of help text.
         self.suppressed_base_arguments.update(
             [
                 "--version",
                 "-v",
                 "--settings",
@@ -63,14 +65,17 @@
                 "--no-color",
                 "--force-color",
             ]
         )
         # Ensure that --skip-checks is not included in help output.
         self.requires_system_checks = []
 
+        # Made utils available to plugins.
+        self.utils = utils
+
         super().__init__()
 
     def create_parser(self, prog_name, subcommand, **kwargs):
         """Customize the ArgumentParser object that will be created."""
         epilog = "For more help, see the full documentation at: "
         epilog += "https://django-simple-deploy.readthedocs.io"
         parser = super().create_parser(
@@ -108,17 +113,23 @@
             self._log_cli_args(options)
 
         self._validate_command()
         self._inspect_system()
         self._inspect_project()
         self._add_simple_deploy_req()
 
-        self._create_deployer()
-        self._confirm_automate_all()
-        self.platform_deployer.deploy()
+        # Get the platform-specific deployer module.
+        platform_module = import_module(
+            f".{self.platform}.deploy", package="simple_deploy.management.commands"
+        )
+        pm.register(platform_module, self.platform)
+        self._check_required_hooks(pm)
+
+        self._confirm_automate_all(pm)
+        pm.hook.simple_deploy_deploy(sd=self)
 
     # --- Methods used here, and also by platform-specific modules ---
 
     def write_output(self, output, write_to_console=True, skip_logging=False):
         """Write output to the appropriate places.
 
         Typically, this is used for writing output to the console as the configuration
@@ -128,27 +139,27 @@
         Output that's passed to this method typically needs to be logged as well, unless
         skip_logging has been passed. This is useful, for example, when writing
         sensitive information to the console.
 
         Returns:
             None
         """
-        output_str = sd_utils.get_string_from_output(output)
+        output_str = self.utils.get_string_from_output(output)
 
         if write_to_console:
             self.stdout.write(output_str)
 
         if not skip_logging:
             self.log_info(output_str)
 
     def log_info(self, output):
         """Log output, which may be a string or CompletedProcess instance."""
         if self.log_output:
-            output_str = sd_utils.get_string_from_output(output)
-            sd_utils.log_output_string(output_str)
+            output_str = self.utils.get_string_from_output(output)
+            self.utils.log_output_string(output_str)
 
     def run_quick_command(self, cmd, check=False, skip_logging=False):
         """Run a command that should finish quickly.
 
         Commands that should finish quickly can be run more simply than commands that
         will take a long time. For quick commands, we can capture output and then deal
         with it however we like, and the user won't notice that we first captured
@@ -275,15 +286,15 @@
         
         if not m:
             self.log_info(f"No {platform_name}-specific settings block found.")
             return
 
         # A platform-specific settings block exists. Get permission to overwrite it.
         if not self.get_confirmation(msg_found):
-            raise sd_utils.SimpleDeployCommandError(self, msg_cant_overwrite)
+            raise self.utils.SimpleDeployCommandError(self, msg_cant_overwrite)
 
         # Platform-specific settings exist, but we can remove them and start fresh.
         self.settings_path.write_text(m.group(1))
 
         msg = f"  Removed existing {platform_name}-specific settings block."
         self.write_output(msg)
 
@@ -315,20 +326,20 @@
         self.write_output(f"\nLooking for {package_name}...")
 
         if package_name in self.requirements:
             self.write_output(f"  Found {package_name} in requirements file.")
             return
 
         if self.pkg_manager == "pipenv":
-            sd_utils.add_pipenv_pkg(self.pipfile_path, package_name, version)
+            self.utils.add_pipenv_pkg(self.pipfile_path, package_name, version)
         elif self.pkg_manager == "poetry":
             self._check_poetry_deploy_group()
-            sd_utils.add_poetry_pkg(self.pyprojecttoml_path, package_name, version)
+            self.utils.add_poetry_pkg(self.pyprojecttoml_path, package_name, version)
         else:
-            sd_utils.add_req_txt_pkg(self.req_txt_path, package_name, version)
+            self.utils.add_req_txt_pkg(self.req_txt_path, package_name, version)
 
         self.write_output(f"  Added {package_name} to requirements file.")
 
     def commit_changes(self):
         """Commit changes that have been made to the project.
 
         This should only be called when automate_all is being used.
@@ -422,20 +433,20 @@
         Returns:
             None
 
         Raises:
             SimpleDeployCommandError: If requested platform is supported.
         """
         if not self.platform:
-            raise sd_utils.SimpleDeployCommandError(self, d_msgs.requires_platform_flag)
+            raise self.utils.SimpleDeployCommandError(self, deploy_messages.requires_platform_flag)
         elif self.platform in ["fly_io", "platform_sh", "heroku"]:
             self.write_output(f"\nDeployment target: {self.platform}")
         else:
-            error_msg = d_msgs.invalid_platform_msg(self.platform)
-            raise sd_utils.SimpleDeployCommandError(self, error_msg)
+            error_msg = deploy_messages.invalid_platform_msg(self.platform)
+            raise self.utils.SimpleDeployCommandError(self, error_msg)
 
     def _inspect_system(self):
         """Inspect the user's local system for relevant information.
 
         Uses self.on_windows and self.on_macos because those are clean checks to run.
         May want to refactor to self.user_system at some point. Don't ever use
         self.platform, because "platform" refers to the host we're deploying to.
@@ -526,15 +537,15 @@
             self.write_output(f"Found .git dir at {self.git_path}.")
             self.nested_project = True
         else:
             error_msg = "Could not find a .git/ directory."
             error_msg += (
                 f"\n  Looked in {self.project_root} and in {self.project_root.parent}."
             )
-            raise sd_utils.SimpleDeployCommandError(self, error_msg)
+            raise self.utils.SimpleDeployCommandError(self, error_msg)
 
     def _check_git_status(self):
         """Make sure all non-simple_deploy changes have already been committed.
 
         All configuration-specific work should be contained in a single commit. This
         allows users to easily revert back to the version of the project that worked
         locally, if the overall deployment effort fails, or if they don't like what
@@ -563,29 +574,29 @@
         self.log_info(f"{status_output}")
 
         cmd = "git diff --unified=0"
         output_obj = self.run_quick_command(cmd)
         diff_output = output_obj.stdout.decode()
         self.log_info(f"{diff_output}\n")
 
-        proceed = sd_utils.check_status_output(status_output, diff_output)
+        proceed = self.utils.check_status_output(status_output, diff_output)
 
         if proceed:
             msg = "No uncommitted changes, other than simple_deploy work."
             self.write_output(msg)
         else:
             self._raise_unclean_error()
 
     def _raise_unclean_error(self):
         """Raise unclean git status error."""
-        error_msg = d_msgs.unclean_git_status
+        error_msg = deploy_messages.unclean_git_status
         if self.automate_all:
-            error_msg += d_msgs.unclean_git_automate_all
+            error_msg += deploy_messages.unclean_git_automate_all
 
-        raise sd_utils.SimpleDeployCommandError(self, error_msg)
+        raise self.utils.SimpleDeployCommandError(self, error_msg)
 
     def _ignore_sd_logs(self):
         """Add log dir to .gitignore.
 
         Adds a .gitignore file if one is not found.
         """
         ignore_msg = "simple_deploy_logs/\n"
@@ -625,15 +636,15 @@
         elif self._check_using_poetry():
             return "poetry"
         elif (self.git_path / "requirements.txt").exists():
             return "req_txt"
 
         # Exit if we haven't found any requirements.
         error_msg = f"Couldn't find any specified requirements in {self.git_path}."
-        raise sd_utils.SimpleDeployCommandError(self, error_msg)
+        raise self.utils.SimpleDeployCommandError(self, error_msg)
 
     def _check_using_poetry(self):
         """Check if the project appears to be using poetry.
 
         Check for a pyproject.toml file with a [tool.poetry] section.
 
         Returns:
@@ -660,21 +671,21 @@
             List[str]: List of strings, each representing a requirement.
         """
         msg = "Checking current project requirements..."
         self.write_output(msg)
 
         if self.pkg_manager == "req_txt":
             self.req_txt_path = self.git_path / "requirements.txt"
-            requirements = sd_utils.parse_req_txt(self.req_txt_path)
+            requirements = self.utils.parse_req_txt(self.req_txt_path)
         elif self.pkg_manager == "pipenv":
             self.pipfile_path = self.git_path / "Pipfile"
-            requirements = sd_utils.parse_pipfile(self.pipfile_path)
+            requirements = self.utils.parse_pipfile(self.pipfile_path)
         elif self.pkg_manager == "poetry":
             self.pyprojecttoml_path = self.git_path / "pyproject.toml"
-            requirements = sd_utils.parse_pyproject_toml(self.pyprojecttoml_path)
+            requirements = self.utils.parse_pyproject_toml(self.pyprojecttoml_path)
 
         # Report findings.
         msg = "  Found existing dependencies:"
         self.write_output(msg)
         for requirement in requirements:
             msg = f"    {requirement}"
             self.write_output(msg)
@@ -693,39 +704,68 @@
 
     def _check_poetry_deploy_group(self):
         """Make sure a deploy group exists in pyproject.toml."""
         pptoml_data = toml.load(self.pyprojecttoml_path)
         try:
             deploy_group = pptoml_data["tool"]["poetry"]["group"]["deploy"]
         except KeyError:
-            sd_utils.create_poetry_deploy_group(self.pyprojecttoml_path)
+            self.utils.create_poetry_deploy_group(self.pyprojecttoml_path)
             msg = "    Added optional deploy group to pyproject.toml."
             self.write_output(msg)
 
-    def _create_deployer(self):
-        """Instantiate the PlatformDeployer object."""
-        deployer_module = import_module(
-            f".{self.platform}.deploy", package="simple_deploy.management.commands"
-        )
-        self.platform_deployer = deployer_module.PlatformDeployer(self)
+    def _check_required_hooks(self, pm):
+        """Check that all required hooks are implemeted by plugin.
 
-    def _confirm_automate_all(self):
+        Returns:
+            None
+        Raises:
+            SimpleDeployCommandError: If hook not found.
+        """
+        plugin = pm.list_name_plugin()[0][1]
+
+        callers = [caller.name for caller in pm.get_hookcallers(plugin)]
+        required_hooks = ["simple_deploy_automate_all_supported", "simple_deploy_deploy"]
+        for hook in required_hooks:
+            if hook not in callers:
+                msg = f"\nPlugin missing required hook implementation: {hook}()"
+                raise self.utils.SimpleDeployCommandError(self, msg)
+
+        # If plugin supports automate_all, make sure a confirmation message is provided.
+        if not pm.hook.simple_deploy_automate_all_supported()[0]:
+            return
+
+        hook = "simple_deploy_get_automate_all_msg"
+        if hook not in callers:
+            msg = f"\nPlugin missing required hook implementation: {hook}()"
+            raise self.utils.SimpleDeployCommandError(self, msg)
+
+    def _confirm_automate_all(self, pm):
         """Confirm the user understands what --automate-all does.
 
-        If confirmation not granted, exit with a message, but no error.
+        Also confirm that the selected platform/ plugin manager supports fully
+        automated deployments.
 
-        This must be called after the platform-specific deployer object is instantiated,
-        because we need a platform-specific confirmation message.
+        If confirmation not granted, exit with a message, but no error.
         """
         # Placing this check here keeps the handle() method cleaner.
         if not self.automate_all:
             return
 
-        self.write_output(self.platform_deployer.messages.confirm_automate_all)
+        # Make sure this platform supports automate-all.
+        supported = pm.hook.simple_deploy_automate_all_supported()[0]
+        if not supported:
+            msg = "\nThis platform does not support automated deployments."
+            msg += "\nYou may want to try again without the --automate-all flag."
+            raise self.utils.SimpleDeployCommandError(self, msg)
+
+        # Confirm the user wants to automate all steps.
+        msg = pm.hook.simple_deploy_get_automate_all_msg()[0]
+
+        self.write_output(msg)
         confirmed = self.get_confirmation()
 
         if confirmed:
             self.write_output("Automating all steps...")
         else:
             # Quit with a message, but don't raise an error.
-            self.write_output(d_msgs.cancel_automate_all)
+            self.write_output(deploy_messages.cancel_automate_all)
             sys.exit()
```

### Comparing `django_simple_deploy-0.6.5/simple_deploy/management/commands/utils.py` & `django_simple_deploy-0.7.0/simple_deploy/management/commands/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,49 +2,34 @@
 
 Also contains resources useful to platform-specific deployment scripts.
 """
 
 from pathlib import Path
 import inspect, re, sys, subprocess, logging
 
-from django.template.engine import Engine
+from django.template.engine import Engine, Context
 from django.template.utils import get_app_template_dirs
 from django.core.management.base import CommandError
 
 import toml
 
 
-def write_file_from_template(path, template, context=None):
+def write_file_from_template(dest_path, template_path, context=None):
     """Write a file based on a platform-specific template.
-    This may be a whole new file, such as a Dockerfile. Or, we may be
-    modifying an existing file such as settings.py.
+
+    This may be a whole new file, such as a Dockerfile. Or, we may be modifying an
+    existing file such as settings.py.
 
     Returns:
     - None
     """
-
-    # Get the platform name from the file that's importing this function.
-    #   This may need to be moved to its own file if it ends up being imported
-    #   from different places.
-    caller = inspect.stack()[1].filename
-    if sys.platform == "win32":
-        platform_re = r"\\simple_deploy\\management\\commands\\(.*)\\deploy.py"
-    else:
-        platform_re = r"/simple_deploy/management/commands/(.*)/deploy.py"
-    m = re.search(platform_re, caller)
-    platform = m.group(1)
-
-    # Make a template engine that can access the platform's templates.
-    my_dirs = get_app_template_dirs(f"management/commands/{platform}/templates")
-    my_engine = Engine(dirs=my_dirs)
-
-    # Generate the template string, and write it to the given path.
-    template_string = my_engine.render_to_string(template, context)
-    path.write_text(template_string)
-
+    my_engine = Engine()
+    template = my_engine.from_string(template_path.read_text())
+    rendered_template = template.render(Context(context))
+    dest_path.write_text(rendered_template)
 
 def get_numbered_choice(sd_command, prompt, valid_choices, quit_message):
     """Select from a numbered list of choices.
 
     This is used, for example, to select from a number of apps that the user
     has created on a platform.
     """
```

