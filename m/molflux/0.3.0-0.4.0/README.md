# Comparing `tmp/molflux-0.3.0.tar.gz` & `tmp/molflux-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molflux-0.3.0.tar", last modified: Tue Feb 13 09:41:59 2024, max compression
+gzip compressed data, was "molflux-0.4.0.tar", last modified: Mon Jun  3 14:45:14 2024, max compression
```

## Comparing `molflux-0.3.0.tar` & `molflux-0.4.0.tar`

### file list

```diff
@@ -1,936 +1,936 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.719073 molflux-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-02-13 09:41:24.000000 molflux-0.3.0/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.559073 molflux-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.583073 molflux-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/dev-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/docs-build-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/latest-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/main-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/pinned-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/publish-package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/quality-typing-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-13 09:41:24.000000 molflux-0.3.0/.github/workflows/release-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-13 09:41:24.000000 molflux-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-13 09:41:24.000000 molflux-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-13 09:41:24.000000 molflux-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-13 09:41:24.000000 molflux-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-02-13 09:41:59.719073 molflux-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-13 09:41:24.000000 molflux-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.583073 molflux-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.587073 molflux-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.587073 molflux-0.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name 2 colours.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name grey.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo mark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Grey-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Wh-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.587073 molflux-0.3.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/_templates/badges.html
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.587073 molflux-0.3.0/docs/source/pages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.587073 molflux-0.3.0/docs/source/pages/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/datasets/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/datasets/featurising.md
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/datasets/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/datasets/loading.md
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/datasets/saving.md
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/datasets/splitting.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.587073 molflux-0.3.0/docs/source/pages/features/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/features/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/features/how_to_add_reps.md
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/features/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.587073 molflux-0.3.0/docs/source/pages/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/metrics/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/metrics/how_to_add_metrics.md
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/metrics/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.591073 molflux-0.3.0/docs/source/pages/modelzoo/
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/modelzoo/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/modelzoo/how_to_add_models.md
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/modelzoo/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/modelzoo/uncertainty.md
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/philosophy.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.591073 molflux-0.3.0/docs/source/pages/production/
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/production/featurisation.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/production/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/production/models.md
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/production/tracking.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.591073 molflux-0.3.0/docs/source/pages/splits/
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/splits/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/splits/gallery.md
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/splits/how_to_add_splits.md
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/splits/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.591073 molflux-0.3.0/docs/source/pages/standard_api/
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/standard_api/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.595073 molflux-0.3.0/docs/source/pages/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/tutorials/esol_cls.md
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/tutorials/esol_reg.md
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/tutorials/esol_reg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/tutorials/esol_uncertainty.md
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/tutorials/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-02-13 09:41:24.000000 molflux-0.3.0/docs/source/pages/tutorials/qm9_reg_3d.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:41:24.000000 molflux-0.3.0/environment.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-02-13 09:41:24.000000 molflux-0.3.0/init_conda_venv.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-02-13 09:41:24.000000 molflux-0.3.0/init_python_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-02-13 09:41:24.000000 molflux-0.3.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.563073 molflux-0.3.0/pinned-versions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.595073 molflux-0.3.0/pinned-versions/3.10/
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.catboost.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.ensemble.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.lightning.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.mapie.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.pyod.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.pystan.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13243 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.sklearn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.10/lockfile.xgboost.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.599073 molflux-0.3.0/pinned-versions/3.11/
--rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.catboost.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.ensemble.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.lightning.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.mapie.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.pyod.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.pystan.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.sklearn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.11/lockfile.xgboost.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.599073 molflux-0.3.0/pinned-versions/3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.catboost.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.ensemble.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.lightning.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.mapie.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.pyod.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.pystan.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.sklearn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.8/lockfile.xgboost.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.603073 molflux-0.3.0/pinned-versions/3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.catboost.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.ensemble.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14201 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.lightning.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.mapie.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.pyod.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.pystan.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.sklearn.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-02-13 09:41:24.000000 molflux-0.3.0/pinned-versions/3.9/lockfile.xgboost.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24070 2024-02-13 09:41:24.000000 molflux-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 09:41:59.719073 molflux-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.563073 molflux-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.603073 molflux-0.3.0/src/molflux/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.603073 molflux-0.3.0/src/molflux/core/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.603073 molflux-0.3.0/src/molflux/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/featurisation/featurisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/featurisation/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/core/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.607073 molflux-0.3.0/src/molflux/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.607073 molflux-0.3.0/src/molflux/datasets/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.607073 molflux-0.3.0/src/molflux/datasets/builders/ani1x/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/ani1x/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/ani1x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/ani1x/ani1x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.607073 molflux-0.3.0/src/molflux/datasets/builders/ani2x/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/ani2x/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/ani2x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/ani2x/ani2x.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/ani2x/ani2x_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.611073 molflux-0.3.0/src/molflux/datasets/builders/esol/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/esol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/esol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/esol/esol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.611073 molflux-0.3.0/src/molflux/datasets/builders/gdb9/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/gdb9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/gdb9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/gdb9/gdb9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.611073 molflux-0.3.0/src/molflux/datasets/builders/pcqm4m_v2/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/pcqm4m_v2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/pcqm4m_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/pcqm4m_v2/pcqm4m_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.611073 molflux-0.3.0/src/molflux/datasets/builders/spice/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/spice/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/spice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/builders/spice/spice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/featurisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/filesystems.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    17270 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.611073 molflux-0.3.0/src/molflux/features/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.611073 molflux-0.3.0/src/molflux/features/representations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.615073 molflux-0.3.0/src/molflux/features/representations/core/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.615073 molflux-0.3.0/src/molflux/features/representations/core/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/core/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/core/generic/character_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/core/generic/exploded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.615073 molflux-0.3.0/src/molflux/features/representations/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.615073 molflux-0.3.0/src/molflux/features/representations/openeye/canonical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/canonical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/canonical/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/canonical/oemol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/canonical/smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.615073 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/aromatic_ring_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/molecular_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/net_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/num_acceptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/num_donors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/rotatable_bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/tpsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/x_log_p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.619073 molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/circular.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/lingo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/maccs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.619073 molflux-0.3.0/src/molflux/features/representations/openeye/sd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/sd/sd_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.619073 molflux-0.3.0/src/molflux/features/representations/openeye/shape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/shape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/openeye/shape/hermite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.619073 molflux-0.3.0/src/molflux/features/representations/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.619073 molflux-0.3.0/src/molflux/features/representations/rdkit/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/descriptors/rdkit_descriptors_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.623073 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/avalon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/layered.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/maccs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/mhfp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/mhfp_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/morgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/morgan_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/topological.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/toxicophores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.623073 molflux-0.3.0/src/molflux/features/representations/rdkit/reaction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/reaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/reaction/_drfp_vendored.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/representations/rdkit/reaction/drfp.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/features/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.623073 molflux-0.3.0/src/molflux/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.627073 molflux-0.3.0/src/molflux/metrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/balanced_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/diversity_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/top_k_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/top_k_accuracy_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/classification/validity_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.627073 molflux-0.3.0/src/molflux/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/max_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/proportion_within_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/regression/spearman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.627073 molflux-0.3.0/src/molflux/metrics/suites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/suites/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/suites/classification.yml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/suites/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/suites/regression.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/suites/uncertainty.yml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.631073 molflux-0.3.0/src/molflux/metrics/uncertainty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/coefficient_of_variation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/expected_calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/gaussian_nll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/prediction_interval_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/prediction_interval_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/uncertainty_based_rejection.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/metrics/uncertainty/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.631073 molflux-0.3.0/src/molflux/modelzoo/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.631073 molflux-0.3.0/src/molflux/modelzoo/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17922 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/catboost/catboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    22875 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/catboost/catboost_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/core/average_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/ensemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/ensemble/_combo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/ensemble/_combo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/ensemble/_combo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/ensemble/ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/ensemble/ensemble_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/callbacks/stock_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.635073 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/stock_optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.639073 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/stock_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.639073 molflux-0.3.0/src/molflux/modelzoo/models/mapie/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/mapie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/mapie/mapie_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.639073 molflux-0.3.0/src/molflux/modelzoo/models/pyod/
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/abod_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/cblof_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/hbos_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/isolation_forest_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/knn_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/mcd_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/ocsvm_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pyod/pca_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.639073 molflux-0.3.0/src/molflux/modelzoo/models/pystan/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pystan/BayesLinearRegressorHorseshoePrior.stan
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pystan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/pystan/sparse_linear_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.643073 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/bernoulli_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/corrected_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/coverage_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/dummy_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/extra_trees_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/extra_trees_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/kernel_ridge_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/knn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/knn_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/linear_discriminant_analysis_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/linear_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/logistic_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/mlp_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/mlp_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/pipeline_pilot_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/pls_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/random_forest_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/ridge_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.643073 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/bayes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.647073 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/support_vector_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/sklearn/support_vector_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.647073 molflux-0.3.0/src/molflux/modelzoo/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/xgboost/xgboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/models/xgboost/xgboost_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.647073 molflux-0.3.0/src/molflux/modelzoo/store/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/store/artefact.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/store/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/store/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/modelzoo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.647073 molflux-0.3.0/src/molflux/splits/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.647073 molflux-0.3.0/src/molflux/splits/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.651073 molflux-0.3.0/src/molflux/splits/strategies/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/_ordered_split_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/group_k_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/group_shuffle_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/k_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/leave_one_group_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/leave_p_groups_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/linear_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/ordered_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/shuffle_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/stratified_k_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/stratified_ordered_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/stratified_shuffle_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/core/time_series_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.651073 molflux-0.3.0/src/molflux/splits/strategies/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/openeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/openeye/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.651073 molflux-0.3.0/src/molflux/splits/strategies/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/rdkit/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategies/rdkit/tanimoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-13 09:41:24.000000 molflux-0.3.0/src/molflux/splits/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-13 09:41:59.000000 molflux-0.3.0/src/molflux/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.715073 molflux-0.3.0/src/molflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-02-13 09:41:59.000000 molflux-0.3.0/src/molflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36808 2024-02-13 09:41:59.000000 molflux-0.3.0/src/molflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:41:59.000000 molflux-0.3.0/src/molflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-02-13 09:41:59.000000 molflux-0.3.0/src/molflux.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-13 09:41:59.000000 molflux-0.3.0/src/molflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-13 09:41:59.000000 molflux-0.3.0/src/molflux.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.651073 molflux-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.651073 molflux-0.3.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.651073 molflux-0.3.0/tests/core/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.655073 molflux-0.3.0/tests/core/core/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/unit/test_featurisation.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/unit/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/unit/test_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/core/core/unit/test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.655073 molflux-0.3.0/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.655073 molflux-0.3.0/tests/datasets/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/assets/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/assets/config_with_bad_format.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/assets/config_with_bad_version.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/assets/minimal_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.655073 molflux-0.3.0/tests/datasets/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.655073 molflux-0.3.0/tests/datasets/core/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/integration/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/integration/test_splitting_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/core/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/core/unit/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/io/test_load_dataset_from_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    10956 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/io/test_save_dataset_to_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/core/unit/load/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/load/test_load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/load/test_load_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/load/test_load_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/load/test_load_from_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/load/test_load_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_featurise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_filesystems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_flatten_indices_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/core/unit/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.571073 molflux-0.3.0/tests/datasets/plugins/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/plugins/core/esol/
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/core/esol/test_esol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/plugins/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/mock_data/
--rw-r--r--   0 runner    (1001) docker     (127)    69936 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/mock_data/data.h5
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/test_ani1x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.659073 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/
--rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5
--rw-r--r--   0 runner    (1001) docker     (127)    23864 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/test_ani2x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/mock_data/
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/test_gdb9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.571073 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2/raw/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2/raw/data.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2-train.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/test_pcqm4m.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/spice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/spice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.663073 molflux-0.3.0/tests/datasets/plugins/openeye/spice/mock_data/
--rw-r--r--   0 runner    (1001) docker     (127)   229904 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/spice/mock_data/data.h5
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/spice/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/openeye/spice/test_spice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/mock_data/
--rw-r--r--   0 runner    (1001) docker     (127)    69936 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/mock_data/data.h5
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/test_ani1x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/
--rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5
--rw-r--r--   0 runner    (1001) docker     (127)    23864 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/test_ani2x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/mock_data/
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/test_gdb9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.667073 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.571073 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2/raw/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2/raw/data.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2-train.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/test_pcqm4m.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/datasets/plugins/rdkit/spice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/spice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/datasets/plugins/rdkit/spice/mock_data/
--rw-r--r--   0 runner    (1001) docker     (127)   229904 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/spice/mock_data/data.h5
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/spice/mock_data/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/datasets/plugins/rdkit/spice/test_spice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/features/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/assets/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/assets/minimal_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/features/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/features/core/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/integration/test_missing_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.671073 molflux-0.3.0/tests/features/core/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/core/unit/representation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/representation/test_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/core/unit/representations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/representations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/representations/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/test_featurise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/core/unit/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/plugins/core/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/core/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/core/generic/test_exploded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/plugins/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/plugins/openeye/canonical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/canonical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/canonical/test_oemol.py
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/canonical/test_smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.675073 molflux-0.3.0/tests/features/plugins/openeye/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_aromatic_ring_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_molecular_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_net_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_num_acceptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_num_donors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_rotatable_bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_tpsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_x_log_p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.679073 molflux-0.3.0/tests/features/plugins/openeye/fingerprints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/fingerprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_circular.py
--rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_lingo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_maccs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.679073 molflux-0.3.0/tests/features/plugins/openeye/sd/
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/sd/test_sd_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.679073 molflux-0.3.0/tests/features/plugins/openeye/shape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/shape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/shape/test_hermite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/openeye/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.679073 molflux-0.3.0/tests/features/plugins/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.679073 molflux-0.3.0/tests/features/plugins/rdkit/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/descriptors/test_rdkit_descriptors_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_avalon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_layered.py
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_maccs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_mhfp_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_morgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_morgan_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_topological.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion_unfolded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_toxicophores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/features/plugins/rdkit/reaction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/reaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/reaction/test_drfp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/features/plugins/rdkit/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/metrics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/assets/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/assets/minimal_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/metrics/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/metrics/core/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/metrics/core/unit/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/metric/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/metric/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/metric/test_uncertainty_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/metrics/core/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/metrics/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/core/unit/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.683073 molflux-0.3.0/tests/metrics/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.687073 molflux-0.3.0/tests/metrics/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.687073 molflux-0.3.0/tests/metrics/plugins/core/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_balanced_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_diversity_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_top_k_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_top_k_accuracy_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/classification/test_validity_roc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.691073 molflux-0.3.0/tests/metrics/plugins/core/regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_max_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_proportion_within_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/regression/test_spearman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.691073 molflux-0.3.0/tests/metrics/plugins/core/suites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/suites/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/suites/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/suites/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/suites/test_uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.691073 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_coefficient_of_variation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_expected_calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_gaussian_nll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_uncertainty_based_rejection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.691073 molflux-0.3.0/tests/modelzoo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.579073 molflux-0.3.0/tests/modelzoo/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.691073 molflux-0.3.0/tests/modelzoo/assets/core/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/core/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/core/minimal_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.579073 molflux-0.3.0/tests/modelzoo/assets/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.579073 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.691073 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/normalizer-k-neighbors.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/pca-select-k-svc.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/scaler-random-forest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/normalizer-kernel-ridge.json
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/pca-select-k-svr.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/scaler-random-forest.json
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/core/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/integration/test_missing_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/core/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/core/unit/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/model/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/model/test_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/core/unit/store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/store/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/store/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/test_interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/core/unit/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.695073 molflux-0.3.0/tests/modelzoo/plugins/catboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/catboost/test_cat_boost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/catboost/test_cat_boost_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.699073 molflux-0.3.0/tests/modelzoo/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/core/test_average_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.699073 molflux-0.3.0/tests/modelzoo/plugins/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/ensemble/test_combo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/ensemble/test_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/ensemble/test_ensemble_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.699073 molflux-0.3.0/tests/modelzoo/plugins/fortuna/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/fortuna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/fortuna/test_fortuna_mlp_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.699073 molflux-0.3.0/tests/modelzoo/plugins/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/lightning/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/lightning/test_mlp_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/lightning/test_model_checkpoint_apply_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/lightning/test_transfer_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.699073 molflux-0.3.0/tests/modelzoo/plugins/mapie/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/mapie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/mapie/test_mapie_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.703073 molflux-0.3.0/tests/modelzoo/plugins/pyod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_abod_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_cblof_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_hbos_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_isolation_forest_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_knn_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_mcd_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_ocsvm_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pyod/test_pca_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.703073 molflux-0.3.0/tests/modelzoo/plugins/pystan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pystan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/pystan/test_sparse_linear_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.707073 molflux-0.3.0/tests/modelzoo/plugins/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.707073 molflux-0.3.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/test_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_base_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_bernoulli_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_corrected_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_coverage_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_dummy_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_extra_trees_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_extra_trees_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_kernel_ridge_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_knn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_knn_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_linear_discriminant_analysis_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_linear_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_logistic_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_mlp_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_mlp_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_pipeline_pilot_nb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_pls_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_random_forest_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_ridge_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_support_vector_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_support_vector_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.707073 molflux-0.3.0/tests/modelzoo/plugins/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/xgboost/test_xg_boost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/modelzoo/plugins/xgboost/test_xg_boost_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.707073 molflux-0.3.0/tests/splits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.707073 molflux-0.3.0/tests/splits/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/assets/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/assets/minimal_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.707073 molflux-0.3.0/tests/splits/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.711073 molflux-0.3.0/tests/splits/core/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.711073 molflux-0.3.0/tests/splits/core/unit/presets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/presets/test_k_fold_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/presets/test_train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/presets/test_train_validation_test_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.711073 molflux-0.3.0/tests/splits/core/unit/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/strategy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/strategy/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/core/unit/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.711073 molflux-0.3.0/tests/splits/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.715073 molflux-0.3.0/tests/splits/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_group_k_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_group_shuffle_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_k_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_leave_one_group_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_leave_p_groups_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_linear_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_ordered_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_shuffle_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_stratified_k_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_stratified_ordered_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_stratified_shuffle_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/core/test_time_series_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.715073 molflux-0.3.0/tests/splits/plugins/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/openeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/openeye/test_scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:59.715073 molflux-0.3.0/tests/splits/plugins/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/rdkit/test_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-02-13 09:41:24.000000 molflux-0.3.0/tests/splits/plugins/rdkit/test_tanimoto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.667468 molflux-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-06-03 14:45:00.000000 molflux-0.4.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.511466 molflux-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.535466 molflux-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/dev-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/docs-build-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/latest-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/main-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/pinned-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/publish-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/quality-typing-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-03 14:45:00.000000 molflux-0.4.0/.github/workflows/release-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-06-03 14:45:00.000000 molflux-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-03 14:45:00.000000 molflux-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-06-03 14:45:00.000000 molflux-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 14:45:00.000000 molflux-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-06-03 14:45:14.667468 molflux-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-06-03 14:45:00.000000 molflux-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.535466 molflux-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.535466 molflux-0.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.535466 molflux-0.4.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name 2 colours.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name grey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo mark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Grey-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Wh-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.535466 molflux-0.4.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/_templates/badges.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.539466 molflux-0.4.0/docs/source/pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.539466 molflux-0.4.0/docs/source/pages/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/datasets/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/datasets/featurising.md
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/datasets/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/datasets/loading.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/datasets/saving.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/datasets/splitting.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.539466 molflux-0.4.0/docs/source/pages/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/features/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/features/how_to_add_reps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/features/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.539466 molflux-0.4.0/docs/source/pages/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/metrics/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/metrics/how_to_add_metrics.md
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/metrics/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.539466 molflux-0.4.0/docs/source/pages/modelzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/modelzoo/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/modelzoo/how_to_add_models.md
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/modelzoo/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/modelzoo/uncertainty.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/philosophy.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.539466 molflux-0.4.0/docs/source/pages/production/
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/production/featurisation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/production/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/production/models.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/production/tracking.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.543466 molflux-0.4.0/docs/source/pages/splits/
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/splits/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/splits/gallery.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/splits/how_to_add_splits.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/splits/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.543466 molflux-0.4.0/docs/source/pages/standard_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/standard_api/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.543466 molflux-0.4.0/docs/source/pages/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/tutorials/esol_cls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/tutorials/esol_reg.md
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/tutorials/esol_reg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/tutorials/esol_uncertainty.md
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/tutorials/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-06-03 14:45:00.000000 molflux-0.4.0/docs/source/pages/tutorials/qm9_reg_3d.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-03 14:45:00.000000 molflux-0.4.0/environment.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-06-03 14:45:00.000000 molflux-0.4.0/init_conda_venv.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-06-03 14:45:00.000000 molflux-0.4.0/init_python_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-06-03 14:45:00.000000 molflux-0.4.0/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.515466 molflux-0.4.0/pinned-versions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.547466 molflux-0.4.0/pinned-versions/3.10/
+-rw-r--r--   0 runner    (1001) docker     (127)    13001 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.catboost.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13001 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.ensemble.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13851 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.mapie.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13347 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.pyod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.pystan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13000 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.sklearn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13082 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.10/lockfile.xgboost.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.547466 molflux-0.4.0/pinned-versions/3.11/
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.catboost.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.ensemble.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13641 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12788 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.mapie.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13137 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.pyod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.pystan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.sklearn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.11/lockfile.xgboost.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.551466 molflux-0.4.0/pinned-versions/3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.catboost.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.ensemble.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.mapie.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.pyod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.pystan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.sklearn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.8/lockfile.xgboost.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.551466 molflux-0.4.0/pinned-versions/3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.catboost.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.ensemble.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13989 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.mapie.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.pyod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.pystan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.sklearn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-06-03 14:45:00.000000 molflux-0.4.0/pinned-versions/3.9/lockfile.xgboost.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24070 2024-06-03 14:45:00.000000 molflux-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:45:14.667468 molflux-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.515466 molflux-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.551466 molflux-0.4.0/src/molflux/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.555466 molflux-0.4.0/src/molflux/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.555466 molflux-0.4.0/src/molflux/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/featurisation/featurisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/featurisation/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/core/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.559466 molflux-0.4.0/src/molflux/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.559466 molflux-0.4.0/src/molflux/datasets/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.559466 molflux-0.4.0/src/molflux/datasets/builders/ani1x/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/ani1x/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/ani1x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/ani1x/ani1x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.559466 molflux-0.4.0/src/molflux/datasets/builders/ani2x/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/ani2x/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/ani2x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/ani2x/ani2x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/ani2x/ani2x_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.559466 molflux-0.4.0/src/molflux/datasets/builders/esol/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/esol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/esol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/esol/esol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.559466 molflux-0.4.0/src/molflux/datasets/builders/gdb9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/gdb9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/gdb9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/gdb9/gdb9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.559466 molflux-0.4.0/src/molflux/datasets/builders/pcqm4m_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/pcqm4m_v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/pcqm4m_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/pcqm4m_v2/pcqm4m_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.563466 molflux-0.4.0/src/molflux/datasets/builders/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/spice/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/spice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/builders/spice/spice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/featurisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17270 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.563466 molflux-0.4.0/src/molflux/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.563466 molflux-0.4.0/src/molflux/features/representations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.563466 molflux-0.4.0/src/molflux/features/representations/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.563466 molflux-0.4.0/src/molflux/features/representations/core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/core/generic/character_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/core/generic/exploded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.563466 molflux-0.4.0/src/molflux/features/representations/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.567467 molflux-0.4.0/src/molflux/features/representations/openeye/canonical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/canonical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/canonical/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/canonical/oemol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/canonical/smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.567467 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/aromatic_ring_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/molecular_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/net_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/num_acceptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/num_donors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/rotatable_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/tpsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/x_log_p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.567467 molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/lingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/maccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.567467 molflux-0.4.0/src/molflux/features/representations/openeye/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/sd/sd_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.567467 molflux-0.4.0/src/molflux/features/representations/openeye/shape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/shape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/openeye/shape/hermite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.567467 molflux-0.4.0/src/molflux/features/representations/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.571467 molflux-0.4.0/src/molflux/features/representations/rdkit/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/descriptors/rdkit_descriptors_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.571467 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/avalon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/layered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/maccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/mhfp_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/morgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/morgan_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/topological.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/toxicophores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.571467 molflux-0.4.0/src/molflux/features/representations/rdkit/reaction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/reaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/reaction/_drfp_vendored.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/representations/rdkit/reaction/drfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/features/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.575467 molflux-0.4.0/src/molflux/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.575467 molflux-0.4.0/src/molflux/metrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/balanced_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/diversity_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/top_k_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/top_k_accuracy_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/classification/validity_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.579467 molflux-0.4.0/src/molflux/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/max_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/proportion_within_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/regression/spearman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.579467 molflux-0.4.0/src/molflux/metrics/suites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/suites/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/suites/classification.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/suites/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/suites/regression.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/suites/uncertainty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.579467 molflux-0.4.0/src/molflux/metrics/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/coefficient_of_variation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/expected_calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/gaussian_nll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/prediction_interval_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/prediction_interval_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/uncertainty_based_rejection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/metrics/uncertainty/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.583467 molflux-0.4.0/src/molflux/modelzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.583467 molflux-0.4.0/src/molflux/modelzoo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.583467 molflux-0.4.0/src/molflux/modelzoo/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17922 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/catboost/catboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22875 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/catboost/catboost_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.583467 molflux-0.4.0/src/molflux/modelzoo/models/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/core/average_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.583467 molflux-0.4.0/src/molflux/modelzoo/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/ensemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.583467 molflux-0.4.0/src/molflux/modelzoo/models/ensemble/_combo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/ensemble/_combo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/ensemble/_combo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/ensemble/ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/ensemble/ensemble_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.587467 molflux-0.4.0/src/molflux/modelzoo/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.587467 molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.587467 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.587467 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/callbacks/stock_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.587467 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/stock_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.587467 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/stock_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.587467 molflux-0.4.0/src/molflux/modelzoo/models/mapie/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/mapie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/mapie/mapie_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.591467 molflux-0.4.0/src/molflux/modelzoo/models/pyod/
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/abod_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/cblof_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/hbos_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/isolation_forest_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/knn_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/mcd_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/ocsvm_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pyod/pca_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.591467 molflux-0.4.0/src/molflux/modelzoo/models/pystan/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pystan/BayesLinearRegressorHorseshoePrior.stan
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pystan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/pystan/sparse_linear_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.595467 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/bernoulli_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/corrected_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/coverage_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/dummy_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/extra_trees_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/extra_trees_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/kernel_ridge_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/knn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/knn_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/linear_discriminant_analysis_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/linear_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/logistic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/mlp_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/mlp_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/pipeline_pilot_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/pls_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/random_forest_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/ridge_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.595467 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/bayes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.595467 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/support_vector_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/sklearn/support_vector_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.595467 molflux-0.4.0/src/molflux/modelzoo/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/xgboost/xgboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/models/xgboost/xgboost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.599467 molflux-0.4.0/src/molflux/modelzoo/store/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/store/artefact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/store/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/store/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/modelzoo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.599467 molflux-0.4.0/src/molflux/splits/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.599467 molflux-0.4.0/src/molflux/splits/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.603467 molflux-0.4.0/src/molflux/splits/strategies/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/_ordered_split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/group_k_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/group_shuffle_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/k_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/leave_one_group_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/leave_p_groups_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/linear_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/ordered_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/shuffle_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/stratified_k_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/stratified_ordered_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/stratified_shuffle_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/core/time_series_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.603467 molflux-0.4.0/src/molflux/splits/strategies/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/openeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/openeye/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.603467 molflux-0.4.0/src/molflux/splits/strategies/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/rdkit/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategies/rdkit/tanimoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-03 14:45:00.000000 molflux-0.4.0/src/molflux/splits/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 14:45:14.000000 molflux-0.4.0/src/molflux/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.663468 molflux-0.4.0/src/molflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-06-03 14:45:14.000000 molflux-0.4.0/src/molflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36808 2024-06-03 14:45:14.000000 molflux-0.4.0/src/molflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:45:14.000000 molflux-0.4.0/src/molflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-06-03 14:45:14.000000 molflux-0.4.0/src/molflux.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-03 14:45:14.000000 molflux-0.4.0/src/molflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 14:45:14.000000 molflux-0.4.0/src/molflux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.603467 molflux-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.603467 molflux-0.4.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.603467 molflux-0.4.0/tests/core/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.603467 molflux-0.4.0/tests/core/core/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/unit/test_featurisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/unit/test_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/core/core/unit/test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.607467 molflux-0.4.0/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.607467 molflux-0.4.0/tests/datasets/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/assets/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/assets/config_with_bad_format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/assets/config_with_bad_version.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/assets/minimal_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.607467 molflux-0.4.0/tests/datasets/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.607467 molflux-0.4.0/tests/datasets/core/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/integration/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/integration/test_splitting_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.607467 molflux-0.4.0/tests/datasets/core/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/core/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/io/test_load_dataset_from_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10956 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/io/test_save_dataset_to_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/core/unit/load/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/load/test_load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/load/test_load_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/load/test_load_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/load/test_load_from_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/load/test_load_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_featurise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_flatten_indices_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/core/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.523466 molflux-0.4.0/tests/datasets/plugins/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/core/esol/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/core/esol/test_esol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/mock_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    69936 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/mock_data/data.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/test_ani1x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.611467 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/
+-rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    23864 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/test_ani2x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/mock_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/test_gdb9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.523466 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2/raw/data.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2-train.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/test_pcqm4m.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/openeye/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/spice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/openeye/spice/mock_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   229904 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/spice/mock_data/data.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/spice/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/openeye/spice/test_spice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.615467 molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/mock_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    69936 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/mock_data/data.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/test_ani1x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/
+-rw-r--r--   0 runner    (1001) docker     (127)    18576 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    23864 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/test_ani2x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/mock_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/test_gdb9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.523466 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2/raw/data.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2-train.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/test_pcqm4m.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.619467 molflux-0.4.0/tests/datasets/plugins/rdkit/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/spice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/datasets/plugins/rdkit/spice/mock_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   229904 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/spice/mock_data/data.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/spice/mock_data/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/datasets/plugins/rdkit/spice/test_spice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/assets/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/assets/minimal_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/core/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/integration/test_missing_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/core/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/core/unit/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/representation/test_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/core/unit/representations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/representations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/representations/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/test_featurise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/core/unit/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.623467 molflux-0.4.0/tests/features/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.627467 molflux-0.4.0/tests/features/plugins/core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/core/generic/test_exploded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.627467 molflux-0.4.0/tests/features/plugins/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.627467 molflux-0.4.0/tests/features/plugins/openeye/canonical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/canonical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/canonical/test_oemol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/canonical/test_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.627467 molflux-0.4.0/tests/features/plugins/openeye/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_aromatic_ring_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_molecular_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_net_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_num_acceptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_num_donors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_rotatable_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_tpsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_x_log_p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.627467 molflux-0.4.0/tests/features/plugins/openeye/fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/fingerprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_lingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_maccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.627467 molflux-0.4.0/tests/features/plugins/openeye/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/sd/test_sd_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.631467 molflux-0.4.0/tests/features/plugins/openeye/shape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/shape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/shape/test_hermite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/openeye/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.631467 molflux-0.4.0/tests/features/plugins/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.631467 molflux-0.4.0/tests/features/plugins/rdkit/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/descriptors/test_rdkit_descriptors_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.631467 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_avalon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_layered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_maccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_mhfp_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_morgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_morgan_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_topological.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion_unfolded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_toxicophores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.631467 molflux-0.4.0/tests/features/plugins/rdkit/reaction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/reaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/reaction/test_drfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/features/plugins/rdkit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.631467 molflux-0.4.0/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.635467 molflux-0.4.0/tests/metrics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/assets/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/assets/minimal_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.635467 molflux-0.4.0/tests/metrics/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.635467 molflux-0.4.0/tests/metrics/core/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.635467 molflux-0.4.0/tests/metrics/core/unit/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/metric/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/metric/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/metric/test_uncertainty_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.635467 molflux-0.4.0/tests/metrics/core/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/metrics/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/core/unit/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.635467 molflux-0.4.0/tests/metrics/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.635467 molflux-0.4.0/tests/metrics/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.639467 molflux-0.4.0/tests/metrics/plugins/core/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_balanced_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_diversity_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_top_k_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_top_k_accuracy_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/classification/test_validity_roc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.639467 molflux-0.4.0/tests/metrics/plugins/core/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_max_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_proportion_within_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/regression/test_spearman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.639467 molflux-0.4.0/tests/metrics/plugins/core/suites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/suites/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/suites/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/suites/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/suites/test_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.643468 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_coefficient_of_variation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_expected_calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_gaussian_nll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_uncertainty_based_rejection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.643468 molflux-0.4.0/tests/modelzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.527466 molflux-0.4.0/tests/modelzoo/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.643468 molflux-0.4.0/tests/modelzoo/assets/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/core/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/core/minimal_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.527466 molflux-0.4.0/tests/modelzoo/assets/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.527466 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.643468 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/normalizer-k-neighbors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/pca-select-k-svc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_classifier/scaler-random-forest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.643468 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/normalizer-kernel-ridge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/pca-select-k-svr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/assets/plugins/sklearn/sklearn_pipeline_regressor/scaler-random-forest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.643468 molflux-0.4.0/tests/modelzoo/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.643468 molflux-0.4.0/tests/modelzoo/core/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/integration/test_missing_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/core/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/core/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/model/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/model/test_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/core/unit/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/store/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/store/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/test_interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/core/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/plugins/catboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/catboost/test_cat_boost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/catboost/test_cat_boost_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/core/test_average_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/plugins/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/ensemble/test_combo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/ensemble/test_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/ensemble/test_ensemble_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.647467 molflux-0.4.0/tests/modelzoo/plugins/fortuna/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/fortuna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/fortuna/test_fortuna_mlp_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.651468 molflux-0.4.0/tests/modelzoo/plugins/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/lightning/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/lightning/test_mlp_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/lightning/test_model_checkpoint_apply_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/lightning/test_transfer_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.651468 molflux-0.4.0/tests/modelzoo/plugins/mapie/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/mapie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/mapie/test_mapie_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.651468 molflux-0.4.0/tests/modelzoo/plugins/pyod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_abod_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_cblof_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_hbos_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_isolation_forest_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_knn_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_mcd_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_ocsvm_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pyod/test_pca_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.651468 molflux-0.4.0/tests/modelzoo/plugins/pystan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pystan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/pystan/test_sparse_linear_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.655468 molflux-0.4.0/tests/modelzoo/plugins/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.655468 molflux-0.4.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/test_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_base_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_bernoulli_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_corrected_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_coverage_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_dummy_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_extra_trees_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_extra_trees_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_kernel_ridge_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_knn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_knn_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_linear_discriminant_analysis_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_linear_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_logistic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_mlp_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_mlp_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_pipeline_pilot_nb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_pls_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_random_forest_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_ridge_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_support_vector_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_support_vector_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.655468 molflux-0.4.0/tests/modelzoo/plugins/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/xgboost/test_xg_boost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/modelzoo/plugins/xgboost/test_xg_boost_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.655468 molflux-0.4.0/tests/splits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.659468 molflux-0.4.0/tests/splits/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/assets/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/assets/minimal_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.659468 molflux-0.4.0/tests/splits/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.659468 molflux-0.4.0/tests/splits/core/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.659468 molflux-0.4.0/tests/splits/core/unit/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/presets/test_k_fold_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/presets/test_train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/presets/test_train_validation_test_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.659468 molflux-0.4.0/tests/splits/core/unit/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/strategy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/strategy/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/core/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.659468 molflux-0.4.0/tests/splits/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.663468 molflux-0.4.0/tests/splits/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_group_k_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_group_shuffle_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_k_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_leave_one_group_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_leave_p_groups_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_linear_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_ordered_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_shuffle_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_stratified_k_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_stratified_ordered_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_stratified_shuffle_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/core/test_time_series_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.663468 molflux-0.4.0/tests/splits/plugins/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/openeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/openeye/test_scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:14.663468 molflux-0.4.0/tests/splits/plugins/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/rdkit/test_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-06-03 14:45:00.000000 molflux-0.4.0/tests/splits/plugins/rdkit/test_tanimoto.py
```

### Comparing `molflux-0.3.0/.envrc` & `molflux-0.4.0/.envrc`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/.github/workflows/docs-build-deploy.yaml` & `molflux-0.4.0/.github/workflows/docs-build-deploy.yaml`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/.github/workflows/latest-tests.yaml` & `molflux-0.4.0/.github/workflows/latest-tests.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 on:
   workflow_call:
   workflow_dispatch:
   schedule:
     - cron: 0 0 * * *
 
 jobs:
