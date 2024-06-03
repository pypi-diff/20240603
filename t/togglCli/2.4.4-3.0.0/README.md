# Comparing `tmp/togglCli-2.4.4.tar.gz` & `tmp/togglCli-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "togglCli-2.4.4.tar", last modified: Tue Feb 14 19:30:06 2023, max compression
+gzip compressed data, was "togglCli-3.0.0.tar", last modified: Mon Jun  3 13:00:32 2024, max compression
```

## Comparing `togglCli-2.4.4.tar` & `togglCli-3.0.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.324765 togglCli-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-14 19:29:23.000000 togglCli-2.4.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.316765 togglCli-2.4.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-14 19:29:23.000000 togglCli-2.4.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.316765 togglCli-2.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-14 19:29:23.000000 togglCli-2.4.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-14 19:29:23.000000 togglCli-2.4.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-14 19:30:06.000000 togglCli-2.4.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-14 19:29:23.000000 togglCli-2.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-02-14 19:29:23.000000 togglCli-2.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-02-14 19:30:06.000000 togglCli-2.4.4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-14 19:29:23.000000 togglCli-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-02-14 19:30:06.324765 togglCli-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-02-14 19:29:23.000000 togglCli-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.316765 togglCli-2.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-14 19:29:23.000000 togglCli-2.4.4/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-14 19:29:23.000000 togglCli-2.4.4/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-02-14 19:29:23.000000 togglCli-2.4.4/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-02-14 19:29:23.000000 togglCli-2.4.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-14 19:29:23.000000 togglCli-2.4.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-14 19:29:23.000000 togglCli-2.4.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-14 19:29:23.000000 togglCli-2.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-14 19:30:06.324765 togglCli-2.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-02-14 19:29:23.000000 togglCli-2.4.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-14 19:29:23.000000 togglCli-2.4.4/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.316765 togglCli-2.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.316765 togglCli-2.4.4/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/configs/non-premium.config
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/configs/premium.config
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.316765 togglCli-2.4.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/integration/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/integration/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/integration/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/integration/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/integration/test_time_entries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.316765 togglCli-2.4.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/tests/unit/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/api/test_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/cli/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/tests/unit/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/helpers/test_duration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-02-14 19:29:23.000000 togglCli-2.4.4/tests/unit/utils/test_migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/toggl/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/toggl/api/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23466 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    32209 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/api/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/toggl/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    31563 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/assets/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/toggl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53223 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/cli/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/toggl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.320765 togglCli-2.4.4/toggl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/utils/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/utils/metas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/utils/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-02-14 19:29:23.000000 togglCli-2.4.4/toggl/utils/others.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 19:30:06.324765 togglCli-2.4.4/togglCli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-02-14 19:30:06.000000 togglCli-2.4.4/togglCli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-02-14 19:30:06.000000 togglCli-2.4.4/togglCli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 19:30:06.000000 togglCli-2.4.4/togglCli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-14 19:30:06.000000 togglCli-2.4.4/togglCli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 19:30:02.000000 togglCli-2.4.4/togglCli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-14 19:30:06.000000 togglCli-2.4.4/togglCli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-14 19:30:06.000000 togglCli-2.4.4/togglCli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.713269 togglCli-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-03 12:59:43.000000 togglCli-3.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.705269 togglCli-3.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-06-03 12:59:43.000000 togglCli-3.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.705269 togglCli-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-06-03 12:59:43.000000 togglCli-3.0.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-06-03 12:59:43.000000 togglCli-3.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-06-03 13:00:32.000000 togglCli-3.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-06-03 12:59:43.000000 togglCli-3.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-06-03 12:59:43.000000 togglCli-3.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-06-03 13:00:32.000000 togglCli-3.0.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-06-03 12:59:43.000000 togglCli-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-06-03 13:00:32.713269 togglCli-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-06-03 12:59:43.000000 togglCli-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.705269 togglCli-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 12:59:43.000000 togglCli-3.0.0/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-06-03 12:59:43.000000 togglCli-3.0.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-06-03 12:59:43.000000 togglCli-3.0.0/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-06-03 12:59:43.000000 togglCli-3.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-03 12:59:43.000000 togglCli-3.0.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-06-03 12:59:43.000000 togglCli-3.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-03 12:59:43.000000 togglCli-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-06-03 13:00:32.713269 togglCli-3.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-06-03 12:59:43.000000 togglCli-3.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-03 12:59:43.000000 togglCli-3.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.705269 togglCli-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.705269 togglCli-3.0.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/configs/non-premium.config
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/configs/premium.config
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.705269 togglCli-3.0.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/integration/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/integration/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/integration/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/integration/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/integration/test_time_entries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/tests/unit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/api/test_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/cli/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/tests/unit/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/helpers/test_duration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-06-03 12:59:43.000000 togglCli-3.0.0/tests/unit/utils/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/toggl/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/toggl/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32281 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29925 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.709269 togglCli-3.0.0/toggl/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    31563 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/assets/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.713269 togglCli-3.0.0/toggl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53965 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/cli/themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/toggl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.713269 togglCli-3.0.0/toggl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/utils/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/utils/metas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/utils/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-06-03 12:59:43.000000 togglCli-3.0.0/toggl/utils/others.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:32.713269 togglCli-3.0.0/togglCli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 13:00:32.000000 togglCli-3.0.0/togglCli.egg-info/top_level.txt
```

### Comparing `togglCli-2.4.4/.github/workflows/release.yaml` & `togglCli-3.0.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/AUTHORS` & `togglCli-3.0.0/AUTHORS`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,41 @@
 Adam Uhlíř <adam@uhlir.dev>
 Adam Uhlíř <hello@adam-uhlir.me>
 Adams <d.robert.adams@gmail.com>
 Andre-Patrick Bubel <code@andre-bubel.de>
 Beau <beau.raines@gmail.com>
 Beau Raines <beau.raines@gmail.com>
 Christopher Tatro <c.m.tatro@gmail.com>
+Dhanush Kovi <99819848+dkvc@users.noreply.github.com>
 Dominik Stańczak <stanczakdominik@gmail.com>
 Dominik Stańczak-Marikin <stanczakdominik@gmail.com>
 Erik Bjäreholt <erik.bjareholt@gmail.com>
 Federico Vaga <federico.vaga@gmail.com>
 Hugo van Kemenade <hugovk@users.noreply.github.com>
+Jeff Martin <jeffrey.j.martin2@gmail.com>
 Kevin Pulo <kevin.pulo@mongodb.com>
 Lee <lee@revelry.co>
 Leonid Komarovsky <shpoont@users.noreply.github.com>
 Miguel Julián <figarocorso@users.noreply.github.com>
 Mike Purvis <mpurvis@clearpathrobotics.com>
 Morgan Howe <mthowe@gmail.com>
+Ola Herrdahl <olaherrdahl@users.noreply.github.com>
 Olen <github@olen.net>
 Remigijus Jarmalavičius <remigijus@jarmalavicius.lt>
 Robert Adams <adams@cis.gvsu.edu>
 Robert Adams <d.robert.adams@gmail.com>
 Sander <svr003@gmail.com>
 Sander van Rijn <svr003@gmail.com>
 Santiago Castro <santi.1410@hotmail.com>
 Stafford Williams <staff0rd@users.noreply.github.com>
 Stafford Williams <stafford.williams@gmail.com>
 Till <tbrodbeck@uos.de>
 Todd Mazierski <toddmazierski@users.noreply.github.com>
+abk16 <and.theunnamed@gmail.com>
+ddkasa <davidkasakaitis@proton.me>
 dependabot-preview[bot] <27856297+dependabot-preview[bot]@users.noreply.github.com>
 dependabot[bot] <49699333+dependabot[bot]@users.noreply.github.com>
 github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>
 martinm76 <martin.moller@gmail.com>
 matescb <matescb@gmail.com>
 pyup-bot <github-bot@pyup.io>
 pyup.io bot <github-bot@pyup.io>
```

### Comparing `togglCli-2.4.4/CONTRIBUTING.md` & `togglCli-3.0.0/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # Contributing
 
 Any contribution are welcomed.
 
 For submitting PRs, they need to have test coverage which pass the full run in Travis CI. 
 
+## Developing
+
+If you want to run the toggl CLI during development, I recommend you to use flow where you `pip install -e .`, which
+symlinks locally the package and then you can simply use the CLI like `toggl ls`.
+
+Also, if you find yourself with non-descriptive exception, you can set env. variable `export TOGGL_EXCEPTIONS=1` which
+then will give you then the full stack trace. 
+
 ## Tests
 
 For running integration tests you need dummy account on Toggl, where **you don't have any important data** as the data 
 will be messed up with and eventually **deleted**! Get API token for this test account and set it as an environmental variable
-***TOGGL_API_TOKEN***.
+`TOGGL_API_TOKEN`. Also figure out the Workspace ID of your account (`toggl workspace ls`) and set is as `TOGGL_WORKSPACE` 
+environmental variable.
 
 There are two sets of integration tests: normal and premium. To be able to run the premium set you have to have payed
 workspace. As this is quiet unlikely you can leave the testing on Travis CI as it runs also the premium tests set.
 
 Tests are written using `pytest` framework and are split into three categories (each having its own pytest mark):
  *  **unit** - unit tests testing mostly the framework around building the API wrappers
  *  **integration** - Integration tests which tests end to end coherence of API wrapper. Requires connectivity to Toggl API.
  *  **premium**: Subcategory of Integration tests that requires to have Premium/Paid workspace for the tests.
 
 ## Running tests
 
-In order to run tests first you need to have required packages installed. You can install them using `pip install togglCli[test]` or
-`python setup.py test`. 
+In order to run tests first you need to have required packages installed. You can install them using `pip install togglCli[test]`,
+`python setup.py test` or `pip install -r test-requirements.txt`.
 
 By default unit and integration tests are run without the one testing premium functionality, as most probably you don't have access to Premium workspace for testing purposes.
 If you want to run just specific category you can do so using for example`pytest -m unit` for only unit tests.
