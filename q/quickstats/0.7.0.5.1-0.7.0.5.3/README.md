# Comparing `tmp/quickstats-0.7.0.5.1.tar.gz` & `tmp/quickstats-0.7.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.7.0.5.1.tar", last modified: Mon Jun  3 08:47:48 2024, max compression
+gzip compressed data, was "quickstats-0.7.0.5.3.tar", last modified: Mon Jun  3 11:14:05 2024, max compression
```

## Comparing `quickstats-0.7.0.5.1.tar` & `quickstats-0.7.0.5.3.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.1/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:37.000000 quickstats-0.7.0.5.1/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.1/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:37.000000 quickstats-0.7.0.5.1/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-18 15:35:29.000000 quickstats-0.7.0.5.1/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       27 2024-06-03 08:47:15.000000 quickstats-0.7.0.5.1/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/algorithms/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.1/quickstats/algorithms/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/BaseMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/BisectionMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/NovelMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/SteppingMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-18 15:35:43.000000 quickstats-0.7.0.5.1/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7392 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3889 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21365 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/config_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41355 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1311 2024-04-18 15:36:08.000000 quickstats-0.7.0.5.1/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85926 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-05-31 12:42:29.000000 quickstats-0.7.0.5.1/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9290 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    33429 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:39.000000 quickstats-0.7.0.5.1/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23632 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/clis/likelihood_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-04-18 15:43:10.000000 quickstats-0.7.0.5.1/quickstats/clis/nuisance_parameter_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/processor_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/clis/stat_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.5.1/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:41.000000 quickstats-0.7.0.5.1/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1113 2024-04-18 15:39:11.000000 quickstats-0.7.0.5.1/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15274 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/caching_nll_wrapper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/discrete_nuisance.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-04-18 15:34:25.000000 quickstats-0.7.0.5.1/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14097 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.1/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:42.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:42.000000 quickstats-0.7.0.5.1/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-04-18 15:34:50.000000 quickstats-0.7.0.5.1/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:42.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1457 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      358 2024-04-18 15:36:38.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/formatter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1608 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2360 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_hdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2037 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1589 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_parquet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4421 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1049 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_cache.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1826 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-04-18 15:34:47.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1903 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2249 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_output_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-04-18 15:34:47.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_progressbar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1854 2024-04-18 15:36:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      723 2024-04-18 15:36:56.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1770 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1433 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-04-18 15:34:23.000000 quickstats-0.7.0.5.1/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12481 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/roo_process_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15637 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-18 15:35:39.000000 quickstats-0.7.0.5.1/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:43.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-04-18 15:34:27.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-18 15:35:40.000000 quickstats-0.7.0.5.1/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.5.1/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5285 2024-04-18 15:36:29.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10852 2024-04-18 15:36:29.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7694 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_significance.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      411 2024-04-18 15:36:36.000000 quickstats-0.7.0.5.1/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32252 2024-04-18 15:36:37.000000 quickstats-0.7.0.5.1/quickstats/core/configuration.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-18 15:35:34.000000 quickstats-0.7.0.5.1/quickstats/core/constraints.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4603 2024-04-18 15:36:10.000000 quickstats-0.7.0.5.1/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7569 2024-04-18 15:36:10.000000 quickstats-0.7.0.5.1/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7710 2024-06-03 07:36:21.000000 quickstats-0.7.0.5.1/quickstats/core/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-18 15:36:02.000000 quickstats-0.7.0.5.1/quickstats/core/metaclasses.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7624 2024-04-18 15:39:09.000000 quickstats-0.7.0.5.1/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18907 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-18 15:35:28.000000 quickstats-0.7.0.5.1/quickstats/core/setup.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-18 15:36:06.000000 quickstats-0.7.0.5.1/quickstats/core/type_validation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-04-18 15:35:28.000000 quickstats-0.7.0.5.1/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/daq/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      151 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6933 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/remote_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3849 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/servicex_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2553 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/xrootd_source.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/extensions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/extensions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/extensions/extension_dataframe.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:35:04.000000 quickstats-0.7.0.5.1/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      198 2024-04-18 15:39:03.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/basic_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/kerberos/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      109 2024-04-18 15:39:14.000000 quickstats-0.7.0.5.1/quickstats/interface/kerberos/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1709 2024-04-18 15:39:14.000000 quickstats-0.7.0.5.1/quickstats/interface/kerberos/core.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/ModelConfig.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11422 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RDataFrame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsArg.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-04-18 15:34:20.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TChain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11390 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5813 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TH3.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-04-18 15:34:42.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      748 2024-04-18 15:39:11.000000 quickstats-0.7.0.5.1/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.5.1/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.5.1/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      163 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5409 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2872 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/core.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/tinydb/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       67 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/tinydb/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      947 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/tinydb/methods.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      149 2024-04-18 15:39:06.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      448 2024-04-18 15:39:06.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5850 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/filesystem.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1163 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/path.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/xrd_helper.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:37.000000 quickstats-0.7.0.5.1/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-04-18 15:34:34.000000 quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.5.1/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12211 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.1/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    40281 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.1/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.5.1/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.5.1/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/parsers/param_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/parsers/roo_param_setup_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1391 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.1/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27356 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14144 2024-04-18 15:38:50.000000 quickstats-0.7.0.5.1/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.5.1/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-04-18 15:35:22.000000 quickstats-0.7.0.5.1/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6579 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7791 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4061 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/general_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22203 2024-04-18 15:41:03.000000 quickstats-0.7.0.5.1/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6078 2024-04-18 15:38:56.000000 quickstats-0.7.0.5.1/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16926 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25684 2024-04-18 15:41:03.000000 quickstats-0.7.0.5.1/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5096 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10353 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30687 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13785 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/two_axis_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.1/quickstats/plots/two_panel_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9999 2024-04-18 15:42:16.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19292 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13182 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23227 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    34454 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/default_workspace_extensions.json
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/hep.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/science.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.5.1/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19773 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.5.1/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18666 2024-04-18 15:39:08.000000 quickstats-0.7.0.5.1/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.5.1/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3039 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/utils/path_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-04-18 15:35:24.000000 quickstats-0.7.0.5.1/quickstats/utils/py_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27521 2024-04-18 15:36:12.000000 quickstats-0.7.0.5.1/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15330 2024-04-18 15:36:32.000000 quickstats-0.7.0.5.1/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15638 2024-04-18 15:39:31.000000 quickstats-0.7.0.5.1/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2321 2024-04-18 15:36:21.000000 quickstats-0.7.0.5.1/quickstats/utils/sys_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-18 15:35:57.000000 quickstats-0.7.0.5.1/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11106 2024-06-03 08:47:36.000000 quickstats-0.7.0.5.1/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-04-18 15:34:33.000000 quickstats-0.7.0.5.1/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:05.000000 quickstats-0.7.0.5.3/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-06-03 11:14:05.000000 quickstats-0.7.0.5.3/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.3/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.3/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-18 15:35:29.000000 quickstats-0.7.0.5.3/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       26 2024-06-03 11:13:33.000000 quickstats-0.7.0.5.3/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/algorithms/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.3/quickstats/algorithms/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/algorithms/nll_crossing/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/algorithms/nll_crossing/BaseMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/algorithms/nll_crossing/BisectionMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/algorithms/nll_crossing/NovelMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/algorithms/nll_crossing/SteppingMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/algorithms/nll_crossing/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-18 15:35:43.000000 quickstats-0.7.0.5.3/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7392 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3887 2024-06-03 09:42:10.000000 quickstats-0.7.0.5.3/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21365 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/analysis/config_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41355 2024-06-03 09:35:56.000000 quickstats-0.7.0.5.3/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1311 2024-04-18 15:36:08.000000 quickstats-0.7.0.5.3/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85926 2024-06-03 11:12:52.000000 quickstats-0.7.0.5.3/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-05-31 12:42:29.000000 quickstats-0.7.0.5.3/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9290 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    33429 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.3/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23632 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.3/quickstats/clis/likelihood_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-04-18 15:43:10.000000 quickstats-0.7.0.5.3/quickstats/clis/nuisance_parameter_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.3/quickstats/clis/processor_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/clis/stat_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.5.3/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1113 2024-04-18 15:39:11.000000 quickstats-0.7.0.5.3/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15274 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.3/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/caching_nll_wrapper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/discrete_nuisance.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.3/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-04-18 15:34:25.000000 quickstats-0.7.0.5.3/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14097 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.3/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.3/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.3/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.3/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.3/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-04-18 15:34:50.000000 quickstats-0.7.0.5.3/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1457 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      358 2024-04-18 15:36:38.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/formatter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1608 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2492 2024-06-03 09:12:02.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_as_hdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2037 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1589 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_as_parquet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4421 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1049 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_cache.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1826 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-04-18 15:34:47.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1903 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2249 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_output_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-04-18 15:34:47.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_progressbar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1854 2024-04-18 15:36:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      723 2024-04-18 15:36:56.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1770 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1433 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-04-18 15:34:23.000000 quickstats-0.7.0.5.3/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12481 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/components/processors/roo_process_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15637 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.3/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-18 15:35:39.000000 quickstats-0.7.0.5.3/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-04-18 15:34:27.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-18 15:35:40.000000 quickstats-0.7.0.5.3/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.5.3/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.3/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5285 2024-04-18 15:36:29.000000 quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10852 2024-04-18 15:36:29.000000 quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7694 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_significance.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      411 2024-04-18 15:36:36.000000 quickstats-0.7.0.5.3/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.3/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32252 2024-04-18 15:36:37.000000 quickstats-0.7.0.5.3/quickstats/core/configuration.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-18 15:35:34.000000 quickstats-0.7.0.5.3/quickstats/core/constraints.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4603 2024-04-18 15:36:10.000000 quickstats-0.7.0.5.3/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7569 2024-04-18 15:36:10.000000 quickstats-0.7.0.5.3/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7710 2024-06-03 07:36:21.000000 quickstats-0.7.0.5.3/quickstats/core/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-18 15:36:02.000000 quickstats-0.7.0.5.3/quickstats/core/metaclasses.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7624 2024-04-18 15:39:09.000000 quickstats-0.7.0.5.3/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18907 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-18 15:35:28.000000 quickstats-0.7.0.5.3/quickstats/core/setup.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-18 15:36:06.000000 quickstats-0.7.0.5.3/quickstats/core/type_validation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-04-18 15:35:28.000000 quickstats-0.7.0.5.3/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/daq/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      151 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/daq/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6933 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/daq/remote_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3849 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/daq/servicex_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2553 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/daq/xrootd_source.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/extensions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.3/quickstats/extensions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.3/quickstats/extensions/extension_dataframe.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:35:04.000000 quickstats-0.7.0.5.3/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      198 2024-04-18 15:39:03.000000 quickstats-0.7.0.5.3/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.3/quickstats/interface/cppyy/basic_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.5.3/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.3/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/interface/kerberos/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      109 2024-04-18 15:39:14.000000 quickstats-0.7.0.5.3/quickstats/interface/kerberos/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1709 2024-04-18 15:39:14.000000 quickstats-0.7.0.5.3/quickstats/interface/kerberos/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/ModelConfig.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11422 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RDataFrame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooAbsArg.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-04-18 15:34:20.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TChain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11390 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5813 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TH3.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-04-18 15:34:42.000000 quickstats-0.7.0.5.3/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      748 2024-04-18 15:39:11.000000 quickstats-0.7.0.5.3/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.5.3/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.5.3/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.3/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/interface/servicex/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      163 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/servicex/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5409 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/servicex/config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2872 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/servicex/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/interface/tinydb/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       67 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/tinydb/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      947 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/tinydb/methods.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/interface/xrootd/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      149 2024-04-18 15:39:06.000000 quickstats-0.7.0.5.3/quickstats/interface/xrootd/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      448 2024-04-18 15:39:06.000000 quickstats-0.7.0.5.3/quickstats/interface/xrootd/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5850 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/xrootd/filesystem.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1163 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/xrootd/path.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/interface/xrootd/xrd_helper.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:03.000000 quickstats-0.7.0.5.3/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.5.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.5.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/QStringUtils.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-04-18 15:34:34.000000 quickstats-0.7.0.5.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.5.3/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.5.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.5.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.5.3/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12211 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.3/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    40281 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.3/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.5.3/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.5.3/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/parsers/param_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/parsers/roo_param_setup_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:05.000000 quickstats-0.7.0.5.3/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1391 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.3/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27356 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14144 2024-04-18 15:38:50.000000 quickstats-0.7.0.5.3/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.5.3/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-04-18 15:35:22.000000 quickstats-0.7.0.5.3/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6579 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.3/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7791 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4061 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.3/quickstats/plots/general_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22203 2024-04-18 15:41:03.000000 quickstats-0.7.0.5.3/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6078 2024-04-18 15:38:56.000000 quickstats-0.7.0.5.3/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.3/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16926 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.3/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.3/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25684 2024-04-18 15:41:03.000000 quickstats-0.7.0.5.3/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5096 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.3/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10353 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.3/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.3/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30687 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13785 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.3/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.3/quickstats/plots/two_axis_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.3/quickstats/plots/two_panel_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9999 2024-04-18 15:42:16.000000 quickstats-0.7.0.5.3/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19292 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.3/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13182 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.3/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23227 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    34454 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.3/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:05.000000 quickstats-0.7.0.5.3/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.3/quickstats/resources/default_workspace_extensions.json
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:05.000000 quickstats-0.7.0.5.3/quickstats/resources/mpl_stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.3/quickstats/resources/mpl_stylesheets/hep.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.3/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.3/quickstats/resources/mpl_stylesheets/science.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.3/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:05.000000 quickstats-0.7.0.5.3/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.5.3/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19773 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.5.3/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18666 2024-04-18 15:39:08.000000 quickstats-0.7.0.5.3/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.5.3/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3039 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.3/quickstats/utils/path_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-04-18 15:35:24.000000 quickstats-0.7.0.5.3/quickstats/utils/py_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27521 2024-04-18 15:36:12.000000 quickstats-0.7.0.5.3/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.3/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15330 2024-04-18 15:36:32.000000 quickstats-0.7.0.5.3/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15638 2024-04-18 15:39:31.000000 quickstats-0.7.0.5.3/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2321 2024-04-18 15:36:21.000000 quickstats-0.7.0.5.3/quickstats/utils/sys_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-18 15:35:57.000000 quickstats-0.7.0.5.3/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 11:14:04.000000 quickstats-0.7.0.5.3/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-06-03 11:14:03.000000 quickstats-0.7.0.5.3/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11106 2024-06-03 11:14:03.000000 quickstats-0.7.0.5.3/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-06-03 11:14:03.000000 quickstats-0.7.0.5.3/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-06-03 11:14:03.000000 quickstats-0.7.0.5.3/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-06-03 11:14:03.000000 quickstats-0.7.0.5.3/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-06-03 11:14:05.000000 quickstats-0.7.0.5.3/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-04-18 15:34:33.000000 quickstats-0.7.0.5.3/setup.py
```

### Comparing `quickstats-0.7.0.5.1/PKG-INFO` & `quickstats-0.7.0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.5.1
+Version: 0.7.0.5.3
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.5.1/README.md` & `quickstats-0.7.0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/BaseMethod.py` & `quickstats-0.7.0.5.3/quickstats/algorithms/nll_crossing/BaseMethod.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/analysis_base.py` & `quickstats-0.7.0.5.3/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.7.0.5.3/quickstats/analysis/analysis_path_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         "category_summary"                         : ("summary", "category_summary_{channel}.json"),
         "boundary_data"                            : ("summary", "boundary_tree_{channel}.json"),
         "benchmark_significance"                   : ("summary", "benchmark_significance.json")
     }
 
     @property
     def study_name(self):
