# Comparing `tmp/scine_autocas-2.2.0.tar.gz` & `tmp/scine_autocas-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scine_autocas-2.2.0.tar", last modified: Mon Jan 29 15:36:52 2024, max compression
+gzip compressed data, was "dist/scine_autocas-2.3.0.tar", last modified: Mon Jun  3 06:57:34 2024, max compression
```

## Comparing `scine_autocas-2.2.0.tar` & `scine_autocas-2.3.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/dev/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/dev/conan/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-10-05 07:13:51.000000 scine_autocas-2.2.0/dev/conan/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11235 2024-01-29 14:28:07.000000 scine_autocas-2.2.0/dev/conan/base.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2710 2024-01-29 14:28:07.000000 scine_autocas-2.2.0/dev/conan/utils.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-10-05 07:13:51.000000 scine_autocas-2.2.0/dev/__init__.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/docs/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/docs/source/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/docs/source/additional_api/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      272 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/additional_api/scine_autocas.chemical_elements.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      271 2024-01-29 14:48:37.000000 scine_autocas-2.2.0/docs/source/additional_api/scine_autocas.rst
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/docs/source/generated/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      271 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.autocas_utils.active_space.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      323 2023-01-18 13:21:05.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.autocas_utils.cas_combination.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      266 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.autocas_utils.diagnostics.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      275 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.autocas_utils.input_handler.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      294 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.autocas_utils.large_active_spaces.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      254 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.autocas_utils.molecule.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      501 2023-01-18 13:21:04.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.autocas_utils.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      256 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.molcas.dumper.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      276 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.molcas.environment.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      285 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.molcas.input_handler.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      302 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.molcas.molcas_hdf5_utils.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      494 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.molcas.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      313 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.qcmaquis_hdf5_dataset.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      312 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.qcmaquis_hdf5_utils.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      345 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.qcmaquis_orbital_rdm_builder.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      493 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      397 2023-01-18 13:21:05.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      243 2023-01-18 13:21:05.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.interfaces.serenity.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      265 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.plots.entanglement_plot.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      284 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.plots.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      253 2022-10-05 08:19:13.000000 scine_autocas-2.2.0/docs/source/generated/scine_autocas.plots.threshold_plot.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      276 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/api.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2668 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/autocas.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       33 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/changelog.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4795 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/docs/source/conf.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      628 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/index.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1213 2023-01-18 13:59:45.000000 scine_autocas-2.2.0/docs/source/installation.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2497 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/interfaces.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1353 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/plots.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      794 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/quickstart.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       78 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/readme.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      415 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/set_up.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2865 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/source/usage.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      638 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/Makefile
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      804 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/docs/make.bat
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      651 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     9608 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/active_space.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4218 2024-01-29 14:29:38.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/cas_combination.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4124 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/diagnostics.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5213 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/input_handler.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7681 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/large_active_spaces.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10721 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/autocas_utils/molecule.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/interfaces/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/interfaces/molcas/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    27274 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/molcas/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4711 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/molcas/dumper.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5311 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/molcas/environment.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7115 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/molcas/input_handler.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7598 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/molcas/molcas_hdf5_utils.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6703 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5423 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_dataset.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15154 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_utils.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11879 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/qcmaquis_orbital_rdm_builder.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/interfaces/serenity/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14957 2024-01-29 14:30:30.000000 scine_autocas-2.2.0/scine_autocas/interfaces/serenity/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10409 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/interfaces/__init__.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/plots/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      246 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/plots/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13230 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/plots/entanglement_plot.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3659 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/plots/threshold_plot.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas/tests/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      239 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    23243 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/test_autocas.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3324 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/test_input_handler.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6448 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/test_main_functions.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    31159 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/test_molcas_interface.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2879 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/test_molecule.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3630 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/test_plots.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5251 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/tests/test_qcmaquis_utils.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    31743 2024-01-29 14:28:31.000000 scine_autocas-2.2.0/scine_autocas/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1469 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/__main__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      215 2024-01-29 14:28:47.000000 scine_autocas-2.2.0/scine_autocas/_version.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    46690 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/chemical_elements.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25606 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/scine_autocas/main_functions.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas.egg-info/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5868 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas.egg-info/PKG-INFO
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3648 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas.egg-info/SOURCES.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas.egg-info/dependency_links.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       63 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas.egg-info/entry_points.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-10-05 08:48:09.000000 scine_autocas-2.2.0/scine_autocas.egg-info/not-zip-safe
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      237 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas.egg-info/requires.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       14 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/scine_autocas.egg-info/top_level.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      614 2024-01-29 14:27:44.000000 scine_autocas-2.2.0/CHANGELOG.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      349 2022-10-07 08:04:27.000000 scine_autocas-2.2.0/MANIFEST.in
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4146 2023-10-06 07:00:52.000000 scine_autocas-2.2.0/README.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      237 2024-01-29 14:27:24.000000 scine_autocas-2.2.0/requirements.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      781 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/setup.cfg
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2625 2024-01-29 14:29:10.000000 scine_autocas-2.2.0/setup.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5868 2024-01-29 15:36:52.000000 scine_autocas-2.2.0/PKG-INFO
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/dev/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/dev/conan/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-10-05 07:13:51.000000 scine_autocas-2.3.0/dev/conan/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11235 2024-06-03 06:27:53.000000 scine_autocas-2.3.0/dev/conan/base.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2710 2024-01-29 14:28:07.000000 scine_autocas-2.3.0/dev/conan/utils.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-10-05 07:13:51.000000 scine_autocas-2.3.0/dev/__init__.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/docs/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/docs/source/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/docs/source/additional_api/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      272 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/additional_api/scine_autocas.chemical_elements.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      271 2024-01-29 14:48:37.000000 scine_autocas-2.3.0/docs/source/additional_api/scine_autocas.rst
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/docs/source/generated/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      271 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.autocas_utils.active_space.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      323 2023-01-18 13:21:05.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.autocas_utils.cas_combination.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      266 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.autocas_utils.diagnostics.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      275 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.autocas_utils.input_handler.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      294 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.autocas_utils.large_active_spaces.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      254 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.autocas_utils.molecule.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      501 2023-01-18 13:21:04.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.autocas_utils.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      256 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.molcas.dumper.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      276 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.molcas.environment.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      285 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.molcas.input_handler.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      302 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.molcas.molcas_hdf5_utils.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      494 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.molcas.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      313 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.qcmaquis_hdf5_dataset.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      312 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.qcmaquis_hdf5_utils.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      345 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.qcmaquis_orbital_rdm_builder.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      493 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.qcmaquis.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      397 2023-01-18 13:21:05.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      243 2023-01-18 13:21:05.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.interfaces.serenity.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      265 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.plots.entanglement_plot.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      284 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.plots.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      253 2022-10-05 08:19:13.000000 scine_autocas-2.3.0/docs/source/generated/scine_autocas.plots.threshold_plot.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      276 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/api.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2668 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/autocas.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       33 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/changelog.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4795 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/docs/source/conf.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      628 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/index.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1213 2023-01-18 13:59:45.000000 scine_autocas-2.3.0/docs/source/installation.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2497 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/interfaces.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1353 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/plots.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      794 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/quickstart.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       78 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/readme.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      415 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/set_up.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2865 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/source/usage.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      638 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/Makefile
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      804 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/docs/make.bat
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      651 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     9608 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/active_space.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4217 2024-06-03 06:37:34.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/cas_combination.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4124 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/diagnostics.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5213 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/input_handler.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7681 2024-05-30 12:57:09.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/large_active_spaces.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10721 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/autocas_utils/molecule.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/interfaces/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/interfaces/molcas/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    27274 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/molcas/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4711 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/molcas/dumper.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5311 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/molcas/environment.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7115 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/molcas/input_handler.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7598 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/molcas/molcas_hdf5_utils.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6703 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5423 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_dataset.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15154 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_utils.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11879 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/qcmaquis_orbital_rdm_builder.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/interfaces/serenity/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14953 2024-06-03 06:37:34.000000 scine_autocas-2.3.0/scine_autocas/interfaces/serenity/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10409 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/interfaces/__init__.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/plots/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      246 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/plots/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13230 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/plots/entanglement_plot.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3659 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/plots/threshold_plot.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas/tests/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      239 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/tests/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    23243 2024-05-30 12:57:09.000000 scine_autocas-2.3.0/scine_autocas/tests/test_autocas.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3324 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/tests/test_input_handler.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6448 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/tests/test_main_functions.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    31159 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/tests/test_molcas_interface.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2879 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/tests/test_molecule.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3630 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/tests/test_plots.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5251 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/tests/test_qcmaquis_utils.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    31744 2024-06-03 06:37:34.000000 scine_autocas-2.3.0/scine_autocas/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1469 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/__main__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      215 2024-06-03 06:37:34.000000 scine_autocas-2.3.0/scine_autocas/_version.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    46690 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/chemical_elements.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25606 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/scine_autocas/main_functions.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas.egg-info/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5868 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas.egg-info/PKG-INFO
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3648 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas.egg-info/SOURCES.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas.egg-info/dependency_links.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       63 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas.egg-info/entry_points.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-10-05 08:48:09.000000 scine_autocas-2.3.0/scine_autocas.egg-info/not-zip-safe
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      237 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas.egg-info/requires.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       14 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/scine_autocas.egg-info/top_level.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      870 2024-06-03 06:37:34.000000 scine_autocas-2.3.0/CHANGELOG.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      349 2022-10-07 08:04:27.000000 scine_autocas-2.3.0/MANIFEST.in
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4146 2023-10-06 07:00:52.000000 scine_autocas-2.3.0/README.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      237 2024-01-29 14:27:24.000000 scine_autocas-2.3.0/requirements.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      781 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/setup.cfg
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2625 2024-05-30 12:57:09.000000 scine_autocas-2.3.0/setup.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5868 2024-06-03 06:57:34.000000 scine_autocas-2.3.0/PKG-INFO
```

### Comparing `scine_autocas-2.2.0/dev/conan/base.py` & `scine_autocas-2.3.0/dev/conan/base.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/dev/conan/utils.py` & `scine_autocas-2.3.0/dev/conan/utils.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/autocas.rst` & `scine_autocas-2.3.0/docs/source/autocas.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/conf.py` & `scine_autocas-2.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/index.rst` & `scine_autocas-2.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/installation.rst` & `scine_autocas-2.3.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/interfaces.rst` & `scine_autocas-2.3.0/docs/source/interfaces.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/plots.rst` & `scine_autocas-2.3.0/docs/source/plots.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/quickstart.rst` & `scine_autocas-2.3.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/source/usage.rst` & `scine_autocas-2.3.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/Makefile` & `scine_autocas-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/docs/make.bat` & `scine_autocas-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/autocas_utils/__init__.py` & `scine_autocas-2.3.0/scine_autocas/autocas_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/autocas_utils/active_space.py` & `scine_autocas-2.3.0/scine_autocas/autocas_utils/active_space.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/autocas_utils/cas_combination.py` & `scine_autocas-2.3.0/scine_autocas/autocas_utils/cas_combination.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,9 +83,8 @@
     new_occupations: List[List[float]] = [[] for _ in range(n_systems)]
     for i_group, occ in zip(active_orbital_groups, occupation_in_group):
         group = orbital_groups[i_group]
         n_orbitals = len(group[0])
         for i_sys, orbitals in enumerate(group):
             new_active_spaces[i_sys] += orbitals
             new_occupations[i_sys] += [occ for _ in range(n_orbitals)]
