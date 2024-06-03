# Comparing `tmp/gwbench-0.7.5.tar.gz` & `tmp/gwbench-0.8.0.tar.gz`

## Comparing `gwbench-0.7.5.tar` & `gwbench-0.8.0.tar`

### file list

```diff
@@ -1,78 +1,84 @@
--rw-r--r--   0        0        0     9535 2020-02-02 00:00:00.000000 gwbench-0.7.5/CHANGELOG.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 gwbench-0.7.5/requirements_conda.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gwbench-0.7.5/requirements_pip.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 gwbench-0.7.5/setup.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/__init__.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/compute_ant_pat_lpf_psd.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/generate_lambdified_functions.py
--rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/legacy_multi_network_example.py
--rw-r--r--   0        0        0     9228 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/multi_network_gw_benchmarking.py
--rw-r--r--   0        0        0     8802 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/single_network_gw_bencharking.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 gwbench-0.7.5/example_scripts/test_run.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/__init__.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/analytic_derivatives.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/antenna_pattern_np.py
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/antenna_pattern_sp.py
--rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/basic_relations.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/detector.py
--rw-r--r--   0        0        0    10613 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/detector_response_derivatives.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/err_deriv_handling.py
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/fisher_analysis_tools.py
--rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/injections.py
--rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/legacy.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/multi_network.py
--rw-r--r--   0        0        0    24202 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/network.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/psd.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/snr.py
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/utils.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/waveform.py
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_derivatives_num.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_derivatives_sym.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/__init__.py
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/a_plus.txt
--rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/a_sharp.txt
--rw-r--r--   0        0        0    87000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/advirgo_plus.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_10km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_10km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_20km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_20km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_30km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_30km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_40km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce1_40km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_10km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_10km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_20km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_20km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_30km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_30km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_40km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/ce2_40km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_20km.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_20km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_40km.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_40km_lf.txt
--rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/et.txt
--rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/et_10km_xylophone.txt
--rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/kagra_plus.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/voyager_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/noise_curves/voyager_pm.txt
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_models/__init__.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_models/lal_bbh_np.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_models/lal_bns_np.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_models/tf2_np.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_models/tf2_sp.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_models/tf2_tidal_np.py
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 gwbench-0.7.5/gwbench/wf_models/tf2_tidal_sp.py
--rw-r--r--   0        0        0  2500050 2020-02-02 00:00:00.000000 gwbench-0.7.5/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 gwbench-0.7.5/xtra_files/pypi/pyproject.toml
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 gwbench-0.7.5/xtra_files/pypi/tutorial.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gwbench-0.7.5/xtra_files/requirements_txts/requirements_conda_pre2021_09_21.txt
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 gwbench-0.7.5/xtra_files/requirements_txts/requirements_conda_pre2023_06_19.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gwbench-0.7.5/.gitignore
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 gwbench-0.7.5/AUTHORS.md
--rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 gwbench-0.7.5/LICENSE
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 gwbench-0.7.5/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 gwbench-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 gwbench-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0    14583 2020-02-02 00:00:00.000000 gwbench-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 gwbench-0.8.0/requirements_conda.txt
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 gwbench-0.8.0/requirements_pip.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 gwbench-0.8.0/setup.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/__init__.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/compute_ant_pat_lpf_psd.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/generate_lambdified_functions.py
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/legacy_multi_network_example.py
+-rw-r--r--   0        0        0     9228 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/multi_network_gw_benchmarking.py
+-rw-r--r--   0        0        0     8802 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/single_network_gw_bencharking.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 gwbench-0.8.0/example_scripts/test_run.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/__init__.py
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/analytic_derivatives.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/antenna_pattern_jx.py
+-rw-r--r--   0        0        0    13590 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/antenna_pattern_np.py
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/antenna_pattern_sp.py
+-rw-r--r--   0        0        0    31432 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/basic_relations.py
+-rw-r--r--   0        0        0    18440 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/detector.py
+-rw-r--r--   0        0        0    15493 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/detector_response_derivatives.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/err_deriv_handling.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/fisher_analysis_tools.py
+-rw-r--r--   0        0        0    37306 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/injections.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/legacy.py
+-rw-r--r--   0        0        0    23435 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/multi_network.py
+-rw-r--r--   0        0        0    37975 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/network.py
+-rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/psd.py
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/snr.py
+-rw-r--r--   0        0        0    16090 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/utils.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/waveform.py
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_derivatives_num.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_derivatives_sym.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/__init__.py
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/a_plus.txt
+-rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/a_sharp.txt
+-rw-r--r--   0        0        0    87000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/advirgo_plus.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_10km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_10km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_20km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_20km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_30km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_30km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_40km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce1_40km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_10km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_10km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_20km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_20km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_30km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_30km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_40km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/ce2_40km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_20km.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_20km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_40km.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_40km_lf.txt
+-rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/et.txt
+-rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/et_10km_xylophone.txt
+-rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/kagra_plus.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/voyager_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/noise_curves/voyager_pm.txt
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/__init__.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/lal_bbh_np.py
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/lal_bns_np.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2_jx.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2_np.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2_sp.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2_tidal.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2_tidal_jx.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2_tidal_np.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 gwbench-0.8.0/gwbench/wf_models/tf2_tidal_sp.py
+-rw-r--r--   0        0        0   126514 2020-02-02 00:00:00.000000 gwbench-0.8.0/xtra_files/gwbench_logo.png
+-rw-r--r--   0        0        0  2500050 2020-02-02 00:00:00.000000 gwbench-0.8.0/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gwbench-0.8.0/xtra_files/pypi/pyproject.toml
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 gwbench-0.8.0/xtra_files/pypi/tutorial.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gwbench-0.8.0/xtra_files/requirements_txts/requirements_conda_pre2021_09_21.txt
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 gwbench-0.8.0/xtra_files/requirements_txts/requirements_conda_pre2023_06_19.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gwbench-0.8.0/.gitignore
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 gwbench-0.8.0/AUTHORS.md
+-rw-r--r--   0        0        0    18093 2020-02-02 00:00:00.000000 gwbench-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 gwbench-0.8.0/README.md
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gwbench-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 gwbench-0.8.0/PKG-INFO
```

### Comparing `gwbench-0.7.5/example_scripts/README.md` & `gwbench-0.8.0/example_scripts/README.md`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/example_scripts/__init__.py` & `gwbench-0.8.0/example_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/example_scripts/compute_ant_pat_lpf_psd.py` & `gwbench-0.8.0/example_scripts/compute_ant_pat_lpf_psd.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,20 +24,18 @@
 
 # include earth's rotation for Fp, Fc, lpf (location phase factor)
 # (if set = 1, inj_params['Mc'] and inj_params['tc'] cannot be None)
 use_rot = 0
 
 # injection parameters (Mc, tc are only needed, if the motion of earth is relevant)
 inj_params = {
-    'Mc':    None,
-    'tc':    None,
+    'tc':    0.,
     'ra':    np.pi/4,
     'dec':   np.pi/4,
     'psi':   np.pi/4,
-    'gmst0': 0.
     }
 
 # choose frequency array
 f_lo = 1.
 f_hi = 2.**12
 df = 2.**-4
 f = np.arange(f_lo,f_hi+df,df)
