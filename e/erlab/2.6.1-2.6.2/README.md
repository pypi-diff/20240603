# Comparing `tmp/erlab-2.6.1.tar.gz` & `tmp/erlab-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.6.1.tar", last modified: Thu May 30 18:00:17 2024, max compression
+gzip compressed data, was "erlab-2.6.2.tar", last modified: Mon Jun  3 01:25:56 2024, max compression
```

## Comparing `erlab-2.6.1.tar` & `erlab-2.6.2.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.658880 erlab-2.6.1/
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-30 18:00:07.000000 erlab-2.6.1/.codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.606880 erlab-2.6.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.610880 erlab-2.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2200 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.610880 erlab-2.6.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     2508 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-30 18:00:07.000000 erlab-2.6.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1022 2024-05-30 18:00:07.000000 erlab-2.6.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-05-30 18:00:07.000000 erlab-2.6.1/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   133751 2024-05-30 18:00:13.000000 erlab-2.6.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-05-30 18:00:07.000000 erlab-2.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48973 2024-05-30 18:00:17.658880 erlab-2.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-05-30 18:00:07.000000 erlab-2.6.1/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5552 2024-05-30 18:00:07.000000 erlab-2.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.614880 erlab-2.6.1/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.618880 erlab-2.6.1/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    18220 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15203 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)       94 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.utils.rst
--rw-r--r--   0 root         (0) root         (0)     5039 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.622880 erlab-2.6.1/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)  1014848 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   986936 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.626880 erlab-2.6.1/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2604 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1499 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.626880 erlab-2.6.1/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    42487 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2790 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1295 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)    13061 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    54813 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)    10710 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    27572 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-30 18:00:07.000000 erlab-2.6.1/environment.yml
--rw-r--r--   0 root         (0) root         (0)     5938 2024-05-30 18:00:07.000000 erlab-2.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-30 18:00:07.000000 erlab-2.6.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 18:00:17.658880 erlab-2.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.606880 erlab-2.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.626880 erlab-2.6.1/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-30 18:00:13.000000 erlab-2.6.1/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.630880 erlab-2.6.1/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26568 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    30007 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)    16387 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.630880 erlab-2.6.1/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      592 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5322 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.630880 erlab-2.6.1/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.634880 erlab-2.6.1/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10779 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9594 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12774 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20221 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    27488 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    14968 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.634880 erlab-2.6.1/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     8795 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8505 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/utilities.py
--rw-r--r--   0 root         (0) root         (0)     5435 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.634880 erlab-2.6.1/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      721 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14177 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21371 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    23034 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11812 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19370 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    17431 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52053 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114637 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    29113 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    58013 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    14551 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    26142 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16010 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19321 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     2745 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)      257 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/utilities.py
--rw-r--r--   0 root         (0) root         (0)    57036 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2186 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.642880 erlab-2.6.1/src/erlab/io/characterization/
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)    45761 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12460 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6998 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.642880 erlab-2.6.1/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1134 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     6985 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/maestro.py
--rw-r--r--   0 root         (0) root         (0)     8373 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7647 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     7123 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/utils.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/lattice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.642880 erlab-2.6.1/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.646880 erlab-2.6.1/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2113 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30848 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18686 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4420 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    39811 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    38592 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.646880 erlab-2.6.1/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.646880 erlab-2.6.1/src/erlab/utils/
--rw-r--r--   0 root         (0) root         (0)      177 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3754 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/utils/array.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/utils/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.654880 erlab-2.6.1/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48973 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5458 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      667 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-30 18:00:07.000000 erlab-2.6.1/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-30 18:00:07.000000 erlab-2.6.1/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-30 18:00:07.000000 erlab-2.6.1/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4150 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/analysis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)     4497 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_minuit.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_models.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_gold.py
--rw-r--r--   0 root         (0) root         (0)     5791 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     3909 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_image_savgol.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)     2989 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_mask.py
--rw-r--r--   0 root         (0) root         (0)      714 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/interactive/
--rw-r--r--   0 root         (0) root         (0)     4375 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/interactive/test_imagetool.py
--rw-r--r--   0 root         (0) root         (0)     4352 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/interactive/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.654880 erlab-2.6.1/tests/io/
--rw-r--r--   0 root         (0) root         (0)    10028 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/io/test_dataloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.654880 erlab-2.6.1/tests/plotting/
--rw-r--r--   0 root         (0) root         (0)     1305 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_annotations.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_atoms.py
--rw-r--r--   0 root         (0) root         (0)     2015 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_colors.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_general.py
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/test_constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.289551 erlab-2.6.2/
+-rw-r--r--   0 root         (0) root         (0)       74 2024-06-03 01:25:46.000000 erlab-2.6.2/.codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.237551 erlab-2.6.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.245550 erlab-2.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-06-03 01:25:46.000000 erlab-2.6.2/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-06-03 01:25:46.000000 erlab-2.6.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-06-03 01:25:46.000000 erlab-2.6.2/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.245550 erlab-2.6.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-06-03 01:25:46.000000 erlab-2.6.2/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-06-03 01:25:46.000000 erlab-2.6.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-06-03 01:25:46.000000 erlab-2.6.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-06-03 01:25:46.000000 erlab-2.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-06-03 01:25:46.000000 erlab-2.6.2/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   133949 2024-06-03 01:25:52.000000 erlab-2.6.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-06-03 01:25:46.000000 erlab-2.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48973 2024-06-03 01:25:56.289551 erlab-2.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-06-03 01:25:46.000000 erlab-2.6.2/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5552 2024-06-03 01:25:46.000000 erlab-2.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.245550 erlab-2.6.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      726 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       65 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.249551 erlab-2.6.2/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    18220 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15203 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)       94 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/erlab.utils.rst
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.257551 erlab-2.6.2/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)  1014848 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   986936 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.257551 erlab-2.6.2/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.257551 erlab-2.6.2/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    42487 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)    13061 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54813 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    27572 2024-06-03 01:25:46.000000 erlab-2.6.2/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      455 2024-06-03 01:25:46.000000 erlab-2.6.2/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     5938 2024-06-03 01:25:46.000000 erlab-2.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      299 2024-06-03 01:25:46.000000 erlab-2.6.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 01:25:56.289551 erlab-2.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.237551 erlab-2.6.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.257551 erlab-2.6.2/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-06-03 01:25:52.000000 erlab-2.6.2/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.261551 erlab-2.6.2/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26568 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    30007 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    16387 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.261551 erlab-2.6.2/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      592 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.265551 erlab-2.6.2/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.265551 erlab-2.6.2/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12774 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20221 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    27488 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    14968 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.265551 erlab-2.6.2/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     8795 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     5435 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/analysis/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.265551 erlab-2.6.2/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.269551 erlab-2.6.2/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      721 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21371 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23034 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19370 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.269551 erlab-2.6.2/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    17431 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.269551 erlab-2.6.2/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52053 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114637 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    29220 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    58013 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    26142 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16010 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19321 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2745 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)      257 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/utilities.py
+-rw-r--r--   0 root         (0) root         (0)    57036 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/interactive/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.273551 erlab-2.6.2/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.273551 erlab-2.6.2/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    45761 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12460 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.273551 erlab-2.6.2/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     6985 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/plugins/maestro.py
+-rw-r--r--   0 root         (0) root         (0)     8373 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7647 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     7123 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/io/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/lattice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.277551 erlab-2.6.2/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.277551 erlab-2.6.2/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30848 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18686 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39811 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    38592 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.277551 erlab-2.6.2/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.277551 erlab-2.6.2/src/erlab/utils/
+-rw-r--r--   0 root         (0) root         (0)      177 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/utils/array.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-06-03 01:25:46.000000 erlab-2.6.2/src/erlab/utils/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.285551 erlab-2.6.2/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48973 2024-06-03 01:25:56.000000 erlab-2.6.2/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5458 2024-06-03 01:25:56.000000 erlab-2.6.2/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 01:25:56.000000 erlab-2.6.2/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      667 2024-06-03 01:25:56.000000 erlab-2.6.2/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-06-03 01:25:56.000000 erlab-2.6.2/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.281551 erlab-2.6.2/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-06-03 01:25:46.000000 erlab-2.6.2/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-06-03 01:25:46.000000 erlab-2.6.2/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-06-03 01:25:46.000000 erlab-2.6.2/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.281551 erlab-2.6.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.281551 erlab-2.6.2/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.281551 erlab-2.6.2/tests/analysis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.281551 erlab-2.6.2/tests/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/fit/test_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/fit/test_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/fit/test_minuit.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/fit/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_gold.py
+-rw-r--r--   0 root         (0) root         (0)     5791 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_image_savgol.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_mask.py
+-rw-r--r--   0 root         (0) root         (0)      714 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/analysis/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.281551 erlab-2.6.2/tests/interactive/
+-rw-r--r--   0 root         (0) root         (0)     4375 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/interactive/test_imagetool.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/interactive/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.285551 erlab-2.6.2/tests/io/
+-rw-r--r--   0 root         (0) root         (0)    10028 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 01:25:56.285551 erlab-2.6.2/tests/plotting/
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/plotting/test_annotations.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/plotting/test_atoms.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/plotting/test_colors.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/plotting/test_general.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-06-03 01:25:46.000000 erlab-2.6.2/tests/test_constants.py
```

### Comparing `erlab-2.6.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.6.2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.6.2/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/.github/workflows/pr.yml` & `erlab-2.6.2/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/.github/workflows/release.yml` & `erlab-2.6.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/.gitignore` & `erlab-2.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/.pre-commit-config.yaml` & `erlab-2.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/.readthedocs.yaml` & `erlab-2.6.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/CHANGELOG.md` & `erlab-2.6.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v2.6.2 (2024-06-03)
+
+### Fix
+
+* (**interactive.imagetool**) fix regression with nonuniform data ([`67df972`](https://github.com/kmnhan/erlabpy/commit/67df9720193611816e2a562ce71d080fccbbec5e))
+
+
 ## v2.6.1 (2024-05-30)
 
 ### Fix
 
 * re-trigger due to CI failure ([`b6d69b5`](https://github.com/kmnhan/erlabpy/commit/b6d69b556e3d0dbe6d8d71596e32d9d7cfdc5267))
```

### Comparing `erlab-2.6.1/LICENSE` & `erlab-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/PKG-INFO` & `erlab-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.6.1
+Version: 2.6.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.6.1/PythonInterface.ipf` & `erlab-2.6.2/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/README.md` & `erlab-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/Makefile` & `erlab-2.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/environment.yml` & `erlab-2.6.2/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/make.bat` & `erlab-2.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/conf.py` & `erlab-2.6.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/contributing.rst` & `erlab-2.6.2/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/getting-started.rst` & `erlab-2.6.2/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/flowchart_multiple.pdf` & `erlab-2.6.2/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/flowchart_single.pdf` & `erlab-2.6.2/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/imagetool_dark.png` & `erlab-2.6.2/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/imagetool_light.png` & `erlab-2.6.2/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/ktool_1_dark.png` & `erlab-2.6.2/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/ktool_1_light.png` & `erlab-2.6.2/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/ktool_2_dark.png` & `erlab-2.6.2/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/images/ktool_2_light.png` & `erlab-2.6.2/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/index.rst` & `erlab-2.6.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/pyplots/norms.py` & `erlab-2.6.2/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/reference.rst` & `erlab-2.6.2/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/refs.bib` & `erlab-2.6.2/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.6.2/docs/source/user-guide/curve-fitting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/user-guide/imagetool.rst` & `erlab-2.6.2/docs/source/user-guide/imagetool.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/user-guide/index.rst` & `erlab-2.6.2/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/user-guide/indexing.ipynb` & `erlab-2.6.2/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/user-guide/io.ipynb` & `erlab-2.6.2/docs/source/user-guide/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/user-guide/kconv.ipynb` & `erlab-2.6.2/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/docs/source/user-guide/plotting.ipynb` & `erlab-2.6.2/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/pyproject.toml` & `erlab-2.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/accessors/__init__.py` & `erlab-2.6.2/src/erlab/accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/accessors/fit.py` & `erlab-2.6.2/src/erlab/accessors/fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/accessors/kspace.py` & `erlab-2.6.2/src/erlab/accessors/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/accessors/utils.py` & `erlab-2.6.2/src/erlab/accessors/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/__init__.py` & `erlab-2.6.2/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/correlation.py` & `erlab-2.6.2/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.6.2/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.6.2/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/fit/functions/general.py` & `erlab-2.6.2/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/fit/minuit.py` & `erlab-2.6.2/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/fit/models.py` & `erlab-2.6.2/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/fit/spline.py` & `erlab-2.6.2/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/gold.py` & `erlab-2.6.2/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/image.py` & `erlab-2.6.2/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/interpolate.py` & `erlab-2.6.2/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/kspace.py` & `erlab-2.6.2/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/mask/__init__.py` & `erlab-2.6.2/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/mask/polygon.py` & `erlab-2.6.2/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/transform.py` & `erlab-2.6.2/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/analysis/utils.py` & `erlab-2.6.2/src/erlab/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/constants.py` & `erlab-2.6.2/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/__init__.py` & `erlab-2.6.2/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/bzplot.py` & `erlab-2.6.2/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/colors.py` & `erlab-2.6.2/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/curvefittingtool.py` & `erlab-2.6.2/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/derivative.py` & `erlab-2.6.2/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/dtool.ui` & `erlab-2.6.2/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/fermiedge.py` & `erlab-2.6.2/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.6.2/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.6.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.6.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/imagetool/controls.py` & `erlab-2.6.2/src/erlab/interactive/imagetool/controls.py`

 * *Files 0% similar despite different names*

```diff
@@ -773,13 +773,16 @@
         bin_values = self.array_slicer.get_bin_values(self.current_cursor)
 
         for i in range(self.data.ndim):
             self.spins[i].blockSignals(True)
             self.labels[i].setText(f"{self.data.dims[i]!s}")
             self.spins[i].setRange(1, self.data.shape[i] - 1)
             self.spins[i].setValue(bin_numbers[i])
-            self.val_labels[i].setText(f"{bin_values[i]:.3g}")
+            if bin_values[i] is None:
+                self.val_labels[i].setText("")
+            else:
+                self.val_labels[i].setText(f"{bin_values[i]:.3g}")
             self.spins[i].blockSignals(False)
 
     def reset(self):
         for spin in self.spins:
             spin.setValue(1)
```

### Comparing `erlab-2.6.1/src/erlab/interactive/imagetool/core.py` & `erlab-2.6.2/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.6.2/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.6.2/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/kspace.py` & `erlab-2.6.2/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/ktool.ui` & `erlab-2.6.2/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/masktool.py` & `erlab-2.6.2/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/interactive/utils.py` & `erlab-2.6.2/src/erlab/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/__init__.py` & `erlab-2.6.2/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/characterization/resistance.py` & `erlab-2.6.2/src/erlab/io/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/characterization/xrd.py` & `erlab-2.6.2/src/erlab/io/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/dataloader.py` & `erlab-2.6.2/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/exampledata.py` & `erlab-2.6.2/src/erlab/io/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/igor.py` & `erlab-2.6.2/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/plugins/__init__.py` & `erlab-2.6.2/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/plugins/da30.py` & `erlab-2.6.2/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/plugins/kriss.py` & `erlab-2.6.2/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/plugins/maestro.py` & `erlab-2.6.2/src/erlab/io/plugins/maestro.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/plugins/merlin.py` & `erlab-2.6.2/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/plugins/ssrl52.py` & `erlab-2.6.2/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/io/utils.py` & `erlab-2.6.2/src/erlab/io/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/lattice.py` & `erlab-2.6.2/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.6.2/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.6.2/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/__init__.py` & `erlab-2.6.2/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/annotations.py` & `erlab-2.6.2/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/atoms.py` & `erlab-2.6.2/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/bz.py` & `erlab-2.6.2/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/colors.py` & `erlab-2.6.2/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/erplot.py` & `erlab-2.6.2/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/general.py` & `erlab-2.6.2/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/plot3d.py` & `erlab-2.6.2/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.6.2/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.6.2/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.6.2/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.6.2/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.6.2/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.6.2/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/utils/array.py` & `erlab-2.6.2/src/erlab/utils/array.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab/utils/parallel.py` & `erlab-2.6.2/src/erlab/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab.egg-info/PKG-INFO` & `erlab-2.6.2/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.6.1
+Version: 2.6.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.6.1/src/erlab.egg-info/SOURCES.txt` & `erlab-2.6.2/src/erlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/src/erlab.egg-info/requires.txt` & `erlab-2.6.2/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/templates/.macros.j2` & `erlab-2.6.2/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/accessors/test_fit.py` & `erlab-2.6.2/tests/accessors/test_fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/accessors/test_kspace.py` & `erlab-2.6.2/tests/accessors/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/fit/test_functions_dynamic.py` & `erlab-2.6.2/tests/analysis/fit/test_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/fit/test_functions_general.py` & `erlab-2.6.2/tests/analysis/fit/test_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/fit/test_minuit.py` & `erlab-2.6.2/tests/analysis/fit/test_minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/fit/test_models.py` & `erlab-2.6.2/tests/analysis/fit/test_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_fastbinning.py` & `erlab-2.6.2/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_gold.py` & `erlab-2.6.2/tests/analysis/test_gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_image.py` & `erlab-2.6.2/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_image_savgol.py` & `erlab-2.6.2/tests/analysis/test_image_savgol.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_interpolate.py` & `erlab-2.6.2/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_kspace.py` & `erlab-2.6.2/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_mask.py` & `erlab-2.6.2/tests/analysis/test_mask.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/analysis/test_utils.py` & `erlab-2.6.2/tests/analysis/test_utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/interactive/test_imagetool.py` & `erlab-2.6.2/tests/interactive/test_imagetool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/interactive/test_tools.py` & `erlab-2.6.2/tests/interactive/test_tools.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/io/test_dataloader.py` & `erlab-2.6.2/tests/io/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/plotting/test_annotations.py` & `erlab-2.6.2/tests/plotting/test_annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/plotting/test_atoms.py` & `erlab-2.6.2/tests/plotting/test_atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/plotting/test_colors.py` & `erlab-2.6.2/tests/plotting/test_colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.6.1/tests/plotting/test_general.py` & `erlab-2.6.2/tests/plotting/test_general.py`

 * *Files identical despite different names*

