# Comparing `tmp/krotov-1.2.1.tar.gz` & `tmp/krotov-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krotov-1.2.1.tar", last modified: Wed Jan 13 21:24:05 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `krotov-1.2.1.tar` & `krotov-1.3.0.tar`

### file list

```diff
@@ -1,272 +1,123 @@
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/
--rw-r--r--   0 goerz      (501) staff       (20)     1266 2021-01-13 18:59:43.000000 krotov-1.2.1/AUTHORS.rst
--rw-r--r--   0 goerz      (501) staff       (20)    29359 2021-01-09 19:59:22.000000 krotov-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 goerz      (501) staff       (20)     8842 2021-01-13 19:01:52.000000 krotov-1.2.1/HISTORY.rst
--rw-r--r--   0 goerz      (501) staff       (20)     1506 2020-01-02 07:29:19.000000 krotov-1.2.1/LICENSE
--rw-r--r--   0 goerz      (501) staff       (20)      290 2020-01-02 07:29:19.000000 krotov-1.2.1/MANIFEST.in
--rw-r--r--   0 goerz      (501) staff       (20)    20524 2021-01-13 21:24:05.000000 krotov-1.2.1/PKG-INFO
--rw-r--r--   0 goerz      (501) staff       (20)     7871 2021-01-13 19:02:48.000000 krotov-1.2.1/README.rst
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/
--rw-r--r--   0 goerz      (501) staff       (20)     1240 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/01_overview.rst
--rw-r--r--   0 goerz      (501) staff       (20)       33 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/02_contributing.rst
--rw-r--r--   0 goerz      (501) staff       (20)       28 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/03_authors.rst
--rw-r--r--   0 goerz      (501) staff       (20)      801 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/04_features.rst
--rw-r--r--   0 goerz      (501) staff       (20)       28 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/05_history.rst
--rw-r--r--   0 goerz      (501) staff       (20)     6242 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/06_introduction.rst
--rw-r--r--   0 goerz      (501) staff       (20)    30335 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/07_krotovs_method.rst
--rw-r--r--   0 goerz      (501) staff       (20)     3827 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/08_qutip_usage.rst
--rw-r--r--   0 goerz      (501) staff       (20)      594 2021-01-13 19:02:48.000000 krotov-1.2.1/docs/09_examples.rst
--rw-r--r--   0 goerz      (501) staff       (20)    30384 2020-03-24 16:37:32.000000 krotov-1.2.1/docs/10_howto.rst
--rw-r--r--   0 goerz      (501) staff       (20)    27873 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/11_other_methods.rst
--rw-r--r--   0 goerz      (501) staff       (20)     1691 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/12_related_software.rst
--rw-r--r--   0 goerz      (501) staff       (20)       81 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/99_bibliography.rst
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/API/
--rw-r--r--   0 goerz      (501) staff       (20)     1032 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.convergence.rst
--rw-r--r--   0 goerz      (501) staff       (20)     1200 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.conversions.rst
--rw-r--r--   0 goerz      (501) staff       (20)     1372 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.functionals.rst
--rw-r--r--   0 goerz      (501) staff       (20)      645 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.info_hooks.rst
--rw-r--r--   0 goerz      (501) staff       (20)      445 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.mu.rst
--rw-r--r--   0 goerz      (501) staff       (20)      823 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.objectives.rst
--rw-r--r--   0 goerz      (501) staff       (20)      478 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.optimize.rst
--rw-r--r--   0 goerz      (501) staff       (20)     1073 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.parallelization.rst
--rw-r--r--   0 goerz      (501) staff       (20)      718 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.propagators.rst
--rw-r--r--   0 goerz      (501) staff       (20)      408 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.result.rst
--rw-r--r--   0 goerz      (501) staff       (20)     1263 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.rst
--rw-r--r--   0 goerz      (501) staff       (20)      620 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.second_order.rst
--rw-r--r--   0 goerz      (501) staff       (20)      779 2021-01-13 19:22:51.000000 krotov-1.2.1/docs/API/krotov.shapes.rst
--rw-r--r--   0 goerz      (501) staff       (20)     1476 2020-03-15 20:10:17.000000 krotov-1.2.1/docs/Makefile
--rw-r--r--   0 goerz      (501) staff       (20)     7400 2021-01-13 19:24:36.000000 krotov-1.2.1/docs/_README.rst
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_build/
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_build/doctree/
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/
--rw-r--r--   0 goerz      (501) staff       (20)     9935 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_01_example_simple_state_to_state_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9401 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_01_example_simple_state_to_state_25_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13711 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_01_example_simple_state_to_state_33_0.png
--rw-r--r--   0 goerz      (501) staff       (20)   122379 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_01_example_simple_state_to_state_36_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10441 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10370 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_24_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    13960 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_31_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14674 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_43_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    15036 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_43_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    12663 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_45_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    11180 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_45_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    15813 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_02_example_lambda_system_rwa_complex_pulse_48_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13573 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_23_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     8740 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_23_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14685 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_32_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14808 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_32_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    16149 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_35_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9574 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_35_1.png
--rw-r--r--   0 goerz      (501) staff       (20)     8144 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_41_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14208 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_43_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14344 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_43_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    15621 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_45_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11104 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_45_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    12776 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_47_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    11201 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_03_example_lambda_system_rwa_non_hermitian_47_3.png
--rw-r--r--   0 goerz      (501) staff       (20)     9049 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_04_example_dissipative_qubit_reset_27_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    16337 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_04_example_dissipative_qubit_reset_31_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10418 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_04_example_dissipative_qubit_reset_43_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14739 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_04_example_dissipative_qubit_reset_45_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    12497 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13113 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13544 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_24_1.png
--rw-r--r--   0 goerz      (501) staff       (20)     8950 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_33_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    20418 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_36_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11042 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_38_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    28167 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_41_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    27961 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_05_example_transmon_xgate_42_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9093 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_06_example_3states_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    61169 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_06_example_3states_49_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    29063 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_06_example_3states_60_0.png
--rw-r--r--   0 goerz      (501) staff       (20)   194678 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_06_example_3states_66_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9468 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_06_example_3states_68_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     8491 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_07_example_PE_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    65118 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_07_example_PE_42_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    16873 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_07_example_PE_44_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    15817 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_08_example_ensemble_20_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11783 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_08_example_ensemble_29_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    16628 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_08_example_ensemble_53_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    16827 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_08_example_ensemble_53_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    16909 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_08_example_ensemble_56_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    19049 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_08_example_ensemble_64_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9395 2021-01-13 19:24:23.000000 krotov-1.2.1/docs/_build/doctree/nbsphinx/notebooks_09_example_numpy_25_0.png
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_build/html/
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_build/html/_images/
--rw-r--r--   0 goerz      (501) staff       (20)    22180 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/_build/html/_images/energylevels.png
--rw-r--r--   0 goerz      (501) staff       (20)     9935 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_01_example_simple_state_to_state_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9401 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_01_example_simple_state_to_state_25_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13711 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_01_example_simple_state_to_state_33_0.png
--rw-r--r--   0 goerz      (501) staff       (20)   122379 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_01_example_simple_state_to_state_36_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10441 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10370 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_24_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    13960 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_31_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14674 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_43_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    15036 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_43_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    12663 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_45_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    11180 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_45_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    15813 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_02_example_lambda_system_rwa_complex_pulse_48_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13573 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_23_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     8740 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_23_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14685 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_32_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14808 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_32_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    16149 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_35_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9574 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_35_1.png
--rw-r--r--   0 goerz      (501) staff       (20)     8144 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_41_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14208 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_43_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14344 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_43_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    15621 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_45_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11104 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_45_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    12776 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_47_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    11201 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_03_example_lambda_system_rwa_non_hermitian_47_3.png
--rw-r--r--   0 goerz      (501) staff       (20)     9049 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_04_example_dissipative_qubit_reset_27_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    16337 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_04_example_dissipative_qubit_reset_31_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10418 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_04_example_dissipative_qubit_reset_43_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14739 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_04_example_dissipative_qubit_reset_45_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    12497 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13113 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13544 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_24_1.png
--rw-r--r--   0 goerz      (501) staff       (20)     8950 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_33_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    20418 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_36_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11042 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_38_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    28167 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_41_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    27961 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_05_example_transmon_xgate_42_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9093 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_06_example_3states_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    61169 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_06_example_3states_49_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    29063 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_06_example_3states_60_0.png
--rw-r--r--   0 goerz      (501) staff       (20)   194678 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_06_example_3states_66_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9468 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_06_example_3states_68_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     8491 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_07_example_PE_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    65118 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_07_example_PE_42_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    16873 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_07_example_PE_44_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    15817 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_08_example_ensemble_20_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11783 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_08_example_ensemble_29_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    16628 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_08_example_ensemble_53_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    16827 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_08_example_ensemble_53_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    16909 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_08_example_ensemble_56_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    19049 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_08_example_ensemble_64_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9395 2021-01-13 19:24:23.000000 krotov-1.2.1/docs/_build/html/_images/notebooks_09_example_numpy_25_0.png
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_build/html/_static/
--rw-r--r--   0 goerz      (501) staff       (20)      286 2021-01-13 19:00:18.000000 krotov-1.2.1/docs/_build/html/_static/file.png
--rw-r--r--   0 goerz      (501) staff       (20)       90 2021-01-13 19:00:18.000000 krotov-1.2.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 goerz      (501) staff       (20)       90 2021-01-13 19:00:18.000000 krotov-1.2.1/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_build/tex/
--rw-r--r--   0 goerz      (501) staff       (20)     1602 2021-01-13 19:24:44.000000 krotov-1.2.1/docs/_build/tex/Makefile
--rw-r--r--   0 goerz      (501) staff       (20)    22180 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/_build/tex/energylevels.png
--rw-r--r--   0 goerz      (501) staff       (20)      558 2021-01-13 19:24:44.000000 krotov-1.2.1/docs/_build/tex/make.bat
--rw-r--r--   0 goerz      (501) staff       (20)     9935 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/tex/notebooks_01_example_simple_state_to_state_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9401 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/tex/notebooks_01_example_simple_state_to_state_25_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13711 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/tex/notebooks_01_example_simple_state_to_state_33_0.png
--rw-r--r--   0 goerz      (501) staff       (20)   122379 2021-01-13 19:23:04.000000 krotov-1.2.1/docs/_build/tex/notebooks_01_example_simple_state_to_state_36_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10441 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10370 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_24_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    13960 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_31_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14674 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_43_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    15036 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_43_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    12663 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_45_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    11180 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_45_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    15813 2021-01-13 19:23:13.000000 krotov-1.2.1/docs/_build/tex/notebooks_02_example_lambda_system_rwa_complex_pulse_48_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13573 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_23_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     8740 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_23_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14685 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_32_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14808 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_32_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    16149 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_35_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9574 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_35_1.png
--rw-r--r--   0 goerz      (501) staff       (20)     8144 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_41_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14208 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_43_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    14344 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_43_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    15621 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_45_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11104 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_45_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    12776 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_47_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    11201 2021-01-13 19:23:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_03_example_lambda_system_rwa_non_hermitian_47_3.png
--rw-r--r--   0 goerz      (501) staff       (20)     9049 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/tex/notebooks_04_example_dissipative_qubit_reset_27_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    16337 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/tex/notebooks_04_example_dissipative_qubit_reset_31_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    10418 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/tex/notebooks_04_example_dissipative_qubit_reset_43_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    14739 2021-01-13 19:23:33.000000 krotov-1.2.1/docs/_build/tex/notebooks_04_example_dissipative_qubit_reset_45_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    12497 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13113 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    13544 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_24_1.png
--rw-r--r--   0 goerz      (501) staff       (20)     8950 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_33_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    20418 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_36_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11042 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_38_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    28167 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_41_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    27961 2021-01-13 19:23:41.000000 krotov-1.2.1/docs/_build/tex/notebooks_05_example_transmon_xgate_42_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9093 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/tex/notebooks_06_example_3states_24_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    61169 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/tex/notebooks_06_example_3states_49_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    29063 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/tex/notebooks_06_example_3states_60_0.png
--rw-r--r--   0 goerz      (501) staff       (20)   194678 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/tex/notebooks_06_example_3states_66_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9468 2021-01-13 19:23:54.000000 krotov-1.2.1/docs/_build/tex/notebooks_06_example_3states_68_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     8491 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/tex/notebooks_07_example_PE_10_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    65118 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/tex/notebooks_07_example_PE_42_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    16873 2021-01-13 19:24:04.000000 krotov-1.2.1/docs/_build/tex/notebooks_07_example_PE_44_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    15817 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/tex/notebooks_08_example_ensemble_20_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    11783 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/tex/notebooks_08_example_ensemble_29_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    16628 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/tex/notebooks_08_example_ensemble_53_1.png
--rw-r--r--   0 goerz      (501) staff       (20)    16827 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/tex/notebooks_08_example_ensemble_53_3.png
--rw-r--r--   0 goerz      (501) staff       (20)    16909 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/tex/notebooks_08_example_ensemble_56_0.png
--rw-r--r--   0 goerz      (501) staff       (20)    19049 2021-01-13 19:24:15.000000 krotov-1.2.1/docs/_build/tex/notebooks_08_example_ensemble_64_0.png
--rw-r--r--   0 goerz      (501) staff       (20)     9395 2021-01-13 19:24:23.000000 krotov-1.2.1/docs/_build/tex/notebooks_09_example_numpy_25_0.png
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/_templates/
--rw-r--r--   0 goerz      (501) staff       (20)     1361 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/_templates/module.rst
--rw-r--r--   0 goerz      (501) staff       (20)     2557 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/_templates/package.rst
--rw-r--r--   0 goerz      (501) staff       (20)    18013 2021-01-09 23:07:53.000000 krotov-1.2.1/docs/conf.py
--rw-r--r--   0 goerz      (501) staff       (20)     2612 2021-01-13 19:02:48.000000 krotov-1.2.1/docs/index.rst
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/notebooks/
--rw-r--r--   0 goerz      (501) staff       (20)    22180 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/notebooks/energylevels.png
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/docs/pseudocode/
--rw-r--r--   0 goerz      (501) staff       (20)      770 2020-01-02 07:29:19.000000 krotov-1.2.1/docs/pseudocode/Makefile
--rw-r--r--   0 goerz      (501) staff       (20)      730 2021-01-13 21:24:05.000000 krotov-1.2.1/setup.cfg
--rw-r--r--   0 goerz      (501) staff       (20)     3140 2021-01-09 23:07:53.000000 krotov-1.2.1/setup.py
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/src/
--rw-r--r--   0 goerz      (501) staff       (20)      525 2020-01-02 07:29:19.000000 krotov-1.2.1/src/conftest.py
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/src/krotov/
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/src/krotov/.ipynb_checkpoints/
--rw-r--r--   0 goerz      (501) staff       (20)    12712 2020-01-02 07:29:19.000000 krotov-1.2.1/src/krotov/.ipynb_checkpoints/conversions-checkpoint.py
--rw-r--r--   0 goerz      (501) staff       (20)     1852 2021-01-13 18:47:43.000000 krotov-1.2.1/src/krotov/__init__.py
--rw-r--r--   0 goerz      (501) staff       (20)    16863 2020-01-02 07:29:19.000000 krotov-1.2.1/src/krotov/convergence.py
--rw-r--r--   0 goerz      (501) staff       (20)    14074 2020-08-17 14:27:37.000000 krotov-1.2.1/src/krotov/conversions.py
--rw-r--r--   0 goerz      (501) staff       (20)    21396 2020-03-24 16:37:33.000000 krotov-1.2.1/src/krotov/functionals.py
--rw-r--r--   0 goerz      (501) staff       (20)    25189 2020-08-17 14:27:37.000000 krotov-1.2.1/src/krotov/info_hooks.py
--rw-r--r--   0 goerz      (501) staff       (20)     5591 2020-01-02 07:29:19.000000 krotov-1.2.1/src/krotov/mu.py
--rw-r--r--   0 goerz      (501) staff       (20)    52463 2020-03-24 16:37:33.000000 krotov-1.2.1/src/krotov/objectives.py
--rw-r--r--   0 goerz      (501) staff       (20)    36753 2021-01-10 04:46:35.000000 krotov-1.2.1/src/krotov/optimize.py
--rw-r--r--   0 goerz      (501) staff       (20)    22873 2020-03-24 21:57:14.000000 krotov-1.2.1/src/krotov/parallelization.py
--rw-r--r--   0 goerz      (501) staff       (20)    14352 2020-07-30 17:29:40.000000 krotov-1.2.1/src/krotov/propagators.py
--rw-r--r--   0 goerz      (501) staff       (20)    11004 2020-03-24 16:37:33.000000 krotov-1.2.1/src/krotov/result.py
--rw-r--r--   0 goerz      (501) staff       (20)     5109 2020-01-02 07:29:19.000000 krotov-1.2.1/src/krotov/second_order.py
--rw-r--r--   0 goerz      (501) staff       (20)     5509 2020-01-02 07:29:19.000000 krotov-1.2.1/src/krotov/shapes.py
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/src/krotov.egg-info/
--rw-r--r--   0 goerz      (501) staff       (20)    20524 2021-01-13 21:24:04.000000 krotov-1.2.1/src/krotov.egg-info/PKG-INFO
--rw-r--r--   0 goerz      (501) staff       (20)    14062 2021-01-13 21:24:04.000000 krotov-1.2.1/src/krotov.egg-info/SOURCES.txt
--rw-r--r--   0 goerz      (501) staff       (20)        1 2021-01-13 21:24:04.000000 krotov-1.2.1/src/krotov.egg-info/dependency_links.txt
--rw-r--r--   0 goerz      (501) staff       (20)        1 2021-01-13 21:24:00.000000 krotov-1.2.1/src/krotov.egg-info/not-zip-safe
--rw-r--r--   0 goerz      (501) staff       (20)      435 2021-01-13 21:24:04.000000 krotov-1.2.1/src/krotov.egg-info/requires.txt
--rw-r--r--   0 goerz      (501) staff       (20)        7 2021-01-13 21:24:04.000000 krotov-1.2.1/src/krotov.egg-info/top_level.txt
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/tests/
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/tests/test_dump_result/
--rw-r--r--   0 goerz      (501) staff       (20)    41661 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_dump_result/oct_result.dump
--rw-r--r--   0 goerz      (501) staff       (20)     2493 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_dump_result.py
--rw-r--r--   0 goerz      (501) staff       (20)    11477 2020-03-16 05:05:43.000000 krotov-1.2.1/tests/test_functionals.py
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/tests/test_infohooks/
--rw-r--r--   0 goerz      (501) staff       (20)      249 2020-08-17 14:27:37.000000 krotov-1.2.1/tests/test_infohooks/custom_format_out.txt
--rw-r--r--   0 goerz      (501) staff       (20)      468 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_infohooks/custom_header_out.txt
--rw-r--r--   0 goerz      (501) staff       (20)     7584 2020-08-13 04:40:24.000000 krotov-1.2.1/tests/test_infohooks.py
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/tests/test_krotov/
--rw-r--r--   0 goerz      (501) staff       (20)     1152 2020-08-17 14:27:37.000000 krotov-1.2.1/tests/test_krotov/oct.log
--rw-r--r--   0 goerz      (501) staff       (20)    18962 2020-08-13 04:40:24.000000 krotov-1.2.1/tests/test_krotov.py
--rw-r--r--   0 goerz      (501) staff       (20)     4109 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_mu.py
--rw-r--r--   0 goerz      (501) staff       (20)     2320 2021-01-10 04:46:35.000000 krotov-1.2.1/tests/test_numpy_controls.py
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/tests/test_objectives/
--rw-r--r--   0 goerz      (501) staff       (20)    50540 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_objectives/pulse.dat
--rw-r--r--   0 goerz      (501) staff       (20)    28860 2020-03-24 16:37:33.000000 krotov-1.2.1/tests/test_objectives.py
--rw-r--r--   0 goerz      (501) staff       (20)      552 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_overlap.py
--rw-r--r--   0 goerz      (501) staff       (20)     5306 2020-08-17 14:27:37.000000 krotov-1.2.1/tests/test_parallelization.py
--rw-r--r--   0 goerz      (501) staff       (20)     2281 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_pulse_options.py
-drwxr-xr-x   0 goerz      (501) staff       (20)        0 2021-01-13 21:24:05.000000 krotov-1.2.1/tests/test_result_serialization/
--rw-r--r--   0 goerz      (501) staff       (20)    41661 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_result_serialization/oct_result.dump
--rw-r--r--   0 goerz      (501) staff       (20)    25725 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_result_serialization/oct_result_broken.dump
--rw-r--r--   0 goerz      (501) staff       (20)   422502 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_result_serialization/oct_result_incomplete.dump
--rw-r--r--   0 goerz      (501) staff       (20)     1882 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_result_serialization.py
--rw-r--r--   0 goerz      (501) staff       (20)      932 2020-01-02 07:29:19.000000 krotov-1.2.1/tests/test_shapes.py
--rw-r--r--   0 goerz      (501) staff       (20)     8301 2020-10-02 06:06:14.000000 krotov-1.2.1/tests/test_structural_conversions.py
--rw-r--r--   0 goerz      (501) staff       (20)      988 2020-03-24 16:37:33.000000 krotov-1.2.1/tests/transmon_xgate_system_mod.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 krotov-1.3.0/.editorconfig
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 krotov-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 krotov-1.3.0/.pylintrc
+-rw-r--r--   0        0        0    27971 2020-02-02 00:00:00.000000 krotov-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 krotov-1.3.0/HISTORY.rst
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 krotov-1.3.0/Makefile
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 krotov-1.3.0/codecov.yml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 krotov-1.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 krotov-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 krotov-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 krotov-1.3.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 krotov-1.3.0/.github/ISSUE_TEMPLATE/related-software.md
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 krotov-1.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 krotov-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 krotov-1.3.0/binder/environment.yml
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/01_overview.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/02_contributing.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/03_authors.rst
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/04_features.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/05_history.rst
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/06_introduction.rst
+-rw-r--r--   0        0        0    31072 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/07_krotovs_method.rst
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/08_qutip_usage.rst
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/09_examples.rst
+-rw-r--r--   0        0        0    30310 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/10_howto.rst
+-rw-r--r--   0        0        0    27873 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/11_other_methods.rst
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/12_related_software.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/99_bibliography.rst
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/Makefile
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/build_pdf.py
+-rw-r--r--   0        0        0    17658 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/conf.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/conftest.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/index.rst
+-rw-r--r--   0        0        0    62800 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/krotovscheme.pdf
+-rw-r--r--   0        0        0    84892 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/krotovscheme.svg
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/krotovscheme.tex
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/nbval_sanitize.cfg
+-rw-r--r--   0        0        0    75151 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/oct_decision_tree.pdf
+-rw-r--r--   0        0        0   103242 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/oct_decision_tree.svg
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/oct_decision_tree.tex
+-rw-r--r--   0        0        0   102574 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/python37.inv
+-rw-r--r--   0        0        0    42802 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/refs.bib
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/.gitignore
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.convergence.rst
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.conversions.rst
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.functionals.rst
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.info_hooks.rst
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.mu.rst
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.objectives.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.optimize.rst
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.parallelization.rst
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.propagators.rst
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.result.rst
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.second_order.rst
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/API/krotov.shapes.rst
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/_extensions/dollarmath.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/_static/mycss.css
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/_templates/layout.html
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/_templates/module.rst
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/_templates/package.rst
+-rw-r--r--   0        0        0   381391 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/01_example_simple_state_to_state.ipynb
+-rw-r--r--   0        0        0   298003 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/02_example_lambda_system_rwa_complex_pulse.ipynb
+-rw-r--r--   0        0        0   467344 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/03_example_lambda_system_rwa_non_hermitian.ipynb
+-rw-r--r--   0        0        0   163663 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/04_example_dissipative_qubit_reset.ipynb
+-rw-r--r--   0        0        0   357347 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/05_example_transmon_xgate.ipynb
+-rw-r--r--   0        0        0   690343 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/06_example_3states.ipynb
+-rw-r--r--   0        0        0   220430 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/07_example_PE.ipynb
+-rw-r--r--   0        0        0   297104 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/08_example_ensemble.ipynb
+-rw-r--r--   0        0        0    47111 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/09_example_numpy.ipynb
+-rw-r--r--   0        0        0   566834 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/3states_opt_result.dump
+-rw-r--r--   0        0        0    22180 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/energylevels.png
+-rw-r--r--   0        0        0   138987 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/ensemble_opt_result.dump
+-rw-r--r--   0        0        0    40085 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/lambda_rwa_opt_result.dump
+-rw-r--r--   0        0        0   190975 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/non_herm_opt_result.dump
+-rw-r--r--   0        0        0    63287 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/notebooks/transmonxgate_opt_result.dump
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/pseudocode/Makefile
+-rw-r--r--   0        0        0   251477 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/pseudocode/krotov_pseudocode.pdf
+-rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 krotov-1.3.0/docs/pseudocode/krotov_pseudocode.tex
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 krotov-1.3.0/scripts/clean.py
+-rwxr-xr-x   0        0        0     2449 2020-02-02 00:00:00.000000 krotov-1.3.0/scripts/pre-commit.py
+-rw-r--r--   0        0        0    24676 2020-02-02 00:00:00.000000 krotov-1.3.0/scripts/release.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 krotov-1.3.0/src/conftest.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/__init__.py
+-rw-r--r--   0        0        0    16864 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/convergence.py
+-rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/conversions.py
+-rw-r--r--   0        0        0    21573 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/functionals.py
+-rw-r--r--   0        0        0    25189 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/info_hooks.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/mu.py
+-rw-r--r--   0        0        0    52467 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/objectives.py
+-rw-r--r--   0        0        0    36883 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/optimize.py
+-rw-r--r--   0        0        0    22873 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/parallelization.py
+-rw-r--r--   0        0        0    14352 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/propagators.py
+-rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/result.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/second_order.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 krotov-1.3.0/src/krotov/shapes.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_dump_result.py
+-rw-r--r--   0        0        0    11476 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_functionals.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_infohooks.py
+-rw-r--r--   0        0        0    18962 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_krotov.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_mu.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_numpy_controls.py
+-rw-r--r--   0        0        0    28859 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_objectives.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_overlap.py
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_parallelization.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_pulse_options.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_result_serialization.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_shapes.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_structural_conversions.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/transmon_xgate_system_mod.py
+-rw-r--r--   0        0        0   566834 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_dump_result/oct_result.dump
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_infohooks/custom_format_out.txt
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_infohooks/custom_header_out.txt
+-rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_objectives/pulse.dat
+-rw-r--r--   0        0        0    91760 2020-02-02 00:00:00.000000 krotov-1.3.0/tests/test_result_serialization/oct_result.dump
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 krotov-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 krotov-1.3.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 krotov-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 krotov-1.3.0/README.md
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 krotov-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 krotov-1.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `krotov-1.2.1/AUTHORS.rst` & `krotov-1.3.0/AUTHORS.rst`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 * `Michael Goerz`_ <mail@michaelgoerz.net>
 
 
 Development Team
 ----------------
 
-* Daniel Basilewitsch <basilewitsch@physik.uni-kassel.de>
+* Daniel Basilewitsch <daniel.basilewitsch@uibk.ac.at>
 * Fernando Gago Encinas <fernando.gago@fu-berlin.de>
 * Matthias Krauß <matthias.krauss@physik.uni-kassel.de>
 * Karl Horn <karlhorn@physik.uni-kassel.de>
 * `Daniel Reich`_ <danreich@zedat.fu-berlin.de>
 * `Christiane Koch`_ <christiane.koch@fu-berlin.de>
 
 .. _Michael Goerz: https://michaelgoerz.net
@@ -24,14 +24,15 @@
 
 
 Acknowledgements
 ----------------
 
 We thank
 `Alberto Castro`_,
+`@daviehh`_,
 `@TejasAvinasShetty`_,
 `@nathanshammah`_,
 `@timohillmann`_,
 `@loganbvh`_,
 `@uiofgh`_, and
 `@zachmanson`_,
 for reporting bugs and suggesting improvements.
@@ -39,7 +40,8 @@
 .. _Alberto Castro: https://www.bifi.es/~acastro/
 .. _@loganbvh: https://github.com/loganbvh
 .. _@zachmanson: https://github.com/zachmanson
 .. _@TejasAvinasShetty: https://github.com/TejasAvinashShetty
 .. _@nathanshammah: https://github.com/nathanshammah
 .. _@timohillmann: https://github.com/timohillmann
 .. _@uiofgh: https://github.com/uiofgh
+.. _@daviehh: https://github.com/daviehh
```