```

### Comparing `gwbench-0.7.5/example_scripts/generate_lambdified_functions.py` & `gwbench-0.8.0/example_scripts/generate_lambdified_functions.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/example_scripts/legacy_multi_network_example.py` & `gwbench-0.8.0/example_scripts/legacy_multi_network_example.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/example_scripts/multi_network_gw_benchmarking.py` & `gwbench-0.8.0/example_scripts/multi_network_gw_benchmarking.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/example_scripts/single_network_gw_bencharking.py` & `gwbench-0.8.0/example_scripts/single_network_gw_bencharking.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/example_scripts/test_run.py` & `gwbench-0.8.0/example_scripts/test_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,17 +54,16 @@
     'chi2y' : 0.0,
     'chi2z' : -0.5533273077110299,
     'DL'    : 595.845227743203,
     'tc'    : 0.0,
     'phic'  : 0.0,
     'iota'  : 0.2367522187410996,
     'ra'    : 4.043179805492967,
-    'dec'   : 1.1829476432948405, 
+    'dec'   : 1.1829476432948405,
     'psi'   : 3.277322349164817,
-    'gmst0' : 0,
     }
 
 print('injections parameter: ', inj_params)
 print()
 
 # pick the desired frequency range
 f_lo = 1.
@@ -91,48 +90,38 @@
 # initialize the network with the desired detectors
 net = Network(network_spec, logger_name='3_40km_CE', logger_level='INFO')
 # pass all variables to the network
 net.set_net_vars(wf_model_name=wf_model_name, wf_other_var_dic=wf_other_var_dic,
                  f=f, inj_params=inj_params, deriv_symbs_string=deriv_symbs_string,
                  conv_log=conv_log, use_rot=use_rot)
 
-# steps that used to be necessary but are now automatically performed by the Network if necessary
-'''
-# setup antenna patterns, location phase factors, and PSDs
-net.setup_ant_pat_lpf_psds()
-# compute the detector responses and their derivatives
-net.calc_det_responses_derivs_num(step=step, method=method, order=order, num_cores=num_cores)
-# calculate the network and detector SNRs
-net.calc_snrs(only_net=only_net)
-'''
-
 # calculate the network and detector Fisher matrices, condition numbers,
-# covariance matrices, error estimates (including 90%-credible sky area 
+# covariance matrices, error estimates (including 90%-credible sky area
 # in deg), and inversion errors using numeric differentiation mehtod
 net.calc_errors(only_net=only_net, derivs='num', step=1e-9, method='central', order=2)
 
 ############################################################################
 ### Check results
 ############################################################################
 
 # stored from previous evaluation for tf2 waveform and inj_id=0
 snr  = 4324
 errs = {
-    'log_Mc'      : 0.001131,
-    'eta'         : 0.047463,
-    'chi1z'       : 0.817835,
-    'chi2z'       : 1.215632,
-    'log_DL'      : 0.018906,
-    'tc'          : 0.003484,
-    'phic'        : 9.677533,
-    'iota'        : 0.079005,
-    'ra'          : 0.001727,
-    'dec'         : 0.000214,
-    'psi'         : 0.345425,
-    'sky_area_90' : 0.004997,
+    'log_Mc'      : 0.001096,
+    'eta'         : 0.045811,
+    'chi1z'       : 0.788783,
+    'chi2z'       : 1.171784,
+    'log_DL'      : 0.023984,
+    'tc'          : 0.003352,
+    'phic'        : 9.364241,
+    'iota'        : 0.101544,
+    'ra'          : 0.000631,
+    'dec'         : 0.001108,
+    'psi'         : 0.342041,
+    'sky_area_90' : 0.010897,
     }
 
 rtol = 1e-2
 atol = 0
 print(f'\nCheck if calculated and stored values agree up to a relative error of {rtol}.')
 print(f'{"Network SNR".ljust(19)} calculated={str(net.snr).ljust(20)}   stored={str(snr).ljust(18)} agree={np.isclose(net.snr, snr, atol=atol, rtol=rtol)}.')
 for key in errs:
@@ -152,12 +141,33 @@
 net.reset_det_responses()
 net.reset_snrs()
 net.reset_errors()
 
 # perform Fisher analysis using symbolic differentiation
 net.calc_errors(only_net=only_net, derivs='sym', gen_derivs=True)
 
-print(f'\nCheck if calculated and stored value of SNR as well as numericly and symbolicly calculated errors agree up to a relative error of {rtol}.')
+rtol = 1e-1
+print(f'\nCheck if numericly and symbolicly calculated errors agree up to a relative error of {rtol}.')
 for key in errs:
     sval = net.errs[key]
     cval = errs[key]
     print(f'Error {key.ljust(13)}    numeric={str(cval).ljust(22)} symbolic={str(sval).ljust(22)} agree={np.isclose(cval, sval, atol=atol, rtol=rtol)}.')
+
+############################################################################
+### Check against jax method
+############################################################################
+
+# reset intermediate and output Network variables
+net.reset_det_responses()
+net.reset_snrs()
+net.reset_errors()
+
+# perform Fisher analysis using symbolic differentiation
+net.set_net_vars(wf_model_name='tf2_jx')
+net.calc_errors(only_net=only_net, derivs='num')
+
+rtol = 1e-1
+print(f'\nCheck if numericly calculated (numdifftools vs jax) errors agree up to a relative error of {rtol}.')
+for key in errs:
+    sval = net.errs[key]
+    cval = errs[key]
+    print(f'Error {key.ljust(13)}    numdifftools={str(cval).ljust(22)} jax={str(sval).ljust(22)} agree={np.isclose(cval, sval, atol=atol, rtol=rtol)}.')
```

### Comparing `gwbench-0.7.5/gwbench/__init__.py` & `gwbench-0.8.0/gwbench/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/detector.py` & `gwbench-0.8.0/gwbench/err_deriv_handling.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,210 +11,228 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 
-"""This module handles calculations for a single gravitational wave detector.
-
-"""
-
-from copy import copy
-
-import dill
 import numpy as np
+from scipy.integrate import simps
+from scipy.optimize import toms748
 