-  tests-pinned:
+  tests-latest:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: Checkout repo
         uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
-      - name: Run pinned tests
+      - name: Run latest tests
         run: |
           pip install nox
           nox -s tests_run_latest-${{ matrix.python-version }}
       - name: Test Summary
         uses: test-summary/action@v2
         with:
           paths: "test-reports/${{ matrix.python-version }}/.junitxml.*.xml"
```

### Comparing `molflux-0.3.0/.github/workflows/pinned-tests.yaml` & `molflux-0.4.0/.github/workflows/pinned-tests.yaml`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/.github/workflows/publish-package.yaml` & `molflux-0.4.0/.github/workflows/publish-package.yaml`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/.github/workflows/quality-typing-checks.yaml` & `molflux-0.4.0/.github/workflows/quality-typing-checks.yaml`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/.gitignore` & `molflux-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/.pre-commit-config.yaml` & `molflux-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/CHANGELOG.md` & `molflux-0.4.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project
 adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 ---------------------------------------------------------
 
 ## [Unreleased]
 
 ---------------------------------------------------------
+## [0.4.0] - 2024-06-03
+
+## Removed
+
+- Drop parameter `multi_class` and `n_jobs` for `logistic_regressor` in anticipation of `numpy>=1.7` removal
 
 ## [0.3.0] - 2024-02-09
 
 ## Changed
 
 - Upgraded `datasets>=2.17.0` which fixes a problem with flattening indices
 - Removed failure tests for flattening indices
```