### Comparing `krotov-1.2.1/CONTRIBUTING.rst` & `krotov-1.3.0/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -68,86 +68,53 @@
 3. Add your fork as a remote.
 4. Pull in the latest changes from the master branch.
 5. Create a topic branch.
 6. Make your changes and commit them (testing locally).
 7. Push changes to the topic branch on *your* remote.
 8. Make a pull request against the base master branch through the Github website of your fork.
 
-The project uses tox_ for automated testing accross multiple versions of Python
+The project uses hatch_ for automated testing accross multiple versions of Python
 and for various development tasks such as linting and generating the
 documentation. See :ref:`DevelopmentPrerequisites` for details.
 
-There is also a ``Makefile`` that wraps around tox, for
+There is also a ``Makefile`` that wraps around ``hatch``, for
 convenience on Unix-based systems. In your checked-out clone, run
 
 .. code-block:: shell
 
     make help
 
-to see the available make targets. If you cannot use ``make``, but want to use
-``tox`` directly (e.g., on Windows), run
-
-.. code-block:: shell
-
-    tox -av
-
-to see a list of tox environments and a description. For the initial
-configuration of tox environments, you may have to run
-
-.. code-block:: shell
-
-    tox -e bootstrap
-
-in order to set up the ``tox.ini`` configuration file.
-
+to see the available make targets. If you cannot use ``make``, the ``Makefile``
+still provides a convenient reference for ``hatch`` commands that are useful
+for development.
 
 If you are a member of the `qucontrol organization`_, there is no need to fork
 ``krotov`` - you can directly pull and push to ``git@github.com:qucontrol/krotov.git``.
 