-import gwbench.antenna_pattern_np as ant_pat_np
-import gwbench.detector_response_derivatives as drd
-import gwbench.err_deriv_handling as edh
-import gwbench.fisher_analysis_tools as fat
-import gwbench.psd as psd
-import gwbench.snr as snr_mod
-import gwbench.utils as utils
-
-class Detector:
-
-    ###
-    #-----Init methods-----
-    def __init__(self, det_key):
-        #-----detector specification-----
-        # full detector specification, specifying technology and location, e.g. CE2-40-CBO_C
-        self.det_key = det_key
-        # detector technology and locations
-        self.tec = det_key.split('_')[0]
-        self.loc = det_key.split('_')[1]
-
-        #-----waveform and injection based quantities-----
-        # frequency array
-        self.f = None
-
-        #-----technology and location based quantities-----
-        # detector PSD
-        self.psd = None
-        # antenna pattern
-        self.Fp = None
-        self.Fc = None
-        # location phase factor
-        self.Flp = None
-
-        #-----detector reponses-----
-        # detector repsonse
-        self.hf = None
-        # derivative dictionary for detector responses
-        self.del_hf = None
-        # sympy expression of derivative dictionary for detector responses
-        self.del_hf_expr = None
-
-        #-----SNR-----
-        # SNR, SNR^2 and d(SNR^2) calculated from self.hf
-        self.snr = None
-        self.snr_sq = None
-        self.d_snr_sq = None
-
-        #-----errors-----
-        # Fisher matrix
-        self.fisher = None
-        # condition number of Fisher matrix
-        self.cond_num = None
-        # covariance matrix
-        self.cov = None
-        # dictionary containing information about the inversion error between the two matrices
-        self.inv_err = None
-        # dictionary of errors for given derivative variables
-        self.errs = None
-
-
-    ###
-    #-----Setter methods-----
-    def set_f(self, f):
-        self.f = copy(f)
-
-
-    ###
-    #-----PSDs and antenna patterns-----
-    def setup_psds(self, F_lo=-np.inf, F_hi=np.inf, user_psds=None):
-        if user_psds is None or (self.det_key not in user_psds and self.tec not in user_psds):
-            psd_file = None
-            is_asd   = None
-        elif self.det_key in user_psds:
-            psd_file = user_psds[self.det_key]['psd_file']
-            is_asd   = user_psds[self.det_key]['is_asd']
-        else:
-            psd_file = user_psds[self.tec]['psd_file']
-            is_asd   = user_psds[self.tec]['is_asd']
-        self.psd, self.f = psd.psd(self.tec,self.f,F_lo,F_hi,psd_file,is_asd)
-
-    def setup_ant_pat_lpf(self, inj_params, use_rot, user_locs=None):
-        self.Fp, self.Fc, self.Flp = ant_pat_np.antenna_pattern_and_loc_phase_fac(self.f, inj_params.get('Mc'), inj_params.get('tc'),
-            inj_params['ra'], inj_params['dec'], inj_params['psi'], inj_params['gmst0'], self.loc, use_rot, user_locs=user_locs)
-
-
-    ###
-    #-----Detector responses-----
-    def calc_det_responses(self, wf, inj_params):
-        hfp, hfc = wf.calc_wf_polarizations(self.f, inj_params)
-        self.hf = self.Flp * (hfp * self.Fp + hfc * self.Fc)
-        return self.hf, hfp, hfc
-
-    def calc_det_responses_derivs_num(self, inj_params, wf, deriv_symbs_string, deriv_variables, conv_cos, conv_log, use_rot,
-                                      step, method, order, d_order_n, user_locs, ana_deriv_symbs_string):
-        _, hfp, hfc = self.calc_det_responses(wf, inj_params)
-        self.del_hf = drd.calc_det_responses_derivs_num(self.loc, wf, deriv_symbs_string, self.f, inj_params, use_rot=use_rot, label='hf',
-                                                        step=step, method=method, order=order, d_order_n=d_order_n, user_locs=user_locs,
-                                                        ana_deriv_symbs_string=ana_deriv_symbs_string,
-                                                        ana_deriv_aux={'hf':self.hf,   'hfp':hfp,         'hfc':hfc,
-                                                                       'Fp':self.Fp,   'Fc':self.Fc,      'Flp':self.Flp,
-                                                                       'loc':self.loc, 'use_rot':use_rot, 'user_locs':user_locs})
-        self.del_hf, c_quants = edh.get_conv_del_eval_dic(self.del_hf, inj_params, conv_cos, conv_log, deriv_symbs_string)
-        inj_params, deriv_variables = edh.get_conv_inj_params_deriv_variables(c_quants, inj_params, deriv_variables)
-
-    def load_det_responses_derivs_sym(self, wf_model_name, deriv_symbs_string, use_rot, gen_derivs=None, return_bin=0,
-                                      user_lambdified_functions_path=None, logger=None):
-        self.del_hf_expr = drd.load_det_responses_derivs_sym(self.loc, wf_model_name, deriv_symbs_string, use_rot,
-                                                             gen_derivs=gen_derivs, return_bin=return_bin, logger=logger,
-                                                             user_lambdified_functions_path=user_lambdified_functions_path)
-
-    def calc_det_responses_derivs_sym(self, wf, inj_params, deriv_symbs_string, deriv_variables, conv_cos, conv_log):
-        self.calc_det_responses(wf, inj_params)
-        self.del_hf = {}
-        for deriv in self.del_hf_expr:
-            if deriv in ('variables', 'deriv_variables'): continue
-            self.del_hf[deriv] = self.del_hf_expr[deriv](self.f, **utils.get_sub_dict(inj_params, self.del_hf_expr['variables']))
-
-        self.del_hf, c_quants = edh.get_conv_del_eval_dic(self.del_hf, inj_params, conv_cos, conv_log, deriv_symbs_string)
-        inj_params, deriv_variables = edh.get_conv_inj_params_deriv_variables(c_quants, inj_params, deriv_variables)
-
-
-    ###
-    #-----SNR calculations-----
-    def calc_snrs(self, only_net):
-        snr,snr_sq = snr_mod.snr_snr_sq_freq_array(self.hf, self.psd, self.f)
-        if not only_net:
-            self.snr = snr
-            self.snr_sq = snr_sq
-        return snr_sq
-
-    def calc_snr_sq_integrand(self):
-        self.d_snr_sq = snr_mod.snr_square_integrand(self.hf, self.psd)
-
-
-    ###
-    #-----Error calculation and Fisher analysis-----
-    def calc_fisher_cov_matrices(self, only_net, cond_sup, logger=None):
-        del_hf_sub_dict = utils.get_sub_dict(self.del_hf, ('hf',), 0)
-        if not only_net:
-            self.fisher, self.cov, self.cond_num, self.inv_err = fat.calc_fisher_cov_matrices(list(del_hf_sub_dict.values()), self.psd, self.f, only_fisher=0, cond_sup=cond_sup, logger=logger, tag=self.det_key)
-            return self.fisher
-        else:
-            fisher,_,_,_ = fat.calc_fisher_cov_matrices(list(del_hf_sub_dict.values()), self.psd, self.f, only_fisher=1, cond_sup=cond_sup, logger=logger, tag=self.det_key)
-            return fisher
-
-    def calc_inv_err(self):
-        self.inv_err = fat.inv_err_from_fisher_cov(self.fisher,self.cov)
-
-    def calc_errs(self, deriv_variables):
-        self.errs = fat.get_errs_from_cov(self.cov,deriv_variables)
-
-    def calc_sky_area_90(self, deriv_variables, logger=None):
-        if self.cov is None or self.errs is None: return
-        if 'ra' in deriv_variables and ('cos_dec' in deriv_variables or 'dec' in deriv_variables):
-            if 'cos_dec' in deriv_variables: dec_str = 'cos_dec'
-            else:                                 dec_str = 'dec'
-            ra_id      = deriv_variables.index('ra')
-            dec_id     = deriv_variables.index(dec_str)
-            is_cos_dec = (dec_str == 'cos_dec')
-            self.errs['sky_area_90'] = edh.sky_area_90(self.errs['ra'],self.errs[dec_str],self.cov[ra_id,dec_id],self.inj_params['dec'],is_cos_dec)
-        else:
-            utils.log_msg(f'calc_sky_area_90: tag = {self.det_key} - Nothing done due to missing of either RA or COS_DEC (DEC) errors.', logger=logger, level='WARNING')
-
-    def calc_sky_area_90_network(self, ra_id, dec_id, dec_val, is_cos_dec, dec_str):
-        if self.cov is None or self.errs is None: return
-        self.errs['sky_area_90'] = edh.sky_area_90(self.errs['ra'],self.errs[dec_str],self.cov[ra_id,dec_id],dec_val,is_cos_dec)
-
-
-    ###
-    #-----IO methods-----
-    def print_detector(self,print_format=1):
-        if print_format:
-            sepl='-----------------------------------------------------------------------------------'
-            print()
-            print(sepl)
-            print('Printing detector.')
-            print(sepl)
-            print()
-        for key,value in vars(self).items():
-            if type(value) == dict:
-                print('Key: ',key)
-                for key in value.keys():
-                    print('',key)
-                    print('',value[key])
-                print()
-            elif value is not None:
-                print('Key: ',key)
-                print(value)
-                print()
-        if print_format:
-            print(sepl)
-            print('Printing detector done.')
-            print(sepl)
-            print()
+#-----derivative and error manipulations-----
+def convert_to_cos_derivative(deriv, param_key, param_val):
+    '''
+    Convert the partial derivative [del_X(f)] of a function [f] with respect to a parameter [X]
+    to the derivative [del_cos_X(f)] with respect to the cosine of the parameter.
+
+    Parameters
+    ----------
+    deriv : float
+        the partial derivative [del_X(f)] of the function [f] with respect to the parameter [X].
+    param_key : str
+        the name of the parameter [X].
+    param_val : float
+        the value of the parameter [X].
+
+    Returns
+    -------
+    c_deriv : float
+        the derivative [del_cos_X(f)] with respect to the cosine of the parameter.
+    c_param_key : str
+        the name of the converted parameter [cos_X].
+    c_param_val : float
+        the value of the parameter [cos_X].
+    '''
+    c_deriv     = (-1./np.sin(param_val)) * deriv
+    c_param_key = 'cos_'+param_key
+    c_param_val = np.cos(param_val)
+    return c_deriv, c_param_key, c_param_val
+
+def convert_to_log_derivative(deriv, param_key, param_val):
+    '''
+    Convert the partial derivative [del_X(f)] of a function [f] with respect to a parameter [X]
+    to the derivative [del_log_X(f)] with respect to the logarithm of the parameter.
+
+    Parameters
+    ----------
+    deriv : float
+        the partial derivative [del_X(f)] of the function [f] with respect to the parameter [X].
+    param_key : str
+        the name of the parameter [X].
+    param_val : float
+        the value of the parameter [X].
+
+    Returns
+    -------
+    c_deriv : float
+        the derivative [del_log_X(f)] with respect to the logarithm of the parameter.
+    c_param_key : str
+        the name of the converted parameter [log_X].
+    c_param_val : float
+        the value of the parameter [log_X].
+    '''
+    c_deriv     = param_val * deriv
+    c_param_key = 'log_'+param_key
+    c_param_val = np.log(param_val)
+    return c_deriv, c_param_key, c_param_val
+
+def dim_err_to_rel_err(err, param_val, param_key=None, param_kind=None):
+    '''
+    Convert the error [err] of a dimensional parameter [X] to the relative error [err_rel] with respect to the parameter [X].
+
+    Parameters
+    ----------
+    err : float
+        the error of the parameter [X].
+    param_val : float
+        the value of the parameter [X].
+    param_key : str, optional
+        the name of the parameter [X].
+    param_kind : str, optional
+        the kind of the parameter [X].
+
+    Returns
+    -------
+    err_rel : float
+        the relative error of the parameter [X].
+    '''
+    if param_key in ('M','Mc','Dl','DL','tc') or param_kind == 'dim': return np.abs(err/param_val)
+    else:                                                             return err
+
+def one_sigma_to_percent_error(percent, sigma):
+    '''
+    Convert the one-sigma error [sigma] to the percent error [percent].
+
+    Parameters
+    ----------
+    percent : float
+        the percentage desired as a fraction.
+    sigma : float
+        the one-sigma error.
+
+    Returns
+    -------
+    percent : float
+        the percent error.
+    '''
+    sigma_orders = [0, 1, 2, 3, 4, 5, 6]
+    sigma_percents = [0., 68.2689492137, 95.4499736104, 99.7300203937, 99.9936657516, 99.9999426697, 99.9999998027]
+    for i,sigma_order in enumerate(sigma_orders):
+        if percent < sigma_percents[i]: break
+
+    def func(error,percent,sigma,sigma_order):
+        x = np.linspace(0,error,sigma_order*100)
+        return percent/100/2 - simps(np.exp(-x**2/2/sigma**2)/np.sqrt(2*np.pi)/sigma,x)
+
+    if sigma_order == 1: return toms748(func,1e-2*sigma,sigma_order*sigma,args=(percent,sigma,sigma_order))
+    else:                return toms748(func,(sigma_order-1)*sigma,sigma_order*sigma,args=(percent,sigma,sigma_order))
+
+#-----Convert the evaluated derivatives according to conv_cos, conv_log-----
+def get_conv_inj_params_deriv_variables(c_quants, inj_params, deriv_variables):
+    '''
+    Convert the injected parameters and the differentiated variables string according to the conversion dictionary [c_quants].
+
+    Parameters
+    ----------
+    c_quants : dict
+        the conversion dictionary.
+    inj_params : dict
+        the injected parameters.
+    deriv_variables : list
+        the differentiation variables.
+
+    Returns
+    -------
+    inj_params : dict
+        the converted injected parameters.
+    deriv_variables : list
+        the converted differentiation variables.
+    '''
+    if c_quants == {}: return inj_params, deriv_variables
+    else:
+        for o_key in c_quants:
+            c_key = c_quants[o_key][0]
+            c_val = c_quants[o_key][1]
+
+            if c_key not in deriv_variables: deriv_variables[deriv_variables.index(o_key)] = c_key
+            inj_params[c_key] = c_val
+
+        return inj_params, deriv_variables
+
+def get_conv_del_eval_dic(del_eval_dic, params_dic, conv_cos, conv_log):
+    '''
+    Convert the evaluated derivatives according to the conversion dictionaries [conv_cos, conv_log].
+
+    Parameters
+    ----------
+    del_eval_dic : dict
+        the evaluated derivatives.
+    params_dic : dict
+        the parameters dictionary.
+    conv_cos : dict
+        the conversion dictionary for the cosine of the parameters.
+    conv_log : dict
+        the conversion dictionary for the logarithm of the parameters.
+    deriv_symbs_string : str
+        the string of the differentiation variables.
+
+    Returns
+    -------
+    conv_dic : dict
+        the converted evaluated derivatives.
+    c_quants : dict
+        the converted parameters and their values.
+    '''
+    if conv_cos is None and conv_log is None: return del_eval_dic, {}
+    else:
+        conv_dic = {}
+        c_quants = {}
+
+        for deriv in del_eval_dic:
+            key = '_'.join(deriv.split('_')[1:-1])
+            c_key = None
+
+            if   conv_cos is not None and key in conv_cos: c_deriv, c_key, c_val = convert_to_cos_derivative(del_eval_dic[deriv],key,params_dic[key])
+            elif conv_log is not None and key in conv_log: c_deriv, c_key, c_val = convert_to_log_derivative(del_eval_dic[deriv],key,params_dic[key])
+            else:                                          conv_dic[deriv]       = del_eval_dic[deriv]
+
+            if c_key is not None:
+                c_quants[key]   = (c_key, c_val)
+                prefix,suffix   = deriv.split(key)
+                n_key           = prefix + c_key + suffix
+                conv_dic[n_key] = c_deriv
+
+        return conv_dic, c_quants
+
+#-----sky area calculations-----
+def sky_area_90(ra_err, dec_err, cov_ra_dec, dec_val, is_cos_dec):
+    '''
+    Calculate the 90% credible sky area in square degrees.
+
+    Parameters
+    ----------
+    ra_err : float
+        the error of the right ascension in radians.
+    dec_err : float
+        the error of the declination in radians.
+    cov_ra_dec : float
+        the covariance between the right ascension and the declination.
+    dec_val : float
+        the value of the declination in radians.
+    is_cos_dec : bool
+        if True, the declination is in cosine.
+
+    Returns
+    -------
+    sky_area : float
+        the 90% credible sky area in square degrees.
+
+    References
+    ----------
+    [1] arXiv:1403.6915
+    [2] arXiv:gr-qc/0310125v3
+    '''
+    if is_cos_dec: trig_fac = np.abs( 1/np.tan(dec_val) )
+    else:          trig_fac = np.abs(   np.cos(dec_val) )
+    if (ra_err*dec_err)**2 > cov_ra_dec**2: return trig_fac * np.sqrt( (ra_err * dec_err)**2 - cov_ra_dec**2 ) * 2*np.pi * (180./np.pi)**2 * np.log(10)
+    else:                                   return None
```

### Comparing `gwbench-0.7.5/gwbench/detector_response_derivatives.py` & `gwbench-0.8.0/gwbench/detector_response_derivatives.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,77 +15,154 @@
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 
 import os
 
 import dill
 