-        return self.directories['output'].basename
+        return self.directories['study'].basename
         
     def __init__(self, study_name : str = "base_study",
                  base_path:str = None,
                  directories:Optional[Dict[str, str]]=None,
                  files:Optional[Dict[str, Union[str, Tuple[Optional[str], str]]]]=None):
         super().__init__(base_path=base_path, directories=directories, files=files)
         self.set_study_name(study_name)
 
     def set_study_name(self, name: str = "base_study"):
-        self.directories['output'].basename = name
+        self.directories['study'].basename = name
```

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/config_templates.py` & `quickstats-0.7.0.5.3/quickstats/analysis/config_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/data_loading.py` & `quickstats-0.7.0.5.3/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/data_preprocessing.py` & `quickstats-0.7.0.5.3/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/event_categorization.py` & `quickstats-0.7.0.5.3/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.7.0.5.3/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.7.0.5.3/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.7.0.5.3/quickstats/analysis/ntuple_process_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.7.0.5.3/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.7.0.5.3/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.7.0.5.3/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.7.0.5.3/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.7.0.5.3/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/core.py` & `quickstats-0.7.0.5.3/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/inspect_rfile.py` & `quickstats-0.7.0.5.3/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/likelihood_tools.py` & `quickstats-0.7.0.5.3/quickstats/clis/likelihood_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/limit_setting.py` & `quickstats-0.7.0.5.3/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/nuisance_parameter_tools.py` & `quickstats-0.7.0.5.3/quickstats/clis/nuisance_parameter_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/processor_tools.py` & `quickstats-0.7.0.5.3/quickstats/clis/processor_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/stat_tools.py` & `quickstats-0.7.0.5.3/quickstats/clis/stat_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/clis/workspace_tools.py` & `quickstats-0.7.0.5.3/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/__init__.py` & `quickstats-0.7.0.5.3/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/analysis_base.py` & `quickstats-0.7.0.5.3/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/analysis_object.py` & `quickstats-0.7.0.5.3/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/asimov_generator.py` & `quickstats-0.7.0.5.3/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/asymptotic_cls.py` & `quickstats-0.7.0.5.3/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/basics.py` & `quickstats-0.7.0.5.3/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/caching_nll_wrapper.py` & `quickstats-0.7.0.5.3/quickstats/components/caching_nll_wrapper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/discrete_nuisance.py` & `quickstats-0.7.0.5.3/quickstats/components/discrete_nuisance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/extended_minimizer.py` & `quickstats-0.7.0.5.3/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/extended_model.py` & `quickstats-0.7.0.5.3/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/extended_rfile.py` & `quickstats-0.7.0.5.3/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/likelihood.py` & `quickstats-0.7.0.5.3/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/modelling/component_source.py` & `quickstats-0.7.0.5.3/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/modelling/data_modelling.py` & `quickstats-0.7.0.5.3/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/modelling/model_source.py` & `quickstats-0.7.0.5.3/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.7.0.5.3/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.7.0.5.3/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.7.0.5.3/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.7.0.5.3/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.7.0.5.3/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.7.0.5.3/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/__init__.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_hdf.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_as_hdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 @register_action
 class RooProcAsHDF(RooProcOutputAction):
     
     NAME = "AS_HDF"
     
     def __init__(self, filename:str, key:str,
                  columns:Optional[List[str]],
-                 exclude:Optional[List[str]]=None):
+                 exclude:Optional[List[str]]=None,
+                 **kwargs):
         super().__init__(filename=filename,
                          columns=columns,
-                         key=key)
+                         key=key,
+                         **kwargs)
 
     def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
         filename = params['filename']
-        key = params['key']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'Cached output from "{filename}".')
             return rdf, processor
         processor.stdout.info(f'Writing output to "{filename}".')
         import awkward as ak
         import pandas as pd
         columns = params.get('columns', None)
@@ -49,9 +50,10 @@
         #        array = None
         #        processor.stdout.warning("Failed to convert output to numpy arrays with awkward backend. "
         #                                 "Falling back to use ROOT instead")
         #if array is None:
         #    array = rdf.AsNumpy(save_columns)
         df = pd.DataFrame(array)
         self.makedirs(filename)
-        df.to_hdf(filename, key=key)
+        kwargs = {k:v for k, v in params.items() if k not in ['filename', 'columns', 'exclude']}
+        df.to_hdf(filename, **kwargs)
         return rdf, processor
```

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_parquet.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_as_parquet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_cache.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_cache.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_output_action.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_output_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_progressbar.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_progressbar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_define.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_safe_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/builtin_methods.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/roo_process_config.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/roo_process_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/processors/roo_processor.py` & `quickstats-0.7.0.5.3/quickstats/components/processors/roo_processor.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/pvalue_toys.py` & `quickstats-0.7.0.5.3/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/roo_inspector.py` & `quickstats-0.7.0.5.3/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/root_object.py` & `quickstats-0.7.0.5.3/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/toy_limit_calculator.py` & `quickstats-0.7.0.5.3/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/__init__.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/sample.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/settings.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/systematic.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.7.0.5.3/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/concurrent/abstract_runner.py` & `quickstats-0.7.0.5.3/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/concurrent/logging.py` & `quickstats-0.7.0.5.3/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.7.0.5.3/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_significance.py` & `quickstats-0.7.0.5.3/quickstats/concurrent/parameterised_significance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/abstract_object.py` & `quickstats-0.7.0.5.3/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/configuration.py` & `quickstats-0.7.0.5.3/quickstats/core/configuration.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/constraints.py` & `quickstats-0.7.0.5.3/quickstats/core/constraints.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/decorators.py` & `quickstats-0.7.0.5.3/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/enums.py` & `quickstats-0.7.0.5.3/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/io.py` & `quickstats-0.7.0.5.3/quickstats/core/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/metaclasses.py` & `quickstats-0.7.0.5.3/quickstats/core/metaclasses.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/methods.py` & `quickstats-0.7.0.5.3/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/path_manager.py` & `quickstats-0.7.0.5.3/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/setup.py` & `quickstats-0.7.0.5.3/quickstats/core/setup.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/type_validation.py` & `quickstats-0.7.0.5.3/quickstats/core/type_validation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/core/virtual_trees.py` & `quickstats-0.7.0.5.3/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/daq/remote_data_source.py` & `quickstats-0.7.0.5.3/quickstats/daq/remote_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/daq/servicex_source.py` & `quickstats-0.7.0.5.3/quickstats/daq/servicex_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/daq/xrootd_source.py` & `quickstats-0.7.0.5.3/quickstats/daq/xrootd_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/extensions/extension_dataframe.py` & `quickstats-0.7.0.5.3/quickstats/extensions/extension_dataframe.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/cppyy/core.py` & `quickstats-0.7.0.5.3/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/cppyy/macros.py` & `quickstats-0.7.0.5.3/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.7.0.5.3/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/kerberos/core.py` & `quickstats-0.7.0.5.3/quickstats/interface/kerberos/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/ModelConfig.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/ModelConfig.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RDataFrame.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RDataFrame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsArg.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooAbsArg.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsData.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooArgSet.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooArgSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooCategory.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooDataSet.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooMsgService.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/RooRealVar.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/TChain.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/TChain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/TF1.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/TFile.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/TH1.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/TH2.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/TH3.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/TH3.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/__init__.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/helper.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/macros.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/root/roofit_extension.py` & `quickstats-0.7.0.5.3/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/servicex/config.py` & `quickstats-0.7.0.5.3/quickstats/interface/servicex/config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/servicex/core.py` & `quickstats-0.7.0.5.3/quickstats/interface/servicex/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/tinydb/methods.py` & `quickstats-0.7.0.5.3/quickstats/interface/tinydb/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/xrootd/filesystem.py` & `quickstats-0.7.0.5.3/quickstats/interface/xrootd/filesystem.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/xrootd/path.py` & `quickstats-0.7.0.5.3/quickstats/interface/xrootd/path.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/interface/xrootd/xrd_helper.py` & `quickstats-0.7.0.5.3/quickstats/interface/xrootd/xrd_helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.7.0.5.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.7.0.5.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.7.0.5.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.7.0.5.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx` & `quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/QStringUtils.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.7.0.5.3/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.7.0.5.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.7.0.5.3/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.7.0.5.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.7.0.5.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/maths/interpolation.py` & `quickstats-0.7.0.5.3/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/maths/numerics.py` & `quickstats-0.7.0.5.3/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/maths/statistics.py` & `quickstats-0.7.0.5.3/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/maths/statistics_jitted.py` & `quickstats-0.7.0.5.3/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/maths/symbolics.py` & `quickstats-0.7.0.5.3/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/parsers/param_parser.py` & `quickstats-0.7.0.5.3/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/parsers/roo_param_setup_parser.py` & `quickstats-0.7.0.5.3/quickstats/parsers/roo_param_setup_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/__init__.py` & `quickstats-0.7.0.5.3/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/abstract_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/abstract_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.7.0.5.3/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/collective_data_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/color_schemes.py` & `quickstats-0.7.0.5.3/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/core.py` & `quickstats-0.7.0.5.3/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/correlation_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/general_1D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/general_2D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/general_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/general_distribution_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/np_ranking_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/sample_purity_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/score_distribution_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/stat_plot_config.py` & `quickstats-0.7.0.5.3/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/template.py` & `quickstats-0.7.0.5.3/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/two_axis_1D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/two_axis_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/two_panel_1D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/two_panel_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.7.0.5.3/quickstats/plots/variable_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/root_checker.py` & `quickstats-0.7.0.5.3/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/common_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/data_conversion.py` & `quickstats-0.7.0.5.3/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/hep_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/path_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/py_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/roofit_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/roostats_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/root_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/string_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/sys_utils.py` & `quickstats-0.7.0.5.3/quickstats/utils/sys_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats/utils/xml_tools.py` & `quickstats-0.7.0.5.3/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/quickstats.egg-info/PKG-INFO` & `quickstats-0.7.0.5.3/quickstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.5.1
+Version: 0.7.0.5.3
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.5.1/quickstats.egg-info/SOURCES.txt` & `quickstats-0.7.0.5.3/quickstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5.1/setup.py` & `quickstats-0.7.0.5.3/setup.py`

 * *Files identical despite different names*