```

### Comparing `togglCli-2.4.4/ChangeLog` & `togglCli-3.0.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+v3.0.0
+------
+
+* chore(master): release 3.0.0 (#301)
+* feat!: migration to v9 api version (#303)
+* chore: python 3.12 support (#319)
+* feat: print description for toggl start (#316)
+* feat: add limit option to ls (#314)
+* fix: Set default color to toggl's default 1 (#302)
+* feat: respect XDG spec for configuration files (#300)
+
 v2.4.4
 ------
 
 * chore(master): release 2.4.4 (#299)
 * ci: fix build to produced versioned builds
 * ci: build distribution packages
 * revert: pbr removal
```

### Comparing `togglCli-2.4.4/LICENSE` & `togglCli-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/PKG-INFO` & `togglCli-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: togglCli
-Version: 2.4.4
+Version: 3.0.0
 Summary: Command line tool and set of Python wrapper classes for interacting with toggl's API
 Home-page: https://toggl.uhlir.dev
 Author: D. Robert Adams & Adam Uhlir
 Author-email: adam@uhlir.dev
 License: MIT
 Project-URL: Source, https://github.com/auhau/toggl-cli
 Project-URL: Documentation, https://toggl.uhlir.devg
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Office/Business :: Scheduling
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools==69.0.3
+Requires-Dist: pendulum==3.0.0
+Requires-Dist: requests>=2.23.0
+Requires-Dist: click==8.1.7
+Requires-Dist: inquirer==3.2.4
+Requires-Dist: prettytable==3.6.0
+Requires-Dist: validate_email==1.3
+Requires-Dist: click-completion==0.5.2
+Requires-Dist: pbr==6.0.0
+Requires-Dist: notify-py==0.3.42
 
 # Toggl CLI
 
 [![PyPI version](https://badge.fury.io/py/togglCli.svg)](https://badge.fury.io/py/togglCli) 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/togglCli.svg)](https://pypi.org/project/togglCli)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/togglCli.svg)](https://pypi.org/project/togglCli/) 
 [![codecov](https://codecov.io/gh/AuHau/toggl-cli/branch/master/graph/badge.svg)](https://codecov.io/gh/AuHau/toggl-cli)
```

### Comparing `togglCli-2.4.4/README.md` & `togglCli-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/docs/api.md` & `togglCli-3.0.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/docs/cli.md` & `togglCli-3.0.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/docs/index.md` & `togglCli-3.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/mkdocs.yml` & `togglCli-3.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/setup.cfg` & `togglCli-3.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 summary = Command line tool and set of Python wrapper classes for interacting with toggl's API
 description_file = README.md
 description_content_type = text/markdown
 author = D. Robert Adams & Adam Uhlir
 author_email = adam@uhlir.dev
 license = MIT
 home_page = https://toggl.uhlir.dev
-python_requires = >=3.7.0
+python_requires = >=3.8.0
 project_urls = 
 	Source = https://github.com/auhau/toggl-cli
 	Documentation = https://toggl.uhlir.devg
 classifier = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Development Status :: 5 - Production/Stable
 	Topic :: Office/Business :: Scheduling
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: Developers
 
 [files]
```

### Comparing `togglCli-2.4.4/tests/conftest.py` & `togglCli-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/tests/helpers.py` & `togglCli-3.0.0/tests/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,19 +110,21 @@
 
 
 class Cleanup:
     @staticmethod
     def _ids_cleanup(base, config=None, batch=False, *ids):
         config = config or get_config()
 
+        wid = config.default_workspace.id
+        workspace_url = '/workspaces/{}'.format(wid)
         if batch:
-            utils.toggl('/{}/{}'.format(base, ','.join([str(eid) for eid in ids])), 'delete', config=config)
+            utils.toggl('{}/{}/{}'.format(workspace_url, base, ','.join([str(eid) for eid in ids])), 'delete', config=config)
         else:
             for entity_id in ids:
-                utils.toggl('/{}/{}'.format(base, entity_id), 'delete', config=config)
+                utils.toggl('{}/{}/{}'.format(workspace_url, base, entity_id), 'delete', config=config)
 
     @staticmethod
     def _all_cleanup(cls, config=None):
         config = config or get_config()
         entities = cls.objects.all(config=config)
         Cleanup.cleanup(entities)
 
@@ -167,20 +169,24 @@
             Cleanup._ids_cleanup('tags', config, False, *ids)
 
     @staticmethod
     def time_entries(config=None, *ids):
         if not ids:
             config = config or get_config()
             entities = api.TimeEntry.objects.all(config=config)
+            current_entry = api.TimeEntry.objects.current(config=config)
+            if current_entry is not None:
+                current_entry.stop_and_save()
+                entities.append(current_entry)
             ids = [entity.id for entity in entities]
 
         if not ids:
             return
 
-        Cleanup._ids_cleanup('time_entries', config, True, *ids)
+        Cleanup._ids_cleanup('time_entries', config, False, *ids)
 
     @staticmethod
     def project_users(config=None, *ids):
         if not ids:
             Cleanup._all_cleanup(api.ProjectUser, config=config)
         else:
             Cleanup._ids_cleanup('project_users', config, False, *ids)
@@ -191,15 +197,15 @@
             config = config or get_config()
             entities = api.Project.objects.all(config=config)
             ids = [entity.id for entity in entities]
 
         if not ids:
             return
 
-        Cleanup._ids_cleanup('projects', config, True, *ids)
+        Cleanup._ids_cleanup('projects', config, False, *ids)
 
     @staticmethod
     def tasks(config=None, *ids):
         if not ids:
             Cleanup._all_cleanup(api.Task, config=config)
         else:
             Cleanup._ids_cleanup('tasks', config, False, *ids)
```

### Comparing `togglCli-2.4.4/tests/integration/conftest.py` & `togglCli-3.0.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/tests/integration/factories.py` & `togglCli-3.0.0/tests/integration/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     class Meta:
         model = api.Project
 
     name = factory.Faker('name')
     # client = factory.SubFactory(ClientFactory)
     active = True
     is_private = True
-    billable = False
 
 
 class TaskFactory(TogglFactory):
     class Meta:
         model = api.Task
 
     name = factory.Faker('sentence')
```

### Comparing `togglCli-2.4.4/tests/integration/test_clients.py` & `togglCli-3.0.0/tests/integration/test_clients.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/tests/integration/test_projects.py` & `togglCli-3.0.0/tests/integration/test_projects.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,75 +30,75 @@
         assert result.obj.exit_code == 0
         assert Project.objects.get(result.created_id(), config=config).client == client
 
         result = cmd('projects add --name \'{}\' --client \'{}\''.format(fake.word(), client.name))
         assert result.obj.exit_code == 0
         assert Project.objects.get(result.created_id(), config=config).client == client
 
-        result = cmd('projects add --name \'{}\' --private --color 2'.format(fake.word()))
+        result = cmd('projects add --name \'{}\' --private --color #c9806b'.format(fake.word()))
         assert result.obj.exit_code == 0
 
         prj = Project.objects.get(result.created_id(), config=config)  # type: Project
         assert prj.is_private is True
-        assert prj.color == 2
+        assert prj.color == '#c9806b'
 
         with pytest.raises(exceptions.TogglPremiumException):
             cmd('projects add --name \'{}\' --billable'.format(fake.word()))
 
     @pytest.mark.premium
     def test_add_full_premium(self, cmd, fake):
         result = cmd('projects add --name \'{}\' --billable --rate 10.10  --auto-estimates'.format(fake.word()))
         assert result.obj.exit_code == 0
 
     def test_get(self, cmd, fake, factories):
         name = fake.word()
         client = factories.ClientFactory()
-        project = factories.ProjectFactory(name=name, is_private=False, color=2, client=client)
+        project = factories.ProjectFactory(name=name, is_private=False, color='#c9806b', client=client)
 
         result = cmd('projects get \'{}\''.format(project.id))
         id_parsed = result.parse_detail()
 
         assert id_parsed['name'] == name
-        assert id_parsed['billable'] == 'False'
-        assert id_parsed['auto_estimates'] == 'False'
+        assert not bool(id_parsed['billable'])
+        assert not bool(id_parsed['auto_estimates'])
         assert id_parsed['active'] == 'True'
         assert id_parsed['is_private'] == 'False'
-        assert id_parsed['color'] == '2'
+        assert id_parsed['color'] == '#c9806b'
         assert str(client.id) in id_parsed['client']
 
         result = cmd('projects get \'{}\''.format(name))
         name_parsed = result.parse_detail()
 
         assert name_parsed['name'] == name
-        assert name_parsed['billable'] == 'False'
-        assert name_parsed['auto_estimates'] == 'False'
+        assert not bool(name_parsed['billable'])
+        assert not bool(name_parsed['auto_estimates'])
         assert name_parsed['active'] == 'True'
         assert name_parsed['is_private'] == 'False'
-        assert name_parsed['color'] == '2'
+        assert name_parsed['color'] == '#c9806b'
         assert str(client.id) in name_parsed['client']
 
     def test_update(self, cmd, fake, config, factories):
         name = fake.name()
-        project = factories.ProjectFactory(name=name, is_private=False, color=2)
+        project = factories.ProjectFactory(name=name, is_private=False, color='#c9806b')
 
         new_name = fake.name()
         new_client = factories.ClientFactory()
-        result = cmd('projects update --name \'{}\' --client \'{}\' --private --color 1 \'{}\''.format(new_name, new_client.name, name))
+        result = cmd('projects update --name \'{}\' --client \'{}\' --private --color #0b83d9 \'{}\''.format(new_name, new_client.name, name))
         assert result.obj.exit_code == 0
 
         project_obj = Project.objects.get(project.id, config=config)
         assert project_obj.name == new_name
         assert project_obj.client == new_client
-        assert project_obj.color == 1
+        assert project_obj.color == '#0b83d9'
         assert project_obj.is_private is True
 
     @pytest.mark.premium
     def test_update_premium(self, cmd, fake, config, factories):
         name = fake.name()
-        project = factories.ProjectFactory(name=name, is_private=False, color=2)
+        project = factories.ProjectFactory(name=name, is_private=False, color='#c9806b')
 
         result = cmd('projects update --billable --rate 10.10  --auto-estimates \'{}\''.format(name))
         assert result.obj.exit_code == 0
 
         project_obj = Project.objects.get(project.id, config=config)
         assert project_obj.rate == 10.10
         assert project_obj.billable is True
```

### Comparing `togglCli-2.4.4/tests/integration/test_tags.py` & `togglCli-3.0.0/tests/integration/test_tags.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/tests/integration/test_time_entries.py` & `togglCli-3.0.0/tests/integration/test_time_entries.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     def test_add_basic(self, cmd, fake, config):
         start = pendulum.instance(fake.past_datetime(start_date='-9d'))
         result = cmd('add \'{}\' 1h2m2s \'{}\''.format(start.format('MMM D YYYY HH:mm:ss'), fake.sentence()))
         assert result.obj.exit_code == 0
 
         entry = TimeEntry.objects.get(result.created_id(), config=config)  # type: TimeEntry
-        assert entry.start == start
+        assert entry.start == start.replace(microsecond=0)
         assert (entry.stop - entry.start).seconds == 3722
 
     def test_add_tags(self, cmd, fake, config):
         start = pendulum.instance(fake.past_datetime(start_date='-9d'))
         end = start + pendulum.duration(hours=2)
         result = cmd('add \'{}\' \'{}\' \'{}\' --tags \'some tag,another tag\''.format(start.format('MMM D HH:mm:ss'),
                                                                                        end.format('MMM D HH:mm:ss'),
@@ -175,16 +175,24 @@
         assert result.obj.exit_code == 0
         parsed = result.parse_detail()
         assert 'b' not in parsed['tags']
 
     def test_continue(self, cmd, config, factories):
         some_entry = factories.TimeEntryFactory()
 
-        start = pendulum.now('utc')
-        stop = start + pendulum.duration(seconds=10)
+        # Stop and remove any running and recent time entries first
+        pre_running_entry = TimeEntry.objects.current(config=config)
+        if pre_running_entry is not None:
+            pre_running_entry.stop_and_save()
+        recent_entries = TimeEntry.objects.filter(order="desc", config=config, start=pendulum.now('utc') - pendulum.duration(minutes=2), stop=pendulum.now('utc'))
+        for to_delete_entry in recent_entries:
+            to_delete_entry.delete(config=config)
+
+        stop = pendulum.now('utc') - pendulum.duration(seconds=1)
+        start = stop - pendulum.duration(seconds=10)
         last_entry = factories.TimeEntryFactory(start=start, stop=stop)
 
         result = cmd('continue')
         assert result.obj.exit_code == 0
         continuing_entry = TimeEntry.objects.current(config=config)
 
         assert last_entry.description == continuing_entry.description
```

### Comparing `togglCli-2.4.4/tests/unit/api/test_base.py` & `togglCli-3.0.0/tests/unit/api/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from toggl.api import base, fields
 from toggl import exceptions, utils
 
 from ... import helpers
 
 
 class RandomEntity(base.TogglEntity):
+    _endpoints_name = 'random_entities'
+
     some_field = fields.StringField()
 
 
 class EntityWithDummySet(base.TogglEntity):
     objects = 'something'
 
 
@@ -145,22 +147,22 @@
         with pytest.raises(exceptions.TogglException):
             tset.all()
 
         with pytest.raises(exceptions.TogglException):
             tset.filter()
 
         with pytest.raises(exceptions.TogglException):
-            tset.base_url
+            tset.entity_endpoints_name
 
     def test_url(self):
         tset = base.TogglSet(url='http://some-url.com')
-        assert tset.base_url == 'http://some-url.com'
+        assert tset.entity_endpoints_name == 'http://some-url.com'
 
         tset = base.TogglSet(RandomEntity)
-        assert tset.base_url == 'random_entitys'
+        assert tset.entity_endpoints_name == 'random_entities'
 
     def test_can_get_detail(self):
         tset = base.TogglSet(can_get_detail=False)
         assert tset.can_get_detail is False
 
         RandomEntity._can_get_detail = False
         tset = base.TogglSet(RandomEntity)
@@ -185,30 +187,27 @@
         assert tset.can_get_list is True
 
     # Get()
 
     def test_get_detail_basic(self, mocker):
         mocker.patch.object(utils, 'toggl')
         utils.toggl.return_value = {
-            'data': {
-                'some_field': 'asdf'
-            }
+            'id': 123,
+            'some_field': 'asdf'
         }
 
         tset = base.TogglSet(RandomEntity)
         obj = tset.get(id=123)
 
         assert obj is not None
         assert obj.some_field == 'asdf'
 
     def test_get_detail_none(self, mocker):
         mocker.patch.object(utils, 'toggl')
-        utils.toggl.return_value = {
-            'data': None
-        }
+        utils.toggl.return_value = None
 
         tset = base.TogglSet(RandomEntity)
         obj = tset.get(id=123)
 
         assert obj is None
 
     def test_get_detail_none_exception(self, mocker):
@@ -473,14 +472,16 @@
                 some_other_mapped_field = fields.MappingField(RandomEntity, 'mapping_field')
 
 
 #######################################################################################################
 ## TogglEntity
 
 class Entity(base.TogglEntity):
+    _endpoints_name = "entities"
+
     string = fields.StringField()
     integer = fields.IntegerField()
     boolean = fields.BooleanField()
     datetime = fields.DateTimeField()
 
 
 class EntityWithRequired(Entity):
@@ -612,17 +613,15 @@
         assert obj.string == new_obj.string
         assert obj.integer == new_obj.integer
         assert new_obj.id is None
 
     def test_save_create(self, mocker):
         mocker.patch.object(utils, 'toggl')
         utils.toggl.return_value = {
-            'data': {
-                'id': 333
-            }
+            'id': 333
         }
 
         obj = Entity(string='asd', integer=123)
         obj.save()
 
         assert obj.id == 333
         assert utils.toggl.called is True
```

### Comparing `togglCli-2.4.4/tests/unit/api/test_fields.py` & `togglCli-3.0.0/tests/unit/api/test_fields.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/tests/unit/cli/test_types.py` & `togglCli-3.0.0/tests/unit/cli/test_types.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/tests/unit/helpers/test_duration.py` & `togglCli-3.0.0/tests/unit/helpers/test_duration.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/tests/unit/utils/test_migrations.py` & `togglCli-3.0.0/tests/unit/utils/test_migrations.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/api/base.py` & `togglCli-3.0.0/toggl/api/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,24 @@
     Condition's keys and values must match the entries attributes, but not the other way around.
 
     :param contain: If True, then string fields won't be tested on equality but on partial match.
     :param entity: TogglEntity
     :param conditions: dict
     :return:
     """
+    logger.debug(f'EvaluatingConditions: Filtering based on conditions: {conditions}')
+
     for key, value in conditions.items():
         try:
             field = entity.__fields__[key]
         except KeyError:
             try:
                 field = entity.__mapped_fields__[key]
             except KeyError:
+                logger.debug(f'EvaluatingConditions: Field {key} not found in entity {entity}')
                 return False
 
         if isinstance(field, model_fields.MappingField):
             if isinstance(value, TogglEntity):
                 value = value.id
 
                 if value is None:
@@ -43,14 +46,15 @@
             mapped_entity_id = entity.__dict__.get(field.mapped_field)
 
             # When both are None than it is desired ==> both not set
             if value is None and mapped_entity_id is None:
                 continue
 
             if value != mapped_entity_id:
+                logger.debug(f'EvaluatingConditions: Mapped entity\'s ID does not match')
                 return False
 
             continue
 
         entity_value = getattr(entity, key, None)
 
         if isinstance(field, model_fields.SetField):
@@ -78,14 +82,15 @@
         if isinstance(field, model_fields.StringField) and contain:
             if str(value) not in str(entity_value):
                 return False
 
             continue
 
         if str(entity_value) != str(value):
+            logger.debug(f'EvaluatingConditions: String values do not match: {entity_value} != {value}')
             return False
 
     return True
 
 
 # TODO: Caching
 class TogglSet(object):
@@ -111,46 +116,47 @@
         """
         if self.entity_cls is not None:
             raise exceptions.TogglException('The instance is already bound to a class {}!'.format(self.entity_cls))
 
         self.entity_cls = cls
 
     @property
-    def base_url(self):  # type: (TogglSet) -> str
+    def entity_endpoints_name(self):  # type: (TogglSet) -> str
         """
         Returns base URL which will be used for building listing or detail URLs.
         """
         if self._url:
             return self._url
 
         if self.entity_cls is None:
             raise exceptions.TogglException('The TogglSet instance is not binded to any TogglEntity!')
 
-        return self.entity_cls.get_url()
+        return self.entity_cls.get_endpoints_name()
 
     def build_list_url(self, caller, config, conditions):  # type: (str, utils.Config, typing.Dict) -> str
         """
         Build the listing URL.
 
         :param caller: Defines which method called this method, it can be either 'filter' or 'all'.
         :param config: Config
         :param conditions: If caller == 'filter' then contain conditions for filtering. Passed as reference,
         therefore any modifications will result modifications
         """
-        return '/{}'.format(self.base_url)
+        return '/me/{}'.format(self.entity_endpoints_name)
 
-    def build_detail_url(self, eid, config):  # type: (int, utils.Config) -> str
+    def build_detail_url(self, eid, config, conditions):  # type: (int, utils.Config, typing.Dict) -> str
         """
         Build the detail URL.
 
         :param eid: ID of the entity to fetch.
         :param config: Config
+        :param conditions: If caller == 'filter' then contain conditions for filtering. Passed as reference,
+        therefore any modifications will result modifications
         """
-        return '/{}/{}'.format(self.base_url, eid)
-
+        return '/me/{}/{}'.format(self.entity_endpoints_name, eid)
 
     @property
     def can_get_detail(self):  # type: (TogglSet) -> bool
         """
         Property which defines if TogglSet can fetch detail of the binded Entity.
         """
         if self._can_get_detail is not None:
@@ -170,15 +176,15 @@
             return self._can_get_list
 
         if self.entity_cls and self.entity_cls._can_get_list is not None:
             return self.entity_cls._can_get_list
 
         return True
 
-    def get(self, id=None, config=None, **conditions):  # type: (typing.Any, utils.Config, **typing.Any) -> Entity
+    def get(self, id=None, config=None, **conditions):  # type: (typing.Any, utils.Config, **typing.Any) -> typing.Optional[Entity]
         """
         Method for fetching detail object of the entity. it fetches the object based on specified conditions.
 
         If ID is used then detail URL is used to fetch object.
         If other conditions are used to specify the object, then TogglSet will fetch all objects using listing URL and
         filter out objects based on passed conditions.
 
@@ -190,19 +196,19 @@
             raise exceptions.TogglException('The TogglSet instance is not binded to any TogglEntity!')
 
         config = config or utils.Config.factory()
 
         if id is not None:
             if self.can_get_detail:
                 try:
-                    fetched_entity = utils.toggl(self.build_detail_url(id, config), 'get', config=config)
-                    if fetched_entity['data'] is None:
+                    fetched_entity = utils.toggl(self.build_detail_url(id, config, conditions), 'get', config=config)
+                    if fetched_entity is None:
                         return None
 
-                    return self.entity_cls.deserialize(config=config, **fetched_entity['data'])
+                    return self.entity_cls.deserialize(config=config, **fetched_entity)
                 except exceptions.TogglNotFoundException:
                     return None
             else:
                 # TODO: [Q/Design] Is this desired fallback?
                 # Most probably it is desired for Toggl usecase, because some Entities does not have detail view (eq. Users) and need
                 # to do query for whole list and then filter out the entity based on ID.
                 conditions['id'] = id
@@ -219,27 +225,23 @@
 
     def _fetch_all(self, url, order, config):  # type: (str, str, utils.Config) -> typing.List[Entity]
         """
         Helper method that fetches all objects from given URL and deserialize them.
         """
         fetched_entities = utils.toggl(url, 'get', config=config)
 
+        if isinstance(fetched_entities, dict):
+            fetched_entities = fetched_entities.get('data')
+
         if fetched_entities is None:
             return []
 
-        output = []
-        i = 0 if order == 'asc' else len(fetched_entities) - 1
-        while 0 <= i < len(fetched_entities):
-            output.append(self.entity_cls.deserialize(config=config, **fetched_entities[i]))
-
-            if order == 'asc':
-                i += 1
-            else:
-                i -= 1
-
+        output = [self.entity_cls.deserialize(config=config, **entry) for entry in fetched_entities]
+        if order == 'desc':
+            return output[::-1]
         return output
 
     def filter(self, order='asc', config=None, contain=False, **conditions):  # type: (str, utils.Config, bool, **typing.Any) -> typing.List[Entity]
         """
         Method that fetches all entries and filter them out based on specified conditions.
 
         :param order: Strings 'asc' or 'desc' which specifies how the results will be sorted (
@@ -258,14 +260,16 @@
 
         url = self.build_list_url('filter', config, conditions)
         fetched_entities = self._fetch_all(url, order, config)
 
         if fetched_entities is None:
             return []
 
+        logger.debug(f'Filter: Fetched {fetched_entities} entities')
+
         # There are no specified conditions ==> return all
         if not conditions:
             return fetched_entities
 
         return [entity for entity in fetched_entities if evaluate_conditions(conditions, entity, contain)]
 
     def all(self, order='asc', config=None, **kwargs):  # type: (str, utils.Config, **typing.Any) -> typing.List[Entity]
@@ -288,26 +292,41 @@
 
         return self._fetch_all(url, order, config)
 
     def __str__(self):
         return 'TogglSet<{}>'.format(self.entity_cls.__name__)
 
 
-class WorkspaceTogglSet(TogglSet):
+class WorkspacedTogglSet(TogglSet):
     """
     Specialized TogglSet for Workspaced entries.
     """
 
-    def build_list_url(self, caller, config, conditions):  # type: (str, utils.Config, typing.Dict) -> str
+    @classmethod
+    def _get_workspace_id(cls, config, conditions):  # type: (utils.Config, typing.Dict) -> int
         if conditions.get('workspace') is not None:
-            wid = conditions['workspace'].id
+            return conditions['workspace'].id
+        elif conditions.get('workspace_id') is not None:
+            return conditions['workspace_id']
         else:
-            wid = conditions.get('wid') or config.default_workspace.id
+            return conditions.get('wid') or config.default_workspace.id
 
-        return '/workspaces/{}/{}'.format(wid, self.base_url)
+    def build_list_url(self, caller, config, conditions):  # type: (str, utils.Config, typing.Dict) -> str
+        wid = self._get_workspace_id(config, conditions)
+        return f'/workspaces/{wid}/{self.entity_endpoints_name}'
+
+    def build_detail_url(self, eid, config, conditions):  # type: (int, utils.Config, typing.Dict) -> str
+        """
+        Build the detail URL.
+
+        :param eid: ID of the entity to fetch.
+        :param config: Config
+        """
+        wid = self._get_workspace_id(config, conditions)
+        return f"/workspaces/{wid}/{self.entity_endpoints_name}/{eid}"
 
 
 class TogglEntityMeta(ABCMeta):
     """
     Toggl Entity's Meta, which collects all Fields of a Entity and build related properties ('__fields__', '__mapped_fields__', '__signature__')
     Also if not defined it creates TogglSet instance binded to the Entity under 'objects' property.
     """
@@ -333,15 +352,15 @@
         fields = OrderedDict()
         for parent in parents:
             fields.update(parent.__fields__)
 
         for key, field in attrs.items():
             if isinstance(field, model_fields.TogglField):
                 if key in fields:
-                    logger.warning('Field \'{}\' is being overridden'.format(key))
+                    logger.warning(f'Field \'{key}\' is being overridden')
 
                 field.name = key
                 fields[key] = field
 
         return fields
 
     @staticmethod
@@ -370,15 +389,15 @@
         fields = mcs._make_fields(attrs, bases)
         setattr(new_class, '__fields__', fields)
         setattr(new_class, '__mapped_fields__', mcs._make_mapped_fields(fields))
         setattr(new_class, '__signature__', mcs._make_signature(fields))
 
         # Add objects only if they are not defined to allow custom TogglSet implementations
         if 'objects' not in new_class.__dict__:
-            setattr(new_class, 'objects', WorkspaceTogglSet(new_class))
+            setattr(new_class, 'objects', WorkspacedTogglSet(new_class))
         else:
             try:
                 new_class.objects.bind_to_class(new_class)
             except (exceptions.TogglException, AttributeError):
                 pass
 
         return new_class
@@ -394,14 +413,15 @@
     This class handles serialization, saving new instances, updating the existing one, deletion etc.
     Support for these operation can be customized using _can_* attributes, by default everything is enabled.
     """
 
     __signature__ = Signature()
     __fields__ = OrderedDict()
 
+    _endpoints_name = None
     _validate_workspace = True
     _can_create = True
     _can_update = True
     _can_delete = True
     _can_get_detail = True
     _can_get_list = True
 
@@ -462,15 +482,15 @@
         self.validate()
 
         if self.id is not None:  # Update
             utils.toggl('/{}/{}'.format(self.get_url(), self.id), 'put', self.json(update=True), config=config)
             self.__change_dict__ = {}  # Reset tracking changes
         else:  # Create
             data = utils.toggl('/{}'.format(self.get_url()), 'post', self.json(), config=config)
-            self.id = data['data']['id']  # Store the returned ID
+            self.id = data['id']  # Store the returned ID
 
     def delete(self, config=None):  # type: (utils.Config) -> None
         """
         Method for deletion of the entity through API using DELETE call.
 
         This will not delete the instance's object in Python, therefore calling save() method after deletion will
         result in new object created using POST call.
@@ -488,15 +508,15 @@
 
     def json(self, update=False):  # type: (bool) -> str
         """
         Serialize the entity into JSON string.
 
         :param update: Specifies if the resulted JSON should contain only changed fields (for PUT call) or whole entity.
         """
-        return json.dumps({self.get_name(): self.to_dict(serialized=True, changes_only=update)})
+        return json.dumps(self.to_dict(serialized=True, changes_only=update))
 
     def validate(self):  # type: () -> None
         """
         Performs validation across all Entity's fields.
 
         If overloading then don't forget to call super().validate()!
         """
@@ -511,22 +531,29 @@
     def to_dict(self, serialized=False, changes_only=False):  # type: (bool, bool) -> typing.Dict
         """
         Method that returns dict representing the instance.
 
         :param serialized: If True, the returned dict contains only Python primitive types and no objects (eq. so JSON serialization could happen)
         :param changes_only: If True, the returned dict contains only changes to the instance since last call of save() method.
         """
+        from .models import WorkspacedEntity
+        workspace = self.workspace if isinstance(self, WorkspacedEntity) else self
+        allow_premium = getattr(workspace, "premium", False)
+
         source_dict = self.__change_dict__ if changes_only else self.__fields__
         entity_dict = {}
         for field_name in source_dict.keys():
             try:
                 field = self.__fields__[field_name]
             except KeyError:
                 field = self.__mapped_fields__[field_name]
 
+            if field.premium and not allow_premium:
+                continue
+
             try:
                 value = field._get_value(self)
             except AttributeError:
                 value = None
 
             if serialized:
                 try:
@@ -566,16 +593,20 @@
 
         if verbose:
             return name.replace('_', ' ').capitalize()
 
         return name
 
     @classmethod
-    def get_url(cls):  # type: () -> str
-        return cls.get_name() + 's'
+    def get_endpoints_name(self):  # type: () -> str
+        assert self._endpoints_name is not None
+        return self._endpoints_name
+
+    def get_url(self):  # type: () -> str
+        return self.get_endpoints_name()
 
     @classmethod
     def deserialize(cls, config=None, **kwargs):  # type: (utils.Config, **typing.Any) -> typing.Generic[Entity]
         """
         Method which takes kwargs as dict representing the Entity's data and return actuall instance of the Entity.
         """
         try:
```

### Comparing `togglCli-2.4.4/toggl/api/fields.py` & `togglCli-3.0.0/toggl/api/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
     Attribute 'write' specifies if user can set value to the field.
     """
 
     read = True  # type: bool
     """
     Attribute 'read' specifies if user can get value from the field.
-    
+
     It represents fields that are not returned from server, but you can only pass value to them.
     It is allowed to read from the field once you set some value to it, but not before
     """
 
     premium = False  # type: bool
     """
     Attribute 'premium' specifies if the field can be used only for premium workspaces.
@@ -208,15 +208,15 @@
         if not self.name:
             raise RuntimeError('Name of the field is not defined!')
 
         if not self.read and not self._has_value(instance):
             raise exceptions.TogglNotAllowedException('You are not allowed to read from \'{}\' attribute!'
                                                       .format(self.name))
 
-        # When instance is None, then the descriptor as accessed directly from class and not its instance 
+        # When instance is None, then the descriptor as accessed directly from class and not its instance
         # ==> return the descriptors instance.
         if instance is None:
             return self
 
         return self._get_value(instance)
 
     def __set__(self, instance, value):  # type: (base.Entity, T) -> None
@@ -328,14 +328,17 @@
         else:
             raise TypeError('Value which is being set to DateTimeField have to be either '
                             'datetime.datetime or pendulum.DateTime object!')
 
         super().__set__(instance, value)
 
     def parse(self, value, instance):  # type: (str, base.Entity) -> pendulum.DateTime
+        if value is None:
+            return super().parse(value, instance)
+
         config = getattr(instance, '_config', None) or utils.Config.factory()
 
         if isinstance(value, datetime.datetime):
             if self._is_naive(value):
                 return pendulum.instance(value, config.timezone)
 
             return pendulum.instance(value)
```

### Comparing `togglCli-2.4.4/toggl/api/models.py` & `togglCli-3.0.0/toggl/api/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,168 @@
 import json
 import logging
 import typing
 from copy import copy
+from typing import TypedDict
 from urllib.parse import quote_plus
 from validate_email import validate_email
 
 import datetime
 import pendulum
 
 from toggl.api import base, fields
 from toggl import utils, exceptions
 
 logger = logging.getLogger('toggl.api.models')
 
 
+class OrganizationToggleSet(base.TogglSet):
+    """
+    Specialized TogglSet for organization entities
+    """
+
+    def build_detail_url(self, eid, config, conditions):  # type: (int, utils.Config, typing.Dict) -> str
+        return '/{}/{}'.format(self.entity_endpoints_name, eid)
+
+
+class InvitationResult(TypedDict):
+    """
+    API result for creating new invitations
+    """
+    email: str
+    invitation_id: int
+    invite_url: str
+    organization_id: int
+    recipient_id: int
+    sender_id: int
+
+
+# Organization entity
+class Organization(base.TogglEntity):
+    _endpoints_name = "organizations"
+    _can_create = False  # TODO: implement
+    _can_delete = False  # TODO: implement
+
+    name = fields.StringField(required=True)
+    """
+    Name of the organization
+    """
+
+    admin = fields.BooleanField()
+    """
+    Shows whether the current request user is an admin of the organization
+    """
+
+    at = fields.StringField()
+    """
+    Organization's last modification date
+    """
+
+    created_at = fields.StringField()
+    """
+    Organization's creation date
+    """
+
+    is_multi_workspace_enabled = fields.BooleanField()
+    """
+    Is true when the organization option is_multi_workspace_enabled is set
+    """
+
+    is_unified = fields.BooleanField()
+
+    max_data_retention_days = fields.IntegerField()
+    """
+    How far back free workspaces in this org can access data.
+    """
+
+    max_workspaces = fields.IntegerField()
+    """
+    Maximum number of workspaces allowed for the organization
+    """
+
+    owner = fields.BooleanField()
+    """
+    Whether the requester is a the owner of the organization
+    """
+
+    payment_methods = fields.StringField()
+    """
+    Organization's subscription payment methods. Omitted if empty.
+    """
+
+    permissions = fields.StringField()
+
+    pricing_plan_enterprise = fields.BooleanField()
+    """
+    The subscription plan is an enterprise plan
+    """
+
+    pricing_plan_id = fields.IntegerField()  # TODO: map entity?
+    """
+    Organization plan ID
+    """
+
+    pricing_plan_name = fields.StringField()
+    """
+    The subscription plan name the org is currently on. Free or any plan name coming from payment provider
+    """
+
+    server_deleted_at = fields.StringField()
+    """
+    Organization's delete date
+    """
+
+    suspended_at = fields.StringField()
+    """
+    Whether the organization is currently suspended
+    """
+
+    user_count = fields.IntegerField()
+    """
+    Number of organization users
+    """
+
+    objects = OrganizationToggleSet()
+
+    def invite(self, workspace, *emails, admin=False, role=None):  # type: (Workspace, typing.Collection[str], bool, typing.Optional[str]) -> list[InvitationResult]
+        """
+        Invites users defined by email addresses. The users does not have to have account in Toggl, in that case after
+        accepting the invitation, they will go through process of creating the account in the Toggl web.
+
+        :param workspace: The workspace to invite users to.
+        :param emails: List of emails to invite.
+        :param admin: Whether the invited users should be admins.
+        :param role: Role of the invited users.
+        :return: None
+        """
+        for email in emails:
+            if not validate_email(email):
+                raise exceptions.TogglValidationException(f'Supplied email \'{email}\' is not valid email!')
+
+        workspace_invite_data = {'workspace_id': workspace.id, 'admin': admin}
+        if role:
+            workspace_invite_data['role'] = role
+        json_data = json.dumps({'emails': emails, 'workspaces': [workspace_invite_data]})
+
+        result = utils.toggl("/organizations/{}/invitations".format(self.id), "post", json_data, config=self._config)
+        return [InvitationResult(**invite) for invite in result['data']]
+
+
+class WorkspaceToggleSet(base.TogglSet):
+    """
+    Specialized TogglSet for workspace entities (not to be confused with :class:`base.WorkspacedTogglSet`
+    """
+
+    def build_detail_url(self, eid, config, conditions):  # type: (int, utils.Config, typing.Dict) -> str
+        return '/{}/{}'.format(self.entity_endpoints_name, eid)
+
+
 # Workspace entity
 class Workspace(base.TogglEntity):
+    _endpoints_name = "workspaces"
     _can_create = False
     _can_delete = False
 
     name = fields.StringField(required=True)
     """
     Name of the workspace
     """
@@ -35,19 +178,31 @@
     """
 
     only_admins_may_create_projects = fields.BooleanField()
     """
     Whether only the admins can create projects or everybody
     """
 
+    only_admins_may_create_tags = fields.BooleanField()
+    """
+    Whether only the admins can create tags or everybody
+    """
+
     only_admins_see_billable_rates = fields.BooleanField()
     """
     Whether only the admins can see billable rates or everybody
     """
 
+    only_admins_see_team_dashboard = fields.BooleanField()
+    """
+    Whether only the admins can see team dashboard or everybody
+    """
+
+    organization = fields.MappingField(Organization, 'organization_id')  # type: Organization
+
     rounding = fields.IntegerField()
     """
     Type of rounding:
 
     * round down: -1
     * nearest: 0
     * round up: 1
@@ -65,92 +220,109 @@
     """
 
     default_currency = fields.StringField()
     """
     Default currency for workspace
     """
 
-    # As TogglEntityMeta is by default adding WorkspaceTogglSet to TogglEntity,
-    # but we want vanilla TogglSet so defining it here explicitly.
-    objects = base.TogglSet()
+    ical_enabled = fields.BooleanField()
+    ical_url = fields.StringField()
+    logo_url = fields.StringField()
+
+    # As TogglEntityMeta is by default adding WorkspacedTogglSet to TogglEntity,
+    # but we want WorkspaceToggleSet so defining it here explicitly.
+    objects = WorkspaceToggleSet()
 
-    def invite(self, *emails):  # type: (str) -> None
+    def invite(self, *emails, admin=False, role=None):  # type: (Workspace, typing.Collection[str], bool, typing.Optional[str]) -> list[InvitationResult]
         """
         Invites users defined by email addresses. The users does not have to have account in Toggl, in that case after
         accepting the invitation, they will go through process of creating the account in the Toggl web.
 
         :param emails: List of emails to invite.
+        :param admin: Whether the invited users should be admins.
+        :param role: Role of the invited users.
         :return: None
         """
-        for email in emails:
-            if not validate_email(email):
-                raise exceptions.TogglValidationException('Supplied email \'{}\' is not valid email!'.format(email))
+        return self.organization.invite(self, *emails, admin=admin, role=role)
 
-        emails_json = json.dumps({'emails': emails})
-        data = utils.toggl("/workspaces/{}/invite".format(self.id), "post", emails_json, config=self._config)
 
-        if 'notifications' in data and data['notifications']:
-            raise exceptions.TogglException(data['notifications'])
+class WorkspacedEntity(base.TogglEntity):
+    """
+    Abstract entity which has linked Workspace
+    """
+
+    workspace = fields.MappingField(Workspace, 'workspace_id', write=False,
+                                               default=lambda config: config.default_workspace) # type: Workspace
+    """
+    Workspace to which the resource is linked to.
+    """
 
+    def get_url(self):  # type: () -> str
+        return f'workspaces/{self.workspace.id}/{self.get_endpoints_name()}'
 
-class WorkspacedEntity(base.TogglEntity):
+class OldWorkspacedEntity(base.TogglEntity):
     """
     Abstract entity which has linked Workspace
     """
 
     workspace = fields.MappingField(Workspace, 'wid', write=False,
-                                               default=lambda config: config.default_workspace)
+                                               default=lambda config: config.default_workspace) # type: Workspace
     """
     Workspace to which the resource is linked to.
     """
 
+    def get_url(self):  # type: () -> str
+        return f'workspaces/{self.workspace.id}/{self.get_endpoints_name()}'
+
 
 # Premium Entity
 class PremiumEntity(WorkspacedEntity):
     """
     Abstract entity that enforces that linked Workspace is premium (paid).
     """
 
     def save(self, config=None):  # type: (utils.Config) -> None
         if not self.workspace.premium:
-            raise exceptions.TogglPremiumException('The entity {} requires to be associated with Premium workspace!')
+            raise exceptions.TogglPremiumException(f'The entity {self.get_name(verbose=True)} requires to be associated with Premium workspace!')
 
         super().save(config)
 
 
 # ----------------------------------------------------------------------------
 # Entities definitions
 # ----------------------------------------------------------------------------
-class Client(WorkspacedEntity):
+class Client(OldWorkspacedEntity):
     """
     Client entity
     """
 
+    _endpoints_name = "clients"
+
     name = fields.StringField(required=True)
     """
     Name of client (Required)
     """
 
     notes = fields.StringField()
-    """
-    Notes about the client
-    """
+
 
 
 class Project(WorkspacedEntity):
     """
     Project entity
     """
 
+    _endpoints_name = "projects"
+
     name = fields.StringField(required=True)
     """
     Name of the project. (Required)
     """
 
-    client = fields.MappingField(Client, 'cid')
+    client = fields.MappingField(Client, 'client_id')
     """
     Client associated to the project.
     """
 
     active = fields.BooleanField(default=True)
     """
     Whether the project is archived or not. (Default: True)
@@ -179,20 +351,15 @@
     estimated_hours = fields.IntegerField(default=0, premium=True)
     """
     If auto_estimates is true then the sum of task estimations is returned, otherwise user inserted hours.
 
     (Available only for Premium workspaces)
     """
 
-    color = fields.IntegerField()
-    """
-    Id of the color selected for the project
-    """
-
-    hex_color = fields.StringField()
+    color = fields.StringField()
     """
     Hex code of the color selected for the project
     """
 
     rate = fields.FloatField(premium=True)
     """
     Hourly rate of the project.
@@ -211,44 +378,49 @@
         """
         project_user = ProjectUser(project=self, user=user, workspace=self.workspace, manager=manager, rate=rate)
         project_user.save()
 
         return project_user
 
 
-class UserSet(base.WorkspaceTogglSet):
+class UserSet(base.WorkspacedTogglSet):
 
     def current_user(self, config=None):  # type: (utils.Config) -> 'User'
         """
         Fetches details about the current user.
         """
         fetched_entity = utils.toggl('/me', 'get', config=config)
-        return self.entity_cls.deserialize(config=config, **fetched_entity['data'])
+        return self.entity_cls.deserialize(config=config, **fetched_entity)
 
 
 class User(WorkspacedEntity):
     """
     User entity.
     """
 
+    _endpoints_name = "users"
     _can_create = False
     _can_update = False
     _can_delete = False
     _can_get_detail = False
 
     api_token = fields.StringField()
     """
     API token to use for API calls.
 
     (Returned only for User.objects.current_user() call.)
     """
 
-    send_timer_notifications = fields.BooleanField()
+    has_password = fields.BooleanField()
+    country_id = fields.StringField()
+    intercom_hash = fields.StringField()
+    openid_email = fields.StringField()
+    openid_enabled = fields.BooleanField()
 
-    default_workspace = fields.MappingField(Workspace, 'default_wid')  # type: Workspace
+    default_workspace = fields.MappingField(Workspace, 'default_workspace_id')  # type: Workspace
     """
     Default workspace for calls that does not specify Workspace.
 
     (Returned only for User.objects.current_user() call.)
     """
 
     email = fields.EmailField()
@@ -287,31 +459,14 @@
     timezone = fields.StringField()
     """
     Timezone which is used to convert the times into.
 
     May differ from one used in this tool, see toggl.utils.Config().
     """
 
-    # TODO: Add possibility to use this value in Config.time_format
-    timeofday_format = fields.ChoiceField({
-        'H:mm': '24-hour',
-        'h:mm A': '12-hour'
-    })
-    """
-    Format of time used to display time.
-    """
-
-    # TODO: Add possibility to use this value in Config.datetime_format
-    date_format = fields.ChoiceField(
-        ["YYYY-MM-DD", "DD.MM.YYYY", "DD-MM-YYYY", "MM/DD/YYYY", "DD/MM/YYYY", "MM-DD-YYYY"]
-    )
-    """
-    Format of date used to display dates.
-    """
-
     objects = UserSet()
 
     @classmethod
     def signup(cls, email, password, timezone=None, created_with='TogglCLI',
                config=None):  # type: (str, str, str, str, utils.Config) -> User
         """
         Creates brand new user. After creation confirmation email is sent to him.
@@ -334,16 +489,16 @@
 
         user_json = json.dumps({'user': {
             'email': email,
             'password': password,
             'timezone': timezone,
             'created_with': created_with
         }})
-        data = utils.toggl("/signups", "post", user_json, config=config)
-        return cls.deserialize(config=config, **data['data'])
+        data = utils.toggl("/signup", "post", user_json, config=config)
+        return cls.deserialize(config=config, **data)
 
     def is_admin(self, workspace):
         wid = workspace.id if isinstance(workspace, Workspace) else workspace
 
         workspace_user = WorkspaceUser.objects.get(wid=wid, uid=self.id)
         return workspace_user.admin
 
@@ -355,14 +510,15 @@
     """
     Workspace User entity.
 
     This entity represents assignment of specific User into Workspace.
     It additionally configures access rights and several other things.
     """
 
+    _endpoints_name = "workspace_users"
     _can_get_detail = False
     _can_create = False
 
     email = fields.EmailField(write=False)
     """
     Email of the user.
     """
@@ -389,34 +545,36 @@
 class ProjectUser(WorkspacedEntity):
     """
     Project User entity.
 
     Similarly to WorkspaceUser, it is entity which represents assignment of specific User into Project.
     It additionally configures access rights and several other things.
     """
+
+    _endpoints_name = "project_users"
     _can_get_detail = False
 
     rate = fields.FloatField(admin_only=True)
     """
     Hourly rate for the project user in the currency of the project's client or in workspace default currency.
 
     (Available only for Premium workspaces)
     """
 
     manager = fields.BooleanField(default=False)
     """
     Admin rights for this project
     """
 
-    project = fields.MappingField(Project, 'pid', write=False)
+    project = fields.MappingField(Project, 'project_id', write=False)
     """
     Project to which the User is assigned.
     """
 
-    user = fields.MappingField(User, 'uid', write=False)
+    user = fields.MappingField(User, 'user_id', write=False)
     """
     User which is linked to Project.
     """
 
     def __str__(self):
         return '{}/{} (#{})'.format(self.project.name, self.user.email, self.id)
 
@@ -424,14 +582,16 @@
 class Task(PremiumEntity):
     """
     Task entity.
 
     This entity is available only for Premium workspaces.
     """
 
+    _endpoints_name = "tasks"
+
     name = fields.StringField(required=True)
     """
     Name of task
     """
 
     project = fields.MappingField(Project, 'pid', required=True)
     """
@@ -460,14 +620,15 @@
 
 
 class Tag(WorkspacedEntity):
     """
     Tag entity
     """
 
+    _endpoints_name = "tags"
     _can_get_detail = False
 
     name = fields.StringField(required=True)
     """
     Name of tag (Required)
     """
 
@@ -503,15 +664,15 @@
     Getter for Duration Property field.
 
     Handles correctly the conversion of negative running duration (for more refer to the Toggl API doc).
     """
     if instance.is_running:
         return instance.start.int_timestamp * -1
 
-    return int((instance.stop - instance.start).in_seconds())
+    return int((instance.stop.replace(microsecond=0) - instance.start.replace(microsecond=0)).in_seconds())
 
 
 def set_duration(name, instance, value, init=False):  # type: (str, base.Entity, typing.Optional[int], bool) -> typing.Optional[bool]
     """
     Setter for Duration Property field.
     """
     if init is True:
@@ -546,22 +707,22 @@
 
     return '{}:{:02d}:{:02d}'.format(hours, minutes, seconds)
 
 
 datetime_type = typing.Union[datetime.datetime, pendulum.DateTime]
 
 
-class TimeEntrySet(base.TogglSet):
+class TimeEntrySet(base.WorkspacedTogglSet):
     """
     TogglSet which is extended by current() method which returns the currently running TimeEntry.
     Moreover it extends the filtrating mechanism by native filtering according start and/or stop time.
     """
 
     def build_list_url(self, caller, config, conditions):  # type: (str, utils.Config, typing.Dict) -> str
-        url = '/{}'.format(self.base_url)
+        url = '/me/{}'.format(self.entity_endpoints_name)
 
         if caller == 'filter':
             start = conditions.pop('start', None)
             stop = conditions.pop('stop', None)
 
             if start is not None or stop is not None:
                 url += '?'
@@ -570,28 +731,36 @@
                 url += 'start_date={}&'.format(quote_plus(start.isoformat()))
 
             if stop is not None:
                 url += 'end_date={}&'.format(quote_plus(stop.isoformat()))
 
         return url
 
+    def build_detail_url(self, eid, config, conditions):  # type: (int, utils.Config, typing.Dict) -> str
+        return '/me/{}/{}'.format(self.entity_endpoints_name, eid)
+
+    def _fetch_all(self, url, order, config):  # type: (str, str, utils.Config) -> typing.List[base.Entity]
+        output = super()._fetch_all(url, order, config)
+        output.sort(key=lambda e: e.start, reverse=(order == 'desc'))
+        return output
+
     def current(self, config=None):  # type: (utils.Config) -> typing.Optional[TimeEntry]
         """
         Method that returns currently running TimeEntry or None if there is no currently running time entry.
 
         :param config:
         :return:
         """
         config = config or utils.Config.factory()
-        fetched_entity = utils.toggl('/time_entries/current', 'get', config=config)
+        fetched_entity = utils.toggl('/me/time_entries/current', 'get', config=config)
 
-        if fetched_entity.get('data') is None:
+        if fetched_entity is None:
             return None
 
-        return self.entity_cls.deserialize(config=config, **fetched_entity['data'])
+        return self.entity_cls.deserialize(config=config, **fetched_entity)
 
     def _build_reports_url(self, start, stop, page, wid):
         url = '/details?user_agent=toggl_cli&workspace_id={}&page={}'.format(wid, page)
 
         if start is not None:
             url += '&since={}'.format(quote_plus(start.isoformat()))
 
@@ -662,20 +831,22 @@
             if not self._should_fetch_more(page, returned):
                 return
 
             page += 1
 
 
 class TimeEntry(WorkspacedEntity):
+    _endpoints_name = "time_entries"
+
     description = fields.StringField()
     """
     Description of the entry.
     """
 
-    project = fields.MappingField(Project, 'pid')
+    project = fields.MappingField(Project, 'project_id')
     """
     Project to which the Time entry is linked to.
     """
 
     task = fields.MappingField(Task, 'tid', premium=True)
     """
     Task to which the Time entry is linked to.
@@ -726,18 +897,14 @@
             raise ValueError(
                 'You can create only finished time entries through this way! '
                 'You must supply either \'stop\' or \'duration\' parameter!'
             )
 
         super().__init__(start=start, stop=stop, duration=duration, **kwargs)
 
-    @classmethod
-    def get_url(cls):
-        return 'time_entries'
-
     def to_dict(self, serialized=False, changes_only=False):
         # Enforcing serialize duration when start or stop changes
         if changes_only and (self.__change_dict__.get('start') or self.__change_dict__.get('stop')):
             self.__change_dict__['duration'] = None
 
         return super().to_dict(serialized=serialized, changes_only=changes_only)
```

### Comparing `togglCli-2.4.4/toggl/assets/icon.png` & `togglCli-3.0.0/toggl/assets/icon.png`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/cli/commands.py` & `togglCli-3.0.0/toggl/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import pendulum
 from prettytable import PrettyTable
 
 from toggl import api, exceptions, utils, __version__
 from toggl.cli import helpers, types
 from toggl.cli.themes import themes
 
-DEFAULT_CONFIG_PATH = '~/.togglrc'
-
 logger = logging.getLogger('toggl.cli.commands')
 click_completion.init()
 
 
 # TODO: Improve better User's management. Hide all the Project's users/Workspace's users and work only with User object
 #   ==> for that support for mapping filter needs to be written (eq. user.email == 'test@test.org')
 
@@ -211,22 +209,25 @@
 @click.option('--project', '-o', type=types.ResourceType(api.Project),
               help='Filters the entries by project. Can be ID or name of the project.', )
 @click.option('--tags', '-a', type=types.SetType(), help='Filters the entries by list of tags delimited with \',\'')
 @click.option('--fields', '-f', type=types.FieldsType(api.TimeEntry), default='description,duration,start,stop',
               help='Defines a set of fields of time entries, which will be displayed. It is also possible to modify '
                    'default set of fields using \'+\' and/or \'-\' characters. Supported values: '
                    + types.FieldsType.format_fields_for_help(api.TimeEntry))
+@click.option('--limit', '-n', type=int, help='The number of entries to display')
 @click.pass_context
-def entry_ls(ctx, fields, today, use_reports, **conditions):
+def entry_ls(ctx, fields, today, use_reports, limit, **conditions):
     """
     Lists time entries the user has access to.
 
-    By default the command uses API call that has limited number of time entries fetched  with 1000 entries in
-    last 9 days. If you want to overcome this limitation use --use-reports flag, that will use different
-    API call, which overcomes this limitations but currently support only --start/--stop filtration.
+    By default the entries of the last 9 days are fetched, to keep compatibility with older API versions.
+    If you want to select a different time range, use --start and --stop flags.
+    In general, the --start/--stop API is limited to entries from the last 3 months,  # TODO check
+    if you want to overcome this limitation use --use-reports flag, that will use different
+    API call.
 
     The list visible
     through this utility and on toggl's web client might differ in the range
     as they developing new version of API and they are able to see in the future
     and also longer into past.
     """
     config = ctx.obj.get('config')
@@ -235,16 +236,24 @@
     if today:
         if conditions['start'] or conditions['stop']:
             click.echo('You can\'t use --start or --stop parameters with --today parameter!', err=True)
             exit(2)
         conditions['start'] = pendulum.today()
         conditions['stop'] = pendulum.tomorrow()
 
+    if not conditions.get('start'):
+        conditions['start'] = pendulum.now() - pendulum.duration(days=9)
+    if not conditions.get("stop"):
+        conditions['stop'] = pendulum.now()
+
     entities = get_entries(ctx, use_reports, **conditions)
 
+    if limit:
+        entities = entities[:limit]
+
     if ctx.obj.get('simple'):
         if ctx.obj.get('header'):
             click.echo('\t'.join([click.style(field.capitalize(), **theme.header) for field in fields]))
 
         for entity in entities:
             click.echo('\t'.join(
                 [str(entity.__fields__[field].format(getattr(entity, field, ''))) for field in fields]
@@ -448,14 +457,16 @@
 
     api.TimeEntry.start_and_save(
         config=ctx.obj['config'],
         description=descr,
         **kwargs
     )
 
+    click.echo('Started {}'.format(descr))
+
 
 @cli.command('now', short_help='manage current time entry')
 @click.option('--description', '-d', help='Sets description')
 @click.option('--start', '-s', type=types.DateTimeType(allow_now=True), help='Sets starts time.')
 @click.option('--tags', '-a', type=types.ModifierSetType(), help='Modifies the tags. List of values delimited by \',\'.'
                                                                  'Support either modification or specification mode. '
                                                                  'More info above.')
@@ -525,20 +536,23 @@
 @click.pass_context
 def entry_continue(ctx, descr, start):
     """
     If DESCR is specified then it will search this entry and continue it, otherwise it continues the last time entry.
 
     The underhood behaviour of Toggl is that it actually creates a new entry with the same description.
     """
+    config = ctx.obj['config']
     entry = None
     try:
         if descr is None:
-            entry = api.TimeEntry.objects.all(order='desc', config=ctx.obj['config'])[0]
+            entry = api.TimeEntry.objects.current(config=config)
+            if entry is None:
+                entry = api.TimeEntry.objects.all(order='desc', config=config)[0]
         else:
-            entry = api.TimeEntry.objects.filter(contain=True, description=descr, config=ctx.obj['config'])[0]
+            entry = api.TimeEntry.objects.filter(contain=True, description=descr, config=config)[0]
     except IndexError:
         click.echo('You don\'t have any time entries in past 9 days!')
         exit(1)
 
     entry.continue_and_save(start=start)
 
     click.echo('Time entry \'{}\' continue!'.format(getattr(entry, 'description', '<Entry without description>')))
@@ -604,15 +618,15 @@
 
 @clients.command('get', short_help='retrieve details of a client')
 @click.argument('spec')
 @click.pass_context
 def clients_get(ctx, spec):
     """
     Gets details of a client specified by SPEC argument. SPEC can be either ID or Name of the client.
-    Be aware that if you use specify SPEC using Name you won't get note for this client.
+    Be aware that if you specify SPEC using Name you won't get note for this client.
 
     If SPEC is Name, then the lookup is done in the default workspace, unless --workspace is specified.
     """
     helpers.entity_detail(api.Client, spec, obj=ctx.obj)
 
 
 @clients.command('rm', short_help='delete a client')
@@ -654,15 +668,15 @@
                                                     'By default it is public.')
 @click.option('--billable', '-b', is_flag=True, default=False, help='Specifies whether project is billable or not. '
                                                                     '(Premium only)')
 @click.option('--auto-estimates', is_flag=True, default=False,
               help='Specifies whether the estimated hours should be automatically calculated based on task estimations '
                    '(Premium only)')
 @click.option('--rate', '-r', type=click.FLOAT, help='Hourly rate of the project (Premium only)')
-@click.option('--color', type=click.INT, help='ID of color used for the project')
+@click.option('--color', type=click.STRING, default="#0b83d9", help='Hex code of color used for the project')
 @click.pass_context
 def projects_add(ctx, public=None, **kwargs):
     """
     Creates a new project.
     """
     project = api.Project(
         is_private=not public,
@@ -685,15 +699,15 @@
                    ' users (=public) or just only project\'s users.')
 @click.option('--billable/--no-billable', default=None, help='Specifies whether project is billable or not.'
                                                              ' (Premium only)')
 @click.option('--auto-estimates/--no-auto-estimates', default=None,
               help='Specifies whether the estimated hours are automatically calculated based on task estimations or'
                    ' manually fixed based on the value of \'estimated_hours\' (Premium only)')
 @click.option('--rate', '-r', type=click.FLOAT, help='Hourly rate of the project (Premium only)')
-@click.option('--color', type=click.INT, help='ID of color used for the project')
+@click.option('--color', type=click.STRING, default="#0b83d9", help='Hex code of color used for the project')
 @click.pass_context
 def projects_update(ctx, spec, **kwargs):
     """
     Updates a project specified by SPEC which is either ID or Name of the project.
     """
     helpers.entity_update(api.Project, spec, obj=ctx.obj, **kwargs)
 
@@ -751,15 +765,15 @@
 def project_users_ls(ctx, fields):
     """
     Lists all project's users.
     """
     project = ctx.obj['project']
     src = api.ProjectUser.objects.filter(project=project, config=ctx.obj['config'])
 
-    helpers.entity_listing(src, fields)
+    helpers.entity_listing(src, fields, obj=ctx.obj)
 
 
 @project_users.command('add', short_help='add a user into the project')
 @click.option('--user', '-u', prompt='Enter ID or Email of the user to add to project',
               help='User to be added. Can be ID or email of the user',
               type=types.ResourceType(api.User, fields=('id', 'email')))
 @click.option('--rate', '-f', default=None, type=click.FLOAT, help='Hourly rate for the project user')
@@ -854,29 +868,39 @@
     """
     Manages assigned users to a specific workspace specified by --workspace option, if not specified the default
     workspace is used.
     """
     ctx.obj['workspace'] = workspace or ctx.obj['config'].default_workspace
 
 
+# TODO: fix with newer organization API
 @workspace_users.command('invite', short_help='invite an user into workspace')
-@click.option('--email', '-e', help='Email address of the user to invite into the workspace',
-              prompt='Email address of the user to invite into the workspace')
+@click.argument('emails', nargs=-1)
 @click.pass_context
-def workspace_users_invite(ctx, email):
+def workspace_users_invite(ctx, emails):
     """
     Invites an user into the workspace.
 
     It can be either an existing user or somebody who is not present at the Toggl platform.
     After the invitation is sent, the user needs to accept invitation to be fully part of the workspace.
     """
     workspace = ctx.obj['workspace']
-    workspace.invite(email)
+    invitations = workspace.invite(*emails)
 
-    click.echo("User '{}' was successfully invited! He needs to accept the invitation now.".format(email))
+    click.echo(
+        "Invites successfully sent! Invited users need to accept the invitation now."
+    )
+    click.echo(
+        "Created invites IDs:\n{}".format(
+            "\n".join(
+                "- #{}: email {}".format(invite["invitation_id"], invite["email"])
+                for invite in invitations
+            )
+        )
+    )
 
 
 @workspace_users.command('ls', short_help='list workspace\'s users')
 @click.option('--fields', '-f', type=types.FieldsType(api.WorkspaceUser), default='email,active,admin,id',
               help='Defines a set of fields which will be displayed. It is also possible to modify default set of '
                    'fields using \'+\' and/or \'-\' characters. Supported values: '
                    + types.FieldsType.format_fields_for_help(api.WorkspaceUser))
```

### Comparing `togglCli-2.4.4/toggl/cli/helpers.py` & `togglCli-3.0.0/toggl/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/cli/themes.py` & `togglCli-3.0.0/toggl/cli/themes.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/cli/types.py` & `togglCli-3.0.0/toggl/cli/types.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/exceptions.py` & `togglCli-3.0.0/toggl/exceptions.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/utils/bootstrap.py` & `togglCli-3.0.0/toggl/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/utils/config.py` & `togglCli-3.0.0/toggl/utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import platform
 import typing
 from collections import namedtuple
 
 import click
 import requests
 from pbr import version
+from pathlib import Path
 
 from toggl.utils import metas, bootstrap, migrations
 from toggl import exceptions
 
 logger = logging.getLogger('toggl.utils.config')
 
 # Defines which attrs of all parents will be merged into the new config class -> related to ConfigMeta
@@ -58,15 +59,26 @@
     Only attributes that have entry in INI_MAPPING will be considered during the lookup, if the attribute does not have
     entry the look continues with propagating the lookup to next in line, with super().
     """
     INI_MAPPING = {
         'version': IniEntry('version', str),
     }
 
-    DEFAULT_CONFIG_PATH = os.path.expanduser('~/.togglrc')
+    _old_file_path = Path.expanduser(Path('~/.togglrc'))
+
+    if "XDG_CONFIG_HOME" in os.environ:
+        _new_file_path = Path(os.environ["XDG_CONFIG_HOME"]).joinpath(".togglrc")
+
+        if _new_file_path.exists() or not _old_file_path.exists():
+            DEFAULT_CONFIG_PATH = _new_file_path
+        else:
+            DEFAULT_CONFIG_PATH = _old_file_path
+
+    else:
+        DEFAULT_CONFIG_PATH = _old_file_path
 
     def __init__(self, config_path=sentinel, **kwargs):  # type: (typing.Optional[str], **typing.Any) -> None
         self._config_path = self.DEFAULT_CONFIG_PATH if config_path == sentinel else config_path
         self._store = configparser.ConfigParser(interpolation=None)
         self._loaded = False
 
         if self._config_path is not None:
```

### Comparing `togglCli-2.4.4/toggl/utils/metas.py` & `togglCli-3.0.0/toggl/utils/metas.py`

 * *Files identical despite different names*

### Comparing `togglCli-2.4.4/toggl/utils/migrations.py` & `togglCli-3.0.0/toggl/utils/migrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,19 +93,19 @@
             else:
                 parser.set('options', 'datetime_format', value)
                 break
 
     @staticmethod
     def migrate_timezone(parser):  # type: (configparser.ConfigParser) -> None
         tz = parser.get('options', 'timezone')
-        if tz not in pendulum.timezones:
+        if tz not in pendulum.timezones():
             click.echo('We have not recognized your timezone!')
             new_tz = inquirer.shortcuts.text(
                 'Please enter valid timezone. Default is your system\'s timezone.',
-                default='local', validate=lambda _, i: i in pendulum.timezones or i == 'local')
+                default='local', validate=lambda _, i: i in pendulum.timezones() or i == 'local')
             parser.set('options', 'tz', new_tz)
 
     @classmethod
     def migrate(cls, parser):  # type: (configparser.ConfigParser) -> configparser.ConfigParser
         cls.migrate_authentication(parser)
         cls.migrate_datetime(parser)
         cls.migrate_timezone(parser)
```

### Comparing `togglCli-2.4.4/toggl/utils/others.py` & `togglCli-3.0.0/toggl/utils/others.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,19 @@
 
 def convert_credentials_to_api_token(username, password):
     config = Config.factory(None)
     config.username = username
     config.password = password
 
     data = toggl("/me", "get", config=config)
-    return data['data']['api_token']
+    return data['api_token']
 
 
 def handle_error(response):
+    logger.debug(f"Handling error for {response.status_code}: {response.text}")
     if response.status_code == 402:
         raise exceptions.TogglPremiumException(
             "Request tried to utilized Premium functionality on workspace which is not Premium!"
         )
 
     if response.status_code == 403:
         raise exceptions.TogglAuthenticationException(
@@ -161,15 +162,15 @@
     tries = config.retries if config.retries and config.retries > 1 else 1  # There needs to be at least one try!
 
     exception = None
     for _ in range(tries):
         try:
             logger.debug('Default workspace: {}'.format(config._default_workspace))
             response = _toggl_request(url, method, data, headers, config.get_auth())
-            response_json = response.json()
+            response_json = response.json() if response.text else None
             logger.debug('Response {}:\n{}'.format(response.status_code, pformat(response_json)))
             return response_json
         except (exceptions.TogglThrottlingException, requests.exceptions.ConnectionError) as e:
             sleep(0.1)  # Lets give Toggl API some time to recover
             exception = e
             # TODO: Make it exponential
```

### Comparing `togglCli-2.4.4/togglCli.egg-info/PKG-INFO` & `togglCli-3.0.0/togglCli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: togglCli
-Version: 2.4.4
+Version: 3.0.0
 Summary: Command line tool and set of Python wrapper classes for interacting with toggl's API
 Home-page: https://toggl.uhlir.dev
 Author: D. Robert Adams & Adam Uhlir
 Author-email: adam@uhlir.dev
 License: MIT
 Project-URL: Source, https://github.com/auhau/toggl-cli
 Project-URL: Documentation, https://toggl.uhlir.devg
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Office/Business :: Scheduling
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools==69.0.3
+Requires-Dist: pendulum==3.0.0
+Requires-Dist: requests>=2.23.0
+Requires-Dist: click==8.1.7
+Requires-Dist: inquirer==3.2.4
+Requires-Dist: prettytable==3.6.0
+Requires-Dist: validate_email==1.3
+Requires-Dist: click-completion==0.5.2
+Requires-Dist: pbr==6.0.0
+Requires-Dist: notify-py==0.3.42
 
 # Toggl CLI
 
 [![PyPI version](https://badge.fury.io/py/togglCli.svg)](https://badge.fury.io/py/togglCli) 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/togglCli.svg)](https://pypi.org/project/togglCli)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/togglCli.svg)](https://pypi.org/project/togglCli/) 
 [![codecov](https://codecov.io/gh/AuHau/toggl-cli/branch/master/graph/badge.svg)](https://codecov.io/gh/AuHau/toggl-cli)
```

### Comparing `togglCli-2.4.4/togglCli.egg-info/SOURCES.txt` & `togglCli-3.0.0/togglCli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -62,9 +62,10 @@
 toggl/utils/migrations.py
 toggl/utils/others.py
 togglCli.egg-info/PKG-INFO
 togglCli.egg-info/SOURCES.txt
 togglCli.egg-info/dependency_links.txt
 togglCli.egg-info/entry_points.txt
 togglCli.egg-info/not-zip-safe
+togglCli.egg-info/pbr.json
 togglCli.egg-info/requires.txt
 togglCli.egg-info/top_level.txt
```

