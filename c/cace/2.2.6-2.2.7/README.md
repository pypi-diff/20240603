# Comparing `tmp/cace-2.2.6.tar.gz` & `tmp/cace-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cace-2.2.6.tar", last modified: Fri May 24 08:46:33 2024, max compression
+gzip compressed data, was "cace-2.2.7.tar", last modified: Mon Jun  3 07:41:47 2024, max compression
```

## Comparing `cace-2.2.6.tar` & `cace-2.2.7.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.608248 cace-2.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.608248 cace-2.2.6/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.612248 cace-2.2.6/.github/actions/build_nix/
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-24 08:46:09.000000 cace-2.2.6/.github/actions/build_nix/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.612248 cace-2.2.6/.github/actions/check_space/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-24 08:46:09.000000 cace-2.2.6/.github/actions/check_space/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.612248 cace-2.2.6/.github/actions/setup_env/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-24 08:46:09.000000 cace-2.2.6/.github/actions/setup_env/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.612248 cace-2.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-24 08:46:09.000000 cace-2.2.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-05-24 08:46:09.000000 cace-2.2.6/.github/workflows/ci_nix.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-24 08:46:09.000000 cace-2.2.6/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-24 08:46:09.000000 cace-2.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-24 08:46:09.000000 cace-2.2.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-24 08:46:09.000000 cace-2.2.6/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-24 08:46:09.000000 cace-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-24 08:46:09.000000 cace-2.2.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-24 08:46:33.624248 cace-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-24 08:46:09.000000 cace-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.612248 cace-2.2.6/cace/
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-05-24 08:46:09.000000 cace-2.2.6/cace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-24 08:46:09.000000 cace-2.2.6/cace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-24 08:46:09.000000 cace-2.2.6/cace/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6461 2024-05-24 08:46:09.000000 cace-2.2.6/cace/cace_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44315 2024-05-24 08:46:09.000000 cace-2.2.6/cace/cace_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.620248 cace-2.2.6/cace/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_calculate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_collate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_gensim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_launch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_makeplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_measure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_regenerate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_simulate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_unused.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    65589 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/cace_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7999 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/electrical_parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/layout_estimate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/netlist_precheck.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/physical_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/safe_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14919 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/simulation_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22283 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/simulation_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-05-24 08:46:09.000000 cace-2.2.6/cace/common/spiceunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.620248 cace-2.2.6/cace/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1965 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/consoletext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/editparam.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/failreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/helpwindow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/rowwidget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/simhints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/textreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/tksimpledialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-24 08:46:09.000000 cace-2.2.6/cace/gui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 08:46:09.000000 cace-2.2.6/cace/open_pdks_rev
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/cace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-24 08:46:33.000000 cace-2.2.6/cace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-24 08:46:33.000000 cace-2.2.6/cace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:46:33.000000 cace-2.2.6/cace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 08:46:33.000000 cace-2.2.6/cace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 08:46:33.000000 cace-2.2.6/cace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 08:46:33.000000 cace-2.2.6/cace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-24 08:46:09.000000 cace-2.2.6/default.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.620248 cace-2.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 08:46:09.000000 cace-2.2.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 08:46:09.000000 cace-2.2.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.620248 cace-2.2.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/_static/cace_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/characterization.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/dev/codebase.md
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/dev/coding_style.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/dev/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/formats/format_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/formats/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/formats/schematic_description.md
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/usage/cace_cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/usage/cace_gui.md
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-24 08:46:09.000000 cace-2.2.6/docs/source/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-24 08:46:09.000000 cace-2.2.6/flake.lock
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-24 08:46:09.000000 cace-2.2.6/flake.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/nix/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 08:46:09.000000 cace-2.2.6/nix/colab-env.nix
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 08:46:09.000000 cace-2.2.6/nix/create-shell.nix
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-24 08:46:09.000000 cace-2.2.6/nix/docker.nix
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-24 08:46:09.000000 cace-2.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 08:46:09.000000 cace-2.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 08:46:09.000000 cace-2.2.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 08:46:09.000000 cace-2.2.6/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:46:33.624248 cace-2.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-24 08:46:09.000000 cace-2.2.6/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:46:33.624248 cace-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-24 08:46:09.000000 cace-2.2.6/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 08:46:09.000000 cace-2.2.6/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.138018 cace-2.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.118018 cace-2.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.118018 cace-2.2.7/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.122018 cace-2.2.7/.github/actions/build_nix/
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-06-03 07:41:22.000000 cace-2.2.7/.github/actions/build_nix/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.122018 cace-2.2.7/.github/actions/check_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-06-03 07:41:22.000000 cace-2.2.7/.github/actions/check_space/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.122018 cace-2.2.7/.github/actions/setup_env/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-03 07:41:22.000000 cace-2.2.7/.github/actions/setup_env/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.126019 cace-2.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-06-03 07:41:22.000000 cace-2.2.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-06-03 07:41:22.000000 cace-2.2.7/.github/workflows/ci_nix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-03 07:41:22.000000 cace-2.2.7/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 07:41:22.000000 cace-2.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-06-03 07:41:22.000000 cace-2.2.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-06-03 07:41:22.000000 cace-2.2.7/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-03 07:41:22.000000 cace-2.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-03 07:41:22.000000 cace-2.2.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-06-03 07:41:47.138018 cace-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-06-03 07:41:22.000000 cace-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.126019 cace-2.2.7/cace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-06-03 07:41:22.000000 cace-2.2.7/cace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-03 07:41:22.000000 cace-2.2.7/cace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-06-03 07:41:22.000000 cace-2.2.7/cace/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6461 2024-06-03 07:41:22.000000 cace-2.2.7/cace/cace_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44315 2024-06-03 07:41:22.000000 cace-2.2.7/cace/cace_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.130019 cace-2.2.7/cace/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_calculate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_collate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_gensim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_makeplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_measure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47466 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_regenerate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_simulate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_unused.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65589 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/cace_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7999 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/electrical_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/layout_estimate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/netlist_precheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/physical_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/safe_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14919 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/simulation_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22283 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/simulation_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-06-03 07:41:22.000000 cace-2.2.7/cace/common/spiceunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.134019 cace-2.2.7/cace/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1965 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/consoletext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/editparam.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/failreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/helpwindow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/rowwidget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/simhints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/textreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/tksimpledialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-06-03 07:41:22.000000 cace-2.2.7/cace/gui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-03 07:41:22.000000 cace-2.2.7/cace/open_pdks_rev
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.138018 cace-2.2.7/cace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-06-03 07:41:47.000000 cace-2.2.7/cace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-06-03 07:41:47.000000 cace-2.2.7/cace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:41:47.000000 cace-2.2.7/cace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 07:41:47.000000 cace-2.2.7/cace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 07:41:47.000000 cace-2.2.7/cace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 07:41:47.000000 cace-2.2.7/cace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-06-03 07:41:22.000000 cace-2.2.7/default.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.134019 cace-2.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 07:41:22.000000 cace-2.2.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-03 07:41:22.000000 cace-2.2.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.134019 cace-2.2.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.134019 cace-2.2.7/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/_static/cace_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/characterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.134019 cace-2.2.7/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/dev/codebase.md
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/dev/coding_style.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/dev/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.134019 cace-2.2.7/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/formats/format_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/formats/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/formats/schematic_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.138018 cace-2.2.7/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/usage/cace_cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/usage/cace_gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-03 07:41:22.000000 cace-2.2.7/docs/source/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-06-03 07:41:22.000000 cace-2.2.7/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-06-03 07:41:22.000000 cace-2.2.7/flake.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.138018 cace-2.2.7/nix/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-06-03 07:41:22.000000 cace-2.2.7/nix/colab-env.nix
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-06-03 07:41:22.000000 cace-2.2.7/nix/create-shell.nix
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-06-03 07:41:22.000000 cace-2.2.7/nix/docker.nix
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-06-03 07:41:22.000000 cace-2.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 07:41:22.000000 cace-2.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 07:41:22.000000 cace-2.2.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-03 07:41:22.000000 cace-2.2.7/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:41:47.138018 cace-2.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-06-03 07:41:22.000000 cace-2.2.7/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:41:47.138018 cace-2.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-03 07:41:22.000000 cace-2.2.7/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 07:41:22.000000 cace-2.2.7/tests/test1.py
```

### Comparing `cace-2.2.6/.github/actions/build_nix/action.yml` & `cace-2.2.7/.github/actions/build_nix/action.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/.github/actions/check_space/action.yml` & `cace-2.2.7/.github/actions/check_space/action.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/.github/actions/setup_env/action.yml` & `cace-2.2.7/.github/actions/setup_env/action.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/.github/workflows/ci.yaml` & `cace-2.2.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/.github/workflows/ci_nix.yml` & `cace-2.2.7/.github/workflows/ci_nix.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/.github/workflows/pypi.yaml` & `cace-2.2.7/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/.readthedocs.yaml` & `cace-2.2.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/Changelog.md` & `cace-2.2.7/Changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# 2.2.7
+
+## Common
+
+- Improve extraction with only a GDS file
+
 # 2.2.6
 
 ## Common
 
 - Restored functionality of `sequential` runtime option
 
 # 2.2.5