-
     return new_occupations, new_active_spaces
```

### Comparing `scine_autocas-2.2.0/scine_autocas/autocas_utils/diagnostics.py` & `scine_autocas-2.3.0/scine_autocas/autocas_utils/diagnostics.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/autocas_utils/input_handler.py` & `scine_autocas-2.3.0/scine_autocas/autocas_utils/input_handler.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/autocas_utils/large_active_spaces.py` & `scine_autocas-2.3.0/scine_autocas/autocas_utils/large_active_spaces.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/autocas_utils/molecule.py` & `scine_autocas-2.3.0/scine_autocas/autocas_utils/molecule.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/molcas/__init__.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/molcas/__init__.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/molcas/dumper.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/molcas/dumper.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/molcas/environment.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/molcas/environment.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/molcas/input_handler.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/molcas/input_handler.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/molcas/molcas_hdf5_utils.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/molcas/molcas_hdf5_utils.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/__init__.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/__init__.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_dataset.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_utils.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/qcmaquis_hdf5_utils.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/qcmaquis/qcmaquis_orbital_rdm_builder.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/qcmaquis/qcmaquis_orbital_rdm_builder.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/serenity/__init__.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/serenity/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,17 +233,17 @@
         """
         import serenipy as spy
         if len(self.settings.molcas_orbital_files) < len(self.systems):
             raise ValueError("Fewer loading paths for molcas orbitals then systems.")
         for i_sys, sys in enumerate(self.systems):
             loading_path = self.settings.molcas_orbital_files[i_sys]
             if self.settings.uhf:
-                read = spy.ReadOrbitalsTask_U(sys)
+                read = spy.OrbitalsIOTask_U(sys)
             else:
-                read = spy.ReadOrbitalsTask_R(sys)
+                read = spy.OrbitalsIOTask_R(sys)
             read.settings.fileFormat = spy.ORBITAL_FILE_TYPES.MOLCAS
             read.settings.resetCoreOrbitals = False
             read.settings.replaceInFile = write
             read.settings.path = loading_path
             read.run()
 
     @staticmethod
```

### Comparing `scine_autocas-2.2.0/scine_autocas/interfaces/__init__.py` & `scine_autocas-2.3.0/scine_autocas/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/plots/entanglement_plot.py` & `scine_autocas-2.3.0/scine_autocas/plots/entanglement_plot.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/plots/threshold_plot.py` & `scine_autocas-2.3.0/scine_autocas/plots/threshold_plot.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/tests/test_autocas.py` & `scine_autocas-2.3.0/scine_autocas/tests/test_autocas.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/tests/test_input_handler.py` & `scine_autocas-2.3.0/scine_autocas/tests/test_input_handler.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/tests/test_main_functions.py` & `scine_autocas-2.3.0/scine_autocas/tests/test_main_functions.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/tests/test_molcas_interface.py` & `scine_autocas-2.3.0/scine_autocas/tests/test_molcas_interface.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/tests/test_molecule.py` & `scine_autocas-2.3.0/scine_autocas/tests/test_molecule.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/tests/test_plots.py` & `scine_autocas-2.3.0/scine_autocas/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/tests/test_qcmaquis_utils.py` & `scine_autocas-2.3.0/scine_autocas/tests/test_qcmaquis_utils.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/__init__.py` & `scine_autocas-2.3.0/scine_autocas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         thresholds_list, orbitals_index = self._sort_orbitals_by_s1(
             thresholds_list, orbitals_index
         )
         plateau_vector = self._get_plateau(thresholds_list)
         return plateau_vector, orbitals_index
 
     def _make_active_space(self) -> bool:
-        """Make active space by searching plteaus in s1 and reordering
+        """Make active space by searching plateaus in s1 and reordering
         orbitals.
 
         Returns
         -------
         bool
             True if a plateau was found, e.g. a smaller active space; False if no plateau was found
         """