+import gwbench.antenna_pattern_jx as ant_pat_jx
 import gwbench.antenna_pattern_np as ant_pat_np
 import gwbench.antenna_pattern_sp as ant_pat_sp
 import gwbench.waveform as wfc
 import gwbench.wf_derivatives_num as wfd_num
 import gwbench.wf_derivatives_sym as wfd_sym
 import gwbench.utils as utils
 
 lambdified_functions_path = os.path.join(os.getcwd(), 'lambdified_functions')
 
 def calc_det_responses_derivs_num(loc, wf, deriv_symbs_string, f_arr,
                                   params_dic, use_rot=1, label='hf',
                                   step=1e-9, method='central', order=2, d_order_n=1,
                                   user_locs=None, ana_deriv_symbs_string=None,
                                   ana_deriv_aux=None):
+    '''
+    Calculate the partial derivatives of the detector response numerically with respect to the
+    specified variables [deriv_symbs_string] at the specified location [loc] using the waveform
+    model [wf]. The partial derivatives are evaluated at params_dic and calculated using the
+    numerical method specified by [method] and [order] and the step size [step]. The derivative
+    order is specified by [d_order_n]. The user can also specify the analytic derivatives using
+    [ana_deriv_symbs_string] and the corresponding auxiliary functions [ana_deriv_aux].
+
+    Parameters
+    ----------
+    loc : str
+        The location at which the detector response is evaluated.
+    wf : Waveform
+        The waveform model object.
+    deriv_symbs_string : str
+        The string of the derivative variables.
+    f_arr : np.ndarray
+        The array of frequencies at which the detector response is evaluated.
+    params_dic : dict
+        The dictionary of the waveform model parameters.
+    use_rot : bool
+        The flag to use the rotation of the detector response.
+    label : str
+        The label of the partial derivative.
+    step : float
+        The step size for the numerical derivative.
+    method : str
+        The method for the numerical derivative.
+    order : int
+        The order of the numerical derivative.
+    d_order_n : int
+        The derivative order.
+
+    Returns
+    -------
+    dict
+        The partial derivatives of the detector response or waveform polarizatons in the form of a dictionary.
+
+    Note:
+    If the location [loc] is None, the partial derivatives of the waveform polarizations [hfp, hfc]
+    are calculated instead of the detector response.
+    The returned dictionary has the following keys: 'del_var_hf{p,c} where var is indicates the
+    variable with respect to which the derivative is calculated, and {p,c} indicates the plus or cross
+    polarization. The dictionary also contains the keys 'variables' and 'deriv_variables' which
+    indicate the variables and the derivative variables, respectively.
+    '''
 