### Comparing `molflux-0.3.0/LICENSE` & `molflux-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/PKG-INFO` & `molflux-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molflux
-Version: 0.3.0
+Version: 0.4.0
 Summary: A foundational package for molecular predictive modelling
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/molflux/issues
 Project-URL: repository, https://github.com/exscientia/molflux.git
 Project-URL: issue-tracker, https://github.com/exscientia/molflux/issues
 Project-URL: changelog, https://github.com/exscientia/molflux/src/main/CHANGELOG.md
@@ -154,15 +154,15 @@
 [MIT License](LICENSE)
 
 ## Acknowledgements
 
 The ``molflux`` package has been developed by researchers and engineers at Exscientia
 
 * Alan Bilsland
-* Julia Buhmann
-* Ward Haddadin
+* [Julia Buhmann](https://github.com/juliabuhmann)
+* [Ward Haddadin](https://github.com/wardhaddadin1)
 * Jonathan Harrison
 * Dom Miketa
 * Emil Nichita
 * Stefanie Speichert
 * Hagen Triendl
-* Alvise Vianello
+* [Alvise Vianello](https://github.com/amv213)
```

### Comparing `molflux-0.3.0/README.md` & `molflux-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 [MIT License](LICENSE)
 
 ## Acknowledgements
 
 The ``molflux`` package has been developed by researchers and engineers at Exscientia
 
 * Alan Bilsland
-* Julia Buhmann
-* Ward Haddadin
+* [Julia Buhmann](https://github.com/juliabuhmann)
+* [Ward Haddadin](https://github.com/wardhaddadin1)
 * Jonathan Harrison
 * Dom Miketa
 * Emil Nichita
 * Stefanie Speichert
 * Hagen Triendl
-* Alvise Vianello
+* [Alvise Vianello](https://github.com/amv213)
```

### Comparing `molflux-0.3.0/docs/Makefile` & `molflux-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/make.bat` & `molflux-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name 2 colours.svg` & `molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name 2 colours.svg`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name grey.svg` & `molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux Logo mark with name grey.svg`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo mark.svg` & `molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo mark.svg`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Grey-cropped.svg` & `molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Grey-cropped.svg`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Wh-cropped.svg` & `molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name Wh-cropped.svg`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name-cropped.svg` & `molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name-cropped.svg`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name.svg` & `molflux-0.4.0/docs/source/_static/MolFlux_logo_final_MolFlux logo name.svg`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/conf.py` & `molflux-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/index.md` & `molflux-0.4.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/datasets/basic_usage.md` & `molflux-0.4.0/docs/source/pages/datasets/basic_usage.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/datasets/featurising.md` & `molflux-0.4.0/docs/source/pages/datasets/featurising.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/datasets/intro.md` & `molflux-0.4.0/docs/source/pages/datasets/intro.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/datasets/loading.md` & `molflux-0.4.0/docs/source/pages/datasets/loading.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/datasets/saving.md` & `molflux-0.4.0/docs/source/pages/datasets/saving.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/datasets/splitting.md` & `molflux-0.4.0/docs/source/pages/datasets/splitting.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/features/basic_usage.md` & `molflux-0.4.0/docs/source/pages/features/basic_usage.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/features/how_to_add_reps.md` & `molflux-0.4.0/docs/source/pages/features/how_to_add_reps.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/features/intro.md` & `molflux-0.4.0/docs/source/pages/features/intro.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/metrics/basic_usage.md` & `molflux-0.4.0/docs/source/pages/metrics/basic_usage.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/metrics/how_to_add_metrics.md` & `molflux-0.4.0/docs/source/pages/metrics/how_to_add_metrics.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/metrics/intro.md` & `molflux-0.4.0/docs/source/pages/metrics/intro.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/modelzoo/basic_usage.md` & `molflux-0.4.0/docs/source/pages/modelzoo/basic_usage.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/modelzoo/how_to_add_models.md` & `molflux-0.4.0/docs/source/pages/modelzoo/how_to_add_models.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/modelzoo/intro.md` & `molflux-0.4.0/docs/source/pages/modelzoo/intro.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/modelzoo/uncertainty.md` & `molflux-0.4.0/docs/source/pages/modelzoo/uncertainty.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/philosophy.md` & `molflux-0.4.0/docs/source/pages/philosophy.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/production/featurisation.md` & `molflux-0.4.0/docs/source/pages/production/featurisation.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/production/models.md` & `molflux-0.4.0/docs/source/pages/production/models.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/production/tracking.md` & `molflux-0.4.0/docs/source/pages/production/tracking.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/splits/basic_usage.md` & `molflux-0.4.0/docs/source/pages/splits/basic_usage.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/splits/gallery.md` & `molflux-0.4.0/docs/source/pages/splits/gallery.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/splits/how_to_add_splits.md` & `molflux-0.4.0/docs/source/pages/splits/how_to_add_splits.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/splits/intro.md` & `molflux-0.4.0/docs/source/pages/splits/intro.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/standard_api/intro.md` & `molflux-0.4.0/docs/source/pages/standard_api/intro.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/tutorials/esol_cls.md` & `molflux-0.4.0/docs/source/pages/tutorials/esol_cls.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/tutorials/esol_reg.md` & `molflux-0.4.0/docs/source/pages/tutorials/esol_reg.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/tutorials/esol_reg.yaml` & `molflux-0.4.0/docs/source/pages/tutorials/esol_reg.yaml`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/tutorials/esol_uncertainty.md` & `molflux-0.4.0/docs/source/pages/tutorials/esol_uncertainty.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/tutorials/gdb9_trunc.parquet` & `molflux-0.4.0/docs/source/pages/tutorials/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/docs/source/pages/tutorials/qm9_reg_3d.md` & `molflux-0.4.0/docs/source/pages/tutorials/qm9_reg_3d.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/init_conda_venv.sh` & `molflux-0.4.0/init_conda_venv.sh`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/init_python_venv.sh` & `molflux-0.4.0/init_python_venv.sh`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/noxfile.py` & `molflux-0.4.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.catboost.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.rdkit.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,346 +1,357 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='catboost')
+#    nox -s dependencies_pin-3.8(extra='rdkit')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipython
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backcall==0.2.0
+    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
-    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
+exceptiongroup==1.2.1
+    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   domdf-python-tools
+    #   flask
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==1.0.0
+jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.7.5
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
+mhfp==1.9.6
+    # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==0.17.2
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==0.18.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.1
     # via cfn-lint
-numpy==1.26.4
+numpy==1.24.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
@@ -351,202 +362,196 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via pandas
+    # via
+    #   babel
+    #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.3.2
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.10.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==5.3.0
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -554,135 +559,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==1.23.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.0.1
     # via molflux (pyproject.toml)
 sphinx-design==0.5.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.8.0
+sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
+    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.19.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.core.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.xgboost.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,552 +1,557 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra=None)
+#    nox -s dependencies_pin-3.8(extra='xgboost')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipython
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backcall==0.2.0
+    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
-    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
+exceptiongroup==1.2.1
+    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   domdf-python-tools
+    #   flask
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==1.0.0
+jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.7.5
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==0.17.2
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==0.18.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.1
     # via cfn-lint
-numpy==1.26.4
+numpy==1.24.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
     #   matplotlib
     #   molflux (pyproject.toml)
     #   pandas
     #   pyarrow
     #   rdkit
     #   scikit-learn
     #   scipy
+    #   xgboost
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via pandas
+    # via
+    #   babel
+    #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.3.2
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.10.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
+    #   xgboost
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==5.3.0
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -554,135 +559,138 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==1.23.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.0.1
     # via molflux (pyproject.toml)
 sphinx-design==0.5.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.8.0
+sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
+    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
+xgboost==1.7.6
+    # via molflux (pyproject.toml)
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.19.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.ensemble.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.ensemble.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    nox -s dependencies_pin-3.10(extra='ensemble')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,216 +32,212 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -248,97 +246,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -351,202 +349,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -554,27 +540,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -586,103 +572,102 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.lightning.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.lightning.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,249 +1,241 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='lightning')
+#    nox -s dependencies_pin-3.11(extra='lightning')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
     #   torch
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -252,104 +244,104 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-lightning==2.2.0
+lightning==2.2.5
     # via molflux (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via
     #   cfn-lint
     #   torch
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
@@ -367,115 +359,108 @@
     #   scikit-learn
     #   scipy
     #   torchmetrics
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
     #   lightning-utilities
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
-pytorch-lightning==2.2.0
+pytorch-lightning==2.2.5
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
@@ -485,92 +470,87 @@
     #   jupytext
     #   lightning
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -578,27 +558,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -610,121 +590,113 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via
     #   cfn-lint
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 torch==2.0.1
     # via
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
     #   torchmetrics
-torchmetrics==1.3.0.post0
+torchmetrics==1.4.0.post0
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.mapie.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.mapie.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    nox -s dependencies_pin-3.10(extra='mapie')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,216 +32,212 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -248,97 +246,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -351,202 +349,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -554,27 +540,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -586,103 +572,102 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.openeye.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.pyod.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.pyod.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    nox -s dependencies_pin-3.10(extra='pyod')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,220 +32,216 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
 combo==0.1.3
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   combo
     #   molflux (pyproject.toml)
     #   pyod
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -252,103 +250,103 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
 llvmlite==0.42.0
     # via numba
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   combo
     #   molflux (pyproject.toml)
     #   pyod
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
-numba==0.59.0
+numba==0.59.1
     # via
     #   combo
     #   pyod
 numpy==1.26.4
     # via
     #   catboost
     #   combo
@@ -366,211 +364,198 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyod==1.1.3
+pyod==2.0.0
     # via
     #   combo
     #   molflux (pyproject.toml)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   combo
     #   mapie
     #   molflux (pyproject.toml)
     #   pyod
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   combo
     #   mapie
     #   molflux (pyproject.toml)
     #   pyod
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
-    #   pyod
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -578,27 +563,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -610,103 +595,102 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.pystan.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.pystan.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.rdkit.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.sklearn.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='rdkit')
+#    nox -s dependencies_pin-3.10(extra='sklearn')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,216 +32,212 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -248,99 +246,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
-mhfp==1.9.6
-    # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -353,202 +349,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -556,27 +540,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -588,103 +572,102 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.sklearn.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.catboost.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='sklearn')
+#    nox -s dependencies_pin-3.10(extra='catboost')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,216 +32,212 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -248,97 +246,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -351,202 +349,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -554,27 +540,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -586,103 +572,102 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.10/lockfile.xgboost.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.rdkit.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='xgboost')
+#    nox -s dependencies_pin-3.10(extra='rdkit')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,216 +32,212 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -248,97 +246,99 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
+mhfp==1.9.6
+    # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -347,208 +347,194 @@
     #   matplotlib
     #   molflux (pyproject.toml)
     #   pandas
     #   pyarrow
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   xgboost
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
-    #   xgboost
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -556,27 +542,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -588,105 +574,102 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
-xgboost==1.7.6
-    # via molflux (pyproject.toml)
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.catboost.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.ensemble.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,340 +1,355 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='catboost')
+#    nox -s dependencies_pin-3.8(extra='ensemble')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipython
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backcall==0.2.0
+    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2 ; python_version >= "3.11"
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
-    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
+exceptiongroup==1.2.1
+    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   domdf-python-tools
+    #   flask
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==1.0.0
+jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.7.5
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==0.17.2
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==0.18.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.1
     # via cfn-lint
-numpy==1.26.4
+numpy==1.24.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
@@ -345,202 +360,196 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via pandas
+    # via
+    #   babel
+    #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.3.2
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.10.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==5.3.0
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -548,130 +557,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==1.23.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.0.1
     # via molflux (pyproject.toml)
 sphinx-design==0.5.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.8.0
+sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
+tomli==2.0.1
+    # via
+    #   coverage
+    #   jupytext
+    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
+    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.19.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.core.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.core.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    nox -s dependencies_pin-3.11(extra=None)
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -28,212 +30,208 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -242,97 +240,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -345,202 +343,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -548,27 +534,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -580,98 +566,95 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.ensemble.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.ensemble.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    nox -s dependencies_pin-3.11(extra='ensemble')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -28,212 +30,208 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -242,97 +240,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -345,202 +343,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -548,27 +534,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -580,98 +566,95 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.lightning.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.lightning.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,353 +1,368 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='lightning')
+#    nox -s dependencies_pin-3.8(extra='lightning')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipython
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backcall==0.2.0
+    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
-    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
+exceptiongroup==1.2.1
+    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   domdf-python-tools
+    #   flask
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
     #   torch
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==1.0.0
+jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-lightning==2.2.0
+lightning==2.2.5
     # via molflux (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.7.5
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==0.17.2
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==0.18.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.1
     # via
     #   cfn-lint
     #   torch