```

### Comparing `scine_autocas-2.2.0/scine_autocas/__main__.py` & `scine_autocas-2.3.0/scine_autocas/__main__.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/chemical_elements.py` & `scine_autocas-2.3.0/scine_autocas/chemical_elements.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas/main_functions.py` & `scine_autocas-2.3.0/scine_autocas/main_functions.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/scine_autocas.egg-info/PKG-INFO` & `scine_autocas-2.3.0/scine_autocas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scine-autocas
-Version: 2.2.0
+Version: 2.3.0
 Summary: Automated active space selection quantum chemical software
 Home-page: https://www.scine.ethz.ch
 Author: ETH Zurich, Department of Chemistry and Applied Biosciences, Reiher Group
 Author-email: scine@phys.chem.ethz.ch
 License: BSD (3-clause)
 Description: SCINE - AutoCAS
         ===============
```

### Comparing `scine_autocas-2.2.0/scine_autocas.egg-info/SOURCES.txt` & `scine_autocas-2.3.0/scine_autocas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/README.rst` & `scine_autocas-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/setup.cfg` & `scine_autocas-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/setup.py` & `scine_autocas-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `scine_autocas-2.2.0/PKG-INFO` & `scine_autocas-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scine_autocas
-Version: 2.2.0
+Version: 2.3.0
 Summary: Automated active space selection quantum chemical software
 Home-page: https://www.scine.ethz.ch
 Author: ETH Zurich, Department of Chemistry and Applied Biosciences, Reiher Group
 Author-email: scine@phys.chem.ethz.ch
 License: BSD (3-clause)
 Description: SCINE - AutoCAS
         ===============
```