-    wf_symbs_list    = wf.wf_symbs_string.split(' ')
     deriv_symbs_list = deriv_symbs_string.split(' ')
-    if ana_deriv_symbs_string is None: ana_deriv_symbs_list = None
+    wf_symbs_list    = wf.wf_symbs_string.split(' ')
+    ap_symbs_list    = ant_pat_np.ap_symbs_string.split(' ')
+    dr_symbs_list    = utils.reduce_symbols_strings(wf.wf_symbs_string,
+                                                    ant_pat_np.ap_symbs_string).split(' ')
+
+    if ana_deriv_symbs_string is None: ana_deriv_symbs_list = []
     else:                              ana_deriv_symbs_list = ana_deriv_symbs_string.split(' ')
 
-    if 'f' in wf_symbs_list: wf_symbs_list.remove('f')
-    if 'f' in deriv_symbs_list: deriv_symbs_list.remove('f')
+    if 'f' in deriv_symbs_list:     deriv_symbs_list.remove('f')
+    if 'f' in ana_deriv_symbs_list: ana_deriv_symbs_list.remove('f')
+    if 'f' in wf_symbs_list:        wf_symbs_list.remove('f')
+    if 'f' in ap_symbs_list:        ap_symbs_list.remove('f')
+    if 'f' in dr_symbs_list:        dr_symbs_list.remove('f')
 
-    if loc == None:
-        wf_params_list = list(utils.get_sub_dict(params_dic, wf_symbs_list).values())
+    if wf.deriv_mod == 'jax': ant_pat = ant_pat_jx
+    else:                     ant_pat = ant_pat_np
 
+    if loc is None:
         def pc_func(f_arr, *wf_params_list):
-            return wf.calc_wf_polarizations(f_arr, [ wf_params_list[wf_symbs_list.index(el)]
-                                                     for el in wf_symbs_list ])
+            return wf.calc_wf_polarizations(f_arr, wf_params_list)
 
         return wfd_num.part_deriv_hf_func(pc_func, wf_symbs_list, deriv_symbs_list, f_arr, params_dic,
-                                          pl_cr=1, compl=1, label=label,
+                                          wf.deriv_mod, pl_cr=True, compl=True, label=label,
                                           ana_deriv_symbs_list=ana_deriv_symbs_list,
                                           ana_deriv_aux=ana_deriv_aux,
                                           step=step, method=method, order=order, d_order_n=d_order_n)
 
     else:
-        ap_symbs_list = ant_pat_np.ap_symbs_string.split(' ')
-        if 'f' in ap_symbs_list: ap_symbs_list.remove('f')
-
-        dr_symbs_list  = utils.reduce_symbols_strings(wf.wf_symbs_string,
-                                                      ant_pat_np.ap_symbs_string).split(' ')
-        dr_params_list = list(utils.get_sub_dict(params_dic, dr_symbs_list).values())
+        wf_ids = [ dr_symbs_list.index(el) for el in wf_symbs_list ]
+        ap_ids = [ dr_symbs_list.index(el) for el in ap_symbs_list ]
 
         def dr_func(f_arr, *dr_params_list):
-            hfp, hfc    = wf.calc_wf_polarizations(f_arr, [ dr_params_list[dr_symbs_list.index(el)]
-                                                            for el in wf_symbs_list ])
-            Fp, Fc, Flp = ant_pat_np.antenna_pattern_and_loc_phase_fac(f_arr,
-                *[ dr_params_list[dr_symbs_list.index(el)] for el in ap_symbs_list ],
-                loc, use_rot, user_locs=user_locs)
-            return Flp * (hfp * Fp + hfc * Fc)
+            return ant_pat.detector_response(
+                *wf.calc_wf_polarizations(f_arr, [dr_params_list[idx] for idx in wf_ids]),
+                f_arr, *[dr_params_list[idx] for idx in ap_ids ], loc, use_rot, user_locs=user_locs)
 
         return wfd_num.part_deriv_hf_func(dr_func, dr_symbs_list, deriv_symbs_list, f_arr, params_dic,
-                                          pl_cr=0, compl=1, label=label,
+                                          wf.deriv_mod, pl_cr=False, compl=True, label=label,
                                           ana_deriv_symbs_list=ana_deriv_symbs_list,
                                           ana_deriv_aux=ana_deriv_aux,
                                           step=step, method=method, order=order, d_order_n=d_order_n)
 
 
 
 def generate_det_responses_derivs_sym(wf_model_name, wf_other_var_dic, deriv_symbs_string, use_rot,
                                       locs=None, user_locs=None, pl_cr=True, user_waveform=None,
                                       user_lambdified_functions_path=None, logger=None):
+    '''
+    Generate the lambdified partial derivatives of the detector response with respect to the
+    specified variables [deriv_symbs_string] at the specified locations [locs] using the waveform
+    model [wf_model_name]. The user can also specify the locations [user_locs] and the waveform
+    model [user_waveform]. The lambdified functions are stored in the directory specified by
+    [user_lambdified_functions_path].
+
+    Parameters
+    ----------
+    wf_model_name : str
+        The name of the waveform model.
+    wf_other_var_dic : dict
+        The dictionary of the waveform model variables.
+    deriv_symbs_string : str
+        The string of the derivative variables.
+    use_rot : bool
+        The flag to use the rotation of the detector response.
+    locs : list
+        The list of locations at which the detector response is evaluated.
+    user_locs : list
+        The list of user specified locations.
+    pl_cr : bool
+        The flag to generate the plus/cross polarizations.
+    user_waveform : Waveform
+        The user specified waveform model.
+    user_lambdified_functions_path : str
+        The path to the directory to store the lambdified functions.
+    logger : Logger
+        The logger object.
+    '''
 
     # initialize waveform object
     wf = wfc.Waveform(wf_model_name, wf_other_var_dic, user_waveform=user_waveform)
 
     # check that derivative variables are a subset of the detector response variables
     full_set = set( wf.wf_symbs_string.split(' ') + ant_pat_np.ap_symbs_string.split(' ') )
     sub_set  = set( deriv_symbs_string.split(' ') )
@@ -130,16 +207,16 @@
             _deriv_symbs_string = utils.remove_symbols(deriv_symbs_string, wf.wf_symbs_string)
             symbs_string        = wf.wf_symbs_string
         else:
             utils.log_msg(f'Generating lambdified derivatives for {key}.',
                           logger=logger, level='INFO')
             utils.log_msg(f'    Loading the detector response expression for {key}.',
                           logger=logger, level='INFO')
-            responses[key]      = ant_pat_sp.detector_response_expr(hfpc[0], hfpc[1], loc,
-                                                                    use_rot, user_locs=user_locs)
+            responses[key]      = ant_pat_sp.detector_response(hfpc[0], hfpc[1], loc,
+                                                               use_rot, user_locs=user_locs)
             utils.log_msg(f'    Calculating derivatives of the detector responses for: {key}.',
                           logger=logger, level='INFO')
             _deriv_symbs_string = deriv_symbs_string
             symbs_string        = utils.reduce_symbols_strings(wf.wf_symbs_string,
                                                                ant_pat_np.ap_symbs_string)
 
         if not _deriv_symbs_string:
@@ -163,14 +240,52 @@
         utils.log_msg(f'    Stored at: {file_name}', logger=logger, level='INFO')
         with open(file_name, "wb") as fi:
             dill.dump(deriv_dic, fi, recurse=True)
 
 
 def load_det_responses_derivs_sym(loc, wf_model_name, deriv_symbs_string, use_rot, gen_derivs=None,
                                   return_bin=0, user_lambdified_functions_path=None, logger=None):
+    '''
+    Load the lambdified partial derivatives of the detector response with respect to the specified
+    variables [deriv_symbs_string] at the specified location [loc] using the waveform model [wf_model_name].
+    The lambdified functions are loaded from the directory specified by [user_lambdified_functions_path].
+
+    Parameters
+    ----------
+    loc : str
+        The location at which the detector response is evaluated.
+    wf_model_name : str
+        The name of the waveform model.
+    deriv_symbs_string : str
+        The string of the derivative variables.
+    use_rot : bool
+        The flag to use the rotation of the detector response.
+    gen_derivs : dict
+        The dictionary of the generated derivatives.
+    return_bin : bool
+        The flag to return the binary file.
+    user_lambdified_functions_path : str
+        The path to the directory to store the lambdified functions.
+    logger : Logger
+        The logger object.
+
+    Returns
+    -------
+    dict:
+        The partial derivatives of the detector response in the form of a dictionary.
+
+    Note:
+    If the location [loc] is None, the partial derivatives of the waveform polarizations [hfp, hfc]
+    are loaded instead of the detector response.
+    The returned dictionary has the following keys: 'del_var_hf{p,c} where var is indicates the variable
+    with respect to which the derivative is calculated, and {p,c} indicates the plus or cross polarization.
+    The dictionary also contains the keys 'variables' and 'deriv_variables' which indicate the variables
+    and the derivative variables, respectively.
+    '''
+
     if user_lambdified_functions_path is None: _user_lambdified_functions_path = lambdified_functions_path
     file_name = f'par_deriv_WFM_{wf_model_name}_' + \
                 f'DVAR_{deriv_symbs_string.replace(" ", "_")}_ROT_{int(use_rot)}_DET_{loc}.dat'
 
     try:
         with open(os.path.join(_user_lambdified_functions_path, file_name), "rb") as fi:
             if return_bin: return fi.read()