-.. _tox: https://tox.readthedocs.io
+.. _hatch: https://hatch.pypa.io/latest/
 
 .. _Aaron Meurer's Git Workflow Notes:  https://www.asmeurer.com/git-workflow/
 
 .. _qucontrol organization: https://github.com/qucontrol
 
 
 .. _DevelopmentPrerequisites:
 
 
 Development Prerequisites
 -------------------------
 
-Contributing to the package's developments requires that you have Python 3.7
-and tox_ installed. It is strongly recommended that you also have installations
-of all other supported Python versions. The recommended way to install multiple
-versions of Python at the same time is through pyenv_ (or pyenv-win_ on
-Windows).
-
-Alternatively, you may install conda_ (via the Anaconda_ or Miniconda_
-distributions, or also through pyenv_). As ``conda`` can create environments
-with any version of Python (independent of which Python version ``conda`` was
-originally installed with), this alleviates the need for managing multiple
-versions.
-The advantage of using conda_ is that you may be able to avoid installing the
-compilers necessary for Python extension packages. The disadvantage is that
-environment creation is slower and the resulting environments are bigger, and
-that you may run into occasional binary incompatibilities between conda packages.
-
-.. warning::
-   If you want to use `conda`, you must use the ``tox-conda.ini`` configuration
-   file. That is, run all ``make`` comands as e.g.
-   ``make TOXINI=tox-conda.ini test`` and ``tox`` commands as e.g.
-   ``tox -c tox-conda.ini -e py35-test,py36-test,py37-test``. Alternatively,
-   make ``tox-conda.ini`` the default by copying it to ``tox.ini``.
+Contributing to the package's developments requires that you have Python 3.8
+and hatch_ installed (tested with Hatch 1.11). It is strongly recommended that
+you also have installations of all other supported Python versions. The
+recommended way to install multiple versions of Python at the same time is
+through pyenv_ (or pyenv-win_ on Windows).
 
 .. _pyenv: https://github.com/pyenv/pyenv
 .. _pyenv-win: https://github.com/pyenv-win/pyenv-win
-.. _conda: https://conda.io/docs/
-.. _Anaconda: https://www.anaconda.com/distribution/
-.. _Miniconda: https://conda.io/en/latest/miniconda.html
 .. _QuTiP: http://qutip.org
 
 
 .. _BranchingModel:
 
 Branching Model
 ---------------
@@ -260,69 +227,68 @@
 
     make test
 
 to run the entire test suite, or
 
 .. code-block:: shell
 
-    tox -e py35-test,py36-test,py37-test
+    hatch run test
 
 if ``make`` is not available.
 
 The tests are organized in the ``tests`` subfolder. It includes python scripts
 whose name start with ``test_``, which contain functions whose names also start
 with ``test_``. Any such functions in any such files are picked up by `pytest`_
 for testing. In addition, doctests_ from any docstring or any documentation
 file (``*.rst``) are picked up (by the `pytest doctest plugin`_). Lastly, all
 :ref:`example notebooks <ContributeExamples>` are validated as a test, through
 the `nbval plugin`_.
 
 .. _test coverage: https://codecov.io/gh/qucontrol/krotov
 .. _pytest: https://docs.pytest.org/en/latest/
-.. _doctests: https://docs.python.org/3.7/library/doctest.html
+.. _doctests: https://docs.python.org/3.8/library/doctest.html
 .. _pytest doctest plugin: https://docs.pytest.org/en/latest/doctest.html
 .. _nbval plugin: https://nbval.readthedocs.io/en/latest/
 
 
 Code Style
 ----------
 
 All code must be compatible with :pep:`8`. The line length limit
 is 79 characters, although exceptions are permissible if this improves
 readability significantly.
 
 Beyond :pep:`8`, this project adopts the `Black code style`_, with
 ``--skip-string-normalization --line-length 79``. You can
-run ``make black-check`` or ``tox -e run-blackcheck`` to check adherence to the
-code style, and ``make black`` or ``tox -e run-black`` to apply it.
+run ``make black-check`` or ``hatch run lint:black-check`` to check adherence to the
+code style, and ``make black`` or ``hatch run lint:black`` to apply it.
 
 .. _Black code style: https://github.com/ambv/black/#the-black-code-style
 
 Imports within python modules must be sorted according to the isort_
-configuration in ``setup.cfg``. The command ``make isort-check`` or ``tox -e
-run-isortcheck`` checks whether all imports are sorted correctly, and ``make
-isort`` or ``tox -e run-isort`` modifies all Python modules in-place with the
-proper sorting.
+configuration in ``pyproject.toml``. The command ``make isort-check`` or
+``hatch run lint:isort-check`` checks whether all imports are sorted correctly,
+and ``make isort`` or ``hatch run lint:isort`` modifies all Python modules
+in-place with the proper sorting.
 
 .. _isort: https://github.com/timothycrosley/isort#readme
 
 The code style is enforced as part of the test suite, as well as through git
 pre-commit hooks that prevent committing code not does not meet the
 requirements. These hooks are managed through the `pre-commit framework`_.
 
 .. warning::
    After cloning the ``krotov`` repository, you should run
-   ``make bootstrap``, ``tox -e bootstrap``, or ``python scripts/bootstrap.py``
-   from within the project root folder. These set up ``tox``, and the
-   pre-commit hooks
+   ``make init``, or ``pre-commit install``
+   from within the project root folder.
 
 .. _pre-commit framework: https://pre-commit.com
 
-You may use ``make flake8-check`` or ``tox -e run-flake8`` and ``make
-pylint-check`` or ``tox -e run-pylint`` for additional checks on the code with
+You may use ``make flake8-check`` or ``hatch run lint:flake8`` and ``make
+pylint-check`` or ``hatch run lint:pylint`` for additional checks on the code with
 flake8_ and pylint_, but there is no strict requirement for a perfect score
 with either one of these linters. They only serve as a guideline for code that
 might be improved.
 
 .. _flake8: http://flake8.pycqa.org
 .. _pylint: http://pylint.pycqa.org
 
@@ -376,15 +342,15 @@
 
     make docs
 
 or
 
 .. code-block:: shell
 
-   tox -e docs
+   hatch run docs:build
 
 to generate the documentation locally.
 
 .. _Sphinx: http://www.sphinx-doc.org/en/master/
 .. _Restructured Text markup language: http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html
 .. _docstring: https://www.python.org/dev/peps/pep-0257/
 .. _"Google Style" format: http://www.sphinx-doc.org/en/master/usage/extensions/example_google.html#example-google
@@ -588,28 +554,27 @@
 .. _pip: https://pip.readthedocs.io/en/stable/
 
 
 Developers' How-Tos
 -------------------
 
 The following assumes your current working directory is a checkout of
-``krotov``, and that you have successfully run ``make test`` (which creates
-the tox environments that development relies on).
+``krotov``, and that have ``hatch`` installed on your system.
 
 
 How to run a jupyter notebook server for working on the example notebooks
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A notebook server that is isolated to the proper testing environment can be started via the Makefile::
 
     make jupyter-notebook
 
 This is equivalent to::
 
-    tox -e run-cmd -- jupyter notebook --config=/dev/null
+    hatch run -- jupyter lab
 
 You may run this with your own options, if you prefer. The
 ``--config=/dev/null`` guarantees that the notebook server is completely
 isolated. Otherwise, configuration files from your home directly (see
 `Jupyter’s Common Configuration system`_)  may influence the server. Of
 course, if you know what you're doing, you may want this.
 
@@ -620,16 +585,16 @@
 How to convert an example notebook to a script for easier debugging
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Interactive debugging in notebooks is difficult. It becomes much easier if
 you convert the notebook to a script first.  To convert a notebook to an
 (I)Python script and run it with automatic debugging, execute e.g.::
 
-    tox -e run-cmd -- jupyter nbconvert --to=python --stdout docs/notebooks/01_example_transmon_xgate.ipynb > debug.py
-    tox -e run-cmd -- ipython --pdb debug.py
+    hatch run  -- jupyter nbconvert --to=python --stdout docs/notebooks/01_example_transmon_xgate.ipynb > debug.py
+    hatch run -- ipython --pdb debug.py
 
 You can then also set a manual breakpoint by inserting the following line anywhere in the code:
 
 .. code-block:: python
 
     from IPython.terminal.debugger import set_trace; set_trace() # DEBUG
 
