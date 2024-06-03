# Comparing `tmp/django-axes-forked-5.27.0.2.tar.gz` & `tmp/django-axes-forked-5.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-forked-5.27.0.2.tar", last modified: Mon Jun  3 12:36:15 2024, max compression
+gzip compressed data, was "django-axes-forked-5.27.1.tar", last modified: Mon Jun  3 12:11:04 2024, max compression
```

## Comparing `django-axes-forked-5.27.0.2.tar` & `django-axes-forked-5.27.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.566857 django-axes-forked-5.27.0.2/
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.536856 django-axes-forked-5.27.0.2/.github/
--rw-r--r--   0 me        (1000) me        (1000)      147 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/.github/dependabot.yml
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.536856 django-axes-forked-5.27.0.2/.github/workflows/
--rw-r--r--   0 me        (1000) me        (1000)      994 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/.github/workflows/release.yml
--rw-r--r--   0 me        (1000) me        (1000)     1956 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/.github/workflows/test.yml
--rw-r--r--   0 me        (1000) me        (1000)      185 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/.gitignore
--rw-r--r--   0 me        (1000) me        (1000)       10 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/.pre-commit-config.yaml
--rw-r--r--   0 me        (1000) me        (1000)       86 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/.prospector.yaml
--rw-r--r--   0 me        (1000) me        (1000)    28113 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/CHANGES.rst
--rw-r--r--   0 me        (1000) me        (1000)     2375 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 me        (1000) me        (1000)     1184 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/LICENSE
--rw-r--r--   0 me        (1000) me        (1000)    33327 2024-06-03 12:36:15.566857 django-axes-forked-5.27.0.2/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     3419 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/README.rst
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/
--rw-r--r--   0 me        (1000) me        (1000)      160 2024-06-03 11:17:26.000000 django-axes-forked-5.27.0.2/axes/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     2008 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/admin.py
--rw-r--r--   0 me        (1000) me        (1000)     1556 2024-06-03 11:17:22.000000 django-axes-forked-5.27.0.2/axes/apps.py
--rw-r--r--   0 me        (1000) me        (1000)     3041 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/attempts.py
--rw-r--r--   0 me        (1000) me        (1000)     2807 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/backends.py
--rw-r--r--   0 me        (1000) me        (1000)     4551 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/checks.py
--rw-r--r--   0 me        (1000) me        (1000)     5450 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/conf.py
--rw-r--r--   0 me        (1000) me        (1000)      628 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/decorators.py
--rw-r--r--   0 me        (1000) me        (1000)      380 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/exceptions.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/handlers/
--rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/handlers/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     6752 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/handlers/base.py
--rw-r--r--   0 me        (1000) me        (1000)     5889 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/handlers/cache.py
--rw-r--r--   0 me        (1000) me        (1000)    10428 2024-06-03 12:34:47.000000 django-axes-forked-5.27.0.2/axes/handlers/database.py
--rw-r--r--   0 me        (1000) me        (1000)      677 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/handlers/dummy.py
--rw-r--r--   0 me        (1000) me        (1000)     4479 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/handlers/proxy.py
--rw-r--r--   0 me        (1000) me        (1000)      644 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/handlers/test.py
--rw-r--r--   0 me        (1000) me        (1000)    18019 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/helpers.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.536856 django-axes-forked-5.27.0.2/axes/locale/
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.536856 django-axes-forked-5.27.0.2/axes/locale/de/
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 me        (1000) me        (1000)     1549 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 me        (1000) me        (1000)     2123 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.536856 django-axes-forked-5.27.0.2/axes/locale/pl/
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 me        (1000) me        (1000)     1526 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 me        (1000) me        (1000)     2266 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.536856 django-axes-forked-5.27.0.2/axes/locale/ru/
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 me        (1000) me        (1000)     1950 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 me        (1000) me        (1000)     2495 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.536856 django-axes-forked-5.27.0.2/axes/locale/tr/
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 me        (1000) me        (1000)     1450 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 me        (1000) me        (1000)     2075 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/management/
--rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/management/__init__.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.546856 django-axes-forked-5.27.0.2/axes/management/commands/
--rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/management/commands/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      404 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 me        (1000) me        (1000)      409 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/management/commands/axes_reset.py
--rw-r--r--   0 me        (1000) me        (1000)      552 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 me        (1000) me        (1000)      643 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 me        (1000) me        (1000)      579 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_user.py
--rw-r--r--   0 me        (1000) me        (1000)      579 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 me        (1000) me        (1000)     1583 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/middleware.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.556857 django-axes-forked-5.27.0.2/axes/migrations/
--rw-r--r--   0 me        (1000) me        (1000)     2831 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/migrations/0001_initial.py
--rw-r--r--   0 me        (1000) me        (1000)     1723 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 me        (1000) me        (1000)     1948 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 me        (1000) me        (1000)     2197 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 me        (1000) me        (1000)      219 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 me        (1000) me        (1000)      274 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 me        (1000) me        (1000)     1116 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/migrations/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     1473 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/models.py
--rw-r--r--   0 me        (1000) me        (1000)     1782 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/axes/signals.py
--rw-r--r--   0 me        (1000) me        (1000)     1656 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/axes/utils.py
--rw-r--r--   0 me        (1000) me        (1000)      212 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/codecov.yml
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.556857 django-axes-forked-5.27.0.2/django_axes_forked.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)    33327 2024-06-03 12:36:15.000000 django-axes-forked-5.27.0.2/django_axes_forked.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     2577 2024-06-03 12:36:15.000000 django-axes-forked-5.27.0.2/django_axes_forked.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2024-06-03 12:36:15.000000 django-axes-forked-5.27.0.2/django_axes_forked.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2024-06-03 12:09:58.000000 django-axes-forked-5.27.0.2/django_axes_forked.egg-info/not-zip-safe
--rw-r--r--   0 me        (1000) me        (1000)       43 2024-06-03 12:36:15.000000 django-axes-forked-5.27.0.2/django_axes_forked.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)        5 2024-06-03 12:36:15.000000 django-axes-forked-5.27.0.2/django_axes_forked.egg-info/top_level.txt
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.556857 django-axes-forked-5.27.0.2/docs/
--rw-r--r--   0 me        (1000) me        (1000)       43 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/docs/10_changelog.rst
--rw-r--r--   0 me        (1000) me        (1000)      648 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/1_requirements.rst
--rw-r--r--   0 me        (1000) me        (1000)     5527 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/2_installation.rst
--rw-r--r--   0 me        (1000) me        (1000)     4307 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/3_usage.rst
--rw-r--r--   0 me        (1000) me        (1000)    12928 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/4_configuration.rst
--rw-r--r--   0 me        (1000) me        (1000)     5917 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/5_customization.rst
--rw-r--r--   0 me        (1000) me        (1000)     9133 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/6_integration.rst
--rw-r--r--   0 me        (1000) me        (1000)     3596 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/7_architecture.rst
--rw-r--r--   0 me        (1000) me        (1000)      406 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/docs/8_reference.rst
--rw-r--r--   0 me        (1000) me        (1000)     1400 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/9_development.rst
--rw-r--r--   0 me        (1000) me        (1000)     7425 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/Makefile
--rw-r--r--   0 me        (1000) me        (1000)     4043 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/conf.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.556857 django-axes-forked-5.27.0.2/docs/images/
--rw-r--r--   0 me        (1000) me        (1000)   133029 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/docs/images/flow.png
--rw-r--r--   0 me        (1000) me        (1000)      355 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/docs/index.rst
--rw-r--r--   0 me        (1000) me        (1000)      249 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/manage.py
--rw-r--r--   0 me        (1000) me        (1000)      105 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/mypy.ini
--rw-r--r--   0 me        (1000) me        (1000)     1287 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/pyproject.toml
--rw-r--r--   0 me        (1000) me        (1000)       78 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/requirements-qa.txt
--rw-r--r--   0 me        (1000) me        (1000)       97 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/requirements-test.txt
--rw-r--r--   0 me        (1000) me        (1000)       89 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/requirements.txt
--rw-r--r--   0 me        (1000) me        (1000)       38 2024-06-03 12:36:15.566857 django-axes-forked-5.27.0.2/setup.cfg
--rw-r--r--   0 me        (1000) me        (1000)     2466 2024-06-03 12:35:57.000000 django-axes-forked-5.27.0.2/setup.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:36:15.556857 django-axes-forked-5.27.0.2/tests/
--rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/tests/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     5850 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/base.py
--rw-r--r--   0 me        (1000) me        (1000)     2048 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/settings.py
--rw-r--r--   0 me        (1000) me        (1000)      935 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_admin.py
--rw-r--r--   0 me        (1000) me        (1000)     5846 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_attempts.py
--rw-r--r--   0 me        (1000) me        (1000)      747 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/tests/test_backends.py
--rw-r--r--   0 me        (1000) me        (1000)     3585 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_checks.py
--rw-r--r--   0 me        (1000) me        (1000)     1939 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_decorators.py
--rw-r--r--   0 me        (1000) me        (1000)    20031 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_handlers.py
--rw-r--r--   0 me        (1000) me        (1000)    28793 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_helpers.py
--rw-r--r--   0 me        (1000) me        (1000)     4371 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_logging.py
--rw-r--r--   0 me        (1000) me        (1000)    27436 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_login.py
--rw-r--r--   0 me        (1000) me        (1000)     3760 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_management.py
--rw-r--r--   0 me        (1000) me        (1000)     1848 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_middleware.py
--rw-r--r--   0 me        (1000) me        (1000)     1144 2024-06-03 10:51:04.000000 django-axes-forked-5.27.0.2/tests/test_models.py
--rw-r--r--   0 me        (1000) me        (1000)      489 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/tests/test_signals.py
--rw-r--r--   0 me        (1000) me        (1000)      112 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/tests/urls.py
--rw-r--r--   0 me        (1000) me        (1000)       23 2024-06-03 10:34:40.000000 django-axes-forked-5.27.0.2/tests/urls_empty.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.314916 django-axes-forked-5.27.1/
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/.github/
+-rw-r--r--   0 me        (1000) me        (1000)      147 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/.github/dependabot.yml
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/.github/workflows/
+-rw-r--r--   0 me        (1000) me        (1000)      994 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/.github/workflows/release.yml
+-rw-r--r--   0 me        (1000) me        (1000)     1956 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/.github/workflows/test.yml
+-rw-r--r--   0 me        (1000) me        (1000)      185 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/.gitignore
+-rw-r--r--   0 me        (1000) me        (1000)       10 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/.pre-commit-config.yaml
+-rw-r--r--   0 me        (1000) me        (1000)       86 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/.prospector.yaml
+-rw-r--r--   0 me        (1000) me        (1000)    28113 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/CHANGES.rst
+-rw-r--r--   0 me        (1000) me        (1000)     2375 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 me        (1000) me        (1000)     1184 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/LICENSE
+-rw-r--r--   0 me        (1000) me        (1000)    33325 2024-06-03 12:11:04.314916 django-axes-forked-5.27.1/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     3419 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/README.rst
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/
+-rw-r--r--   0 me        (1000) me        (1000)      160 2024-06-03 11:17:26.000000 django-axes-forked-5.27.1/axes/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     2008 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/admin.py
+-rw-r--r--   0 me        (1000) me        (1000)     1556 2024-06-03 11:17:22.000000 django-axes-forked-5.27.1/axes/apps.py
+-rw-r--r--   0 me        (1000) me        (1000)     3041 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/attempts.py
+-rw-r--r--   0 me        (1000) me        (1000)     2807 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/backends.py
+-rw-r--r--   0 me        (1000) me        (1000)     4551 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/checks.py
+-rw-r--r--   0 me        (1000) me        (1000)     5450 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/conf.py
+-rw-r--r--   0 me        (1000) me        (1000)      628 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/decorators.py
+-rw-r--r--   0 me        (1000) me        (1000)      380 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/exceptions.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/handlers/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/handlers/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     6752 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/handlers/base.py
+-rw-r--r--   0 me        (1000) me        (1000)     5889 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/handlers/cache.py
+-rw-r--r--   0 me        (1000) me        (1000)    10336 2024-06-03 12:02:36.000000 django-axes-forked-5.27.1/axes/handlers/database.py
+-rw-r--r--   0 me        (1000) me        (1000)      677 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/handlers/dummy.py
+-rw-r--r--   0 me        (1000) me        (1000)     4479 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/handlers/proxy.py
+-rw-r--r--   0 me        (1000) me        (1000)      644 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/handlers/test.py
+-rw-r--r--   0 me        (1000) me        (1000)    18019 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/helpers.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/de/
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 me        (1000) me        (1000)     1549 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 me        (1000) me        (1000)     2123 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/pl/
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 me        (1000) me        (1000)     1526 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 me        (1000) me        (1000)     2266 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/ru/
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 me        (1000) me        (1000)     1950 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 me        (1000) me        (1000)     2495 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/tr/
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 me        (1000) me        (1000)     1450 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 me        (1000) me        (1000)     2075 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/management/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/management/__init__.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/management/commands/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/management/commands/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      404 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 me        (1000) me        (1000)      409 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/management/commands/axes_reset.py
+-rw-r--r--   0 me        (1000) me        (1000)      552 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 me        (1000) me        (1000)      643 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 me        (1000) me        (1000)      579 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/management/commands/axes_reset_user.py
+-rw-r--r--   0 me        (1000) me        (1000)      579 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 me        (1000) me        (1000)     1583 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/middleware.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/axes/migrations/
+-rw-r--r--   0 me        (1000) me        (1000)     2831 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/migrations/0001_initial.py
+-rw-r--r--   0 me        (1000) me        (1000)     1723 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 me        (1000) me        (1000)     1948 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 me        (1000) me        (1000)     2197 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 me        (1000) me        (1000)      219 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 me        (1000) me        (1000)      274 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 me        (1000) me        (1000)     1116 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/migrations/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     1473 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/models.py
+-rw-r--r--   0 me        (1000) me        (1000)     1782 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/axes/signals.py
+-rw-r--r--   0 me        (1000) me        (1000)     1656 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/axes/utils.py
+-rw-r--r--   0 me        (1000) me        (1000)      212 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/codecov.yml
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/django_axes_forked.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)    33325 2024-06-03 12:11:04.000000 django-axes-forked-5.27.1/django_axes_forked.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     2577 2024-06-03 12:11:04.000000 django-axes-forked-5.27.1/django_axes_forked.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2024-06-03 12:11:04.000000 django-axes-forked-5.27.1/django_axes_forked.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2024-06-03 12:09:58.000000 django-axes-forked-5.27.1/django_axes_forked.egg-info/not-zip-safe
+-rw-r--r--   0 me        (1000) me        (1000)       43 2024-06-03 12:11:04.000000 django-axes-forked-5.27.1/django_axes_forked.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)        5 2024-06-03 12:11:04.000000 django-axes-forked-5.27.1/django_axes_forked.egg-info/top_level.txt
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/docs/
+-rw-r--r--   0 me        (1000) me        (1000)       43 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/docs/10_changelog.rst
+-rw-r--r--   0 me        (1000) me        (1000)      648 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/1_requirements.rst
+-rw-r--r--   0 me        (1000) me        (1000)     5527 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/2_installation.rst
+-rw-r--r--   0 me        (1000) me        (1000)     4307 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/3_usage.rst
+-rw-r--r--   0 me        (1000) me        (1000)    12928 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/4_configuration.rst
+-rw-r--r--   0 me        (1000) me        (1000)     5917 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/5_customization.rst
+-rw-r--r--   0 me        (1000) me        (1000)     9133 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/6_integration.rst
+-rw-r--r--   0 me        (1000) me        (1000)     3596 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/7_architecture.rst
+-rw-r--r--   0 me        (1000) me        (1000)      406 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/docs/8_reference.rst
+-rw-r--r--   0 me        (1000) me        (1000)     1400 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/9_development.rst
+-rw-r--r--   0 me        (1000) me        (1000)     7425 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/Makefile
+-rw-r--r--   0 me        (1000) me        (1000)     4043 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/conf.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.304916 django-axes-forked-5.27.1/docs/images/
+-rw-r--r--   0 me        (1000) me        (1000)   133029 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/docs/images/flow.png
+-rw-r--r--   0 me        (1000) me        (1000)      355 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/docs/index.rst
+-rw-r--r--   0 me        (1000) me        (1000)      249 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/manage.py
+-rw-r--r--   0 me        (1000) me        (1000)      105 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/mypy.ini
+-rw-r--r--   0 me        (1000) me        (1000)     1287 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/pyproject.toml
+-rw-r--r--   0 me        (1000) me        (1000)       78 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/requirements-qa.txt
+-rw-r--r--   0 me        (1000) me        (1000)       97 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/requirements-test.txt
+-rw-r--r--   0 me        (1000) me        (1000)       89 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/requirements.txt
+-rw-r--r--   0 me        (1000) me        (1000)       38 2024-06-03 12:11:04.314916 django-axes-forked-5.27.1/setup.cfg
+-rw-r--r--   0 me        (1000) me        (1000)     2465 2024-06-03 12:10:52.000000 django-axes-forked-5.27.1/setup.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2024-06-03 12:11:04.314916 django-axes-forked-5.27.1/tests/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/tests/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     5850 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/base.py
+-rw-r--r--   0 me        (1000) me        (1000)     2048 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/settings.py
+-rw-r--r--   0 me        (1000) me        (1000)      935 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_admin.py
+-rw-r--r--   0 me        (1000) me        (1000)     5846 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_attempts.py
+-rw-r--r--   0 me        (1000) me        (1000)      747 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/tests/test_backends.py
+-rw-r--r--   0 me        (1000) me        (1000)     3585 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_checks.py
+-rw-r--r--   0 me        (1000) me        (1000)     1939 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_decorators.py
+-rw-r--r--   0 me        (1000) me        (1000)    20031 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_handlers.py
+-rw-r--r--   0 me        (1000) me        (1000)    28793 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_helpers.py
+-rw-r--r--   0 me        (1000) me        (1000)     4371 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_logging.py
+-rw-r--r--   0 me        (1000) me        (1000)    27436 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_login.py
+-rw-r--r--   0 me        (1000) me        (1000)     3760 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_management.py
+-rw-r--r--   0 me        (1000) me        (1000)     1848 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_middleware.py
+-rw-r--r--   0 me        (1000) me        (1000)     1144 2024-06-03 10:51:04.000000 django-axes-forked-5.27.1/tests/test_models.py
+-rw-r--r--   0 me        (1000) me        (1000)      489 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/tests/test_signals.py
+-rw-r--r--   0 me        (1000) me        (1000)      112 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/tests/urls.py
+-rw-r--r--   0 me        (1000) me        (1000)       23 2024-06-03 10:34:40.000000 django-axes-forked-5.27.1/tests/urls_empty.py
```

### Comparing `django-axes-forked-5.27.0.2/.github/workflows/release.yml` & `django-axes-forked-5.27.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/.github/workflows/test.yml` & `django-axes-forked-5.27.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/CHANGES.rst` & `django-axes-forked-5.27.1/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/CODE_OF_CONDUCT.md` & `django-axes-forked-5.27.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/LICENSE` & `django-axes-forked-5.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/PKG-INFO` & `django-axes-forked-5.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes-forked
-Version: 5.27.0.2
+Version: 5.27.1
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/youssef3laa/django-axes/tree/fork-5.27.0
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
```

### Comparing `django-axes-forked-5.27.0.2/README.rst` & `django-axes-forked-5.27.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/admin.py` & `django-axes-forked-5.27.1/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/apps.py` & `django-axes-forked-5.27.1/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/attempts.py` & `django-axes-forked-5.27.1/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/backends.py` & `django-axes-forked-5.27.1/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/checks.py` & `django-axes-forked-5.27.1/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/conf.py` & `django-axes-forked-5.27.1/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/decorators.py` & `django-axes-forked-5.27.1/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/handlers/base.py` & `django-axes-forked-5.27.1/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/handlers/cache.py` & `django-axes-forked-5.27.1/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/handlers/database.py` & `django-axes-forked-5.27.1/axes/handlers/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,25 +152,24 @@
 
             # 3. database query if there were previous attempts in the database
             # Update failed attempt information but do not touch the username, IP address, or user agent fields,
             # because attackers can request the site with multiple different configurations
             # in order to bypass the defense mechanisms that are used by the site.
             else:
                 separator = "\n---------\n"