```

### Comparing `gwbench-0.7.5/gwbench/legacy.py` & `gwbench-0.8.0/gwbench/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,18 +170,18 @@
     if logger is None: glob_logger.info(f'   {loc}')
     else:              logger.info(f'   {loc}')
     del_hf = {}
     del_hf_expr = dill.loads(del_hf_expr)
     for deriv in del_hf_expr:
         if deriv in ('variables','deriv_variables'): continue
         del_hf[deriv] = del_hf_expr[deriv](f,**utils.get_sub_dict(inj_params,del_hf_expr['variables']))
-    return edh.get_conv_del_eval_dic(del_hf,inj_params,conv_cos,conv_log, deriv_symbs_string)
+    return edh.get_conv_del_eval_dic(del_hf,inj_params,conv_cos,conv_log)
 
 
 def eval_loc_num(loc, wf, deriv_symbs_string, f, inj_params, conv_cos, conv_log, use_rot,
                  step, method, order, d_order_n, user_locs, ana_deriv_symbs_string, logger=None):
     if logger is None: glob_logger.info(f'   {loc}')
     else:              logger.info(f'   {loc}')
     del_hf = drd.calc_det_responses_derivs_num(loc, wf, deriv_symbs_string, f, inj_params, use_rot=use_rot, label='hf',
                                                step=step, method=method, order=order, d_order_n=d_order_n, user_locs=user_locs,
                                                ana_deriv_symbs_string=ana_deriv_symbs_string)
-    return edh.get_conv_del_eval_dic(del_hf,inj_params,conv_cos,conv_log, deriv_symbs_string)
+    return edh.get_conv_del_eval_dic(del_hf,inj_params,conv_cos,conv_log)
```

### Comparing `gwbench-0.7.5/gwbench/psd.py` & `gwbench-0.8.0/gwbench/psd.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,46 @@
 
 import os
 
 import scipy.interpolate as si
 from numpy import power, logical_and, inf, pi, exp, tanh, cos, sin, square, ones_like
 from pandas import read_csv
 
-from gwbench.utils import cLight
+from gwbench.utils import cLight, available_tecs
 
 noise_curves_path=os.path.join(os.path.dirname(os.path.abspath(__file__)),'noise_curves')
 
-def psd(tec,f,F_lo=-inf,F_hi=inf,psd_file=None,is_asd=None):
+def psd(tec, f, F_lo=-inf, F_hi=inf, psd_file=None, is_asd=None):
+    '''
+    Calculate the power spectral density (PSD) for a given detector or analytical PSDs specified by tec
+    given a frequency array f, and the low and high frequency cutoffs F_lo and F_hi. If a psd_file is handed over,
+    the PSD is read from that file. If is_asd is True, the ASD is returned instead of the PSD.
+
+    Parameters
+    ----------
+    tec : str
+        The name of the detector or the analytical PSD.
+    f : array
+        The frequency array.
+    F_lo : float
+        The low frequency cutoff.
+    F_hi : float
+        The high frequency cutoff.
+    psd_file : str
+        The name of the file containing the PSD.
+    is_asd : bool
+        If True, the ASD is returned instead of the PSD.
+
+    Returns
+    -------
+    np.ndarray
+        The PSD.
+    np.ndarray
+        The frequency array.
+    '''
 
     # limit the PSD to a certain freq range
     f=f[logical_and(f>=F_lo,f<=F_hi)]
 
     # if a psd file is handed over, reset the tec label
     if psd_file is not None: tec = ''
 
@@ -241,14 +268,14 @@
         asd = 1
     elif tec == 'CE2-30-PMO':
         filename = 'ce2_30km_pm.txt'
         asd = 1
     elif tec == 'CE2-40-PMO':
         filename = 'ce2_40km_pm.txt'
         asd = 1
-    else: raise ValueError(f'Specified PSD "{tec}" not known, choose from {tecs}.')
+    else: raise ValueError(f'Specified PSD "{tec}" not known, choose from {available_tecs}.')
 
     return filename, asd
 
 def check_f(tec,f,f_lo,f_hi):
     if f[-1] < f_lo: raise ValueError('The maximum frequency is below the low-frequency cutoff of the PSD for '+tec,f[-1],f_lo)
     if f[0]  > f_hi: raise ValueError('The minimum frequency is above the high-frequency cutoff of the PSD for '+tec,f[-1],f_hi)
```

### Comparing `gwbench-0.7.5/gwbench/wf_derivatives_sym.py` & `gwbench-0.8.0/gwbench/wf_derivatives_sym.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,52 +17,66 @@
 
 '''This module contains two methods that calculate the lambdified functions
 of the the derivatives as well as of the function/expression itself.
 
  Input:  sympy function/expression, string of variables, boolean that determines
          if the function/expression has one (hf) or two (hfp, hfc) outputs.
  Output: dictionary that contains the lambdified functions:
-         output['hf'] / output['hfp'], output['hfc']
          output['del_x_hf'] / output['del_x_hfp'], output['del_x_hfc']
            (x being the variable wrt which the derivative was taken)
 
  Disclaimer: These methods can be used on any sympy functions/expressions
              that have one or two outputs only (labels are set with
              gravitational waveforms in mind.
 '''
 
 from sympy import symbols, lambdify, diff
 
 # hf is a sympy expression
 def part_deriv_hf_expr(hf, symbols_string, deriv_symbs_string=None, pl_cr=0, label='hf'):
-    symb_dic = {}
-
-    for name in symbols_string.split(' '):
-        symb_dic[name] = symbols(name,real=True)
+    '''
+    Calculate the lambdified functions of the partial derivatives of the waveform expression.
 
+    Parameters
+    ----------
+    hf : sympy expression
+        the waveform expression. If it's a tuple, the first element is the plus polarization and the second element is the cross polarization
+    symbols_string : str
+        the string of variables that the function/expression depends on.
+    deriv_symbs_string : str, optional
+        the string of variables for which the derivatives are calculated, default is None.
+    pl_cr : bool, optional
+        if True, the derivatives are calculated for the plus and cross polarizations separately, default is False.
+    label : str, optional
+        the label of waveform (hf, hfp, hfc), default is 'hf'.
+
+    Returns
+    -------
+    lamdified_dic : dict
+        dictionary that contains the lambdified partial derivatives.
+    '''
+    symb_dic  = { name : symbols(name, real=True) for name in symbols_string.split(' ') }
     symb_list = list(symb_dic.values())
 
-    if deriv_symbs_string == None:
-        deriv_symbs_list = list(symb_dic.keys())
-    else:
-        deriv_symbs_list = deriv_symbs_string.split(' ')
+    if deriv_symbs_string == None: deriv_symbs_list = list(symb_dic.keys())
+    else:                          deriv_symbs_list = deriv_symbs_string.split(' ')
 
     if pl_cr:
         lamdified_dic = {}
         for name in deriv_symbs_list:
             if name == 'f': continue
 
             key_string = 'del_'+name+'_'+label+'p'
-            lamdified_dic[key_string] = lambdify(symb_list, diff(hf[0],symb_dic[name]), modules='numpy')
+            lamdified_dic[key_string] = lambdify(symb_list, diff(hf[0], symb_dic[name]), modules='numpy')
 
             key_string = 'del_'+name+'_'+label+'c'