@@ -83,8 +89,8 @@
 
 ## GUI
 
 - Use argparse
 
 ## Common
 
-- Fixed two issues deemed "severe" [#47](https://github.com/efabless/cace/pull/47)
+- Fixed two issues deemed "severe" [#47](https://github.com/efabless/cace/pull/47)
```

### Comparing `cace-2.2.6/LICENSE` & `cace-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/Makefile` & `cace-2.2.7/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/PKG-INFO` & `cace-2.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.6
+Version: 2.2.7
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.6 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.7 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.6/README.md` & `cace-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/__init__.py` & `cace-2.2.7/cace/__init__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/__main__.py` & `cace-2.2.7/cace/__main__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/__version__.py` & `cace-2.2.7/nix/colab-env.nix`

 * *Files 21% similar despite different names*

```diff
@@ -7,11 +7,17 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '2.2.6'
-
-if __name__ == '__main__':
-    print(__version__, end='')
+{
+  system,
+  cace,
+  python3,
+  symlinkJoin,
+}:
+symlinkJoin {
+  name = "cace-colab-env";
+  paths = cace.includedTools;
+}
```

### Comparing `cace-2.2.6/cace/cace_cli.py` & `cace-2.2.7/cace/cace_cli.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/cace_gui.py` & `cace-2.2.7/cace/cace_gui.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_calculate.py` & `cace-2.2.7/cace/common/cace_calculate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_collate.py` & `cace-2.2.7/cace/common/cace_collate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_compat.py` & `cace-2.2.7/cace/common/cace_compat.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_evaluate.py` & `cace-2.2.7/cace/common/cace_evaluate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_gensim.py` & `cace-2.2.7/cace/common/cace_gensim.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_launch.py` & `cace-2.2.7/cace/common/cace_launch.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_makeplot.py` & `cace-2.2.7/cace/common/cace_makeplot.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_measure.py` & `cace-2.2.7/cace/common/cace_measure.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_read.py` & `cace-2.2.7/cace/common/cace_read.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_regenerate.py` & `cace-2.2.7/cace/common/cace_regenerate.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,22 @@
     if 'layout' in paths:
         gdspath = paths['layout']
         gdsfilename = os.path.join(gdspath, gdsname)
     else:
         gdspath = None
         gdsfilename = None
 
+    # Schematic-captured netlist
+    if 'netlist' in paths:
+        schem_netlist_path = os.path.join(paths['netlist'], 'schematic')
+        schem_netlist = os.path.join(schem_netlist_path, netlistname)
+    else:
+        schem_netlist_path = None
+        schem_netlist = None
+
     # Layout-extracted netlist with R-C parasitics
     if 'netlist' in paths:
         rcx_netlist_path = os.path.join(paths['netlist'], 'rcx')
         rcx_netlist = os.path.join(rcx_netlist_path, netlistname)
     else:
         rcx_netlist = None
         rcx_netlist = None
@@ -476,22 +484,22 @@
 
     if need_rcx_extract:
         print('Forcing regeneration of parasitic-extracted netlist.')
 
     if need_rcx_extract:
         # Layout parasitic netlist needs regenerating.  Check for magic layout.
 
-        if not magicfilename or not os.path.isfile(magicfilename):
-            print('Error:  No netlist or layout for project ' + dname + '.')
+        if (not magicfilename or not os.path.isfile(magicfilename)) and (
+            not gdsfilename or not os.path.isfile(gdsfilename)
+        ):
+            print(f'Error: No netlist or layout for project {dname}. ', end='')
             if magicfilename:
-                print(
-                    '(layout master file ' + magicfilename + ' not found.)\n'
-                )
+                print(f'(layout master file {magicfilename} not found.)\n')
             else:
-                print('(layout master file ' + gdsfilename + ' not found.)\n')
+                print(f'(layout master file {gdsfilename} not found.)\n')
             return False
 
         # Check for parasitic netlist directory
         if not os.path.exists(rcx_netlist_path):
             os.makedirs(rcx_netlist_path)
 
         rcfile = get_magic_rcfile(dsheet, magicfilename)
@@ -523,19 +531,21 @@
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             cwd=root_path,
             env=newenv,
             universal_newlines=True,
         )
-        if magicfilename:
+        if magicfilename and os.path.isfile(magicfilename):
             mproc.stdin.write('load ' + magicfilename + '\n')
         else:
             mproc.stdin.write('gds read ' + gdsfilename + '\n')
             mproc.stdin.write('load ' + dname + '\n')
+            # Use readspice to get the port order
+            mproc.stdin.write('readspice ' + schem_netlist + '\n')
         mproc.stdin.write('select top cell\n')
         mproc.stdin.write('expand\n')
         mproc.stdin.write('flatten ' + dname + '_flat\n')
         mproc.stdin.write('load ' + dname + '_flat\n')
         mproc.stdin.write('select top cell\n')
         mproc.stdin.write('cellname delete ' + dname + '\n')
         mproc.stdin.write('cellname rename ' + dname + '_flat ' + dname + '\n')
@@ -559,15 +569,15 @@
             print(
                 'Magic process returned error code '
                 + str(mproc.returncode)
                 + '\n'
             )
 
         if need_rcx_extract and not os.path.isfile(rcx_netlist):
-            print('Error:  No netlist with parasitics extracted from magic.')
+            print('Error: No netlist with parasitics extracted from magic.')
 
         # Remove the temporary directory of extraction files "cace_extfiles"
         try:
             shutil.rmtree(os.path.join(root_path, 'cace_extfiles'))
         except:
             print('Warning: Directory for extraction files was not created.')
 
@@ -624,14 +634,22 @@
     if 'layout' in paths:
         gdspath = paths['layout']
         gdsfilename = os.path.join(gdspath, gdsname)
     else:
         gdspath = None
         gdsfilename = None
 
+    # Schematic-captured netlist
+    if 'netlist' in paths:
+        schem_netlist_path = os.path.join(paths['netlist'], 'schematic')
+        schem_netlist = os.path.join(schem_netlist_path, netlistname)
+    else:
+        schem_netlist_path = None
+        schem_netlist = None
+
     if pex == True:
         nettype = 'pex'
     else:
         nettype = 'layout'
 
     # Layout-extracted netlist for LVS
     if 'netlist' in paths:
@@ -652,22 +670,24 @@
             lvs_netlist, valid_layoutpath, debug
         )
 
     if need_lvs_extract:
         print('Forcing regeneration of layout-extracted netlist.')
 
         # Layout LVS netlist needs regenerating.  Check for magic layout.