-numpy==1.26.4
+numpy==1.24.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   lightning
@@ -361,210 +376,204 @@
     #   scikit-learn
     #   scipy
     #   torchmetrics
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
     #   lightning-utilities
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
-pytorch-lightning==2.2.0
+pytorch-lightning==2.2.5
     # via lightning
 pytz==2024.1
-    # via pandas
+    # via
+    #   babel
+    #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.3.2
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.10.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==5.3.0
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -572,148 +581,155 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==1.23.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.0.1
     # via molflux (pyproject.toml)
 sphinx-design==0.5.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.8.0
+sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via
     #   cfn-lint
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
+tomli==2.0.1
+    # via
+    #   coverage
+    #   jupytext
+    #   pytest
 torch==2.0.1
     # via
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
     #   torchmetrics
-torchmetrics==1.3.0.post0
+torchmetrics==1.4.0.post0
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux (pyproject.toml)
     #   myst-nb
+    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
-tzdata==2023.4
+    #   torchmetrics
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.19.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.mapie.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.mapie.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,340 +1,355 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='mapie')
+#    nox -s dependencies_pin-3.8(extra='mapie')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipython
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backcall==0.2.0
+    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
-    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
+exceptiongroup==1.2.1
+    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   domdf-python-tools
+    #   flask
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==1.0.0
+jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.7.5
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==0.17.2
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==0.18.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.1
     # via cfn-lint
-numpy==1.26.4
+numpy==1.24.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
@@ -345,202 +360,196 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via pandas
+    # via
+    #   babel
+    #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.3.2
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.10.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==5.3.0
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -548,130 +557,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==1.23.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.0.1
     # via molflux (pyproject.toml)
 sphinx-design==0.5.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.8.0
+sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
+tomli==2.0.1
+    # via
+    #   coverage
+    #   jupytext
+    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
+    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.19.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.openeye.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.pyod.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.sklearn.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,570 +1,555 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='pyod')
+#    nox -s dependencies_pin-3.8(extra='sklearn')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipython
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backcall==0.2.0
+    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-combo==0.1.3
-    # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
-    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
+exceptiongroup==1.2.1
+    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   domdf-python-tools
+    #   flask
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
-    #   combo
     #   molflux (pyproject.toml)
-    #   pyod
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==1.0.0
+jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-llvmlite==0.42.0
-    # via numba
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.7.5
     # via
     #   catboost
-    #   combo
     #   molflux (pyproject.toml)
-    #   pyod
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==0.17.2
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==0.18.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.1
     # via cfn-lint
-numba==0.59.0
-    # via
-    #   combo
-    #   pyod
-numpy==1.26.4
+numpy==1.24.4
     # via
     #   catboost
-    #   combo
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
     #   matplotlib
     #   molflux (pyproject.toml)
-    #   numba
     #   pandas
     #   pyarrow
-    #   pyod
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyod==1.1.3
-    # via
-    #   combo
-    #   molflux (pyproject.toml)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via pandas
+    # via
+    #   babel
+    #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.3.2
     # via
-    #   combo
     #   mapie
     #   molflux (pyproject.toml)
-    #   pyod
-scipy==1.12.0
+scipy==1.10.1
     # via
     #   catboost
-    #   combo
     #   mapie
     #   molflux (pyproject.toml)
-    #   pyod
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
-    #   pyod
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==5.3.0
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -572,130 +557,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==1.23.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.0.1
     # via molflux (pyproject.toml)
 sphinx-design==0.5.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.8.0
+sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
+tomli==2.0.1
+    # via
+    #   coverage
+    #   jupytext
+    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
+    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.19.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.pystan.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.pystan.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.rdkit.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.core.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,239 +1,243 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='rdkit')
+#    nox -s dependencies_pin-3.10(extra=None)
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -242,99 +246,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
-mhfp==1.9.6
-    # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -347,202 +349,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -550,27 +540,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -582,98 +572,102 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
+tomli==2.0.1
+    # via
+    #   coverage
+    #   jupytext
+    #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.sklearn.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.rdkit.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,239 +1,248 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='sklearn')
+#    nox -s dependencies_pin-3.9(extra='rdkit')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   flask
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -242,89 +251,91 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
+mhfp==1.9.6
+    # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -345,202 +356,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -548,27 +547,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -580,98 +579,104 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
+tomli==2.0.1
+    # via
+    #   coverage
+    #   jupytext
+    #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.19.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.11/lockfile.xgboost.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.xgboost.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,239 +1,243 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='xgboost')
+#    nox -s dependencies_pin-3.10(extra='xgboost')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -242,97 +246,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -346,203 +350,191 @@
     #   scikit-learn
     #   scipy
     #   xgboost
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
     #   xgboost
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -550,27 +542,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -582,100 +574,104 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
+tomli==2.0.1
+    # via
+    #   coverage
+    #   jupytext
+    #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xgboost==1.7.6
     # via molflux (pyproject.toml)
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.catboost.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.core.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='catboost')
+#    nox -s dependencies_pin-3.8(extra=None)
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via
     #   ipykernel
@@ -32,163 +34,155 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 backcall==0.2.0
     # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
 contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
 docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
@@ -196,61 +190,65 @@
     #   domdf-python-tools
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
     #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -259,49 +257,49 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.7.5
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
@@ -309,19 +307,19 @@
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
@@ -333,15 +331,15 @@
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
 nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -362,18 +360,17 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
@@ -382,94 +379,88 @@
     #   sphinx
 pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
 pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via
     #   babel
     #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
@@ -478,65 +469,61 @@
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
 scikit-learn==1.3.2
     # via
     #   mapie
     #   molflux (pyproject.toml)
@@ -546,15 +533,14 @@
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
@@ -583,15 +569,15 @@
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -603,107 +589,104 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.core.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.catboost.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra=None)
+#    nox -s dependencies_pin-3.8(extra='catboost')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via
     #   ipykernel
@@ -32,163 +34,155 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 backcall==0.2.0
     # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
 contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
 docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
@@ -196,61 +190,65 @@
     #   domdf-python-tools
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
     #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -259,49 +257,49 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.7.5
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
@@ -309,19 +307,19 @@
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
@@ -333,15 +331,15 @@
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
 nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -362,18 +360,17 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
@@ -382,94 +379,88 @@
     #   sphinx
 pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
 pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via
     #   babel
     #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
@@ -478,65 +469,61 @@
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
 scikit-learn==1.3.2
     # via
     #   mapie
     #   molflux (pyproject.toml)