@@ -676,58 +641,58 @@
 How to run a subset of tests
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To run e.g. only the tests defined in ``tests/test_krotov.py``, use any of the following::
 
     make test TESTS=tests/test_krotov.py
 
-    tox -e py37-test -- tests/test_krotov.py
-
-    tox -e run-cmd -- pytest tests/test_krotov.py
+    hatch run test -- tests/test_krotov.py
 
-    .tox/py37/bin/pytest tests/test_krotov.py
+    hatch -e py38 run test -- test/test_krotov.py
 
-See the `pytest test selection docs`_ for details.
+See the `pytest test selection docs`_ for details. The ``-e py38`` selects the
+Python version to run the tests under. You may replace this with an equivalent
+name for any supported Python versions.
 
 
 How to run only as single test
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Decorate the test with e.g. ``@pytest.mark.xxx``, and then run, e.g::
 
-    tox -e run-cmd -- pytest -m xxx tests/
+    hatch run -- pytest -m xxx tests/
 
 See the `pytest documentation on markers`_ for details.
 
 
 How to run only the doctests
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Run the following::
 
-    tox -e run-cmd -- pytest --doctest-modules src
+    hatch run -- pytest --doctest-modules src
 
 
 How to go into an interactive debugger
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Optionally, install the `pdbpp` package into the testing environment, for a
 better experience::
 
-    tox -e run-cmd -- pip install pdbpp
+    hatch run -- pip install pdbpp
 
 Then:
 
 - before the line where you went to enter the debugger, insert a line::
 
     from IPython.terminal.debugger import set_trace; set_trace() # DEBUG
 
 - Run ``pytest`` with the option ``-s``, e.g.::
 
-    tox -e run-cmd -- pytest -m xxx -s tests/
+    hatch run -- pytest -m xxx -s tests/
 
 You may also see the `pytest documentation on automatic debugging`_.
 
 
 How to see the debug logger output in the example notebooks
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `krotov-1.2.1/HISTORY.rst` & `krotov-1.3.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =======
 History
 =======
 
+
+1.3.0 (2024-06-03)
+------------------
+
+* Bugfix: `∫gₐdt` and total functional were reported incorrectly (`#96`_, thanks to `@daviehh`_)
+* Bugfix: Restrict ``qutip`` to version 4. Support for ``qutip 5.0`` will be added in a later release
+* Changed: Dropped support for Python 3.5 and Python 3.6
+* Changed: The documentation will no longer be provided in PDF format
+* Changed: Development is now organized around hatch_ instead of tox_
+
+
 1.2.1 (2021-01-13)
 ------------------
 
 * Bugfix: Crash when initializing discretized numpy-array controls (`#79`_, thanks to `@loganbvh`_)
 * Bugfix: Corrected definition of co-states in Dissipative Qubit Reset example (`#80`_, thanks to `Alberto Castro`_)
 * Update: Switched Testing and Documentation deployment from Travis to Github Actions (`#82`_)
 
@@ -122,15 +133,18 @@
 .. _threadpoolctl: https://github.com/joblib/threadpoolctl
 .. _@uiofgh: https://github.com/uiofgh
 .. _@TejasAvinashShetty: https://github.com/TejasAvinashShetty
 .. _@timohillmann: https://github.com/timohillmann
 .. _@nathanshammah: https://github.com/nathanshammah
 .. _@zachmanson: https://github.com/zachmanson
 .. _@loganbvh: https://github.com/loganbvh
+.. _@daviehh: https://github.com/daviehh
 .. _Alberto Castro: https://www.bifi.es/~acastro/
+.. _hatch: https://hatch.pypa.io/latest/
+.. _tox: https://tox.wiki/en/latest/
 .. _#26: https://github.com/qucontrol/krotov/issues/26
 .. _#29: https://github.com/qucontrol/krotov/issues/29
 .. _#32: https://github.com/qucontrol/krotov/issues/32
 .. _#35: https://github.com/qucontrol/krotov/issues/35
 .. _#36: https://github.com/qucontrol/krotov/issues/36
 .. _#39: https://github.com/qucontrol/krotov/issues/39
 .. _#41: https://github.com/qucontrol/krotov/issues/41
@@ -152,7 +166,8 @@
 .. _#68: https://github.com/qucontrol/krotov/issues/68
 .. _#72: https://github.com/qucontrol/krotov/issues/72
 .. _#74: https://github.com/qucontrol/krotov/issues/74
 .. _#76: https://github.com/qucontrol/krotov/issues/76
 .. _#79: https://github.com/qucontrol/krotov/issues/79
 .. _#80: https://github.com/qucontrol/krotov/issues/80
 .. _#82: https://github.com/qucontrol/krotov/issues/82
+.. _#96: https://github.com/qucontrol/krotov/issues/96
```

### Comparing `krotov-1.2.1/LICENSE` & `krotov-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/README.rst` & `krotov-1.3.0/docs/01_overview.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 =====================
 Krotov Python Package
 =====================
 
-.. image:: https://img.shields.io/badge/github-qucontrol/krotov-blue.svg
-   :alt: Source code on Github
-   :target: https://github.com/qucontrol/krotov
-.. image:: https://img.shields.io/badge/docs-gh--pages-blue.svg
-   :alt: Documentation
-   :target: https://qucontrol.github.io/krotov
-.. image:: https://img.shields.io/pypi/v/krotov.svg
-   :alt: Krotov on the Python Package Index
-   :target: https://pypi.python.org/pypi/krotov
-.. image:: https://badges.gitter.im/qucontrol_krotov/Lobby.svg
-   :alt: Join the chat at https://gitter.im/qucontrol_krotov/Lobby
-   :target: https://gitter.im/qucontrol_krotov/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. image:: https://github.com/qucontrol/krotov/workflows/Docs/badge.svg?branch=master
-   :alt: Docs
-   :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ADocs
-.. image:: https://github.com/qucontrol/krotov/workflows/Tests/badge.svg?branch=master
-   :alt: Tests
-   :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ATests
-.. image:: https://codecov.io/gh/qucontrol/krotov/branch/master/graph/badge.svg
-   :alt: Codecov
-   :target: https://codecov.io/gh/qucontrol/krotov
-.. image:: https://img.shields.io/badge/License-BSD-green.svg
-   :alt: BSD License
-   :target: https://opensource.org/licenses/BSD-3-Clause
-.. image:: https://mybinder.org/badge_logo.svg
-   :alt: Launch Binder
-   :target: https://mybinder.org/v2/gh/qucontrol/krotov/v1.2.1?filepath=docs%2Fnotebooks
-.. image:: https://img.shields.io/badge/DOI-10.21468/SciPostPhys.7.6.080-blue.svg
-   :alt: DOI
-   :target: https://doi.org/10.21468/SciPostPhys.7.6.080
+.. only:: html
+
+   .. image:: https://img.shields.io/badge/github-qucontrol/krotov-blue.svg
+      :alt: Source code on Github
+      :target: https://github.com/qucontrol/krotov
+   .. image:: https://img.shields.io/badge/docs-gh--pages-blue.svg
+      :alt: Documentation
+      :target: https://qucontrol.github.io/krotov
+   .. image:: https://img.shields.io/pypi/v/krotov.svg
+      :alt: Krotov on the Python Package Index
+      :target: https://pypi.python.org/pypi/krotov
+   .. image:: https://github.com/qucontrol/krotov/actions/workflows/docs.yml/badge.svg?branch=master
+      :alt: Docs
+      :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ADocs
+   .. image:: https://github.com/qucontrol/krotov/actions/workflows/test.yml/badge.svg?branch=master
+      :alt: Tests
+      :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ATests
+   .. image:: https://codecov.io/gh/qucontrol/krotov/branch/master/graph/badge.svg
+      :alt: Codecov
+      :target: https://codecov.io/gh/qucontrol/krotov
+   .. image:: https://img.shields.io/badge/License-BSD-green.svg
+      :alt: BSD License
+      :target: https://opensource.org/licenses/BSD-3-Clause
+   .. image:: https://mybinder.org/badge_logo.svg
+      :alt: Launch Binder
+      :target: https://mybinder.org/v2/gh/qucontrol/krotov/v1.3.0?filepath=docs%2Fnotebooks
+   .. image:: https://img.shields.io/badge/DOI-10.21468/SciPostPhys.7.6.080-blue.svg
+      :alt: DOI
+      :target: https://doi.org/10.21468/SciPostPhys.7.6.080
+
+
 
 Python implementation of Krotov's method for quantum optimal control.
 
 This implementation follows the original implementation in the `QDYN Fortran library`_.
 
-The ``krotov`` package is built on top of `QuTiP`_.
+The :mod:`krotov` package is built on top of `QuTiP`_.
 
-Development happens on `Github`_. You can read the full documentation `online`__ or `download a PDF version`_.
+Development happens on `Github`_. You can read the full documentation `online`__.
 
 .. _Documentation: https://qucontrol.github.io/krotov
 __ Documentation_
 
-If you use the ``krotov`` package in your research, please `cite it <https://qucontrol.github.io/krotov/v1.2.1/01_overview.html#citing-the-krotov-package>`_.
+If you use the :mod:`krotov` package in your research, please :ref:`cite it <CitingKrotov>`.
 
 .. _QDYN Fortran library: https://www.qdyn-library.net
 .. _QuTiP: http://qutip.org
-.. _download a PDF version: https://github.com/qucontrol/krotov/tree/master/docs/pdf
 
 
 Purpose
 -------
 
 Optimal control is a cornerstone of quantum technology: relying not
 just on a passive understanding of quantum mechanics, but on the *active*
@@ -86,72 +86,54 @@
 * Enable the more widespread use of Krotov's method, for example in the design
   of experiments.
 
 
 Prerequisites
 -------------
 
-The Krotov package is available for Python versions >= 3.5. Its main dependency is `QuTiP`_
+The Krotov package is available for Python versions >= 3.7. Its main dependency is `QuTiP`_
 (apart from the `core packages of the Python scientific ecosystem`_).
 Thus, you should consider `QuTiP's installation instructions`_.
 
 In any case, using some sort of `virtual environment`_ is strongly encouraged.
 Most packages in the Python scientific ecosystem are now available as
-`wheels`_, making installation via `pip`_ easy. However, `QuTiP currently does
-not provide wheels`_. Thus, on systems that do not have the necessary compilers
-installed (Windows, macOS), the `conda`_ package manager provides a good solution.
-
-Assuming ``conda`` is installed (e.g. through `Miniconda`_), the following
-commands set up a virtual (conda) environment into which the Krotov package can
-then be installed:
-
-.. code-block:: shell
-
-    conda create -n qucontrolenv "python=3.7"
-    conda activate qucontrolenv
-    conda config --append channels conda-forge
-    conda install qutip
+`wheels`_, making installation via `pip`_ easy. If you need to install packages
+that do not provide compiled whels, and if you do not have the necessary
+compilers installed (Windows, macOS), the `conda`_ package manager provides a
+good solution.
 
 .. _core packages of the Python scientific ecosystem: https://www.scipy.org
 .. _QuTiP's installation instructions: http://qutip.org/docs/latest/installation.html
 .. _virtual environment: https://docs.python.org/3/glossary.html#term-virtual-environment
 .. _wheels: https://packaging.python.org/tutorials/installing-packages/#source-distributions-vs-wheels
 .. _QuTiP currently does not provide wheels: https://github.com/qutip/qutip/issues/933
 .. _conda: https://conda.io/docs/index.html
-.. _Miniconda: https://conda.io/miniconda.html
 
 
 Installation
 ------------
-To install the latest released version of ``krotov`` into your current (conda)
+
+To install the latest released version of :mod:`krotov` into your current (conda)
 environment, run this command in your terminal:
 
 .. code-block:: shell
 
     python -m pip install krotov
 
-This is the preferred method to install the ``krotov`` package, as it will always install the most recent stable release.
-
-You may also do
-
-.. code-block:: shell
-
-    python -m pip install krotov[dev,extras]
-
-to install additional development dependencies, including packages required to run the example notebooks.
+This is the preferred method to install the :mod:`krotov` package, as it will always install the most recent stable release.
 
 If you don't have `pip`_ installed, the `Python installation guide`_, respectively the `Python Packaging User Guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 .. _Python Packaging User Guide: https://packaging.python.org/tutorials/installing-packages/
 
 
-To install the latest development version of ``krotov`` from `Github`_:
+To install the latest development version of :mod:`krotov` from `Github`_:
 
 .. code-block:: shell
 
     python -m pip install git+https://github.com/qucontrol/krotov.git@master#egg=krotov
 
 .. _Github: https://github.com/qucontrol/krotov
 
@@ -163,21 +145,49 @@
 
     import krotov
     import qutip
 
 Then,
 
 1. define the necessary quantum operators and states using `QuTiP`_.