-        if not magicfilename or not os.path.isfile(magicfilename):
-            print('Error:  No netlist or layout for project ' + dname + '.')
+        if (not magicfilename or not os.path.isfile(magicfilename)) and (
+            not gdsfilename or not os.path.isfile(gdsfilename)
+        ):
+            print(
+                f'Error:  No netlist or layout for project {dname}. ', end=''
+            )
             if magicfilename:
-                print(
-                    '(layout master file ' + magicfilename + ' not found.)\n'
-                )
+                print(f'(layout master file {magicfilename} not found.)')
             else:
-                print('(layout master file ' + gdsfilename + ' not found.)\n')
+                print(f'(layout master file {gdsfilename} not found.)')
             return False
 
         # Check for LVS netlist directory
         if not os.path.exists(lvs_netlist_path):
             os.makedirs(lvs_netlist_path)
 
         if 'PDK_ROOT' in dsheet:
@@ -701,19 +721,21 @@
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             cwd=root_path,
             env=newenv,
             universal_newlines=True,
         )
-        if magicfilename:
+        if magicfilename and os.path.isfile(magicfilename):
             mproc.stdin.write('load ' + magicfilename + '\n')
         else:
             mproc.stdin.write('gds read ' + gdsfilename + '\n')
             mproc.stdin.write('load ' + dname + '\n')