@@ -546,15 +533,14 @@
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
@@ -583,15 +569,15 @@
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -603,107 +589,104 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.ensemble.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.mapie.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,357 +1,349 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='ensemble')
+#    nox -s dependencies_pin-3.9(extra='mapie')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via
-    #   ipykernel
-    #   ipython
+    # via ipykernel
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.19
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via pytest
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   domdf-python-tools
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
-    #   openapi-spec-validator
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.12.3
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==0.6.1
+jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==0.17.2
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==0.18.1
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.7.4
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.1
+networkx==3.2.1
     # via cfn-lint
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
@@ -362,208 +354,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.0.3
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.14.4
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via
-    #   babel
-    #   pandas
+    # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.3.2
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.10.1
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -571,139 +545,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==1.23.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.0.1
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
-    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.lightning.txt` & `molflux-0.4.0/pinned-versions/3.10/lockfile.lightning.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,370 +1,357 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='lightning')
+#    nox -s dependencies_pin-3.10(extra='lightning')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via
-    #   ipykernel
-    #   ipython
+    # via ipykernel
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.19
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via pytest
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   domdf-python-tools
-    #   flask
     #   jupyter-cache
-    #   jupyter-client
     #   myst-nb
     #   qlient-core
-    #   sphinx
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
-    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.12.3
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
     #   torch
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==0.6.1
+jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-lightning==2.2.0
+lightning==2.2.5
     # via molflux (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==0.17.2
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==0.18.1
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.7.4
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.1
+networkx==3.3
     # via
     #   cfn-lint
     #   torch
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   lightning
@@ -378,216 +365,198 @@
     #   scikit-learn
     #   scipy
     #   torchmetrics
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
     #   lightning-utilities
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.0.3
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.14.4
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
-pytorch-lightning==2.2.0
+pytorch-lightning==2.2.5
     # via lightning
 pytz==2024.1
-    # via
-    #   babel
-    #   pandas
+    # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.3.2
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.10.1
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -595,158 +564,152 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==1.23.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.0.1
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via
     #   cfn-lint
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 torch==2.0.1
     # via
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
     #   torchmetrics
-torchmetrics==1.3.0.post0
+torchmetrics==1.4.0.post0
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux (pyproject.toml)
     #   myst-nb
-    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
-    #   torchmetrics
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.19.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.mapie.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.sklearn.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,357 +1,349 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='mapie')
+#    nox -s dependencies_pin-3.9(extra='sklearn')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via
-    #   ipykernel
-    #   ipython
+    # via ipykernel
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.19
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via pytest
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   domdf-python-tools
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
-    #   openapi-spec-validator
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.12.3
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==0.6.1
+jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==0.17.2
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==0.18.1
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.7.4
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.1
+networkx==3.2.1
     # via cfn-lint
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
@@ -362,208 +354,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.0.3
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.14.4
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via
-    #   babel
-    #   pandas
+    # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.3.2
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.10.1
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -571,139 +545,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==1.23.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.0.1
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
-    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.openeye.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.pyod.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.pyod.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    nox -s dependencies_pin-3.8(extra='pyod')
 #
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via
     #   ipykernel
@@ -32,165 +34,157 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 backcall==0.2.0
     # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
 combo==0.1.3
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
 contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
 docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
@@ -199,63 +193,67 @@
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   numba
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
     #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   combo
     #   molflux (pyproject.toml)
     #   pyod
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -264,53 +262,53 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
 llvmlite==0.41.1
     # via numba
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.7.5
     # via
     #   catboost
     #   combo
     #   molflux (pyproject.toml)
     #   pyod
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
@@ -318,19 +316,19 @@
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
@@ -342,15 +340,15 @@
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
 nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -378,18 +376,17 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
@@ -398,98 +395,92 @@
     #   sphinx
 pandas==2.0.3
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
 pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyod==1.1.3
+pyod==2.0.0
     # via
     #   combo
     #   molflux (pyproject.toml)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via
     #   babel
     #   pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
@@ -498,65 +489,61 @@
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
 scikit-learn==1.3.2
     # via
     #   combo
     #   mapie
@@ -570,18 +557,16 @@
     #   molflux (pyproject.toml)
     #   pyod
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
-    #   pyod
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==5.3.0
@@ -608,15 +593,15 @@
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.5.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -628,107 +613,104 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.pystan.txt` & `molflux-0.4.0/pinned-versions/3.8/lockfile.pystan.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.rdkit.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.pyod.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,571 +1,566 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='rdkit')
+#    nox -s dependencies_pin-3.9(extra='pyod')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via
-    #   ipykernel
-    #   ipython
+    # via ipykernel
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+combo==0.1.3
+    # via molflux (pyproject.toml)
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.19
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via pytest
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   domdf-python-tools
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
-    #   openapi-spec-validator
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.12.3
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
+    #   combo
     #   molflux (pyproject.toml)
+    #   pyod
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==0.6.1
+jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+llvmlite==0.42.0
+    # via numba
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.9.0
     # via
     #   catboost
+    #   combo
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+    #   pyod
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
-mhfp==1.9.6
-    # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==0.17.2
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==0.18.1
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.7.4
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.1
+networkx==3.2.1
     # via cfn-lint
-numpy==1.24.4
+numba==0.59.1
+    # via
+    #   combo
+    #   pyod
+numpy==1.26.4
     # via
     #   catboost
+    #   combo
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
     #   matplotlib
     #   molflux (pyproject.toml)
+    #   numba
     #   pandas
     #   pyarrow
+    #   pyod
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.0.3
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.14.4
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyod==2.0.0
+    # via
+    #   combo
+    #   molflux (pyproject.toml)
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via
-    #   babel
-    #   pandas
+    # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.3.2
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
+    #   combo
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.10.1
+    #   pyod
+scipy==1.13.1
     # via
     #   catboost
+    #   combo
     #   mapie
     #   molflux (pyproject.toml)
+    #   pyod
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -573,139 +568,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==1.23.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.0.1
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
-    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.sklearn.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.mapie.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,357 +1,338 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='sklearn')
+#    nox -s dependencies_pin-3.11(extra='mapie')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via
-    #   ipykernel
-    #   ipython
+    # via ipykernel
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.19
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   domdf-python-tools
-    #   flask
     #   jupyter-cache
-    #   jupyter-client
     #   myst-nb
     #   qlient-core
-    #   sphinx
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
-    #   openapi-spec-validator
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.12.3
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==0.6.1
+jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==0.17.2
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==0.18.1
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.7.4
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.1
+networkx==3.3
     # via cfn-lint
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
@@ -362,208 +343,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.0.3
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.14.4
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via
-    #   babel
-    #   pandas
+    # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.3.2
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.10.1
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -571,139 +534,127 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==1.23.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.0.1
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
-    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.19.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.8/lockfile.xgboost.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.catboost.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,571 +1,543 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='xgboost')
+#    nox -s dependencies_pin-3.9(extra='catboost')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via
-    #   ipykernel
-    #   ipython
+    # via ipykernel
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.19
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via pytest
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   domdf-python-tools
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
-    #   openapi-spec-validator
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.12.3
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
     # via openapi-spec-validator
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
-jupyter-cache==0.6.1
+jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.7.4
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==0.17.2
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==0.18.1
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.7.4
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.1
+networkx==3.2.1
     # via cfn-lint
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
     #   matplotlib
     #   molflux (pyproject.toml)
     #   pandas
     #   pyarrow
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   xgboost
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.0.3
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.14.4
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
-    # via
-    #   babel
-    #   pandas
+    # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.3.2
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.10.1
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
-    #   xgboost
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -573,141 +545,136 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==1.23.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.0.1
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
-    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
-xgboost==1.7.6
-    # via molflux (pyproject.toml)
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.catboost.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.core.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='catboost')
+#    nox -s dependencies_pin-3.9(extra=None)
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,221 +32,217 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -253,89 +251,89 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -356,202 +354,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -559,27 +545,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -591,106 +577,104 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.core.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.ensemble.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra=None)
+#    nox -s dependencies_pin-3.9(extra='ensemble')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,221 +32,217 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -253,89 +251,89 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -356,202 +354,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -559,27 +545,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -591,106 +577,104 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.ensemble.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.xgboost.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='ensemble')
+#    nox -s dependencies_pin-3.9(extra='xgboost')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,221 +32,217 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -253,89 +251,89 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -352,206 +350,196 @@
     #   matplotlib
     #   molflux (pyproject.toml)
     #   pandas
     #   pyarrow
     #   rdkit
     #   scikit-learn
     #   scipy
+    #   xgboost
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
+    #   xgboost
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -559,27 +547,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -591,106 +579,106 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
+xgboost==1.7.6
+    # via molflux (pyproject.toml)
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.lightning.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.lightning.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    nox -s dependencies_pin-3.9(extra='lightning')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
@@ -30,225 +32,221 @@
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   flask
     #   jupyter-cache
     #   jupyter-client
     #   myst-nb
     #   qlient-core
     #   sphinx
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
     #   torch
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -257,96 +255,96 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-lightning==2.2.0
+lightning==2.2.5
     # via molflux (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -372,115 +370,108 @@
     #   scikit-learn
     #   scipy
     #   torchmetrics
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
     #   lightning-utilities
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
-pytorch-lightning==2.2.0
+pytorch-lightning==2.2.5
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
@@ -490,92 +481,87 @@
     #   jupytext
     #   lightning
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -583,27 +569,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -615,76 +601,74 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via
     #   cfn-lint
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
 tomli==2.0.1
     # via
     #   coverage
+    #   jupytext
     #   pytest
+    #   sphinx
 torch==2.0.1
     # via
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
     #   torchmetrics
-torchmetrics==1.3.0.post0
+torchmetrics==1.4.0.post0
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux (pyproject.toml)
     #   pytorch-lightning
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
@@ -693,46 +677,46 @@
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.19.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.mapie.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.sklearn.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,250 +1,237 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='mapie')
+#    nox -s dependencies_pin-3.11(extra='sklearn')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   flask
     #   jupyter-cache
-    #   jupyter-client
     #   myst-nb
     #   qlient-core
-    #   sphinx
-importlib-resources==6.1.1
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -253,97 +240,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -356,202 +343,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -559,27 +534,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -591,106 +566,95 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.19.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.openeye.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.pyod.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.catboost.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,254 +1,237 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='pyod')
+#    nox -s dependencies_pin-3.11(extra='catboost')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5 ; python_version >= "3.11"
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-combo==0.1.3
-    # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   flask
     #   jupyter-cache
-    #   jupyter-client
     #   myst-nb
     #   qlient-core
-    #   sphinx
-importlib-resources==6.1.1
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
-    #   combo
     #   molflux (pyproject.toml)
-    #   pyod
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -257,325 +240,293 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-llvmlite==0.42.0
-    # via numba
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
-    #   combo
     #   molflux (pyproject.toml)
-    #   pyod
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
-numba==0.59.0
-    # via
-    #   combo
-    #   pyod
 numpy==1.26.4
     # via
     #   catboost
-    #   combo
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
     #   matplotlib
     #   molflux (pyproject.toml)
-    #   numba
     #   pandas
     #   pyarrow
-    #   pyod
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyod==1.1.3
-    # via
-    #   combo
-    #   molflux (pyproject.toml)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
-    #   combo
     #   mapie
     #   molflux (pyproject.toml)
-    #   pyod
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
-    #   combo
     #   mapie
     #   molflux (pyproject.toml)
-    #   pyod
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
-    #   pyod
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -583,27 +534,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -615,106 +566,95 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.19.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.pystan.txt` & `molflux-0.4.0/pinned-versions/3.9/lockfile.pystan.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.rdkit.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.rdkit.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,250 +1,237 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='rdkit')
+#    nox -s dependencies_pin-3.11(extra='rdkit')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   flask
     #   jupyter-cache
-    #   jupyter-client
     #   myst-nb
     #   qlient-core
-    #   sphinx
-importlib-resources==6.1.1
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -253,99 +240,99 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mhfp==1.9.6
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -358,202 +345,190 @@
     #   rdkit
     #   scikit-learn
     #   scipy
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -561,27 +536,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -593,106 +568,95 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.19.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.sklearn.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.xgboost.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,250 +1,237 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='sklearn')
+#    nox -s dependencies_pin-3.11(extra='xgboost')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   flask
     #   jupyter-cache
-    #   jupyter-client
     #   myst-nb
     #   qlient-core
-    #   sphinx
-importlib-resources==6.1.1
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
     #   molflux (pyproject.toml)
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -253,97 +240,97 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
 numpy==1.26.4
     # via
     #   catboost
     #   contourpy
     #   datasets
     #   evaluate
@@ -352,206 +339,196 @@
     #   matplotlib
     #   molflux (pyproject.toml)
     #   pandas
     #   pyarrow
     #   rdkit
     #   scikit-learn
     #   scipy
+    #   xgboost
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   catboost
     #   mapie
     #   molflux (pyproject.toml)
     #   scikit-learn
+    #   xgboost
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -559,27 +536,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -591,106 +568,97 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
+xgboost==1.7.6
+    # via molflux (pyproject.toml)
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.19.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pinned-versions/3.9/lockfile.xgboost.txt` & `molflux-0.4.0/pinned-versions/3.11/lockfile.pyod.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,250 +1,241 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='xgboost')
+#    nox -s dependencies_pin-3.11(extra='pyod')
 #
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+antlr4-python3-runtime==4.13.1
+    # via moto
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jschema-to-python
     #   jsonschema
     #   jupyter-cache
     #   referencing
     #   sarif-om
 autodocsumm==0.2.12
     # via sphinx-toolbox
-aws-sam-translator==1.84.0
+aws-sam-translator==1.89.0
     # via cfn-lint
-aws-xray-sdk==2.12.1
+aws-xray-sdk==2.13.1
     # via moto
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-blinker==1.7.0
+blinker==1.8.2
     # via flask
-boto3==1.34.38
+boto3==1.34.117
     # via
     #   aws-sam-translator
     #   cloudpathlib
     #   molflux (pyproject.toml)
     #   moto
-botocore==1.34.38
+botocore==1.34.117
     # via
     #   aws-xray-sdk
     #   boto3
     #   molflux (pyproject.toml)
     #   moto
     #   s3transfer
 cachecontrol==0.14.0
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
-catboost==1.2.2
+    # via sphinx-toolbox
+catboost==1.2.5
     # via molflux (pyproject.toml)
-certifi==2024.2.2
+certifi==2024.6.2
     # via requests
 cffi==1.16.0
     # via cryptography
-cfn-lint==0.85.1
+cfn-lint==0.87.4
     # via moto
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   flask
     #   jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux (pyproject.toml)
 colorama==0.4.6
     # via molflux (pyproject.toml)
-comm==0.2.1
+combo==0.1.3
+    # via molflux (pyproject.toml)
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.3
     # via molflux (pyproject.toml)
-cryptography==42.0.2
+cryptography==42.0.7
     # via
+    #   joserfc
     #   moto