-                print('current', attempt.failures_since_start)
+
                 attempt.get_data = Concat("get_data", Value(separator + get_data))
                 attempt.post_data = Concat(
                     "post_data", Value(separator + post_data)
                 )
                 attempt.http_accept = request.axes_http_accept
                 attempt.path_info = request.axes_path_info
-                attempt.failures_since_start =+ 1
+                attempt.failures_since_start = F("failures_since_start") + 1
                 attempt.attempt_time = request.axes_attempt_time
                 attempt.save()
-                print('saved attempt', attempt.__dict__)
 
                 log.warning(
                     "AXES: Repeated login failure by %s. Updated existing record in the database.",
                     client_str,
                 )
 
         # 3. or 4. database query: Calculate the current maximum failure number from the existing attempts
```

### Comparing `django-axes-forked-5.27.0.2/axes/handlers/dummy.py` & `django-axes-forked-5.27.1/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/handlers/proxy.py` & `django-axes-forked-5.27.1/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/handlers/test.py` & `django-axes-forked-5.27.1/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/helpers.py` & `django-axes-forked-5.27.1/axes/helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-forked-5.27.1/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-forked-5.27.1/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-forked-5.27.1/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-forked-5.27.1/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-forked-5.27.1/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-forked-5.27.1/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-forked-5.27.1/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-forked-5.27.1/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_ip.py` & `django-axes-forked-5.27.1/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_logs.py` & `django-axes-forked-5.27.1/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_user.py` & `django-axes-forked-5.27.1/axes/management/commands/axes_reset_user.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/management/commands/axes_reset_username.py` & `django-axes-forked-5.27.1/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/middleware.py` & `django-axes-forked-5.27.1/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/migrations/0001_initial.py` & `django-axes-forked-5.27.1/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-forked-5.27.1/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-forked-5.27.1/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-forked-5.27.1/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-forked-5.27.1/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/models.py` & `django-axes-forked-5.27.1/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/signals.py` & `django-axes-forked-5.27.1/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/axes/utils.py` & `django-axes-forked-5.27.1/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/django_axes_forked.egg-info/PKG-INFO` & `django-axes-forked-5.27.1/django_axes_forked.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes-forked
-Version: 5.27.0.2
+Version: 5.27.1
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/youssef3laa/django-axes/tree/fork-5.27.0
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
```

### Comparing `django-axes-forked-5.27.0.2/django_axes_forked.egg-info/SOURCES.txt` & `django-axes-forked-5.27.1/django_axes_forked.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/1_requirements.rst` & `django-axes-forked-5.27.1/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/2_installation.rst` & `django-axes-forked-5.27.1/docs/2_installation.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/3_usage.rst` & `django-axes-forked-5.27.1/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/4_configuration.rst` & `django-axes-forked-5.27.1/docs/4_configuration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/5_customization.rst` & `django-axes-forked-5.27.1/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/6_integration.rst` & `django-axes-forked-5.27.1/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/7_architecture.rst` & `django-axes-forked-5.27.1/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/9_development.rst` & `django-axes-forked-5.27.1/docs/9_development.rst`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/Makefile` & `django-axes-forked-5.27.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/conf.py` & `django-axes-forked-5.27.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/docs/images/flow.png` & `django-axes-forked-5.27.1/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/pyproject.toml` & `django-axes-forked-5.27.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/setup.py` & `django-axes-forked-5.27.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name="django-axes-forked",
-    version = '5.27.0.2',
+    version = '5.27.01',
     description="Keep track of failed login attempts in Django-powered sites.",
     long_description="\n".join(
         [
             open("README.rst", encoding="utf-8").read(),
             open("CHANGES.rst", encoding="utf-8").read(),
         ]
     ),
```

### Comparing `django-axes-forked-5.27.0.2/tests/base.py` & `django-axes-forked-5.27.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/settings.py` & `django-axes-forked-5.27.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_admin.py` & `django-axes-forked-5.27.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_attempts.py` & `django-axes-forked-5.27.1/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_backends.py` & `django-axes-forked-5.27.1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_checks.py` & `django-axes-forked-5.27.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_decorators.py` & `django-axes-forked-5.27.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_handlers.py` & `django-axes-forked-5.27.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_helpers.py` & `django-axes-forked-5.27.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_logging.py` & `django-axes-forked-5.27.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_login.py` & `django-axes-forked-5.27.1/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_management.py` & `django-axes-forked-5.27.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_middleware.py` & `django-axes-forked-5.27.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-forked-5.27.0.2/tests/test_models.py` & `django-axes-forked-5.27.1/tests/test_models.py`

 * *Files identical despite different names*