-            lamdified_dic[key_string] = lambdify(symb_list, diff(hf[1],symb_dic[name]), modules='numpy')
+            lamdified_dic[key_string] = lambdify(symb_list, diff(hf[1], symb_dic[name]), modules='numpy')
 
     else:
         lamdified_dic = {}
         for name in deriv_symbs_list:
             if name == 'f': continue
 
             key_string = 'del_'+name+'_'+label
-            lamdified_dic[key_string] = lambdify(symb_list, diff(hf,symb_dic[name]), modules='numpy')
+            lamdified_dic[key_string] = lambdify(symb_list, diff(hf, symb_dic[name]), modules='numpy')
 
     return lamdified_dic
```

### Comparing `gwbench-0.7.5/gwbench/noise_curves/__init__.py` & `gwbench-0.8.0/gwbench/noise_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/a_plus.txt` & `gwbench-0.8.0/gwbench/noise_curves/a_plus.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/a_sharp.txt` & `gwbench-0.8.0/gwbench/noise_curves/a_sharp.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/advirgo_plus.txt` & `gwbench-0.8.0/gwbench/noise_curves/advirgo_plus.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_10km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_10km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_10km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_10km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_20km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_20km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_20km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_20km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_30km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_30km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_30km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_30km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_40km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_40km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce1_40km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce1_40km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_10km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_10km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_10km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_10km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_20km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_20km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_20km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_20km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_30km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_30km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_30km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_30km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_40km_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_40km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/ce2_40km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/ce2_40km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_20km.txt` & `gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_20km.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_20km_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_20km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_40km.txt` & `gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_40km.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/cosmic_explorer_40km_lf.txt` & `gwbench-0.8.0/gwbench/noise_curves/cosmic_explorer_40km_lf.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/et.txt` & `gwbench-0.8.0/gwbench/noise_curves/et.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/et_10km_xylophone.txt` & `gwbench-0.8.0/gwbench/noise_curves/et_10km_xylophone.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/kagra_plus.txt` & `gwbench-0.8.0/gwbench/noise_curves/kagra_plus.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/voyager_cb.txt` & `gwbench-0.8.0/gwbench/noise_curves/voyager_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/noise_curves/voyager_pm.txt` & `gwbench-0.8.0/gwbench/noise_curves/voyager_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/gwbench/wf_models/__init__.py` & `gwbench-0.8.0/gwbench/wf_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt` & `gwbench-0.8.0/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/xtra_files/pypi/pyproject.toml` & `gwbench-0.8.0/xtra_files/pypi/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gwbench"
-version = "0.7.5"
+version = "0.8.0"
 authors = [
   { name="Ssohrab Borhanian", email="sborhanian@gmail.com" },
 ]
 dependencies = [
     "astropy",
     "dill",
+    "jax",
+    "jaxlib",
     "lalsuite",
     "mpmath",
     "numdifftools",
     "numpy",
     "pandas",
     "pathos",
     "scipy",
     "sympy",
     "tqdm",
 ]
 description = "A Python package for gravitational-wave benchmarking, particularly with Fisher information matrices."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `gwbench-0.7.5/xtra_files/pypi/tutorial.md` & `gwbench-0.8.0/xtra_files/pypi/tutorial.md`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.5/LICENSE` & `gwbench-0.8.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- GNU GENERAL PUBLIC LICENSE
+                     GNU GENERAL PUBLIC LICENSE
                        Version 2, June 1991
 
  Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
  51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
@@ -273,8 +273,67 @@
 INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
 OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
 TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
 YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
 PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGES.
 
-                     END OF TERMS AND CONDITIONS
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software; you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation; either version 2 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License along
+    with this program; if not, write to the Free Software Foundation, Inc.,
+    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If the program is interactive, make it output a short notice like this
+when it starts in an interactive mode:
+
+    Gnomovision version 69, Copyright (C) year name of author
+    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, the commands you use may
+be called something other than `show w' and `show c'; they could even be
+mouse-clicks or menu items--whatever suits your program.
+
+You should also get your employer (if you work as a programmer) or your
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary.  Here is a sample; alter the names:
+
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
+  `Gnomovision' (which makes passes at compilers) written by James Hacker.
+
+  <signature of Ty Coon>, 1 April 1989
+  Ty Coon, President of Vice
+
+This General Public License does not permit incorporating your program into
+proprietary programs.  If your program is a subroutine library, you may
+consider it more useful to permit linking proprietary applications with the
+library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.
```

### Comparing `gwbench-0.7.5/README.md` & `gwbench-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 which conda
 ```
 
 The last line should print `/cvmfs/oasis.opensciencegrid.org/ligo/sw/conda/condabin/conda` or similar.
 
 #### Setup conda virtual environment
 ```
-conda create -y --name gwbench python=3.7  
+conda create -y --name gwbench python=3.9  
 conda activate gwbench  
 conda install -y -c conda-forge --file requirements_conda.txt  
 ```
 
 ### Using `python -m venv` and pip
 Replace `~/gwbench` with the appropriate path of choice in the following instructions:
 ```
@@ -64,9 +64,9 @@
 ```
 pip uninstall gwbench
 ```
 
 ### Test
 ```
 cd example_scripts  
-python quick_start.py
+python test_run.py
 ```
```

### Comparing `gwbench-0.7.5/pyproject.toml` & `gwbench-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gwbench"
-version = "0.7.5"
+version = "0.8.0"
 authors = [
   { name="Ssohrab Borhanian", email="sborhanian@gmail.com" },
 ]
 dependencies = [
     "astropy",
     "dill",
+    "jax",
+    "jaxlib",
     "lalsuite",
     "mpmath",
     "numdifftools",
     "numpy",
     "pandas",
     "pathos",
     "scipy",
     "sympy",
     "tqdm",
 ]
 description = "A Python package for gravitational-wave benchmarking, particularly with Fisher information matrices."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `gwbench-0.7.5/PKG-INFO` & `gwbench-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gwbench
-Version: 0.7.5
+Version: 0.8.0
 Summary: A Python package for gravitational-wave benchmarking, particularly with Fisher information matrices.
 Project-URL: Homepage, https://gitlab.com/sborhanian/gwbench
 Project-URL: Bug Tracker, https://gitlab.com/sborhanian/gwbench/-/issues
 Author-email: Ssohrab Borhanian <sborhanian@gmail.com>
 License-File: AUTHORS.md
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: astropy
 Requires-Dist: dill
+Requires-Dist: jax
+Requires-Dist: jaxlib
 Requires-Dist: lalsuite
 Requires-Dist: mpmath
 Requires-Dist: numdifftools
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pathos
 Requires-Dist: scipy
@@ -63,15 +65,15 @@
 which conda
 ```
 
 The last line should print `/cvmfs/oasis.opensciencegrid.org/ligo/sw/conda/condabin/conda` or similar.
 
 #### Setup conda virtual environment
 ```
-conda create -y --name gwbench python=3.7  
+conda create -y --name gwbench python=3.9  
 conda activate gwbench  
 conda install -y -c conda-forge --file requirements_conda.txt  
 ```
 
 ### Using `python -m venv` and pip
 Replace `~/gwbench` with the appropriate path of choice in the following instructions:
 ```
@@ -90,9 +92,9 @@
 ```
 pip uninstall gwbench
 ```
 
 ### Test
 ```
 cd example_scripts  
-python quick_start.py
+python test_run.py
 ```
```