+            # Use readspice to get the port order
+            mproc.stdin.write('readspice ' + schem_netlist + '\n')
         mproc.stdin.write('select top cell\n')
         mproc.stdin.write('expand\n')
         mproc.stdin.write('extract path cace_extfiles\n')
         mproc.stdin.write('extract all\n')
         mproc.stdin.write('ext2spice lvs\n')
         if pex == True:
             mproc.stdin.write('ext2spice cthresh 0.01\n')
```

### Comparing `cace-2.2.6/cace/common/cace_simulate.py` & `cace-2.2.7/cace/common/cace_simulate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_unused.txt` & `cace-2.2.7/cace/common/cace_unused.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/cace_write.py` & `cace-2.2.7/cace/common/cace_write.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/electrical_parameter.py` & `cace-2.2.7/cace/common/electrical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/layout_estimate.py` & `cace-2.2.7/cace/common/layout_estimate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/netlist_precheck.py` & `cace-2.2.7/cace/common/netlist_precheck.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/physical_parameter.py` & `cace-2.2.7/cace/common/physical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/safe_eval.py` & `cace-2.2.7/cace/common/safe_eval.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/simulation_job.py` & `cace-2.2.7/cace/common/simulation_job.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/simulation_manager.py` & `cace-2.2.7/cace/common/simulation_manager.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/common/spiceunits.py` & `cace-2.2.7/cace/common/spiceunits.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/consoletext.py` & `cace-2.2.7/cace/gui/consoletext.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/editparam.py` & `cace-2.2.7/cace/gui/editparam.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/failreport.py` & `cace-2.2.7/cace/gui/failreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/helpwindow.py` & `cace-2.2.7/cace/gui/helpwindow.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/rowwidget.py` & `cace-2.2.7/cace/gui/rowwidget.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/settings.py` & `cace-2.2.7/cace/gui/settings.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/simhints.py` & `cace-2.2.7/cace/gui/simhints.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/style.py` & `cace-2.2.7/cace/gui/style.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/textreport.py` & `cace-2.2.7/cace/gui/textreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/tksimpledialog.py` & `cace-2.2.7/cace/gui/tksimpledialog.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace/gui/tooltip.py` & `cace-2.2.7/cace/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/cace.egg-info/PKG-INFO` & `cace-2.2.7/cace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.6
+Version: 2.2.7
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.6 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.7 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.6/cace.egg-info/SOURCES.txt` & `cace-2.2.7/cace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/default.nix` & `cace-2.2.7/default.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/Makefile` & `cace-2.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/make.bat` & `cace-2.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/_static/cace_screenshot.png` & `cace-2.2.7/docs/source/_static/cace_screenshot.png`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/characterization.md` & `cace-2.2.7/docs/source/characterization.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/conf.py` & `cace-2.2.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/formats/format_description.md` & `cace-2.2.7/docs/source/formats/format_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/formats/schematic_description.md` & `cace-2.2.7/docs/source/formats/schematic_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/index.md` & `cace-2.2.7/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/usage/cace_cli.md` & `cace-2.2.7/docs/source/usage/cace_cli.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/usage/cace_gui.md` & `cace-2.2.7/docs/source/usage/cace_gui.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/docs/source/usage/getting_started.md` & `cace-2.2.7/docs/source/usage/getting_started.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/flake.lock` & `cace-2.2.7/flake.lock`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/flake.nix` & `cace-2.2.7/flake.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/nix/colab-env.nix` & `cace-2.2.7/cace/__version__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,17 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-{
-  system,
-  cace,
-  python3,
-  symlinkJoin,
-}:
-symlinkJoin {
-  name = "cace-colab-env";
-  paths = cace.includedTools;
-}
+__version__ = '2.2.7'
+
+if __name__ == '__main__':
+    print(__version__, end='')
```

### Comparing `cace-2.2.6/nix/create-shell.nix` & `cace-2.2.7/nix/create-shell.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/nix/docker.nix` & `cace-2.2.7/nix/docker.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.6/pyproject.toml` & `cace-2.2.7/pyproject.toml`

 * *Files identical despite different names*