-    #   python-jose
-    #   sshpubkeys
-cssutils==2.9.0
+cssutils==2.11.0
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.0
+datasets==2.19.2
     # via
     #   evaluate
     #   molflux (pyproject.toml)
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docker==7.0.0
+docker==7.1.0
     # via moto
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-domdf-python-tools==3.8.0.post2
+domdf-python-tools==3.8.1
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
-ecdsa==0.18.0
-    # via
-    #   moto
-    #   python-jose
-    #   sshpubkeys
-evaluate==0.4.1
+evaluate==0.4.2
     # via molflux (pyproject.toml)
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
-flask==3.0.2
+flask==3.0.3
     # via
     #   flask-cors
     #   moto
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via moto
-fonttools==4.48.1
+fonttools==4.53.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
 graphql-core==3.2.3
     # via moto
-graphviz==0.20.1
+graphviz==0.20.3
     # via catboost
-h5py==3.10.0
+h5py==3.11.0
     # via molflux (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.23.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   flask
     #   jupyter-cache
-    #   jupyter-client
     #   myst-nb
     #   qlient-core
-    #   sphinx
-importlib-resources==6.1.1
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.25.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
-ipywidgets==8.1.2
+ipywidgets==8.1.3
     # via molflux (pyproject.toml)
-itsdangerous==2.1.2
+itsdangerous==2.2.0
     # via flask
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   moto
     #   myst-parser
     #   sphinx
     #   sphinx-jinja2-compat
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.2
     # via
+    #   combo
     #   molflux (pyproject.toml)
+    #   pyod
     #   scikit-learn
+joserfc==0.10.0
+    # via moto
 jschema-to-python==1.2.3
     # via cfn-lint
 jsondiff==2.0.0
     # via moto
 jsonpatch==1.33
     # via cfn-lint
-jsonpickle==3.0.2
+jsonpath-ng==1.6.1
+    # via moto
+jsonpickle==3.0.4
     # via jschema-to-python
 jsonpointer==2.4
     # via jsonpatch
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   aws-sam-translator
     #   cfn-lint
     #   nbformat
     #   openapi-schema-validator
     #   openapi-spec-validator
 jsonschema-path==0.3.2
@@ -253,307 +244,312 @@
     # via
     #   jsonschema
     #   openapi-schema-validator
 junit-xml==1.9
     # via cfn-lint
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
-jupyterlab-widgets==3.0.10
+jupyterlab-widgets==3.0.11
     # via ipywidgets
-jupytext==1.16.1
+jupytext==1.16.2
     # via molflux (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-object-proxy==1.10.0
     # via openapi-spec-validator
-mapie==0.8.2
+llvmlite==0.42.0
+    # via numba
+mapie==0.8.3
     # via molflux (pyproject.toml)
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
     #   werkzeug
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   catboost
+    #   combo
     #   molflux (pyproject.toml)
-matplotlib-inline==0.1.6
+    #   pyod
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux (pyproject.toml)
 mock==5.1.0
     # via molflux (pyproject.toml)
 more-itertools==10.2.0
     # via molflux (pyproject.toml)