-2. create a list of objectives, as instances of
-   |krotov.Objective|_.
-3. call |krotov.optimize_pulses|_ to perform an optimization of an arbitrary
+2. create a list of objectives, as instances of :class:`krotov.Objective <krotov.objectives.Objective>`.
+3. call :func:`krotov.optimize_pulses <krotov.optimize.optimize_pulses>` to perform an optimization of an arbitrary
    number of control fields over all the objectives.
 
-.. |krotov.Objective| replace:: ``krotov.Objective``
-.. _krotov.Objective: https://qucontrol.github.io/krotov/v1.2.1/API/krotov.objectives.html#krotov.objectives.Objective
-
-.. |krotov.optimize_pulses| replace:: ``krotov.optimize_pulses``
-.. _krotov.optimize_pulses: https://qucontrol.github.io/krotov/v1.2.1/API/krotov.optimize.html#krotov.optimize.optimize_pulses
 
-See `Using Krotov with QuTiP <https://qucontrol.github.io/krotov/v1.2.1/08_qutip_usage.html#using-krotov-with-qutip>`_ and `Examples <https://qucontrol.github.io/krotov/v1.2.1/09_examples.html>`_ for details.
+See :ref:`using-krotov-with-qutip` and :ref:`krotov-example-notebooks` for details.
 
 .. _Jupyter notebook: https://jupyter.org
+
+.. _CitingKrotov:
+
+Citing the Krotov Package
+-------------------------
+
+
+.. attention::
+
+   Please cite the :mod:`krotov` package as
+
+   * \M. H. Goerz *et al*., *Krotov: A Python implementation of Krotov's method for quantum optimal control*, `SciPost Phys. 7, 080 <https://scipost.org/SciPostPhys.7.6.080>`_ (2019)
+
+You can also print this from ``krotov.__citation__``:
+
+.. doctest::
+
+   >>> print(krotov.__citation__)
+   M. H. Goerz et al., Krotov: A Python implementation of Krotov's method for quantum optimal control, SciPost Phys. 7, 080 (2019)
+
+The corresponding BibTeX entry is available in ``krotov.__bibtex__``:
+
+.. doctest::
+
+   >>> print(krotov.__bibtex__)
+   @article{GoerzSPP2019,
+       author = {Michael H. Goerz and Daniel Basilewitsch and Fernando Gago-Encinas and Matthias G. Krauss and Karl P. Horn and Daniel M. Reich and Christiane P. Koch},
+       title = {Krotov: A {Python} implementation of {Krotov's} method for quantum optimal control},
+       journal={SciPost Phys.},
+       volume={7},
+       pages={80},
+       year={2019},
+       doi={10.21468/SciPostPhys.7.6.080},
+   }
```

### Comparing `krotov-1.2.1/docs/04_features.rst` & `krotov-1.3.0/docs/04_features.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/06_introduction.rst` & `krotov-1.3.0/docs/06_introduction.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/07_krotovs_method.rst` & `krotov-1.3.0/docs/07_krotovs_method.rst`

 * *Files 2% similar despite different names*

```diff
@@ -411,14 +411,26 @@
           \Bigg\vert_{(i-1)} \\
       &= \left(\Braket{\phi^\tgt}{\phi^{(i-1)}(T)}\right) \Ket{\phi^\tgt}\,,
    \end{split}
 
 cf. :func:`krotov.functionals.chis_ss` and the :mod:`krotov.functionals` module
 in general.
 
+More precisely, the right hand side of Eq. :eq:`chi_boundary` is a `Wirtinger derivative`_. That is, if the j'th component of $\ket{\phi_k(T)}$ is the complex number $x_j + \ii y_j$ then the j'th component of $\ket{\chi_k(T)}$ is
+
+.. math::
+   :label: wirtinger_deriv
+
+    \chi_j = - \frac{1}{2} \left(\frac{\partial J_T}{\partial x_j} + \ii \frac{\partial J_T}{\partial y_j} \right)\,.
+
+Generally, though, the state $\ket{\chi_k(T)}$ can be calculated simply by fully expanding $J_T$ and treating co-states as independent variables, as in the example for $J_{T,ss}$ above. Hence the intuitive notation in Eq. :eq:`chi_boundary`.
+
+
+.. _Wirtinger derivative: https://en.wikipedia.org/wiki/Wirtinger_derivatives
+
 
 
 .. _SecondOrderUpdate:
 
 Second order update
 -------------------
 
@@ -531,15 +543,15 @@
 field (no index :math:`l`), and assuming the first-order update is
 sufficient to guarantee monotonic convergence for the chosen functional.
 For simplicity, we also assume that the Hamiltonian is linear in the
 control, so that :math:`\partial \Op{H} / \partial \epsilon(t)` is not
 time-dependent. The scheme proceeds as follows:
 
 #. Construct the states :math:`\{\ket{\chi^{(i-1)}_k(T)}\}` according to
-   Eq. :eq:`chi_boundary`. For most functionals,
+   Wirtinger derivative in Eq. :eq:`chi_boundary`. For most functionals,
    specifically any that are more than linear in the overlaps
    :math:`\tau_k` defined in Eq. :eq:`tauk`, the states
    :math:`\{\ket{\chi^{(i-1)}_k(T)}\}` depend on the states
    :math:`\{\ket{\phi^{(i-1)}_k(T)}\}` forward-propagated under the
    optimized pulse from the previous iteration, that is, the guess pulse
    in the current iteration.
```

### Comparing `krotov-1.2.1/docs/08_qutip_usage.rst` & `krotov-1.3.0/docs/08_qutip_usage.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/09_examples.rst` & `krotov-1.3.0/docs/09_examples.rst`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 
 ========
 Examples
 ========
 
 .. raw:: html
 
-    <a href="http://nbviewer.jupyter.org/github/qucontrol/krotov/blob/v1.2.1/docs/notebooks" target="_blank"><img alt="Render on nbviewer" src="https://img.shields.io/badge/render%20on-nbviewer-orange.svg" style="vertical-align:text-bottom"></a>&nbsp;<a href="https://mybinder.org/v2/gh/qucontrol/krotov/v1.2.1?filepath=docs%2Fnotebooks" target="_blank"><img alt="Launch Binder" src="https://mybinder.org/badge_logo.svg" style="vertical-align:text-bottom"></a>
+    <a href="http://nbviewer.jupyter.org/github/qucontrol/krotov/blob/v1.3.0/docs/notebooks" target="_blank"><img alt="Render on nbviewer" src="https://img.shields.io/badge/render%20on-nbviewer-orange.svg" style="vertical-align:text-bottom"></a>&nbsp;<a href="https://mybinder.org/v2/gh/qucontrol/krotov/v1.3.0?filepath=docs%2Fnotebooks" target="_blank"><img alt="Launch Binder" src="https://mybinder.org/badge_logo.svg" style="vertical-align:text-bottom"></a>
 
 .. toctree::
     :maxdepth: 1
     :glob:
 
     notebooks/*
```

### Comparing `krotov-1.2.1/docs/10_howto.rst` & `krotov-1.3.0/docs/10_howto.rst`

 * *Files 1% similar despite different names*

```diff
@@ -528,16 +528,15 @@
 
 
 
 How to parallelize the optimization
 -----------------------------------
 
 Krotov's method is inherently parallel across different objectives. See
-:mod:`krotov.parallelization`, and the
-:ref:`/notebooks/05_example_transmon_xgate.ipynb` for an example.
+:mod:`krotov.parallelization`.
 
 It is exceedingly important to ensure that you do not use any accidental nested
 parallelization. The :mod:`numpy` library is often eager to run in a
 multi-threaded mode that does not combine well with the process-based
 parallelization in :mod:`krotov.parallelization`. See
 :ref:`HowtoLimitThreadpool`.
```

### Comparing `krotov-1.2.1/docs/11_other_methods.rst` & `krotov-1.3.0/docs/11_other_methods.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/12_related_software.rst` & `krotov-1.3.0/docs/12_related_software.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.convergence.rst` & `krotov-1.3.0/docs/API/krotov.convergence.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.conversions.rst` & `krotov-1.3.0/docs/API/krotov.conversions.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.functionals.rst` & `krotov-1.3.0/docs/API/krotov.functionals.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.info_hooks.rst` & `krotov-1.3.0/docs/API/krotov.info_hooks.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.objectives.rst` & `krotov-1.3.0/docs/API/krotov.objectives.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.parallelization.rst` & `krotov-1.3.0/docs/API/krotov.parallelization.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.propagators.rst` & `krotov-1.3.0/docs/API/krotov.propagators.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.rst` & `krotov-1.3.0/docs/API/krotov.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.second_order.rst` & `krotov-1.3.0/docs/API/krotov.second_order.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/API/krotov.shapes.rst` & `krotov-1.3.0/docs/API/krotov.shapes.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/Makefile` & `krotov-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/_build/html/_images/energylevels.png` & `krotov-1.3.0/docs/notebooks/energylevels.png`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/_templates/module.rst` & `krotov-1.3.0/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/_templates/package.rst` & `krotov-1.3.0/docs/_templates/package.rst`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/docs/conf.py` & `krotov-1.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 from unittest import mock
 
 import git
+import krotov
 import pybtex.style.formatting
 import pybtex.style.formatting.unsrt
 import pybtex.style.template
 from pybtex.plugin import register_plugin as pybtex_register_plugin
 from sphinx.ext.autodoc import (
     ClassLevelDocumenter,
     InstanceAttributeDocumenter,
 )
 
-import krotov
-
 
 DOCS = Path(__file__).parent
 ROOT = DOCS / ".."
 
 sys.path.insert(0, str((DOCS / "_extensions").resolve()))
 
 exclude_patterns = [
@@ -48,30 +47,22 @@
             "-o",
             str(DOCS / "API"),
             str(DOCS / ".." / "src" / "krotov"),
         ]
     )
 
 
-# -- Generate patched README documentation ------------------------------------
-def generate_patched_readme(_):
-    shutil.copyfile(DOCS / ".." / "README.rst", DOCS / "_README.rst")
-    cmd = ["patch", str(DOCS / "_README.rst"), str(DOCS / "_README.patch")]
-    subprocess.run(cmd, check=True)
-    assert (DOCS / "_README.rst").is_file()
-
-
 # -- General configuration -----------------------------------------------------
 
 # Report broken links as warnings
 nitpicky = True
 nitpick_ignore = [("py:class", "callable")]
 
 extensions = [
-    "doctr_versions_menu",
+    "docs_versions_menu",
     "nbsphinx",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.extlinks",
     "sphinx.ext.ifconfig",
@@ -97,15 +88,15 @@
     # for :class:`multiprocessing.context.Process`. The patched files was
     # created with the help of https://sphobjinv.readthedocs.io/
     "python": ("https://docs.python.org/3.7", "python37.inv"),
     "sympy": ("https://docs.sympy.org/latest/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/reference/", None),
     "numpy": ("https://docs.scipy.org/doc/numpy/", None),
     "matplotlib": ("https://matplotlib.org/", None),
-    "qutip": ("http://qutip.org/docs/latest/", None),
+    "qutip": ("https://qutip.org/docs/4.5/", None),
     "glom": ("https://glom.readthedocs.io/en/latest/", None),
     "weylchamber": ("https://weylchamber.readthedocs.io/en/latest/", None),
     "loky": ("https://loky.readthedocs.io/en/stable/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
@@ -219,15 +210,15 @@
 latex_preamble = r"""
 \usepackage[titles]{tocloft}
 \cftsetpnumwidth {1.25cm}\cftsetrmarg{1.5cm}
 \setlength{\cftchapnumwidth}{0.75cm}
 \setlength{\cftsecindent}{\cftchapnumwidth}
 \setlength{\cftsecnumwidth}{1.25cm}
 \usepackage{emptypage}
-\usepackage{braket}
+\usepackage{braket} \newcommand{\ii}{\textnormal{i}} % imaginary i
 \newcommand{\tr}[0]{\operatorname{tr}}
 \newcommand{\diag}[0]{\operatorname{diag}}
 \newcommand{\abs}[0]{\operatorname{abs}}
 \newcommand{\pop}[0]{\operatorname{pop}}
 \newcommand{\aux}[0]{\text{aux}}
 \newcommand{\opt}[0]{\text{opt}}
 \newcommand{\tgt}[0]{\text{tgt}}
@@ -289,23 +280,23 @@
     def __init__(
         self,
         label_style=None,
         name_style=None,
         sorting_style=None,
         abbreviate_names=True,
         min_crossrefs=2,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             label_style=label_style,
             name_style=name_style,
             sorting_style=sorting_style,
             abbreviate_names=abbreviate_names,
             min_crossrefs=min_crossrefs,
-            **kwargs
+            **kwargs,
         )
 
     def format_title(self, e, which_field, as_sentence=True):
         """Set titles in italics."""
         formatted_title = pybtex.style.template.field(
             which_field, apply_func=lambda text: text.capitalize()
         )
@@ -502,15 +493,15 @@
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
-doctr_versions_menu_conf = {'menu_title': 'Docs'}
+docs_versions_menu_conf = {'menu_title': 'Docs'}
 
 # -- Options for nbsphinx -0---------------------------------------------------
 
 nbsphinx_prolog = r"""
 {% set docname = env.doc2path(env.docname, base='docs') %}
 
 .. only:: html
@@ -523,8 +514,7 @@
     "<<GIT_TAG>>", git_tag
 )
 
 
 # -----------------------------------------------------------------------------
 def setup(app):
     app.connect("builder-inited", run_apidoc)
-    app.connect("builder-inited", generate_patched_readme)
```

### Comparing `krotov-1.2.1/docs/index.rst` & `krotov-1.3.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Welcome to the Krotov package's documentation!
 ==============================================
 
-.. image:: https://img.shields.io/badge/github-qucontrol/krotov-blue.svg
-   :alt: Source code on Github
-   :target: https://github.com/qucontrol/krotov
-.. image:: https://img.shields.io/badge/docs-gh--pages-blue.svg
-   :alt: Documentation
-   :target: https://qucontrol.github.io/krotov
-.. image:: https://img.shields.io/pypi/v/krotov.svg
-   :alt: Krotov on the Python Package Index
-   :target: https://pypi.python.org/pypi/krotov
-.. image:: https://badges.gitter.im/qucontrol_krotov/Lobby.svg
-   :alt: Join the chat at https://gitter.im/qucontrol_krotov/Lobby
-   :target: https://gitter.im/qucontrol_krotov/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. image:: https://github.com/qucontrol/krotov/workflows/Docs/badge.svg?branch=master
-   :alt: Docs
-   :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ADocs
-.. image:: https://github.com/qucontrol/krotov/workflows/Tests/badge.svg?branch=master
-   :alt: Tests
-   :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ATests
-.. image:: https://codecov.io/gh/qucontrol/krotov/branch/master/graph/badge.svg
-   :alt: Codecov
-   :target: https://codecov.io/gh/qucontrol/krotov
-.. image:: https://img.shields.io/badge/License-BSD-green.svg
-   :alt: BSD License
-   :target: https://opensource.org/licenses/BSD-3-Clause
-.. image:: https://mybinder.org/badge_logo.svg
-   :alt: Launch Binder
-   :target: https://mybinder.org/v2/gh/qucontrol/krotov/v1.2.1?filepath=docs%2Fnotebooks
-.. image:: https://img.shields.io/badge/DOI-10.21468/SciPostPhys.7.6.080-blue.svg
-   :alt: DOI
-   :target: https://doi.org/10.21468/SciPostPhys.7.6.080
+.. only:: html
+
+   .. image:: https://img.shields.io/badge/github-qucontrol/krotov-blue.svg
+      :alt: Source code on Github
+      :target: https://github.com/qucontrol/krotov
+   .. image:: https://img.shields.io/badge/docs-gh--pages-blue.svg
+      :alt: Documentation
+      :target: https://qucontrol.github.io/krotov
+   .. image:: https://img.shields.io/pypi/v/krotov.svg
+      :alt: Krotov on the Python Package Index
+      :target: https://pypi.python.org/pypi/krotov
+   .. image:: https://github.com/qucontrol/krotov/actions/workflows/docs.yml/badge.svg?branch=master
+      :alt: Docs
+      :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ADocs
+   .. image:: https://github.com/qucontrol/krotov/actions/workflows/test.yml/badge.svg?branch=master
+      :alt: Tests
+      :target: https://github.com/qucontrol/krotov/actions?query=workflow%3ATests
+   .. image:: https://codecov.io/gh/qucontrol/krotov/branch/master/graph/badge.svg
+      :alt: Codecov
+      :target: https://codecov.io/gh/qucontrol/krotov
+   .. image:: https://img.shields.io/badge/License-BSD-green.svg
+      :alt: BSD License
+      :target: https://opensource.org/licenses/BSD-3-Clause
+   .. image:: https://mybinder.org/badge_logo.svg
+      :alt: Launch Binder
+      :target: https://mybinder.org/v2/gh/qucontrol/krotov/v1.3.0?filepath=docs%2Fnotebooks
+   .. image:: https://img.shields.io/badge/DOI-10.21468/SciPostPhys.7.6.080-blue.svg
+      :alt: DOI
+      :target: https://doi.org/10.21468/SciPostPhys.7.6.080
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    01_overview
```

### Comparing `krotov-1.2.1/docs/pseudocode/Makefile` & `krotov-1.3.0/docs/pseudocode/Makefile`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/src/conftest.py` & `krotov-1.3.0/src/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 This file is automatically evaluated by py.test. It ensures that we can write
 doctests without distracting import statements in the doctest.
 """
 import inspect
 from collections import OrderedDict
 
+import krotov
 import numpy
 import pytest
 
-import krotov
-
 
 @pytest.fixture(autouse=True)
 def set_doctest_env(doctest_namespace):
     doctest_namespace['numpy'] = numpy
     doctest_namespace['krotov'] = krotov
     doctest_namespace['inspect'] = inspect
     doctest_namespace['OrderedDict'] = OrderedDict
```

### Comparing `krotov-1.2.1/src/krotov/.ipynb_checkpoints/conversions-checkpoint.py` & `krotov-1.3.0/src/krotov/conversions.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,23 +29,23 @@
     if isinstance(l, list):
         return [copy.copy(h) if isinstance(h, list) else h for h in l]
     else:
         return l
 
 
 def _tlist_midpoints(tlist):
-    """Calculate array of midpoints in `tlist`"""
+    """Calculate array of midpoints in `tlist`."""
     tlist_midpoints = []
     for i in range(len(tlist) - 1):
         tlist_midpoints.append(0.5 * (tlist[i + 1] + tlist[i]))
     return np.array(tlist_midpoints)
 
 
 def _find_in_list(val, list_to_search):
-    """Return index of `val` in `list_to_search`, or -1
+    """Return index of `val` in `list_to_search`, or -1.
 
     Works even if `val` is a `numpy.ndarray`. In this case, comparison is by
     object identity.
     """
     if isinstance(val, np.ndarray):
         for i, v in enumerate(list_to_search):
             if v is val:
@@ -54,52 +54,79 @@
     else:
         try:
             return list_to_search.index(val)
         except ValueError:
             return -1
 
 
-def discretize(control, tlist, args=(None,), kwargs=None):
-    """Discretize the given `control` onto the `tlist` time grid
+def discretize(control, tlist, args=(None,), kwargs=None, via_midpoints=False):
+    """Discretize the given `control` onto the `tlist` time grid.
 
     If `control` is a callable, return array of values for `control` evaluated
-    at all points in `tlist`.  If `control` is already discretized, check that
-    the discretization matches `tlist`
+    for all points in `tlist`.  If `control` is already discretized, check that
+    the discretization matches `tlist` (by size).
 
     Args:
         control (callable or numpy.ndarray): control to be discretized. If
             callable, must take time value `t` as its first argument.
         tlist (numpy.ndarray): time grid to discretize one
         args (tuple or list): If `control` is a callable, further positional
             arguments to pass to `control`. The default passes a single value
             None, to match the requirements for a callable control function in
             QuTiP.
         kwargs (None or dict): If `control` is callable, further keyword
             arguments to pass to `control`. If None, no keyword arguments will
             be passed.
+        via_midpoints (bool): If True, sample `control` at the midpoints of
+            `tlist` (except for the initial and final values which are
+            evaluated at ``tlist[0]`` and ``tlist[1]`` to preseve exact
+            boundary conditions) and then un-average via
+            :func:`pulse_onto_tlist` to fit onto `tlist`. If False, evaluate
+            directly on `tlist`.
+
+    Note:
+        If ``via_midpoints=True``, the discretized values are generally not
+        *exactly* the result of evaluating `control` at the values of `tlist`.
+        Instead, the values are adjusted slightly to guarantee numerical
+        stability when converting between a sampling on the time grid and a
+        sampling on the mid points of the time grid intervals, as required by
+        Krotov's method, see :ref:`TimeDiscretization`.
 
     Returns:
         numpy.ndarray: Discretized array of real `control` values, same length
-            as `tlist`
+        as `tlist`
 
     Raises:
         TypeError: If `control` is not a function that takes two arguments
-            (`t`, None), or a numpy array
+            (`t`, `args`), or a numpy array
         ValueError: If `control` is numpy array of incorrect size.
     """
     warnings.filterwarnings(action="error", category=np.ComplexWarning)
     # see https://stackoverflow.com/q/54814133/152544
     if callable(control):
         if kwargs is None:
             kwargs = {}
-        # relies on np.ComplexWarning being thrown as an error
-        return np.array(
-            [float(control(t, *args, **kwargs)) for t in tlist],
-            dtype=np.float64,
-        )
+        if via_midpoints:
+            tlist_midpoints = (tlist + 0.5 * (tlist[1] - tlist[0]))[:-1]
+            tlist_midpoints[0] = tlist[0]
+            tlist_midpoints[-1] = tlist[-1]
+            pulse_on_midpoints = discretize(
+                control,
+                tlist_midpoints,
+                args=args,
+                kwargs=kwargs,
+                via_midpoints=False,
+            )
+            return pulse_onto_tlist(pulse_on_midpoints)
+        else:
+            # relies on np.ComplexWarning being thrown as an error
+            return np.array(
+                [float(control(t, *args, **kwargs)) for t in tlist],
+                dtype=np.float64,
+            )
     elif isinstance(control, (np.ndarray, list)):
         # relies on np.ComplexWarning being thrown as an error
         control = np.array([float(v) for v in control], dtype=np.float64)
         if len(control) != len(tlist):
             raise ValueError(
                 "If control is an array, it must of the same length as tlist"
             )
@@ -107,15 +134,15 @@
     else:
         raise TypeError(
             "control must be either a callable func(t, args) or a numpy array"
         )
 
 
 def extract_controls(objectives):
-    """Extract a list of (unique) controls from the `objectives`
+    """Extract a list of (unique) controls from the `objectives`.
 
     Controls are unique if they are not the same object, cf.
     `Python's is keyword`_.
 
     .. _Python's is keyword: https://docs.python.org/3/reference/expressions.html#is
 
     Args:
@@ -146,15 +173,15 @@
             assert len(item) == 2
             if item[1] is control:
                 result.append(i)
     return result
 
 
 def extract_controls_mapping(objectives, controls):
-    """Extract a map of where `controls` are used in `objectives`
+    """Extract a map of where `controls` are used in `objectives`.
 
     The result is a nested list where the first index relates to the
     `objectives`, the second index relates to the Hamiltonian (0) or the
     `c_ops` (1...), and the third index relates to the `controls`.
 
     Example:
 
@@ -224,15 +251,15 @@
                     for control in controls
                 ]
             )
     return controls_mapping
 
 
 def pulse_options_dict_to_list(pulse_options, controls):
-    """Convert `pulse_options` into a list
+    """Convert `pulse_options` into a list.
 
     Given a dict `pulse_options` that contains an options-dict
     for every control in `controls` (cf. :func:`.optimize_pulses`), return a
     list of the options-dicts in the same order as `controls`.
 
     Raises:
         ValueError: if `pulse_options` to not contain all of the `controls`
@@ -255,15 +282,15 @@
                 "The control %s does not have any associated pulse options"
                 % str(control)
             )
     return pulse_options_list
 
 
 def plug_in_pulse_values(H, pulses, mapping, time_index, conjugate=False):
-    """Plug pulse values into H
+    """Plug pulse values into H.
 
     Args:
         H (list): nested list for a QuTiP-time-dependent operator
         pulses (list): list of pulses in array format
         mapping (list): nested list: for each pulse, a list of indices in `H`
             where pulse value should be inserted
         time_index (int): Index of the value of each pulse that should be
@@ -300,15 +327,15 @@
                 H[i][1] = np.conjugate(pulse[time_index])
             else:
                 H[i][1] = pulse[time_index]
     return H
 
 
 def control_onto_interval(control):
-    """Convert control on time grid to control on time grid intervals
+    """Convert control on time grid to control on time grid intervals.
 
     Args:
         control (numpy.ndarray): values of controls on time grid
 
     Returns:
         numpy.ndarray: pulse defined on the intervals of the time grid
 
@@ -335,15 +362,15 @@
     else:
         raise ValueError(
             "Not implemented: control type %s" % control.__class__.__name__
         )
 
 
 def pulse_onto_tlist(pulse):
-    """Convert `pulse` from time-grid intervals to time-grid points
+    """Convert `pulse` from time-grid intervals to time-grid points.
 
     Args:
         pulse (numpy.ndarray): values defined on the interval of a time grid
 
     Returns:
         numpy.ndarray: values of the control defined directly on the time grid
         points. The size of the returned array is one greater than the size