-moto==5.0.1
+moto==5.0.9
     # via molflux (pyproject.toml)
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via molflux (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via cfn-lint
+numba==0.59.1
+    # via
+    #   combo
+    #   pyod
 numpy==1.26.4
     # via
     #   catboost
+    #   combo
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   mapie
     #   matplotlib
     #   molflux (pyproject.toml)
+    #   numba
     #   pandas
     #   pyarrow
+    #   pyod
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   xgboost
 openapi-schema-validator==0.6.2
     # via openapi-spec-validator
 openapi-spec-validator==0.7.1
     # via moto
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
-    #   docker
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   mapie
     #   matplotlib
     #   plotly
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   catboost
     #   datasets
     #   evaluate
     #   molflux (pyproject.toml)
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathable==0.4.3
     # via jsonschema-path
 pbr==6.0.0
     # via
     #   jschema-to-python
     #   sarif-om
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   apeye
     #   jupyter-core
-plotly==5.18.0
+plotly==5.22.0
     # via catboost
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
+ply==3.11
+    # via jsonpath-ng
+prompt-toolkit==3.0.45
     # via ipython
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py-partiql-parser==0.5.1
+py-partiql-parser==0.5.5
     # via moto
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via
     #   datasets
     #   molflux (pyproject.toml)
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   python-jose
-    #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   aws-sam-translator
     #   molflux (pyproject.toml)
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.15.3
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyod==2.0.0
+    # via
+    #   combo
+    #   molflux (pyproject.toml)
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   moto
-pytest==8.0.0
+pytest==8.2.1
     # via molflux (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux (pyproject.toml)
     #   moto
     #   pandas
-python-jose==3.3.0
-    # via
-    #   moto
-    #   python-jose
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   cfn-lint
     #   datasets
     #   huggingface-hub
     #   jsonschema-path
     #   jupyter-cache
     #   jupytext
     #   molflux (pyproject.toml)
     #   moto
     #   myst-nb
     #   myst-parser
-pyzmq==25.1.2
+    #   responses
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux (pyproject.toml)
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.9.3
     # via thefuzz
-rdkit==2023.9.4
+rdkit==2023.9.6
     # via molflux (pyproject.toml)
 referencing==0.31.1
     # via
     #   jsonschema
     #   jsonschema-path
     #   jsonschema-specifications
-regex==2023.12.25
+regex==2024.5.15
     # via cfn-lint
-requests==2.31.0
+requests==2.32.3
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   docker
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   jsonschema-path
     #   molflux (pyproject.toml)
     #   moto
     #   qlient
     #   responses
     #   sphinx
-responses==0.18.0
-    # via
-    #   evaluate
-    #   moto
+responses==0.25.0
+    # via moto
 rfc3339-validator==0.1.4
     # via openapi-schema-validator
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via python-jose
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
-scikit-learn==1.4.0 ; python_version > "3.8"
+scikit-learn==1.5.0 ; python_version > "3.8"
     # via
+    #   combo
     #   mapie
     #   molflux (pyproject.toml)
-scipy==1.12.0
+    #   pyod
+scipy==1.13.1
     # via
     #   catboost
+    #   combo
     #   mapie
     #   molflux (pyproject.toml)
+    #   pyod
     #   scikit-learn
-    #   xgboost
 six==1.16.0
     # via
     #   asttokens
     #   catboost
-    #   ecdsa
     #   html5lib
     #   junit-xml
     #   python-dateutil
     #   rfc3339-validator
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   molflux (pyproject.toml)
     #   myst-nb
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -561,27 +557,27 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.0
+sphinx-book-theme==1.1.2
     # via molflux (pyproject.toml)
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via molflux (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via molflux (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
-sphinx-sitemap==2.5.1
+sphinx-sitemap==2.6.0
     # via molflux (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via molflux (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via molflux (pyproject.toml)
@@ -593,108 +589,95 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.25
+sqlalchemy==2.0.30
     # via jupyter-cache
-sshpubkeys==3.3.1
-    # via moto
 stack-data==0.6.3
     # via ipython
-sympy==1.12
+sympy==1.12.1
     # via cfn-lint
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
-tenacity==8.2.3
+tenacity==8.3.0
     # via
     #   molflux (pyproject.toml)
     #   plotly
 thefuzz==0.22.1
     # via molflux (pyproject.toml)
-threadpoolctl==3.2.0
+threadpoolctl==3.5.0
     # via scikit-learn
-toml==0.10.2
-    # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.66.1
+tqdm==4.66.4
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   molflux (pyproject.toml)
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.12.1
     # via
     #   aws-sam-translator
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   molflux (pyproject.toml)
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   sphinx-toolbox
     #   sqlalchemy
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   docker
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
+werkzeug==3.0.3
     # via
     #   flask
     #   moto
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
-widgetsnbextension==4.0.10
+widgetsnbextension==4.0.11
     # via ipywidgets
 wrapt==1.16.0
     # via aws-xray-sdk
-xgboost==1.7.6
-    # via molflux (pyproject.toml)
 xmltodict==0.13.0
     # via moto
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.19.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molflux-0.3.0/pyproject.toml` & `molflux-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/core/environment.py` & `molflux-0.4.0/src/molflux/core/environment.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/core/featurisation/featurisation.py` & `molflux-0.4.0/src/molflux/core/featurisation/featurisation.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/core/featurisation/metadata.py` & `molflux-0.4.0/src/molflux/core/featurisation/metadata.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/core/io.py` & `molflux-0.4.0/src/molflux/core/io.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/core/models.py` & `molflux-0.4.0/src/molflux/core/models.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/core/scoring.py` & `molflux-0.4.0/src/molflux/core/scoring.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/core/tracking.py` & `molflux-0.4.0/src/molflux/core/tracking.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/ani1x/README.md` & `molflux-0.4.0/src/molflux/datasets/builders/ani1x/README.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/ani1x/ani1x.py` & `molflux-0.4.0/src/molflux/datasets/builders/ani1x/ani1x.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/ani2x/README.md` & `molflux-0.4.0/src/molflux/datasets/builders/ani2x/README.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/ani2x/ani2x.py` & `molflux-0.4.0/src/molflux/datasets/builders/ani2x/ani2x.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/ani2x/ani2x_configs.py` & `molflux-0.4.0/src/molflux/datasets/builders/ani2x/ani2x_configs.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/esol/README.md` & `molflux-0.4.0/src/molflux/datasets/builders/esol/README.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/esol/esol.py` & `molflux-0.4.0/src/molflux/datasets/builders/esol/esol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/gdb9/README.md` & `molflux-0.4.0/src/molflux/datasets/builders/gdb9/README.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/gdb9/gdb9.py` & `molflux-0.4.0/src/molflux/datasets/builders/gdb9/gdb9.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/pcqm4m_v2/README.md` & `molflux-0.4.0/src/molflux/datasets/builders/pcqm4m_v2/README.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/pcqm4m_v2/pcqm4m_v2.py` & `molflux-0.4.0/src/molflux/datasets/builders/pcqm4m_v2/pcqm4m_v2.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/spice/README.md` & `molflux-0.4.0/src/molflux/datasets/builders/spice/README.md`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/builders/spice/spice.py` & `molflux-0.4.0/src/molflux/datasets/builders/spice/spice.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/catalogue.py` & `molflux-0.4.0/src/molflux/datasets/catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/exceptions.py` & `molflux-0.4.0/src/molflux/datasets/exceptions.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/featurisation.py` & `molflux-0.4.0/src/molflux/datasets/featurisation.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/filesystems.py` & `molflux-0.4.0/src/molflux/datasets/filesystems.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/interfaces.py` & `molflux-0.4.0/src/molflux/datasets/interfaces.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/io.py` & `molflux-0.4.0/src/molflux/datasets/io.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/load.py` & `molflux-0.4.0/src/molflux/datasets/load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/parsers.py` & `molflux-0.4.0/src/molflux/datasets/parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/splitting.py` & `molflux-0.4.0/src/molflux/datasets/splitting.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/typing.py` & `molflux-0.4.0/src/molflux/datasets/typing.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/datasets/utils.py` & `molflux-0.4.0/src/molflux/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/bases.py` & `molflux-0.4.0/src/molflux/features/bases.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/catalogue.py` & `molflux-0.4.0/src/molflux/features/catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/errors.py` & `molflux-0.4.0/src/molflux/features/errors.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/info.py` & `molflux-0.4.0/src/molflux/features/info.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/load.py` & `molflux-0.4.0/src/molflux/features/load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/parsers.py` & `molflux-0.4.0/src/molflux/features/parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representation.py` & `molflux-0.4.0/src/molflux/features/representation.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/core/generic/character_count.py` & `molflux-0.4.0/src/molflux/features/representations/core/generic/character_count.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/core/generic/exploded.py` & `molflux-0.4.0/src/molflux/features/representations/core/generic/exploded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/_utils.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/canonical/_utils.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/canonical/_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/canonical/oemol.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/canonical/oemol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/canonical/smiles.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/canonical/smiles.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/aromatic_ring_count.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/aromatic_ring_count.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/molecular_weight.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/molecular_weight.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/net_charge.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/net_charge.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/num_acceptors.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/num_acceptors.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/num_donors.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/num_donors.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/rotatable_bonds.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/rotatable_bonds.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/tpsa.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/tpsa.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/descriptors/x_log_p.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/descriptors/x_log_p.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/circular.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/circular.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/lingo.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/lingo.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/maccs.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/maccs.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/path.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/path.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/fingerprints/tree.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/fingerprints/tree.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/sd/sd_feature.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/sd/sd_feature.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/openeye/shape/hermite.py` & `molflux-0.4.0/src/molflux/features/representations/openeye/shape/hermite.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/_utils.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/descriptors/rdkit_descriptors_2d.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/descriptors/rdkit_descriptors_2d.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair_unfolded.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/atom_pair_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/avalon.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/avalon.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/layered.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/layered.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/maccs.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/maccs.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/mhfp.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/mhfp.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/mhfp_unfolded.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/mhfp_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/morgan.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/morgan.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/morgan_unfolded.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/morgan_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/pattern.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/pattern.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/topological.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/topological.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion_unfolded.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/topological_torsion_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/fingerprints/toxicophores.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/fingerprints/toxicophores.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/reaction/_drfp_vendored.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/reaction/_drfp_vendored.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/representations/rdkit/reaction/drfp.py` & `molflux-0.4.0/src/molflux/features/representations/rdkit/reaction/drfp.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/features/utils.py` & `molflux-0.4.0/src/molflux/features/utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/__init__.py` & `molflux-0.4.0/src/molflux/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/bases.py` & `molflux-0.4.0/src/molflux/metrics/bases.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/catalogue.py` & `molflux-0.4.0/src/molflux/metrics/catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/accuracy.py` & `molflux-0.4.0/src/molflux/metrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/average_precision.py` & `molflux-0.4.0/src/molflux/metrics/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/balanced_accuracy.py` & `molflux-0.4.0/src/molflux/metrics/classification/balanced_accuracy.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/diversity_roc.py` & `molflux-0.4.0/src/molflux/metrics/classification/diversity_roc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/f1_score.py` & `molflux-0.4.0/src/molflux/metrics/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/matthews_corrcoef.py` & `molflux-0.4.0/src/molflux/metrics/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/precision.py` & `molflux-0.4.0/src/molflux/metrics/classification/precision.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/recall.py` & `molflux-0.4.0/src/molflux/metrics/classification/recall.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/roc_auc.py` & `molflux-0.4.0/src/molflux/metrics/classification/roc_auc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/top_k_accuracy.py` & `molflux-0.4.0/src/molflux/metrics/classification/top_k_accuracy.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/top_k_accuracy_roc.py` & `molflux-0.4.0/src/molflux/metrics/classification/top_k_accuracy_roc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/classification/validity_roc.py` & `molflux-0.4.0/src/molflux/metrics/classification/validity_roc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/load.py` & `molflux-0.4.0/src/molflux/metrics/load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/metric.py` & `molflux-0.4.0/src/molflux/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/parsers.py` & `molflux-0.4.0/src/molflux/metrics/parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/protocols.py` & `molflux-0.4.0/src/molflux/metrics/protocols.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/explained_variance.py` & `molflux-0.4.0/src/molflux/metrics/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/max_error.py` & `molflux-0.4.0/src/molflux/metrics/regression/max_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/mean_absolute_error.py` & `molflux-0.4.0/src/molflux/metrics/regression/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/mean_squared_error.py` & `molflux-0.4.0/src/molflux/metrics/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/median_absolute_error.py` & `molflux-0.4.0/src/molflux/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/pearson.py` & `molflux-0.4.0/src/molflux/metrics/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/proportion_within_fold.py` & `molflux-0.4.0/src/molflux/metrics/regression/proportion_within_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/r2.py` & `molflux-0.4.0/src/molflux/metrics/regression/r2.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/root_mean_squared_error.py` & `molflux-0.4.0/src/molflux/metrics/regression/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/regression/spearman.py` & `molflux-0.4.0/src/molflux/metrics/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/suites/catalogue.py` & `molflux-0.4.0/src/molflux/metrics/suites/catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/uncertainty/coefficient_of_variation.py` & `molflux-0.4.0/src/molflux/metrics/uncertainty/coefficient_of_variation.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/uncertainty/expected_calibration_error.py` & `molflux-0.4.0/src/molflux/metrics/uncertainty/expected_calibration_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/uncertainty/gaussian_nll.py` & `molflux-0.4.0/src/molflux/metrics/uncertainty/gaussian_nll.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/uncertainty/prediction_interval_coverage.py` & `molflux-0.4.0/src/molflux/metrics/uncertainty/prediction_interval_coverage.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/uncertainty/prediction_interval_width.py` & `molflux-0.4.0/src/molflux/metrics/uncertainty/prediction_interval_width.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/uncertainty/uncertainty_based_rejection.py` & `molflux-0.4.0/src/molflux/metrics/uncertainty/uncertainty_based_rejection.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/metrics/uncertainty/utils.py` & `molflux-0.4.0/src/molflux/metrics/uncertainty/utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/__init__.py` & `molflux-0.4.0/src/molflux/modelzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/catalogue.py` & `molflux-0.4.0/src/molflux/modelzoo/catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/errors.py` & `molflux-0.4.0/src/molflux/modelzoo/errors.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/info.py` & `molflux-0.4.0/src/molflux/modelzoo/info.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/interchange.py` & `molflux-0.4.0/src/molflux/modelzoo/interchange.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/load.py` & `molflux-0.4.0/src/molflux/modelzoo/load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/model.py` & `molflux-0.4.0/src/molflux/modelzoo/model.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/catboost/catboost_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/catboost/catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/catboost/catboost_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/catboost/catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/core/average_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/core/average_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/ensemble/_combo/utils.py` & `molflux-0.4.0/src/molflux/modelzoo/models/ensemble/_combo/utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/ensemble/ensemble_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/ensemble/ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/ensemble/ensemble_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/ensemble/ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/config.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/config.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/datamodule.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_config.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_config.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_datamodule.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_datamodule.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_model.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_model.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_module.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/mlp_regressor/mlp_module.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/model.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/model.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/module.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/module.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/callbacks/stock_callbacks.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/callbacks/stock_callbacks.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/stock_optimizers.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/optimizers/stock_optimizers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/stock_schedulers.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/trainer/schedulers/stock_schedulers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/lightning/utils.py` & `molflux-0.4.0/src/molflux/modelzoo/models/lightning/utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/mapie/mapie_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/mapie/mapie_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/__init__.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/__init__.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/abod_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/abod_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/cblof_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/cblof_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/hbos_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/hbos_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/isolation_forest_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/isolation_forest_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/knn_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/knn_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/mcd_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/mcd_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/ocsvm_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/ocsvm_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pyod/pca_detector.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pyod/pca_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/pystan/sparse_linear_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/pystan/sparse_linear_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/__init__.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/bernoulli_nb_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/bernoulli_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/corrected_nb_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/corrected_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/coverage_nb_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/coverage_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/dummy_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/dummy_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/extra_trees_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/extra_trees_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/extra_trees_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/extra_trees_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/kernel_ridge_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/kernel_ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/knn_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/knn_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/knn_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/knn_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/linear_discriminant_analysis_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/linear_discriminant_analysis_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/linear_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/logistic_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/logistic_regressor.py`

 * *Files 13% similar despite different names*

```diff
@@ -100,34 +100,21 @@
     .. seealso::
        Refer to the User Guide for more information regarding
        :class:`LogisticRegression` and more specifically the
        `Table <https://scikit-learn.org/dev/modules/linear_model.html#logistic-regression>`_
        summarazing solver/penalty supports.
 max_iter : int, default=100
     Maximum number of iterations taken for the solvers to converge.
-multi_class : {'auto', 'ovr', 'multinomial'}, default='auto'
-    If the option chosen is 'ovr', then a binary problem is fit for each
-    label. For 'multinomial' the loss minimised is the multinomial loss fit
-    across the entire probability distribution, *even when the data is
-    binary*. 'multinomial' is unavailable when solver='liblinear'.
-    'auto' selects 'ovr' if the data is binary, or if solver='liblinear',
-    and otherwise selects 'multinomial'.
 verbose : int, default=0
     For the liblinear and lbfgs solvers set verbose to any positive
     number for verbosity.
 warm_start : bool, default=False
     When set to True, reuse the solution of the previous call to fit as
     initialization, otherwise, just erase the previous solution.
     Useless for liblinear solver.
-n_jobs : int, default=None
-    Number of CPU cores used when parallelizing over classes if
-    multi_class='ovr'". This parameter is ignored when the ``solver`` is
-    set to 'liblinear' regardless of whether 'multi_class' is specified or
-    not. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
-    context. ``-1`` means using all processors.
 l1_ratio : float, default=None
     The Elastic-Net mixing parameter, with ``0 <= l1_ratio <= 1``. Only
     used if ``penalty='elasticnet'``. Setting ``l1_ratio=0`` is equivalent
     to using ``penalty='l2'``, while setting ``l1_ratio=1`` is equivalent
     to using ``penalty='l1'``. For ``0 < l1_ratio <1``, the penalty is a
     combination of L1 and L2.
 """
@@ -150,18 +137,16 @@
     C: float = 1
     fit_intercept: bool = True
     intercept_scaling: float = 1
     class_weight: ClassWeight = None
     random_state: Optional[Union[int, RandomState]] = None
     solver: Solver = "lbfgs"
     max_iter: int = 100
-    multi_class: MultiClass = "auto"
     verbose: int = 0
     warm_start: bool = False
-    n_jobs: Optional[int] = None
     l1_ratio: Optional[float] = None
 
 
 class LogisticRegressor(
     SKLearnClassificationMixin,
     SKLearnModelBase[LogisticRegressorConfig],
 ):
@@ -184,13 +169,11 @@
             C=config.C,
             fit_intercept=config.fit_intercept,
             intercept_scaling=config.intercept_scaling,
             class_weight=config.class_weight,
             random_state=config.random_state,
             solver=config.solver,
             max_iter=config.max_iter,
-            multi_class=config.multi_class,
             verbose=config.verbose,
             warm_start=config.warm_start,
-            n_jobs=config.n_jobs,
             l1_ratio=config.l1_ratio,
         )
```

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/mlp_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/mlp_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/mlp_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/pipeline_pilot_nb_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/pipeline_pilot_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/pls_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/pls_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/random_forest_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/random_forest_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/ridge_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/bayes.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_discrete_nb/bayes.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/_utils.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/sklearn_pipeline/sklearn_pipeline_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/support_vector_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/support_vector_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/sklearn/support_vector_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/sklearn/support_vector_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/xgboost/xgboost_classifier.py` & `molflux-0.4.0/src/molflux/modelzoo/models/xgboost/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/models/xgboost/xgboost_regressor.py` & `molflux-0.4.0/src/molflux/modelzoo/models/xgboost/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/parsers.py` & `molflux-0.4.0/src/molflux/modelzoo/parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/protocols.py` & `molflux-0.4.0/src/molflux/modelzoo/protocols.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/store/artefact.py` & `molflux-0.4.0/src/molflux/modelzoo/store/artefact.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/store/io.py` & `molflux-0.4.0/src/molflux/modelzoo/store/io.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/store/manager.py` & `molflux-0.4.0/src/molflux/modelzoo/store/manager.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/typing.py` & `molflux-0.4.0/src/molflux/modelzoo/typing.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/modelzoo/utils.py` & `molflux-0.4.0/src/molflux/modelzoo/utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/bases.py` & `molflux-0.4.0/src/molflux/splits/bases.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/catalogue.py` & `molflux-0.4.0/src/molflux/splits/catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/errors.py` & `molflux-0.4.0/src/molflux/splits/errors.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/info.py` & `molflux-0.4.0/src/molflux/splits/info.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/load.py` & `molflux-0.4.0/src/molflux/splits/load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/parsers.py` & `molflux-0.4.0/src/molflux/splits/parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/presets.py` & `molflux-0.4.0/src/molflux/splits/presets.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/_ordered_split_utils.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/_ordered_split_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/group_k_fold.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/group_k_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/group_shuffle_split.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/group_shuffle_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/k_fold.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/k_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/leave_one_group_out.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/leave_one_group_out.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/leave_p_groups_out.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/leave_p_groups_out.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/linear_split.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/linear_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/ordered_split.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/ordered_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/shuffle_split.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/shuffle_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/stratified_k_fold.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/stratified_k_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/stratified_ordered_split.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/stratified_ordered_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/stratified_shuffle_split.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/stratified_shuffle_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/core/time_series_split.py` & `molflux-0.4.0/src/molflux/splits/strategies/core/time_series_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/openeye/scaffold.py` & `molflux-0.4.0/src/molflux/splits/strategies/openeye/scaffold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/rdkit/scaffold.py` & `molflux-0.4.0/src/molflux/splits/strategies/rdkit/scaffold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategies/rdkit/tanimoto.py` & `molflux-0.4.0/src/molflux/splits/strategies/rdkit/tanimoto.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/strategy.py` & `molflux-0.4.0/src/molflux/splits/strategy.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux/splits/utils.py` & `molflux-0.4.0/src/molflux/splits/utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux.egg-info/PKG-INFO` & `molflux-0.4.0/src/molflux.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molflux
-Version: 0.3.0
+Version: 0.4.0
 Summary: A foundational package for molecular predictive modelling
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/molflux/issues
 Project-URL: repository, https://github.com/exscientia/molflux.git
 Project-URL: issue-tracker, https://github.com/exscientia/molflux/issues
 Project-URL: changelog, https://github.com/exscientia/molflux/src/main/CHANGELOG.md
@@ -154,15 +154,15 @@
 [MIT License](LICENSE)
 
 ## Acknowledgements
 
 The ``molflux`` package has been developed by researchers and engineers at Exscientia
 
 * Alan Bilsland
-* Julia Buhmann
-* Ward Haddadin
+* [Julia Buhmann](https://github.com/juliabuhmann)
+* [Ward Haddadin](https://github.com/wardhaddadin1)
 * Jonathan Harrison
 * Dom Miketa
 * Emil Nichita
 * Stefanie Speichert
 * Hagen Triendl
-* Alvise Vianello
+* [Alvise Vianello](https://github.com/amv213)
```

### Comparing `molflux-0.3.0/src/molflux.egg-info/SOURCES.txt` & `molflux-0.4.0/src/molflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux.egg-info/entry_points.txt` & `molflux-0.4.0/src/molflux.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/src/molflux.egg-info/requires.txt` & `molflux-0.4.0/src/molflux.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/core/conftest.py` & `molflux-0.4.0/tests/core/conftest.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/core/core/unit/test_api.py` & `molflux-0.4.0/tests/core/core/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/core/core/unit/test_featurisation.py` & `molflux-0.4.0/tests/core/core/unit/test_featurisation.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/core/core/unit/test_models.py` & `molflux-0.4.0/tests/core/core/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/core/core/unit/test_scoring.py` & `molflux-0.4.0/tests/core/core/unit/test_scoring.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/core/core/unit/test_tracking.py` & `molflux-0.4.0/tests/core/core/unit/test_tracking.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/__init__.py` & `molflux-0.4.0/tests/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/conftest.py` & `molflux-0.4.0/tests/datasets/conftest.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/conftest.py` & `molflux-0.4.0/tests/datasets/core/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/io/test_load_dataset_from_store.py` & `molflux-0.4.0/tests/datasets/core/unit/io/test_load_dataset_from_store.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/io/test_save_dataset_to_store.py` & `molflux-0.4.0/tests/datasets/core/unit/io/test_save_dataset_to_store.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/load/test_load_dataset.py` & `molflux-0.4.0/tests/datasets/core/unit/load/test_load_dataset.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/load/test_load_dataset_builder.py` & `molflux-0.4.0/tests/datasets/core/unit/load/test_load_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/load/test_load_from_dict.py` & `molflux-0.4.0/tests/datasets/core/unit/load/test_load_from_dict.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_api.py` & `molflux-0.4.0/tests/datasets/core/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_catalogue.py` & `molflux-0.4.0/tests/datasets/core/unit/test_catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_featurise.py` & `molflux-0.4.0/tests/datasets/core/unit/test_featurise.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_filesystems.py` & `molflux-0.4.0/tests/datasets/core/unit/test_filesystems.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_flatten_indices_failure.py` & `molflux-0.4.0/tests/datasets/core/unit/test_flatten_indices_failure.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_parsers.py` & `molflux-0.4.0/tests/datasets/core/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_splitting.py` & `molflux-0.4.0/tests/datasets/core/unit/test_splitting.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/core/unit/test_utils.py` & `molflux-0.4.0/tests/datasets/core/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/core/esol/test_esol.py` & `molflux-0.4.0/tests/datasets/plugins/core/esol/test_esol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/mock_data/data.h5` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/mock_data/data.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani1x/test_ani1x.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani1x/test_ani1x.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/ani2x/test_ani2x.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/ani2x/test_ani2x.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf` & `molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf.csv` & `molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/mock_data/gdb9.sdf.csv`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/gdb9/test_gdb9.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/gdb9/test_gdb9.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2-train.sdf` & `molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/pcqm4m-v2-train.sdf`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/pcqm4m/test_pcqm4m.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/pcqm4m/test_pcqm4m.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/spice/mock_data/data.h5` & `molflux-0.4.0/tests/datasets/plugins/openeye/spice/mock_data/data.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/spice/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/spice/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/openeye/spice/test_spice.py` & `molflux-0.4.0/tests/datasets/plugins/openeye/spice/test_spice.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/mock_data/data.h5` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/mock_data/data.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani1x/test_ani1x.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani1x/test_ani1x.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-B973c-def2mTZVP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MD3BJ-def2TZVPP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97MV-def2TZVPP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-631Gd.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/final_h5/ANI-2x-wB97X-def2TZVPP.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/ani2x/test_ani2x.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/ani2x/test_ani2x.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf` & `molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf.csv` & `molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/mock_data/gdb9.sdf.csv`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/gdb9/test_gdb9.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/gdb9/test_gdb9.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2-train.sdf` & `molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/pcqm4m-v2-train.sdf`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/pcqm4m/test_pcqm4m.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/pcqm4m/test_pcqm4m.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/spice/mock_data/data.h5` & `molflux-0.4.0/tests/datasets/plugins/rdkit/spice/mock_data/data.h5`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/spice/mock_data/script.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/spice/mock_data/script.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/datasets/plugins/rdkit/spice/test_spice.py` & `molflux-0.4.0/tests/datasets/plugins/rdkit/spice/test_spice.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/core/integration/test_missing_dependencies.py` & `molflux-0.4.0/tests/features/core/integration/test_missing_dependencies.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/core/unit/representation/test_protocol.py` & `molflux-0.4.0/tests/features/core/unit/representation/test_protocol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/core/unit/representations/test_protocol.py` & `molflux-0.4.0/tests/features/core/unit/representations/test_protocol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/core/unit/test_api.py` & `molflux-0.4.0/tests/features/core/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/core/unit/test_featurise.py` & `molflux-0.4.0/tests/features/core/unit/test_featurise.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/core/unit/test_load.py` & `molflux-0.4.0/tests/features/core/unit/test_load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/core/unit/test_parsers.py` & `molflux-0.4.0/tests/features/core/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/core/generic/test_exploded.py` & `molflux-0.4.0/tests/features/plugins/core/generic/test_exploded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/canonical/test_oemol.py` & `molflux-0.4.0/tests/features/plugins/openeye/canonical/test_oemol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/canonical/test_smiles.py` & `molflux-0.4.0/tests/features/plugins/openeye/canonical/test_smiles.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_aromatic_ring_count.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_aromatic_ring_count.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_molecular_weight.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_molecular_weight.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_net_charge.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_net_charge.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_num_acceptors.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_num_acceptors.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_num_donors.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_num_donors.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_rotatable_bonds.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_rotatable_bonds.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_tpsa.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_tpsa.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/descriptors/test_x_log_p.py` & `molflux-0.4.0/tests/features/plugins/openeye/descriptors/test_x_log_p.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_circular.py` & `molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_circular.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_lingo.py` & `molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_lingo.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_maccs.py` & `molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_maccs.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_path.py` & `molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_path.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/fingerprints/test_tree.py` & `molflux-0.4.0/tests/features/plugins/openeye/fingerprints/test_tree.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/sd/test_sd_feature.py` & `molflux-0.4.0/tests/features/plugins/openeye/sd/test_sd_feature.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/shape/test_hermite.py` & `molflux-0.4.0/tests/features/plugins/openeye/shape/test_hermite.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/openeye/test_utils.py` & `molflux-0.4.0/tests/features/plugins/openeye/test_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/descriptors/test_rdkit_descriptors_2d.py` & `molflux-0.4.0/tests/features/plugins/rdkit/descriptors/test_rdkit_descriptors_2d.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair_unfolded.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_atom_pair_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_avalon.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_avalon.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_layered.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_layered.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_maccs.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_maccs.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_mhfp.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_mhfp.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_mhfp_unfolded.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_mhfp_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_morgan.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_morgan.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_morgan_unfolded.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_morgan_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_pattern.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_pattern.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_topological.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_topological.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion_unfolded.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_topological_torsion_unfolded.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/fingerprints/test_toxicophores.py` & `molflux-0.4.0/tests/features/plugins/rdkit/fingerprints/test_toxicophores.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/reaction/test_drfp.py` & `molflux-0.4.0/tests/features/plugins/rdkit/reaction/test_drfp.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/features/plugins/rdkit/test_utils.py` & `molflux-0.4.0/tests/features/plugins/rdkit/test_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/metric/test_compute.py` & `molflux-0.4.0/tests/metrics/core/unit/metric/test_compute.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/metric/test_protocol.py` & `molflux-0.4.0/tests/metrics/core/unit/metric/test_protocol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/metric/test_uncertainty_protocol.py` & `molflux-0.4.0/tests/metrics/core/unit/metric/test_uncertainty_protocol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/metrics/test_protocol.py` & `molflux-0.4.0/tests/metrics/core/unit/metrics/test_protocol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/test_api.py` & `molflux-0.4.0/tests/metrics/core/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/test_catalogue.py` & `molflux-0.4.0/tests/metrics/core/unit/test_catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/test_load.py` & `molflux-0.4.0/tests/metrics/core/unit/test_load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/core/unit/test_parsers.py` & `molflux-0.4.0/tests/metrics/core/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_accuracy.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_average_precision.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_average_precision.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_balanced_accuracy.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_balanced_accuracy.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_diversity_roc.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_diversity_roc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_f1_score.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_f1_score.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_matthews_corrcoef.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_precision.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_precision.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_recall.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_recall.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_roc_auc.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_roc_auc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_top_k_accuracy.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_top_k_accuracy.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_top_k_accuracy_roc.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_top_k_accuracy_roc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/classification/test_validity_roc.py` & `molflux-0.4.0/tests/metrics/plugins/core/classification/test_validity_roc.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_explained_variance.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_explained_variance.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_max_error.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_max_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_mean_absolute_error.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_mean_squared_error.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_median_absolute_error.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_pearson.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_pearson.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_proportion_within_fold.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_proportion_within_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_r2.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_r2.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_root_mean_squared_error.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/regression/test_spearman.py` & `molflux-0.4.0/tests/metrics/plugins/core/regression/test_spearman.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/suites/test_classification.py` & `molflux-0.4.0/tests/metrics/plugins/core/suites/test_classification.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/suites/test_load.py` & `molflux-0.4.0/tests/metrics/plugins/core/suites/test_load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/suites/test_regression.py` & `molflux-0.4.0/tests/metrics/plugins/core/suites/test_regression.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/suites/test_uncertainty.py` & `molflux-0.4.0/tests/metrics/plugins/core/suites/test_uncertainty.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_coefficient_of_variation.py` & `molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_coefficient_of_variation.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_expected_calibration_error.py` & `molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_expected_calibration_error.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_gaussian_nll.py` & `molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_gaussian_nll.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_coverage.py` & `molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_coverage.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_width.py` & `molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_prediction_interval_width.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/metrics/plugins/core/uncertainty/test_uncertainty_based_rejection.py` & `molflux-0.4.0/tests/metrics/plugins/core/uncertainty/test_uncertainty_based_rejection.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/integration/test_missing_dependencies.py` & `molflux-0.4.0/tests/modelzoo/core/integration/test_missing_dependencies.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/conftest.py` & `molflux-0.4.0/tests/modelzoo/core/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/model/test_model.py` & `molflux-0.4.0/tests/modelzoo/core/unit/model/test_model.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/model/test_predict.py` & `molflux-0.4.0/tests/modelzoo/core/unit/model/test_predict.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/model/test_protocol.py` & `molflux-0.4.0/tests/modelzoo/core/unit/model/test_protocol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/store/conftest.py` & `molflux-0.4.0/tests/modelzoo/core/unit/store/conftest.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/store/test_disk.py` & `molflux-0.4.0/tests/modelzoo/core/unit/store/test_disk.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/store/test_s3.py` & `molflux-0.4.0/tests/modelzoo/core/unit/store/test_s3.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/test_api.py` & `molflux-0.4.0/tests/modelzoo/core/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/test_interchange.py` & `molflux-0.4.0/tests/modelzoo/core/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/test_load.py` & `molflux-0.4.0/tests/modelzoo/core/unit/test_load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/test_parsers.py` & `molflux-0.4.0/tests/modelzoo/core/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/core/unit/test_utils.py` & `molflux-0.4.0/tests/modelzoo/core/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/catboost/test_cat_boost_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/catboost/test_cat_boost_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/catboost/test_cat_boost_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/catboost/test_cat_boost_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/core/test_average_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/core/test_average_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/ensemble/test_combo_utils.py` & `molflux-0.4.0/tests/modelzoo/plugins/ensemble/test_combo_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/ensemble/test_ensemble_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/ensemble/test_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/ensemble/test_ensemble_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/ensemble/test_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/fortuna/test_fortuna_mlp_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/fortuna/test_fortuna_mlp_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/lightning/conftest.py` & `molflux-0.4.0/tests/modelzoo/plugins/lightning/conftest.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/lightning/test_mlp_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/lightning/test_mlp_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/lightning/test_model_checkpoint_apply_callback.py` & `molflux-0.4.0/tests/modelzoo/plugins/lightning/test_model_checkpoint_apply_callback.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/lightning/test_transfer_learning.py` & `molflux-0.4.0/tests/modelzoo/plugins/lightning/test_transfer_learning.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/mapie/test_mapie_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/mapie/test_mapie_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_abod_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_abod_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_cblof_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_cblof_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 )
 predict_df = train_df
 empty_predict_df = pd.DataFrame([], columns=_X_FEATURES)
 
 
 @pytest.fixture(scope="function")
 def fixture_model() -> Model:
-    return load_model(model_name, x_features=_X_FEATURES)
+    return load_model(model_name, x_features=_X_FEATURES, alpha=0.5)
 
 
 def test_in_catalogue():
     """That the model is registered in the catalogue."""
     catalogue = list_models()
     all_names = [name for names in catalogue.values() for name in names]
     assert model_name in all_names
```

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_hbos_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_hbos_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_isolation_forest_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_isolation_forest_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_knn_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_knn_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_mcd_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_mcd_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_ocsvm_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_ocsvm_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pyod/test_pca_detector.py` & `molflux-0.4.0/tests/modelzoo/plugins/pyod/test_pca_detector.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/pystan/test_sparse_linear_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/pystan/test_sparse_linear_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/test_bayes.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/sklearn_discrete_nb/test_bayes.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_base_mixin.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_base_mixin.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_bernoulli_nb_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_bernoulli_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_corrected_nb_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_corrected_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_coverage_nb_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_coverage_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_dummy_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_dummy_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_extra_trees_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_extra_trees_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_extra_trees_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_extra_trees_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_kernel_ridge_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_kernel_ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_knn_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_knn_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_knn_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_linear_discriminant_analysis_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_linear_discriminant_analysis_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_linear_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_linear_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_logistic_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_logistic_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_mlp_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_mlp_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_mlp_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_pipeline_pilot_nb_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_pipeline_pilot_nb_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_pls_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_pls_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_random_forest_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_random_forest_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_ridge_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_sklearn_pipeline_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_support_vector_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_support_vector_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/sklearn/test_support_vector_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/sklearn/test_support_vector_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/xgboost/test_xg_boost_classifier.py` & `molflux-0.4.0/tests/modelzoo/plugins/xgboost/test_xg_boost_classifier.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/modelzoo/plugins/xgboost/test_xg_boost_regressor.py` & `molflux-0.4.0/tests/modelzoo/plugins/xgboost/test_xg_boost_regressor.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/presets/test_k_fold_split.py` & `molflux-0.4.0/tests/splits/core/unit/presets/test_k_fold_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/presets/test_train_test_split.py` & `molflux-0.4.0/tests/splits/core/unit/presets/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/presets/test_train_validation_test_split.py` & `molflux-0.4.0/tests/splits/core/unit/presets/test_train_validation_test_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_api.py` & `molflux-0.4.0/tests/splits/core/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_catalogue.py` & `molflux-0.4.0/tests/splits/core/unit/test_catalogue.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_info.py` & `molflux-0.4.0/tests/splits/core/unit/test_info.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_load.py` & `molflux-0.4.0/tests/splits/core/unit/test_load.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_naming.py` & `molflux-0.4.0/tests/splits/core/unit/test_naming.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_parsers.py` & `molflux-0.4.0/tests/splits/core/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_protocol.py` & `molflux-0.4.0/tests/splits/core/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/core/unit/test_utils.py` & `molflux-0.4.0/tests/splits/core/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_group_k_fold.py` & `molflux-0.4.0/tests/splits/plugins/core/test_group_k_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_group_shuffle_split.py` & `molflux-0.4.0/tests/splits/plugins/core/test_group_shuffle_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_k_fold.py` & `molflux-0.4.0/tests/splits/plugins/core/test_k_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_leave_one_group_out.py` & `molflux-0.4.0/tests/splits/plugins/core/test_leave_one_group_out.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_leave_p_groups_out.py` & `molflux-0.4.0/tests/splits/plugins/core/test_leave_p_groups_out.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_linear_split.py` & `molflux-0.4.0/tests/splits/plugins/core/test_linear_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_ordered_split.py` & `molflux-0.4.0/tests/splits/plugins/core/test_ordered_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_shuffle_split.py` & `molflux-0.4.0/tests/splits/plugins/core/test_shuffle_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_stratified_k_fold.py` & `molflux-0.4.0/tests/splits/plugins/core/test_stratified_k_fold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_stratified_ordered_split.py` & `molflux-0.4.0/tests/splits/plugins/core/test_stratified_ordered_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_stratified_shuffle_split.py` & `molflux-0.4.0/tests/splits/plugins/core/test_stratified_shuffle_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/core/test_time_series_split.py` & `molflux-0.4.0/tests/splits/plugins/core/test_time_series_split.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/openeye/test_scaffold.py` & `molflux-0.4.0/tests/splits/plugins/openeye/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/rdkit/test_scaffold.py` & `molflux-0.4.0/tests/splits/plugins/rdkit/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `molflux-0.3.0/tests/splits/plugins/rdkit/test_tanimoto.py` & `molflux-0.4.0/tests/splits/plugins/rdkit/test_tanimoto.py`

 * *Files identical despite different names*