```

### Comparing `krotov-1.2.1/src/krotov/__init__.py` & `krotov-1.3.0/src/krotov/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 functions for constructing control fields (guess pulses), optimization
 functionals, convergence checks, analysis tools, and propagators, as well as
 more technical routines for parallelization, low-level data conversion, and
 estimators for second-order updates.
 """
 # fmt: off
 
-__version__ = '1.2.1'
+__version__ = '1.3.0'
 
 __arxiv__ = '1902.11284'
 
 __citation__ = (
     "M. H. Goerz et al., "
     "Krotov: A Python implementation of Krotov's method for quantum optimal "
     "control, "
```

### Comparing `krotov-1.2.1/src/krotov/convergence.py` & `krotov-1.3.0/src/krotov/convergence.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
 def delta_below(
     limit,
     spec1=('info_vals', glom.T[-1]),
     spec0=('info_vals', glom.T[-2]),
     absolute_value=True,
     name=None,
-    **kwargs
+    **kwargs,
 ):
     r"""Constructor for a routine that checks if
     $\Abs{v_1 - v_0} < \varepsilon$
 
     Args:
         limit (float or str): A float value (or str-representation of a float)
             for $\varepsilon$
```

### Comparing `krotov-1.2.1/src/krotov/functionals.py` & `krotov-1.3.0/src/krotov/functionals.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,26 @@
    \Op{\chi}_k^{(i)}(T)
       = - \left.\frac{\partial J_T}
         {\partial \langle\!\langle\Op{\rho}_k\vert}
         \right\vert_{\rho^{(i)}(T)}
 
 in Liouville space, using the abstract
 Hilbert-Schmidt notation :math:`\langle\!\langle a \vert b \rangle\!\rangle
-\equiv \tr[a^\dagger b]`.
-Passing a specific `chi_constructor` results in the minimization of the final
-time functional from which that `chi_constructor` was derived.
+\equiv \tr[a^\dagger b]`. The notation on the right hand side is a `Wirtinger
+derivative`_, see Eq. :eq:`wirtinger_deriv`. Passing a specific
+`chi_constructor` results in the minimization of the final time functional from
+which that `chi_constructor` was derived.
 
 The functions in this module that evaluate functionals are intended for use
 inside a function that is passed as an `info_hook` to :func:`.optimize_pulses`.
 Thus, they calculate $J_T$ from the same keyword arguments as the `info_hook`.
 The values for $J_T$ may be used in a convergence analysis, see
 :mod:`krotov.convergence`.
+
+.. _Wirtinger derivative: https://en.wikipedia.org/wiki/Wirtinger_derivatives
 """
 import logging
 
 import numpy as np
 import qutip
 
 from .second_order import _overlap
```

### Comparing `krotov-1.2.1/src/krotov/info_hooks.py` & `krotov-1.3.0/src/krotov/info_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     shared_data,
     propagator,
     chi_constructor,
     mu,
     sigma,
     iter_start,
     iter_stop,
-    out=sys.stdout
+    out=sys.stdout,
 ):
     r"""Print full debug information about the current Krotov iteration.
 
     This routine is intended to be passed to :func:`.optimize_pulses` as
     `info_hook`, and it exemplifies the full signature of a routine suitable
     for this purpose.
 
@@ -221,15 +221,15 @@
     )
     out.write(
         "    ∫gₐ(t)dt: %s\n" % (", ".join(["%.2e" % v for v in g_a_integrals]))
     )
     out.write("    λₐ: %s\n" % (", ".join(["%.2e" % λ for λ in lambda_vals])))
     try:
         MB_per_timeslot = sum(_qobj_nbytes(state) for state in fw_states_T) / (
-            1024 ** 2
+            1024**2
         )
     except AttributeError:
         # e.g. fw_states_T = None (skip_initial_forward_propagation)
         MB_per_timeslot = 0
     out.write("    storage (bw, fw, fw0): ")
     if backward_states is None:
         out.write("None, ")
@@ -353,15 +353,15 @@
     *,
     J_T,
     show_g_a_int_per_pulse=False,
     J_T_prev=None,
     unicode=True,
     col_formats=('%d', '%.2e', '%.2e', '%.2e', '%.2e', '%.2e', '%.2e', '%d'),
     col_headers=None,
-    out=sys.stdout
+    out=sys.stdout,
 ):
     r"""Print a tabular overview of the functional values in the iteration.
 
     An example output is:
 
     .. code-block:: console
```

### Comparing `krotov-1.2.1/src/krotov/mu.py` & `krotov-1.3.0/src/krotov/mu.py`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/src/krotov/objectives.py` & `krotov-1.3.0/src/krotov/objectives.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         tlist,
         *,
         rho0=None,
         H=None,
         c_ops=None,
         e_ops=None,
         args=None,
-        **kwargs
+        **kwargs,
     ):
         """Run :func:`qutip.mesolve.mesolve` on the system of the objective.
 
         Solve the dynamics for the :attr:`H` and :attr:`c_ops` of the
         objective, starting from the objective's :attr:`initial_state`, by
         delegating to :func:`qutip.mesolve.mesolve`. Both the initial state and
         the dynamical generator for the propagation can be overridden by
@@ -328,28 +328,28 @@
             H=H,
             rho0=rho0,
             tlist=tlist,
             c_ops=c_ops,
             e_ops=e_ops,
             args=args,
             options=options,
-            **kwargs
+            **kwargs,
         )
 
     def propagate(
         self,
         tlist,
         *,
         propagator,
         rho0=None,
         H=None,
         c_ops=None,
         e_ops=None,
         args=None,
-        expect=qutip.expect
+        expect=qutip.expect,
     ):
         """Propagate the system of the objective over the entire time grid.
 
         Solve the dynamics for the `H` and `c_ops` of the objective. If `rho0`
         is not given, the `initial_state` will be propagated. This is similar
         to the :meth:`mesolve` method, but instead of using
         :func:`qutip.mesolve.mesolve`, the `propagate` function is used to go
@@ -706,15 +706,15 @@
     gate,
     H,
     *,
     c_ops=None,
     local_invariants=False,
     liouville_states_set=None,
     weights=None,
-    normalize_weights=True
+    normalize_weights=True,
 ):
     r"""Construct a list of objectives for optimizing towards a quantum gate
 
     Args:
         basis_states (list[qutip.Qobj]): A list of $n$ canonical basis states
         gate: The gate to optimize for, as a $n \times n$ matrix-like object
             (must have a `shape` attribute, and be indexable by two indices).
```

### Comparing `krotov-1.2.1/src/krotov/optimize.py` & `krotov-1.3.0/src/krotov/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     storage='array',
     parallel_map=None,
     store_all_pulses=False,
     continue_from=None,
     skip_initial_forward_propagation=False,
     norm=None,
     overlap=None,
-    limit_thread_pool=None
+    limit_thread_pool=None,
 ):
     r"""Use Krotov's method to optimize towards the given `objectives`.
 
     Optimize all time-dependent controls found in the Hamiltonians or
     Liouvillians of the given `objectives`.
 
     Args:
@@ -466,16 +466,18 @@
                     update = overlap(χ, μ(Ψ))  # ⟨χ|μ|Ψ⟩ ∈ ℂ
                     update *= chi_norms[i_obj]
                     if second_order:
                         update += 0.5 * σ * overlap(delta_phis[i_obj], μ(Ψ))
                     delta_eps[i_pulse][time_index] += update
                 λₐ = lambda_vals[i_pulse]
                 S_t = shape_arrays[i_pulse][time_index]
-                Δϵ = (S_t / λₐ) * delta_eps[i_pulse][time_index].imag  # ∈ ℝ
-                g_a_integrals[i_pulse] += abs(Δϵ) ** 2 * dt  # dt may vary!
+                Δϵ_1 = delta_eps[i_pulse][time_index].imag  # for "step size" 1
+                Δϵ = (S_t / λₐ) * Δϵ_1  # ∈ ℝ
+                g_a_integrals[i_pulse] += (S_t / λₐ) * abs(Δϵ_1) ** 2 * dt
+                # dt may vary! -- hence we've included it in each summand
                 optimized_pulses[i_pulse][time_index] += Δϵ
             # forward propagation
             fw_states = parallel_map[2](
                 _forward_propagation_step,
                 list(range(len(objectives))),
                 (
                     fw_states,
```

### Comparing `krotov-1.2.1/src/krotov/parallelization.py` & `krotov-1.3.0/src/krotov/parallelization.py`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/src/krotov/propagators.py` & `krotov-1.3.0/src/krotov/propagators.py`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/src/krotov/result.py` & `krotov-1.3.0/src/krotov/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module defining the :class:`Result` object that is returned by
 :func:`.optimize_pulses`.
 """
 import copyreg
-import datetime
 import logging
 import pickle
 import time
+from datetime import datetime, timedelta
 from textwrap import dedent
 
 from .conversions import _nested_list_shallow_copy, pulse_onto_tlist
 from .objectives import Objective, _ControlPlaceholder, _Objective_reduce
 
 
 __all__ = ['Result']
@@ -74,34 +74,37 @@
         self.all_pulses = []
         self.states = []
         self.start_local_time = None
         self.end_local_time = None
         self.message = ''
 
     def __str__(self):
+        time_delta = ""
+        try:
+            start_dt = datetime(*self.start_local_time[:6])
+            end_dt = datetime(*self.end_local_time[:6])
+            delta = timedelta(seconds=(end_dt - start_dt).total_seconds())
+            time_delta = f" ({delta})"
+        except:
+            pass
         return dedent(
             r'''
         Krotov Optimization Result
         --------------------------
         - Started at {start_local_time}
         - Number of objectives: {n_objectives}
         - Number of iterations: {n_iters}
         - Reason for termination: {message}
-        - Ended at {end_local_time} ({time_delta})
+        - Ended at {end_local_time}{time_delta}
         '''.format(
                 start_local_time=self.start_local_time_str,
                 n_objectives=len(self.objectives),
                 n_iters=len(self.iters) - 1,  # do not count zero iteration
                 end_local_time=self.end_local_time_str,
-                time_delta=str(
-                    datetime.timedelta(
-                        seconds=time.mktime(self.end_local_time)
-                        - time.mktime(self.start_local_time)
-                    )
-                ),
+                time_delta=time_delta,
                 message=self.message,
             )
         ).strip()
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `krotov-1.2.1/src/krotov/second_order.py` & `krotov-1.3.0/src/krotov/second_order.py`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/src/krotov/shapes.py` & `krotov-1.3.0/src/krotov/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     The flattop function starts at 0, and ramps to to 1 during the `t_rise`
     interval. For ``func='blackman'``, the switch-on shape is half of a
     Blackman window (see :func:`blackman`). For ``func='sinsq``, it is a
     sine-squared curve. The function then remains at value 1, before ramping
     down to 0 again during `t_fall`.
 
     Args:
-        t (float): Time  point or time grid
+        t (float): Time  point
         t_start (float): Start of flattop window
         t_stop (float): Stop of flattop window
         t_rise (float): Duration of ramp-up, starting at `t_start`
         t_fall (float): Duration of ramp-down, ending at `t_stop`.
             If not given, ``t_fall=t_rise``.
         func (str): One of 'blackman', 'sinsq'
```

### Comparing `krotov-1.2.1/tests/test_dump_result.py` & `krotov-1.3.0/tests/test_dump_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Test the dump_result convergence routine"""
 import copy
 import os
 
-import pytest
-
 import krotov
+import pytest
 
 
 def incl_range(a, b, step=1):
     e = 1 if step > 0 else -1
     return range(a, b + e, step)
 
 
+# Note: The `oct_result.dump` file was manually created from
+# docs/notebooks/01_example_simple_state_to_state.ipynb (the `opt_result`
+# variable)
+
+
 @pytest.fixture
 def oct_result_20(request):
     testdir = os.path.splitext(request.module.__file__)[0]
     filename = os.path.join(testdir, "oct_result.dump")
     return krotov.result.Result.load(filename)
```

### Comparing `krotov-1.2.1/tests/test_functionals.py` & `krotov-1.3.0/tests/test_functionals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Tests of krotov.functionals"""
 import copy
 from itertools import product
 
+import krotov
 import numpy as np
 import pytest
 import qutip
 from qutip import ket
 
-import krotov
-
 
 try:
     import qutip.qip.gates as qutip_gates
 except ImportError:
     import qutip.qip.operations.gates as qutip_gates
```

### Comparing `krotov-1.2.1/tests/test_infohooks.py` & `krotov-1.3.0/tests/test_infohooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Test for modify_params_after_iter/info_hook"""
 import contextlib
 import io
 import os
 from pathlib import Path
 
+import krotov
 import numpy as np
 import pytest
-
-import krotov
 from krotov.info_hooks import print_table
 from test_krotov import simple_state_to_state_system
 from test_objectives import transmon_ham_and_states
 
 
 def test_infohook_chaining(transmon_ham_and_states):
     """Test that transmon_ham_and_states and info_hooks get chained together
```

### Comparing `krotov-1.2.1/tests/test_krotov.py` & `krotov-1.3.0/tests/test_krotov.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import io
 import logging
 import os
 from copy import deepcopy
 from shutil import copyfile
 
-import numpy as np
-import pytest
-import qutip
 from pkg_resources import parse_version
 
 import krotov
+import numpy as np
+import pytest
+import qutip
 
 
 def test_valid_version():
     """Check that the package defines a valid __version__"""
     assert parse_version(krotov.__version__) >= parse_version("0.1.0")
```

### Comparing `krotov-1.2.1/tests/test_mu.py` & `krotov-1.3.0/tests/test_mu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Tests for krotov.mu"""
+import krotov
 import pytest
 from qutip import ket, sigmam, sigmap, sigmax, sigmaz
 
-import krotov
-
 
 @pytest.fixture
 def tls_control_system():
     """Non-trivial control system defined on a TLS"""
     eps1 = lambda t, args: 0.5
     eps2 = lambda t, args: 1
     H1 = [0.5 * sigmaz(), [sigmap(), eps1], [sigmam(), eps1]]
```

### Comparing `krotov-1.2.1/tests/test_numpy_controls.py` & `krotov-1.3.0/tests/test_numpy_controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Test using numpy controls."""
+import krotov
 import numpy as np
 import pytest
 import qutip
 
-import krotov
-
 
 @pytest.fixture
 def numpy_control_system():
     """Optimization system for State-to-State Transfer
 
     This is the same as in 01_example_simple_state_to_state.ipynb, but using a
     numpy array as the control.
```

### Comparing `krotov-1.2.1/tests/test_objectives/pulse.dat` & `krotov-1.3.0/tests/test_objectives/pulse.dat`

 * *Files identical despite different names*

### Comparing `krotov-1.2.1/tests/test_objectives.py` & `krotov-1.3.0/tests/test_objectives.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import copyreg
 import io
 import os
 import pickle
 from collections import OrderedDict
 from itertools import product
 
+import krotov
 import numpy as np
 import pytest
 import qutip
 import scipy
 from qutip import identity, ket, sigmam, sigmap, sigmax, sigmay, sigmaz, tensor
 
-import krotov
-
 
 try:
     import qutip.qip.gates as qutip_gates
 except ImportError:
     import qutip.qip.operations.gates as qutip_gates
```

### Comparing `krotov-1.2.1/tests/test_overlap.py` & `krotov-1.3.0/tests/test_overlap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import krotov
 import numpy as np
 import qutip
 from qutip import ket
 
-import krotov
-
 
 def test_overlap():
     Qmagic = (1.0 / np.sqrt(2.0)) * qutip.Qobj(
         np.array(
             [[1, 0, 0, 1j], [0, 1j, 1, 0], [0, 1j, -1, 0], [1, 0, 0, -1j]],
             dtype=np.complex128,
         ),
```

### Comparing `krotov-1.2.1/tests/test_parallelization.py` & `krotov-1.3.0/tests/test_parallelization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 """Tests of krotov.parallelization."""
 import io
 from functools import partial
 
+import krotov
 import numpy as np
 import pytest
 import qutip
 import scipy
-
-import krotov
 import transmon_xgate_system_mod
 
 
 def _func_global(x, power, *, use_sqrt=False):
     """Test function to map."""
-    y = x ** power
+    y = x**power
     if use_sqrt:
         y = np.sqrt(y)
     return y
 
 
 def test_parallel_map():
     """Test that parallel_map and serial_map give the same result."""
 
     def func(x, power, *, use_sqrt=False):
         """Test function to map."""
         # This can't be pickled so we can only map it with loky
-        y = x ** power
+        y = x**power
         if use_sqrt:
             y = np.sqrt(y)
         return y
 
     xs = [0, 1, 2, 4]
     expected = np.sqrt(np.array(xs) ** 2)
 
     ys_serial = krotov.parallelization.serial_map(
         func, xs, task_args=(2,), task_kwargs={'use_sqrt': True}
     )
     assert np.max(np.abs(ys_serial - expected)) < 1e-15
 
-    krotov.parallelization.USE_LOKY = True
-    ys_parallel = krotov.parallelization.parallel_map(
-        func, xs, task_args=(2,), task_kwargs={'use_sqrt': True}
-    )
-    assert np.max(np.abs(ys_parallel - expected)) < 1e-15
+    if krotov.parallelization._HAS_LOKY:
+        krotov.parallelization.USE_LOKY = True
+        ys_parallel = krotov.parallelization.parallel_map(
+            func, xs, task_args=(2,), task_kwargs={'use_sqrt': True}
+        )
+        assert np.max(np.abs(ys_parallel - expected)) < 1e-15
 
     krotov.parallelization.USE_LOKY = False
     ys_parallel = krotov.parallelization.parallel_map(
         _func_global, xs, task_args=(2,), task_kwargs={'use_sqrt': True}
     )
     assert np.max(np.abs(ys_parallel - expected)) < 1e-15
 
@@ -110,35 +110,38 @@
     return objectives, pulse_options, tlist
 
 
 def test_parallel_map_fw_prop_step_loky(transmon_xgate_system):
     """Test optimization with parallel_map parameter, using loky."""
     objectives, pulse_options, tlist = transmon_xgate_system
 
-    krotov.parallelization.USE_LOKY = True
-    log = io.StringIO()
-    opt_result_loky = krotov.optimize_pulses(
-        objectives,
-        pulse_options,
-        tlist,
-        propagator=krotov.propagators.expm,
-        chi_constructor=krotov.functionals.chis_re,
-        info_hook=partial(krotov.info_hooks.print_debug_information, out=log),
-        iter_stop=1,
-        skip_initial_forward_propagation=True,
-        parallel_map=(
-            krotov.parallelization.parallel_map,
-            krotov.parallelization.parallel_map,
-            krotov.parallelization.parallel_map_fw_prop_step,
-        ),
-    )
-    tau1_loky = abs(opt_result_loky.tau_vals[0][0])
-    tau2_loky = abs(opt_result_loky.tau_vals[0][1])
-    assert abs(tau1_loky - 0.9693) < 1e-3
-    assert abs(tau2_loky - 0.7743) < 1e-3
+    if krotov.parallelization._HAS_LOKY:
+        krotov.parallelization.USE_LOKY = True
+        log = io.StringIO()
+        opt_result_loky = krotov.optimize_pulses(
+            objectives,
+            pulse_options,
+            tlist,
+            propagator=krotov.propagators.expm,
+            chi_constructor=krotov.functionals.chis_re,
+            info_hook=partial(
+                krotov.info_hooks.print_debug_information, out=log
+            ),
+            iter_stop=1,
+            skip_initial_forward_propagation=True,
+            parallel_map=(
+                krotov.parallelization.parallel_map,
+                krotov.parallelization.parallel_map,
+                krotov.parallelization.parallel_map_fw_prop_step,
+            ),
+        )
+        tau1_loky = abs(opt_result_loky.tau_vals[0][0])
+        tau2_loky = abs(opt_result_loky.tau_vals[0][1])
+        assert abs(tau1_loky - 0.9693) < 1e-3
+        assert abs(tau2_loky - 0.7743) < 1e-3
 
     krotov.parallelization.USE_LOKY = False
     # in order to be pickleable, all functions must be defined in a module
     # (transmon_xgate_system_mod)
     H = transmon_xgate_system_mod.transmon_hamiltonian()
     pulse_options = {
         H[1][1]: dict(lambda_a=1, update_shape=transmon_xgate_system_mod.S)
```

### Comparing `krotov-1.2.1/tests/test_pulse_options.py` & `krotov-1.3.0/tests/test_pulse_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Tests of PulseOptions"""
+import krotov
 import numpy as np
 import pytest
 import qutip
-
-import krotov
 from krotov.optimize import _initialize_krotov_controls
 
 
 def test_shape_validation():
     """Test that OCT pulse shapes are converted and verified correctly"""
 
     H = [qutip.Qobj(), [qutip.Qobj(), lambda t, args: 0]]
```

### Comparing `krotov-1.2.1/tests/test_result_serialization.py` & `krotov-1.3.0/tests/test_result_serialization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """Test that we can serialize a Resuls object"""
-
+import copy
 import logging
 import os
 import pickle
 
 import numpy as np
-
+import pytest
 from krotov.result import Result
 
 
+def incl_range(a, b, step=1):
+    e = 1 if step > 0 else -1
+    return range(a, b + e, step)
+
+
+# Note: The `oct_result.dump` file is a copy of
+# ../docs/notebooks/3states_opt_result.dump
+
+
 def test_serialization_roundtrip(request, tmpdir, caplog):
     """Test load/dump of Result"""
     testdir = os.path.splitext(request.module.__file__)[0]
     with caplog.at_level(logging.WARNING):
         result = Result.load(os.path.join(testdir, 'oct_result.dump'))
     assert 'Result.objectives contains control placeholders' in caplog.text
     assert isinstance(result, Result)
@@ -22,29 +31,53 @@
         result2 = pickle.load(dump_fh)
     for name in result.__dict__:
         val1 = getattr(result, name)
         val2 = getattr(result2, name)
         _check_recursive_equality(val1, val2)
 
 
-def test_serialization_finalize(request, caplog):
+@pytest.fixture
+def dumpfile_unfinalized(request, tmpdir, caplog):
     testdir = os.path.splitext(request.module.__file__)[0]
-    dumpfile = os.path.join(testdir, 'oct_result_incomplete.dump')
+    with caplog.at_level(logging.WARNING):
+        result = Result.load(os.path.join(testdir, 'oct_result.dump'))
+    assert len(result.optimized_controls) == 1
+    result.optimized_controls[0] = np.concatenate(
+        (result.optimized_controls[0][0:-2], [0.0])
+    )
+    dumpfile = str(tmpdir.join('oct_result_incomplete.dump'))
+    result.dump(dumpfile)
+    return dumpfile
+
+
+def test_serialization_finalize(dumpfile_unfinalized, caplog):
+    dumpfile = dumpfile_unfinalized
     with caplog.at_level(logging.WARNING):
         result = Result.load(dumpfile)
     assert "not finalized" in caplog.text
     nt = len(result.tlist)
     assert len(result.optimized_controls[0]) == nt - 1
     result = Result.load(dumpfile, finalize=True)
     assert len(result.optimized_controls[0]) == nt
 
 
-def test_serialization_broken(request, caplog):
+@pytest.fixture
+def dumpfile_broken(request, tmpdir, caplog):
     testdir = os.path.splitext(request.module.__file__)[0]
-    dumpfile = os.path.join(testdir, 'oct_result_broken.dump')
+    with caplog.at_level(logging.WARNING):
+        result = Result.load(os.path.join(testdir, 'oct_result.dump'))
+    assert len(result.optimized_controls) == 1
+    result.optimized_controls[0] = np.array([0.0, 0.0])
+    dumpfile = str(tmpdir.join('oct_result_broken.dump'))
+    result.dump(dumpfile)
+    return dumpfile
+
+
+def test_serialization_broken(dumpfile_broken, caplog):
+    dumpfile = dumpfile_broken
     with caplog.at_level(logging.ERROR):
         Result.load(dumpfile)
     assert "incongruent" in caplog.text
 
 
 def _check_recursive_equality(val1, val2):
     if isinstance(val1, list):
```

### Comparing `krotov-1.2.1/tests/test_shapes.py` & `krotov-1.3.0/tests/test_shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Test of krotov.shape functions"""
 from functools import partial
 
 import pytest
-
 from krotov.shapes import flattop
 
 
 def test_flattop_blackman():
     """Check basic properties of a Blackman flattop shape"""
     shape = partial(flattop, t_start=10, t_stop=20, t_rise=2, func='blackman')
     assert shape(9.9) == 0
```

### Comparing `krotov-1.2.1/tests/test_structural_conversions.py` & `krotov-1.3.0/tests/test_structural_conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Test of structural conversions"""
 import logging
 from functools import partial
 
+import krotov
 import numpy as np
 import pytest
 import qutip
-
-import krotov
 from krotov.conversions import (
     discretize,
     extract_controls,
     extract_controls_mapping,
     pulse_options_dict_to_list,
 )
 from krotov.shapes import qutip_callback
```

### Comparing `krotov-1.2.1/tests/transmon_xgate_system_mod.py` & `krotov-1.3.0/tests/transmon_xgate_system_mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """The transmon_xgate_system fixture for test_parallelization.py in module
 form.
 
 This needs to be in a module so that all the functions are pickleable
 
 """
+import krotov
 import numpy as np
 import qutip
 import scipy
 
-import krotov
-
 
 def eps0(t, args):
     T = 10
     return 4 * np.exp(-40.0 * (t / T - 0.5) ** 2)
 
 
 def transmon_hamiltonian(Ec=0.386, EjEc=45, nstates=2, ng=0.0, T=10.0):
```

