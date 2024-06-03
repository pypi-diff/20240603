# Comparing `tmp/quickstats-0.7.0.5.tar.gz` & `tmp/quickstats-0.7.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.7.0.5.tar", last modified: Sun Jun  2 15:12:53 2024, max compression
+gzip compressed data, was "quickstats-0.7.0.5.1.tar", last modified: Mon Jun  3 08:47:48 2024, max compression
```

## Comparing `quickstats-0.7.0.5.tar` & `quickstats-0.7.0.5.1.tar`

### file list

```diff
@@ -1,297 +1,296 @@
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.200507 quickstats-0.7.0.5/
--rw-r--r--   0 chlcheng (102623) chlcheng (102623)     4125 2024-06-02 15:12:53.199930 quickstats-0.7.0.5/PKG-INFO
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3567 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/README.md
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.968936 quickstats-0.7.0.5/bin/
--rwxrwx---   0 chlcheng (102623) chlcheng (102623)       93 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/bin/quickstats
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.970417 quickstats-0.7.0.5/quickstats/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      134 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       24 2024-06-02 15:12:25.000000 quickstats-0.7.0.5/quickstats/_version.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.974188 quickstats-0.7.0.5/quickstats/algorithms/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.5/quickstats/algorithms/__init__.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.977282 quickstats-0.7.0.5/quickstats/algorithms/nll_crossing/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4350 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/algorithms/nll_crossing/BaseMethod.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.5/quickstats/algorithms/nll_crossing/BisectionMethod.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.5/quickstats/algorithms/nll_crossing/NovelMethod.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.5/quickstats/algorithms/nll_crossing/SteppingMethod.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.5/quickstats/algorithms/nll_crossing/__init__.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.986319 quickstats-0.7.0.5/quickstats/analysis/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      428 2024-04-02 17:36:13.000000 quickstats-0.7.0.5/quickstats/analysis/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7392 2024-06-02 15:09:17.000000 quickstats-0.7.0.5/quickstats/analysis/analysis_base.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3889 2024-06-02 15:09:17.000000 quickstats-0.7.0.5/quickstats/analysis/analysis_path_manager.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    21365 2024-06-02 15:09:17.000000 quickstats-0.7.0.5/quickstats/analysis/config_templates.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    41102 2024-06-02 15:09:17.000000 quickstats-0.7.0.5/quickstats/analysis/data_loading.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1311 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/analysis/data_preprocessing.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    85926 2024-06-02 15:09:17.000000 quickstats-0.7.0.5/quickstats/analysis/event_categorization.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     8048 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/analysis/multi_class_boundary_tree.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     9290 2024-06-02 15:09:17.000000 quickstats-0.7.0.5/quickstats/analysis/ntuple_conversion_tool.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    33252 2024-04-23 13:33:55.000000 quickstats-0.7.0.5/quickstats/analysis/ntuple_process_tool.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     8906 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/analysis/sample_poly_param_tool.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.990722 quickstats-0.7.0.5/quickstats/analysis/systematics/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      241 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/analysis/systematics/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    29468 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/analysis/systematics/base_systematics.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     9760 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6753 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/analysis/systematics/normalization_systematics.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    11890 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.998299 quickstats-0.7.0.5/quickstats/clis/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      237 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/clis/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2816 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/clis/core.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1908 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/clis/inspect_rfile.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    23632 2024-04-24 20:02:12.000000 quickstats-0.7.0.5/quickstats/clis/likelihood_tools.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    15027 2024-03-02 09:26:25.000000 quickstats-0.7.0.5/quickstats/clis/limit_setting.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    19517 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/clis/nuisance_parameter_tools.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1609 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/clis/processor_tools.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    18230 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/clis/stat_tools.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    18810 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/clis/workspace_tools.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.016455 quickstats-0.7.0.5/quickstats/components/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1113 2024-04-16 04:58:47.000000 quickstats-0.7.0.5/quickstats/components/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3136 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/components/analysis_base.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    15274 2024-04-24 20:13:29.000000 quickstats-0.7.0.5/quickstats/components/analysis_object.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7330 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/components/asimov_generator.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    31508 2024-03-02 09:26:25.000000 quickstats-0.7.0.5/quickstats/components/asymptotic_cls.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3273 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/basics.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3156 2024-02-09 19:22:50.000000 quickstats-0.7.0.5/quickstats/components/caching_nll_wrapper.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10479 2024-03-02 09:26:25.000000 quickstats-0.7.0.5/quickstats/components/discrete_nuisance.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    56823 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/components/extended_minimizer.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)   105095 2024-03-02 09:26:25.000000 quickstats-0.7.0.5/quickstats/components/extended_model.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5859 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/extended_rfile.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    14097 2024-04-24 19:51:22.000000 quickstats-0.7.0.5/quickstats/components/likelihood.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.022736 quickstats-0.7.0.5/quickstats/components/modelling/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      207 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/modelling/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2504 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/modelling/component_source.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    20116 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/components/modelling/data_modelling.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      735 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/modelling/model_source.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4502 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/modelling/parameter_templates.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5550 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/modelling/pdf_fit_tool.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3483 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/modelling/tree_data_source.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10864 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/nuisance_parameter_harmonizer.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    17594 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/nuisance_parameter_pull.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    12380 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/components/nuisance_parameter_ranking.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.026114 quickstats-0.7.0.5/quickstats/components/processors/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      111 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/__init__.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.059106 quickstats-0.7.0.5/quickstats/components/processors/actions/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1457 2024-04-24 09:12:07.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      388 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/auxiliary.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      358 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/formatter.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1608 2024-04-16 12:24:10.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_alias.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2360 2024-04-24 10:06:22.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_as_hdf.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2037 2024-04-24 10:03:17.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1589 2024-04-24 09:17:14.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_as_parquet.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4421 2024-04-16 12:43:49.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_base_action.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1049 2024-04-24 09:24:54.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_cache.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      866 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_declare.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1826 2024-04-16 13:51:20.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_define.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1228 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_export.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1903 2024-04-23 13:39:48.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_filter.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1331 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      506 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      586 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      755 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      763 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      726 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1211 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      226 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_max.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      225 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_mean.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      226 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_min.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      636 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2249 2024-04-24 09:49:14.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_output_action.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      757 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_progressbar.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      462 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      481 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_redefine.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1854 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_report.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      723 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      539 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1770 2024-04-24 09:17:06.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_save.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      735 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1433 2024-04-16 12:24:30.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_stat.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      226 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_sum.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      606 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_treename.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    13111 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/components/processors/builtin_methods.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    12481 2024-04-23 14:29:19.000000 quickstats-0.7.0.5/quickstats/components/processors/roo_process_config.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    13843 2024-05-18 08:17:55.000000 quickstats-0.7.0.5/quickstats/components/processors/roo_processor.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5406 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/pvalue_toys.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2978 2024-04-02 17:06:13.000000 quickstats-0.7.0.5/quickstats/components/roo_inspector.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3103 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/root_object.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    21325 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/toy_limit_calculator.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.074264 quickstats-0.7.0.5/quickstats/components/workspaces/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      591 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/workspaces/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     9877 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/workspaces/asimov_handler.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1727 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/workspaces/core_argument_sets.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1997 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/workspaces/sample.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1991 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/workspaces/settings.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     8910 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/workspaces/systematic.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2303 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/components/workspaces/systematics_domain.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    53148 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/components/workspaces/ws_comparer.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     8787 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/components/workspaces/ws_decomposer.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1724 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/workspaces/ws_modifier_config.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10827 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_base.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    87015 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    76446 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    52888 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_combiner.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    55314 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_modifier.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.081242 quickstats-0.7.0.5/quickstats/concurrent/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      372 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/concurrent/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4197 2024-04-02 17:05:55.000000 quickstats-0.7.0.5/quickstats/concurrent/abstract_runner.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      627 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/concurrent/logging.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5209 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5285 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10852 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/concurrent/parameterised_likelihood.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5822 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/concurrent/parameterised_runner.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7694 2024-04-18 14:43:04.000000 quickstats-0.7.0.5/quickstats/concurrent/parameterised_significance.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.098192 quickstats-0.7.0.5/quickstats/core/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      411 2024-05-30 21:59:23.000000 quickstats-0.7.0.5/quickstats/core/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      783 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/core/abstract_object.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    32252 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/core/configuration.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4546 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/core/constraints.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4603 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/core/decorators.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7569 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/core/enums.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7710 2024-05-30 21:58:05.000000 quickstats-0.7.0.5/quickstats/core/io.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2106 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/core/metaclasses.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7624 2024-04-16 04:59:38.000000 quickstats-0.7.0.5/quickstats/core/methods.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    18907 2024-05-27 11:31:30.000000 quickstats-0.7.0.5/quickstats/core/path_manager.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      721 2024-04-02 16:59:53.000000 quickstats-0.7.0.5/quickstats/core/setup.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6584 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/core/type_validation.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3895 2024-03-29 08:37:19.000000 quickstats-0.7.0.5/quickstats/core/virtual_trees.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.101534 quickstats-0.7.0.5/quickstats/daq/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      151 2024-04-23 12:17:50.000000 quickstats-0.7.0.5/quickstats/daq/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6933 2024-04-23 13:26:47.000000 quickstats-0.7.0.5/quickstats/daq/remote_data_source.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3849 2024-04-23 14:31:53.000000 quickstats-0.7.0.5/quickstats/daq/servicex_source.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2553 2024-04-23 14:41:51.000000 quickstats-0.7.0.5/quickstats/daq/xrootd_source.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.102905 quickstats-0.7.0.5/quickstats/extensions/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       85 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/extensions/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4147 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/extensions/extension_dataframe.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.103764 quickstats-0.7.0.5/quickstats/interface/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/interface/__init__.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.107509 quickstats-0.7.0.5/quickstats/interface/cppyy/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      198 2024-04-15 04:00:33.000000 quickstats-0.7.0.5/quickstats/interface/cppyy/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      392 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/cppyy/basic_methods.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      513 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/cppyy/core.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    12794 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/cppyy/macros.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4540 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/interface/cppyy/vectorize.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.108986 quickstats-0.7.0.5/quickstats/interface/kerberos/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      109 2024-04-15 21:52:35.000000 quickstats-0.7.0.5/quickstats/interface/kerberos/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1709 2024-04-15 21:56:47.000000 quickstats-0.7.0.5/quickstats/interface/kerberos/core.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.129780 quickstats-0.7.0.5/quickstats/interface/root/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3819 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/ModelConfig.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10737 2024-04-24 09:58:20.000000 quickstats-0.7.0.5/quickstats/interface/root/RDataFrame.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2306 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/RooAbsArg.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      621 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/RooAbsData.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    21668 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/interface/root/RooAbsPdf.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3531 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/RooArgSet.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1182 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/RooCategory.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    44967 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/interface/root/RooDataSet.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      588 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/RooMsgService.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6728 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/interface/root/RooRealVar.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      130 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/TArrayData.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2905 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/interface/root/TChain.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      983 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/TF1.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    11390 2024-04-23 03:24:44.000000 quickstats-0.7.0.5/quickstats/interface/root/TFile.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    13146 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/interface/root/TH1.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5813 2024-04-19 22:59:06.000000 quickstats-0.7.0.5/quickstats/interface/root/TH2.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6043 2024-04-19 22:51:24.000000 quickstats-0.7.0.5/quickstats/interface/root/TH3.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      378 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/interface/root/TObject.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      748 2024-04-16 04:58:25.000000 quickstats-0.7.0.5/quickstats/interface/root/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1069 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/helper.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      235 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/io.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    27713 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/macros.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5634 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/interface/root/roofit_extension.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.132240 quickstats-0.7.0.5/quickstats/interface/servicex/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      163 2024-04-22 09:59:18.000000 quickstats-0.7.0.5/quickstats/interface/servicex/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5409 2024-04-24 08:55:03.000000 quickstats-0.7.0.5/quickstats/interface/servicex/config.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2872 2024-04-24 09:30:06.000000 quickstats-0.7.0.5/quickstats/interface/servicex/core.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.133896 quickstats-0.7.0.5/quickstats/interface/tinydb/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       67 2024-04-24 07:55:07.000000 quickstats-0.7.0.5/quickstats/interface/tinydb/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      947 2024-04-24 08:54:00.000000 quickstats-0.7.0.5/quickstats/interface/tinydb/methods.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.137999 quickstats-0.7.0.5/quickstats/interface/xrootd/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      149 2024-04-16 06:14:52.000000 quickstats-0.7.0.5/quickstats/interface/xrootd/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      448 2024-04-15 05:41:21.000000 quickstats-0.7.0.5/quickstats/interface/xrootd/core.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5850 2024-04-23 03:15:06.000000 quickstats-0.7.0.5/quickstats/interface/xrootd/filesystem.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1163 2024-04-23 03:14:39.000000 quickstats-0.7.0.5/quickstats/interface/xrootd/path.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2573 2024-04-23 07:02:17.000000 quickstats-0.7.0.5/quickstats/interface/xrootd/xrd_helper.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.965519 quickstats-0.7.0.5/quickstats/macros/
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.139759 quickstats-0.7.0.5/quickstats/macros/AsymptoticCLsTool/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7366 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1591 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.141576 quickstats-0.7.0.5/quickstats/macros/FlexibleInterpVarMkII/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    12372 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2498 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.145197 quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3133 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/QStringUtils.cxx
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1259 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10312 2024-02-23 18:55:02.000000 quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3868 2024-02-23 18:55:02.000000 quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.147003 quickstats-0.7.0.5/quickstats/macros/ResponseFunction/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    13749 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2982 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.148705 quickstats-0.7.0.5/quickstats/macros/RooTwoSidedCBShape/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3689 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1358 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.153322 quickstats-0.7.0.5/quickstats/maths/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/maths/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4366 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/maths/interpolation.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    12211 2024-05-29 11:25:58.000000 quickstats-0.7.0.5/quickstats/maths/numerics.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    40281 2024-04-18 13:39:14.000000 quickstats-0.7.0.5/quickstats/maths/statistics.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3506 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/maths/statistics_jitted.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      613 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/maths/symbolics.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.158925 quickstats-0.7.0.5/quickstats/parsers/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      187 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/parsers/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      337 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/parsers/config_parser.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    16764 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/parsers/param_parser.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5204 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/parsers/roo_param_setup_parser.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.183832 quickstats-0.7.0.5/quickstats/plots/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1391 2024-06-02 11:51:24.000000 quickstats-0.7.0.5/quickstats/plots/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    27356 2024-05-07 03:52:59.000000 quickstats-0.7.0.5/quickstats/plots/abstract_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5196 2024-04-16 21:04:46.000000 quickstats-0.7.0.5/quickstats/plots/bar_chart.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    14144 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/bidirectional_bar_chart.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1634 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/plots/collective_data_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3467 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/quickstats/plots/color_schemes.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6579 2024-04-30 03:37:06.000000 quickstats-0.7.0.5/quickstats/plots/core.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4951 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/plots/correlation_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7791 2024-04-26 23:31:28.000000 quickstats-0.7.0.5/quickstats/plots/general_1D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4061 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/general_2D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    22203 2024-04-17 08:14:07.000000 quickstats-0.7.0.5/quickstats/plots/general_distribution_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6078 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/hypotest_inverter_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     8981 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/plots/likelihood_1D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    16926 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/likelihood_2D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    29155 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/plots/np_ranking_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    25684 2024-04-17 08:14:13.000000 quickstats-0.7.0.5/quickstats/plots/pdf_distribution_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5096 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/sample_purity_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10353 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/score_distribution_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4122 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/plots/stat_plot_config.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    30687 2024-04-30 14:14:10.000000 quickstats-0.7.0.5/quickstats/plots/template.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    13785 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/test_statistic_distribution_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     5122 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/plots/two_axis_1D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6651 2024-06-02 11:49:15.000000 quickstats-0.7.0.5/quickstats/plots/two_panel_1D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     9999 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/upper_limit_1D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    19292 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/upper_limit_2D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    13182 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/plots/upper_limit_3D_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    23227 2024-04-25 09:01:39.000000 quickstats-0.7.0.5/quickstats/plots/upper_limit_benchmark_plot.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    34454 2024-05-28 16:17:28.000000 quickstats-0.7.0.5/quickstats/plots/variable_distribution_plot.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.184752 quickstats-0.7.0.5/quickstats/resources/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       90 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/resources/default_workspace_extensions.json
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.186396 quickstats-0.7.0.5/quickstats/resources/mpl_stylesheets/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      379 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/resources/mpl_stylesheets/hep.mplstyle
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      325 2024-03-22 01:36:00.000000 quickstats-0.7.0.5/quickstats/resources/mpl_stylesheets/science.mplstyle
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     4604 2024-02-23 18:55:02.000000 quickstats-0.7.0.5/quickstats/root_checker.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:53.198798 quickstats-0.7.0.5/quickstats/utils/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2024-03-22 01:35:33.000000 quickstats-0.7.0.5/quickstats/utils/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    19773 2024-04-23 05:00:30.000000 quickstats-0.7.0.5/quickstats/utils/common_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/utils/condor_tasks.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    18666 2024-04-19 21:42:21.000000 quickstats-0.7.0.5/quickstats/utils/data_conversion.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1187 2023-10-16 18:13:04.000000 quickstats-0.7.0.5/quickstats/utils/hep_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3039 2024-04-23 10:35:13.000000 quickstats-0.7.0.5/quickstats/utils/path_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      563 2024-03-29 07:47:20.000000 quickstats-0.7.0.5/quickstats/utils/py_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    27521 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/utils/roofit_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    10914 2024-02-09 19:22:51.000000 quickstats-0.7.0.5/quickstats/utils/roostats_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    15330 2024-04-19 21:42:42.000000 quickstats-0.7.0.5/quickstats/utils/root_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    15638 2024-04-16 13:51:02.000000 quickstats-0.7.0.5/quickstats/utils/string_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2321 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/utils/sys_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    15128 2024-04-15 03:46:28.000000 quickstats-0.7.0.5/quickstats/utils/xml_tools.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:12:52.973691 quickstats-0.7.0.5/quickstats.egg-info/
--rw-r--r--   0 chlcheng (102623) chlcheng (102623)     4125 2024-06-02 15:12:52.972153 quickstats-0.7.0.5/quickstats.egg-info/PKG-INFO
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    11136 2024-06-02 15:12:52.972614 quickstats-0.7.0.5/quickstats.egg-info/SOURCES.txt
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        1 2024-06-02 15:12:52.973002 quickstats-0.7.0.5/quickstats.egg-info/dependency_links.txt
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       39 2024-06-02 15:12:52.973385 quickstats-0.7.0.5/quickstats.egg-info/requires.txt
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       11 2024-06-02 15:12:52.973761 quickstats-0.7.0.5/quickstats.egg-info/top_level.txt
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       38 2024-06-02 15:12:53.200576 quickstats-0.7.0.5/setup.cfg
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1771 2024-03-27 08:35:59.000000 quickstats-0.7.0.5/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.1/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:37.000000 quickstats-0.7.0.5.1/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.1/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:37.000000 quickstats-0.7.0.5.1/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-18 15:35:29.000000 quickstats-0.7.0.5.1/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       27 2024-06-03 08:47:15.000000 quickstats-0.7.0.5.1/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/algorithms/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.5.1/quickstats/algorithms/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/BaseMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/BisectionMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/NovelMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/SteppingMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-18 15:35:43.000000 quickstats-0.7.0.5.1/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7392 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3889 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21365 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/config_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41355 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1311 2024-04-18 15:36:08.000000 quickstats-0.7.0.5.1/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85926 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-05-31 12:42:29.000000 quickstats-0.7.0.5.1/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9290 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    33429 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:39.000000 quickstats-0.7.0.5.1/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23632 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/clis/likelihood_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-04-18 15:43:10.000000 quickstats-0.7.0.5.1/quickstats/clis/nuisance_parameter_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.5.1/quickstats/clis/processor_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/clis/stat_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.5.1/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:41.000000 quickstats-0.7.0.5.1/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1113 2024-04-18 15:39:11.000000 quickstats-0.7.0.5.1/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15274 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/caching_nll_wrapper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/discrete_nuisance.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-04-18 15:34:25.000000 quickstats-0.7.0.5.1/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14097 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.1/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:42.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:42.000000 quickstats-0.7.0.5.1/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-04-18 15:34:50.000000 quickstats-0.7.0.5.1/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:42.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1457 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      358 2024-04-18 15:36:38.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/formatter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1608 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2360 2024-04-25 03:40:17.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_hdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2037 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1589 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_parquet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4421 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1049 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_cache.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1826 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-04-18 15:34:47.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1903 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2249 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_output_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-04-18 15:34:47.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_progressbar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1854 2024-04-18 15:36:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      723 2024-04-18 15:36:56.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1770 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1433 2024-04-18 15:39:37.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-04-18 15:34:45.000000 quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-04-18 15:34:23.000000 quickstats-0.7.0.5.1/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12481 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/components/processors/roo_process_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15637 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-18 15:35:39.000000 quickstats-0.7.0.5.1/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:43.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-04-18 15:34:27.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-18 15:35:32.000000 quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-18 15:35:40.000000 quickstats-0.7.0.5.1/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.5.1/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.5.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5285 2024-04-18 15:36:29.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10852 2024-04-18 15:36:29.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7694 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_significance.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      411 2024-04-18 15:36:36.000000 quickstats-0.7.0.5.1/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32252 2024-04-18 15:36:37.000000 quickstats-0.7.0.5.1/quickstats/core/configuration.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-18 15:35:34.000000 quickstats-0.7.0.5.1/quickstats/core/constraints.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4603 2024-04-18 15:36:10.000000 quickstats-0.7.0.5.1/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7569 2024-04-18 15:36:10.000000 quickstats-0.7.0.5.1/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7710 2024-06-03 07:36:21.000000 quickstats-0.7.0.5.1/quickstats/core/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-18 15:36:02.000000 quickstats-0.7.0.5.1/quickstats/core/metaclasses.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7624 2024-04-18 15:39:09.000000 quickstats-0.7.0.5.1/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18907 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-18 15:35:28.000000 quickstats-0.7.0.5.1/quickstats/core/setup.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-18 15:36:06.000000 quickstats-0.7.0.5.1/quickstats/core/type_validation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-04-18 15:35:28.000000 quickstats-0.7.0.5.1/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/daq/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      151 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6933 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/remote_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3849 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/servicex_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2553 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/daq/xrootd_source.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/extensions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/extensions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/extensions/extension_dataframe.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:35:04.000000 quickstats-0.7.0.5.1/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:44.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      198 2024-04-18 15:39:03.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/basic_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/kerberos/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      109 2024-04-18 15:39:14.000000 quickstats-0.7.0.5.1/quickstats/interface/kerberos/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1709 2024-04-18 15:39:14.000000 quickstats-0.7.0.5.1/quickstats/interface/kerberos/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/ModelConfig.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11422 2024-06-03 07:36:23.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RDataFrame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsArg.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-04-18 15:34:20.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TChain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11390 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5813 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TH3.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-04-18 15:34:42.000000 quickstats-0.7.0.5.1/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      748 2024-04-18 15:39:11.000000 quickstats-0.7.0.5.1/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.5.1/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.5.1/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.5.1/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      163 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5409 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2872 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/servicex/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:45.000000 quickstats-0.7.0.5.1/quickstats/interface/tinydb/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       67 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/tinydb/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      947 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/tinydb/methods.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      149 2024-04-18 15:39:06.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      448 2024-04-18 15:39:06.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5850 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/filesystem.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1163 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/path.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/interface/xrootd/xrd_helper.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:37.000000 quickstats-0.7.0.5.1/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-04-18 15:34:34.000000 quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.5.1/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12211 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.1/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    40281 2024-04-18 15:41:02.000000 quickstats-0.7.0.5.1/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.5.1/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:46.000000 quickstats-0.7.0.5.1/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.5.1/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/parsers/param_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/parsers/roo_param_setup_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1391 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.1/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27356 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14144 2024-04-18 15:38:50.000000 quickstats-0.7.0.5.1/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.5.1/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-04-18 15:35:22.000000 quickstats-0.7.0.5.1/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6579 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.5.1/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7791 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4061 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/general_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22203 2024-04-18 15:41:03.000000 quickstats-0.7.0.5.1/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6078 2024-04-18 15:38:56.000000 quickstats-0.7.0.5.1/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16926 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25684 2024-04-18 15:41:03.000000 quickstats-0.7.0.5.1/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5096 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10353 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30687 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13785 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.5.1/quickstats/plots/two_axis_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2024-06-03 07:36:22.000000 quickstats-0.7.0.5.1/quickstats/plots/two_panel_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9999 2024-04-18 15:42:16.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19292 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13182 2024-04-18 15:38:51.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23227 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    34454 2024-05-31 13:13:54.000000 quickstats-0.7.0.5.1/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/default_workspace_extensions.json
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/hep.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/resources/mpl_stylesheets/science.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.5.1/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19773 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.5.1/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18666 2024-04-18 15:39:08.000000 quickstats-0.7.0.5.1/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.5.1/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3039 2024-04-25 03:40:18.000000 quickstats-0.7.0.5.1/quickstats/utils/path_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-04-18 15:35:24.000000 quickstats-0.7.0.5.1/quickstats/utils/py_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27521 2024-04-18 15:36:12.000000 quickstats-0.7.0.5.1/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.5.1/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15330 2024-04-18 15:36:32.000000 quickstats-0.7.0.5.1/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15638 2024-04-18 15:39:31.000000 quickstats-0.7.0.5.1/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2321 2024-04-18 15:36:21.000000 quickstats-0.7.0.5.1/quickstats/utils/sys_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-18 15:35:57.000000 quickstats-0.7.0.5.1/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-06-03 08:47:38.000000 quickstats-0.7.0.5.1/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11106 2024-06-03 08:47:36.000000 quickstats-0.7.0.5.1/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-06-03 08:47:35.000000 quickstats-0.7.0.5.1/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-06-03 08:47:48.000000 quickstats-0.7.0.5.1/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-04-18 15:34:33.000000 quickstats-0.7.0.5.1/setup.py
```

### Comparing `quickstats-0.7.0.5/PKG-INFO` & `quickstats-0.7.0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.5
+Version: 0.7.0.5.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.5/README.md` & `quickstats-0.7.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/algorithms/nll_crossing/BaseMethod.py` & `quickstats-0.7.0.5.1/quickstats/algorithms/nll_crossing/BaseMethod.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/analysis_base.py` & `quickstats-0.7.0.5.1/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.7.0.5.1/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/config_templates.py` & `quickstats-0.7.0.5.1/quickstats/analysis/config_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/data_loading.py` & `quickstats-0.7.0.5.1/quickstats/analysis/data_loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,30 +544,34 @@
         return selection
 
     @semistaticmethod
     def _read_data_from_file(self, filename:str, key:Optional[str]=None,
                              columns:Optional[List[str]]=None,
                              selection:Optional[str]=None) -> pd.DataFrame:
         """
-            Load array data from a file (csv or h5).
+            Load array data from a file (csv, h5 or parquet).
             
             Arguments:
                 filename: string
                     Path to the input data (only csv or h5 formats are allowed).
                 selection: (optional) str
                     Selection applied to the input data (via pandas.DataFrame.query)
         """        
         extension = os.path.splitext(filename)[-1]
-        if extension not in [".csv", ".h5"]:
+        if extension not in [".csv", ".h5", ".hdf", ".parquet"]:
             raise RuntimeError(f'unsupported data format "{extension.strip(".")}"; allowed '
-                               'formats are: csv, h5')
+                               'formats are: csv, h5, hdf, parquet')
         if extension == ".csv":
             df = pd.read_csv(filename, usecols=columns)
-        else:
+        elif extension in ['.h5', '.hdf']:
             df = pd.read_hdf(filename, key=key, columns=columns)
+        elif extension == '.parquet':
+            df = pd.read_parquet(filename, columns=columns)
+        else:
+            raise ValueError(f'invalid file extension: {extension}')
         if selection not in [None, "1", 1]:
             df = df.query(selection).reset_index(drop=True)
         return df
 
     def get_sample_df(self, sample:str, key:Optional[str]=None,
                       columns:Optional[List[str]]=None,
                       selection:Optional[str]=None,
```

### Comparing `quickstats-0.7.0.5/quickstats/analysis/data_preprocessing.py` & `quickstats-0.7.0.5.1/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/event_categorization.py` & `quickstats-0.7.0.5.1/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.7.0.5.1/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.7.0.5.1/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.7.0.5.1/quickstats/analysis/ntuple_process_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import math
 
 import numpy as np
 
 from quickstats import semistaticmethod, ConfigurableObject, ConfigUnit
 from quickstats.utils.common_utils import (combine_dict, reindex_dataframe,
                                            filter_dataframe_by_index_values)
+from quickstats.utils.string_utils import split_str
 from .analysis_path_manager import AnalysisPathManager
 from .config_templates import SampleConfig
 
 class NTupleProcessTool(ConfigurableObject):
     """ Tool for processing root ntuples
     """
 
@@ -244,19 +245,22 @@
                            fmt:str="dict"):
         samples = self.get_validated_samples(samples)
         sample_types = self.get_validated_sample_types(sample_types)
         syst_themes = self.get_validated_syst_themes(syst_themes)
         df = self.sample_df
         selected_df = filter_dataframe_by_index_values(df, (syst_themes, samples, sample_types),
                                                        ('syst_theme', 'sample', 'sample_type'))
+
+
         if fullpath:
             sample_dir = self.sample_config['sample_dir']
             for sample_type in self.sample_type_list:
                 sample_subdir = self.sample_config['sample_subdir'].get(sample_type, '')
-                path_lambda = lambda x: os.path.join(sample_dir, sample_subdir, x)
+                # # need to also consider friends
+                path_lambda = lambda x: ";".join([os.path.join(sample_dir, sample_subdir, path) for path in split_str(x, sep=";")])
                 mask = selected_df.index.get_level_values('sample_type') == sample_type
                 selected_df.loc[mask, ['filepath']] = selected_df.loc[mask, 'filepath'].apply(path_lambda)
         # reindex to the order given in the arguments
         selected_df = reindex_dataframe(selected_df, (syst_themes,
                                                       samples,
                                                       sample_types))
         if fmt.lower() in ["dataframe", "df"]:
@@ -375,14 +379,15 @@
         if self.processor is None:
             raise RuntimeError("processor not initialized (probably missing a process config)")
         paths = self.get_selected_paths(syst_themes=['Nominal'],
                                         samples=samples,
                                         sample_types=sample_types)
         if not paths:
             self.stdout.warning('No inputs matching the given conditions. Skipped processing.')
+            return None
         paths = paths['Nominal']
         outdir = self.path_manager.base_path
         for sample in paths:
             self.processor.set_flags(self.process_flags)
             for sample_type in paths[sample]:
                 sample_paths = paths[sample][sample_type]
                 sample_config = {
```

### Comparing `quickstats-0.7.0.5/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.7.0.5.1/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.7.0.5.1/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.7.0.5.1/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.7.0.5.1/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.7.0.5.1/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/core.py` & `quickstats-0.7.0.5.1/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/inspect_rfile.py` & `quickstats-0.7.0.5.1/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/likelihood_tools.py` & `quickstats-0.7.0.5.1/quickstats/clis/likelihood_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/limit_setting.py` & `quickstats-0.7.0.5.1/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/nuisance_parameter_tools.py` & `quickstats-0.7.0.5.1/quickstats/clis/nuisance_parameter_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/processor_tools.py` & `quickstats-0.7.0.5.1/quickstats/clis/processor_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/stat_tools.py` & `quickstats-0.7.0.5.1/quickstats/clis/stat_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/clis/workspace_tools.py` & `quickstats-0.7.0.5.1/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/__init__.py` & `quickstats-0.7.0.5.1/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/analysis_base.py` & `quickstats-0.7.0.5.1/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/analysis_object.py` & `quickstats-0.7.0.5.1/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/asimov_generator.py` & `quickstats-0.7.0.5.1/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/asymptotic_cls.py` & `quickstats-0.7.0.5.1/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/basics.py` & `quickstats-0.7.0.5.1/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/caching_nll_wrapper.py` & `quickstats-0.7.0.5.1/quickstats/components/caching_nll_wrapper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/discrete_nuisance.py` & `quickstats-0.7.0.5.1/quickstats/components/discrete_nuisance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/extended_minimizer.py` & `quickstats-0.7.0.5.1/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/extended_model.py` & `quickstats-0.7.0.5.1/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/extended_rfile.py` & `quickstats-0.7.0.5.1/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/likelihood.py` & `quickstats-0.7.0.5.1/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/modelling/component_source.py` & `quickstats-0.7.0.5.1/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/modelling/data_modelling.py` & `quickstats-0.7.0.5.1/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/modelling/model_source.py` & `quickstats-0.7.0.5.1/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.7.0.5.1/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.7.0.5.1/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.7.0.5.1/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.7.0.5.1/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/__init__.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_as_hdf.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_hdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_as_parquet.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_as_parquet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_cache.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_cache.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_output_action.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_output_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_progressbar.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_progressbar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_safe_define.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_safe_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/builtin_methods.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/roo_process_config.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/roo_process_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/processors/roo_processor.py` & `quickstats-0.7.0.5.1/quickstats/components/processors/roo_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from typing import Optional, List, Dict, Union
 import os
+import copy
 import glob
 import json
 import time
+
+import numpy as np
 import ROOT
 
 from .builtin_methods import BUILTIN_METHODS
 from .actions import *
 from .roo_process_config import RooProcessConfig
 
-from quickstats import timer, AbstractObject, GeneralEnum, module_exist
+from quickstats import timer, AbstractObject, GeneralEnum, module_exist, semistaticmethod
 from quickstats.interface.root import TFile, RDataFrame, RDataFrameBackend
 from quickstats.interface.xrootd import get_cachedir, set_cachedir, switch_cachedir
 from quickstats.utils.root_utils import declare_expression, close_all_root_files, set_multithread
 from quickstats.utils.path_utils import is_remote_path
 from quickstats.utils.common_utils import get_cpu_count, combine_dict
+from quickstats.utils.string_utils import split_str
 from quickstats.daq import DEFAULT_CACHE_DIR, XRootDSource, ServiceXSource
 
 class RDFVerbosity(GeneralEnum):
     UNSET   = (0, 'kUnset')
     FATAL   = (1, 'kFatal')
     ERROR   = (2, 'kError')
     WARNING = (3, 'kWarning')
@@ -82,14 +86,15 @@
         super().__init__(verbosity=verbosity)
         self.cache = cache
         self.action_tree = None
         if flags is not None:
             self.flags = list(flags)
         else:
             self.flags = []
+        self._file_chains = {}
         self.rdf_frames = {}
         self.rdf = None
         self.global_variables = {}
         self.external_variables = {}
         self.default_treename = None
         self.use_template = use_template
         self.rdf_verbosity = None
@@ -249,39 +254,73 @@
         data_source = data_source_cls(**data_service_options)
         data_source.add_files(filenames)
         filenames = data_source.deliver(**deliver_options)
         if self.data_service == DataDeliveryService.SERVICEX:
             # TO FIX
             self.default_treename = "servicex"
         return filenames
+
+    @staticmethod
+    def _resolve_filechains(filenames:Union[List[str], str]):
+        if isinstance(filenames, str):
+            filenames = [filenames]
+        filechains = {}
+        for filename in filenames:
+            filenames_chain = split_str(filename, sep=';', strip=True)
+            for i, filename_chain in enumerate(filenames_chain):
+                filechains.setdefault(i, [])
+                filechains[i].append(filename_chain)
+        return filechains
+
+    def get_source_filechains(self, filechains:Dict[str, List[str]]):
+        source_filechains = {}
+        nchains = len(filechains)
+        for chain_index, filenames in filechains.items():
+            source_filenames = self.get_source_files(filenames)
+            source_filechains[chain_index] = source_filenames
+            if (not source_filenames):
+                # not matching files
+                if chain_index == 0:
+                    return source_filechains
+                raise RuntimeError(f'No friend files matching the expressions: {filenames}')
+            if (nchains > 1) and (len(source_filenames) > 1):
+                raise RuntimeError('Multiple input files with friends is not supported')
+        return source_filechains
         
     def load_rdf(self,
                  filenames:Union[List[str], str],
                  treename:Optional[str]=None):
-            
-        filenames = self.get_source_files(filenames)
-        if not filenames:
+        filechains = self._resolve_filechains(filenames)
+        filechains = self.get_source_filechains(filechains)
+        if not filechains[0]:
             self.stdout.info('No files to be processed. Skipping.')
             return None
-        self._filenames = filenames
-
+        
         if treename is None:
             treename = self.default_treename
         if treename is None:
-            treename = TFile._get_main_treename(filenames[0])
+            treename = TFile._get_main_treename(filechains[0][0])
             self.stdout.info(f"Using deduced treename: {treename}")
 
-        if len(filenames) == 1:
+        if len(filechains) == 1:
+            filenames = filechains[0]
+        else:
+            filenames = list(zip(*filechains.values()))
+
+        self._filenames = filenames
+        if (len(filechains) == 1) and (len(filenames) == 1):
             self.stdout.info(f'Processing file "{filenames[0]}".')
         else:
-            self.stdout.info("Professing files")
+            def get_filename_repr(filename:str):
+                return "(" + ", ".join(filename) + ")" if isinstance(filename, tuple) else f'"{filename}"'
+            self.stdout.info("Processing files")
             for filename in filenames:
-                self.stdout.info(f'  "{filename}"', bare=True)
+                self.stdout.info(f"  {get_filename_repr(filename)}", bare=True)
                 
-        rdf = RDataFrame.from_files(filenames, treename=treename,
+        rdf = RDataFrame.from_files(*filechains.values(), treename=treename,
                                     backend=self.backend,
                                     backend_options=self.backend_options,
                                     multithread_safe=self.multithread)
         self.rdf = rdf
         return self
     
     def run(self, filenames:Optional[Union[List[str], str]]=None):
@@ -290,15 +329,15 @@
             if filenames is not None:
                 self.load_rdf(filenames)
             self.action_tree.reset()
             self.run_all_actions()
             self.shallow_cleanup()
         self.stdout.info(f"Task finished. Total time taken: {t.interval:.3f} s.")
         result_metadata = {
-            "files": list(self._filenames),
+            "files": copy.deepcopy(self._filenames),
             "real_time": t.real_time_elapsed,
             "cpu_time": t.cpu_time_elapsed
         }
         self.result_metadata = result_metadata
         return self
 
     def get_rdf(self, frame:Optional[str]=None):
```

### Comparing `quickstats-0.7.0.5/quickstats/components/pvalue_toys.py` & `quickstats-0.7.0.5.1/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/roo_inspector.py` & `quickstats-0.7.0.5.1/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/root_object.py` & `quickstats-0.7.0.5.1/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/toy_limit_calculator.py` & `quickstats-0.7.0.5.1/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/__init__.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/sample.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/settings.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/systematic.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.7.0.5.1/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/concurrent/abstract_runner.py` & `quickstats-0.7.0.5.1/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/concurrent/logging.py` & `quickstats-0.7.0.5.1/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.7.0.5.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/concurrent/parameterised_significance.py` & `quickstats-0.7.0.5.1/quickstats/concurrent/parameterised_significance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/abstract_object.py` & `quickstats-0.7.0.5.1/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/configuration.py` & `quickstats-0.7.0.5.1/quickstats/core/configuration.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/constraints.py` & `quickstats-0.7.0.5.1/quickstats/core/constraints.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/decorators.py` & `quickstats-0.7.0.5.1/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/enums.py` & `quickstats-0.7.0.5.1/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/io.py` & `quickstats-0.7.0.5.1/quickstats/core/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/metaclasses.py` & `quickstats-0.7.0.5.1/quickstats/core/metaclasses.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/methods.py` & `quickstats-0.7.0.5.1/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/path_manager.py` & `quickstats-0.7.0.5.1/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/setup.py` & `quickstats-0.7.0.5.1/quickstats/core/setup.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/type_validation.py` & `quickstats-0.7.0.5.1/quickstats/core/type_validation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/core/virtual_trees.py` & `quickstats-0.7.0.5.1/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/daq/remote_data_source.py` & `quickstats-0.7.0.5.1/quickstats/daq/remote_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/daq/servicex_source.py` & `quickstats-0.7.0.5.1/quickstats/daq/servicex_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/daq/xrootd_source.py` & `quickstats-0.7.0.5.1/quickstats/daq/xrootd_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/extensions/extension_dataframe.py` & `quickstats-0.7.0.5.1/quickstats/extensions/extension_dataframe.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/cppyy/core.py` & `quickstats-0.7.0.5.1/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/cppyy/macros.py` & `quickstats-0.7.0.5.1/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.7.0.5.1/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/kerberos/core.py` & `quickstats-0.7.0.5.1/quickstats/interface/kerberos/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/ModelConfig.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/ModelConfig.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RDataFrame.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RDataFrame.py`

 * *Files 7% similar despite different names*

```diff
@@ -157,42 +157,60 @@
     def awkward_array(self, columns:Optional[List[str]]=None, **kwargs):
         rdf = self.rdf
         if rdf is None:
             RuntimeError('RDataFrame instance not initialized')
         return self._awkward_array(rdf, columns=columns, **kwargs)
 
     @semistaticmethod
-    def from_files(self, filenames:Union[List[str], str],
+    def from_files(self, *filenames_chain,
                    treename:Optional[str]=None,
                    columns:Optional[List[str]]=None,
                    backend:str=None,
                    backend_options:Optional[Dict]=None,
                    multithread_safe=True):
         """
         Create RDataFrame instance from a list of input files.
 
         It considers the generic case of files with different treenames. 
         """
-        spec = self.create_spec(filenames,
-                                default_treename=treename)
-        files, trees = self._get_spec_files_and_trees(spec)
+        if not filenames_chain:
+            raise ValueError('No files specified')
         backend = self._parse_backend(backend)
-        if ((backend == RDataFrameBackend.DEFAULT) and \
-            (not self._requires_unsafe_tchain(files)) and \
-            quickstats.root_version >= (6, 28, 0)):
-            dataset_spec = self.get_dataset_spec(spec)
-            return self.from_dataset_spec(dataset_spec, backend=backend,
-                                          backend_options=backend_options)
+        has_friends = len(filenames_chain) > 1
+        specs = []
+        for filenames in filenames_chain:
+            spec = self.create_spec(filenames, default_treename=treename)
+            specs.append(spec)
+        
+        files, trees = self._get_spec_files_and_trees(spec)
+
+        if (not has_friends) and (backend == RDataFrameBackend.DEFAULT) and \
+            (quickstats.root_version >= (6, 28, 0)):
+            spec = specs[0]
+            files, trees = self._get_spec_files_and_trees(spec)
+            if (not self._requires_unsafe_tchain(files)):
+                dataset_spec = self.get_dataset_spec(spec)
+                return self.from_dataset_spec(dataset_spec, backend=backend,
+                                              backend_options=backend_options)
         kernel = self._get_kernel(backend)
-        # do not require TChain
-        if len(set(trees)) == 1:
-            args = (trees[0], files)
+        if not has_friends:
+            # do not require TChain
+            if len(set(trees)) == 1:
+                args = (trees[0], files)
+            else:
+                chain = self.get_chain_from_spec(spec, multithread_safe=multithread_safe)
+                args = (chain,)
         else:
-            chain = self.get_chain_from_spec(spec, multithread_safe=multithread_safe)
-            args = (chain,)
+            main_chain = None
+            for spec in specs:
+                chain = self.get_chain_from_spec(spec, multithread_safe=multithread_safe)
+                if main_chain is None:
+                    main_chain = chain
+                main_chain.AddFriend(chain)
+            args = (main_chain,)
         if columns is not None:
             args += (columns,)
         if backend_options is None:
             backend_options = {}
         return kernel(*args, **backend_options)
 
     @semistaticmethod
```

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooAbsArg.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsArg.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooAbsData.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooArgSet.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooArgSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooCategory.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooDataSet.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooMsgService.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/RooRealVar.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/TChain.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/TChain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/TF1.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/TFile.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/TH1.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/TH2.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/TH3.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/TH3.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/__init__.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/helper.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/macros.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/root/roofit_extension.py` & `quickstats-0.7.0.5.1/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/servicex/config.py` & `quickstats-0.7.0.5.1/quickstats/interface/servicex/config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/servicex/core.py` & `quickstats-0.7.0.5.1/quickstats/interface/servicex/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/tinydb/methods.py` & `quickstats-0.7.0.5.1/quickstats/interface/tinydb/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/xrootd/filesystem.py` & `quickstats-0.7.0.5.1/quickstats/interface/xrootd/filesystem.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/xrootd/path.py` & `quickstats-0.7.0.5.1/quickstats/interface/xrootd/path.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/interface/xrootd/xrd_helper.py` & `quickstats-0.7.0.5.1/quickstats/interface/xrootd/xrd_helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.7.0.5.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.7.0.5.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/QStringUtils.cxx` & `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.7.0.5.1/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.7.0.5.1/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.7.0.5.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/maths/interpolation.py` & `quickstats-0.7.0.5.1/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/maths/numerics.py` & `quickstats-0.7.0.5.1/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/maths/statistics.py` & `quickstats-0.7.0.5.1/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/maths/statistics_jitted.py` & `quickstats-0.7.0.5.1/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/maths/symbolics.py` & `quickstats-0.7.0.5.1/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/parsers/param_parser.py` & `quickstats-0.7.0.5.1/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/parsers/roo_param_setup_parser.py` & `quickstats-0.7.0.5.1/quickstats/parsers/roo_param_setup_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/__init__.py` & `quickstats-0.7.0.5.1/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/abstract_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/abstract_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/bar_chart.py` & `quickstats-0.7.0.5.1/quickstats/plots/two_axis_1D_plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,105 @@
 from typing import Dict, Optional, Union, List, Tuple
 import pandas as pd
 import numpy as np
 
-from quickstats.plots import AbstractPlot
+from quickstats.plots import AbstractPlot, General1DPlot
+from quickstats.utils.common_utils import combine_dict
+from quickstats.plots.template import handle_has_label
 
-class General1DPlot(AbstractPlot):
-
-    STYLES = {
-    }
-    
-    CONFIG = {
-    }
+class TwoAxis1DPlot(General1DPlot):
     
     def __init__(self, data_map:Union[pd.DataFrame, Dict[str, pd.DataFrame]],
-                 label_map:Optional[Dict]=None,
-                 styles_map:Optional[Dict]=None,
-                 color_cycle=None,
-                 styles:Optional[Union[Dict, str]]=None,
-                 analysis_label_options:Optional[Dict]=None,
-                 config:Optional[Dict]=None):
-        
-        self.data_map = data_map
-        self.label_map = label_map
-        self.styles_map = styles_map
+                 **kwargs):
+        super().__init__(data_map=data_map, **kwargs)
         
-        super().__init__(color_cycle=color_cycle,
-                         styles=styles,
-                         analysis_label_options=analysis_label_options,
-                         config=config)
-        
-    def get_default_legend_order(self):
-        if not isinstance(self.data_map, dict):
-            return []
-        else:
-            return list(self.data_map)
-        
-    def draw_single_data(self, ax, data:pd.DataFrame,
-                         xattrib:str, yattrib:str,
-                         yerrloattrib:Optional[str]=None,
-                         yerrhiattrib:Optional[str]=None,
-                         stat_configs:Optional[List[StatPlotConfig]]=None,
-                         styles:Optional[Dict]=None,
-                         label:Optional[str]=None):
-        pass
-
-    # issue of coloring
-    def draw(self, yattrib:str, *xattribs,
-             targets:Optional[List]=None,
-             target_alignment:str="vertical",
-             width:float=1, spacing:float=0.1,
-             xlabel:Optional[str]=None, ylabel:Optional[str]=None,
-             ypad:Optional[float]=0.3, logy:bool=False):
-        
-        ax = self.draw_frame(logx=logx, logy=logy)
+    def draw(self, xattrib:str, yattrib:str,
+             targets_first:List[str],
+             targets_second:List[str],
+             yerrloattrib:Optional[str]=None,
+             yerrhiattrib:Optional[str]=None,
+             xlabel:Optional[str]=None,
+             ylabel_first:Optional[str]=None,
+             ylabel_second:Optional[str]=None,
+             xmin:Optional[float]=None, xmax:Optional[float]=None,
+             ymin_first:Optional[float]=None, ymax_first:Optional[float]=None,
+             ymin_second:Optional[float]=None, ymax_second:Optional[float]=None,
+             ypad_first:Optional[float]=0.3,
+             ypad_second:Optional[float]=0.3,
+             logx:bool=False,
+             logy_first:bool=False,
+             logy_second:bool=False,
+             draw_stats:bool=True):
+        
+        ax1 = self.draw_frame(logx=logx, logy=logy_first)
+        ax2 = ax1.twinx()
+        if logy_second:
+            ax2.set_yscale('log')
         
         legend_order = []
-        if isinstance(self.data_map, pd.DataFrame):
-            if draw_stats and (None in self.stat_configs):
-                stat_configs = self.stat_configs[None]
-            else:
-                stat_configs = None
-            handle, stat_handles = self.draw_single_data(ax, self.data_map,
-                                                         xattrib=xattrib,
-                                                         yattrib=yattrib,
-                                                         yerrloattrib=yerrloattrib,
-                                                         yerrhiattrib=yerrhiattrib,
-                                                         stat_configs=stat_configs,
-                                                         styles=self.styles_map)
-        elif isinstance(self.data_map, dict):
-            if targets is None:
-                targets = list(self.data_map.keys())
+        if isinstance(self.data_map, dict):
             if self.styles_map is None:
                 styles_map = {k:None for k in self.data_map}
             else:
                 styles_map = self.styles_map
             if self.label_map is None:
                 label_map = {k:k for k in self.data_map}
             else:
                 label_map = self.label_map
             handles = {}
-            for target in targets:
-                data = self.data_map[target]
-                styles = styles_map.get(target, None)
-                label = label_map.get(target, "")
-                if draw_stats:
-                    if target in self.stat_configs:
-                        stat_configs = self.stat_configs[target]
-                    elif None in self.stat_configs:
-                        stat_configs = self.stat_configs[None]
+            for ax, targets in [(ax1, targets_first), (ax2, targets_second)]:
+                for target in targets:
+                    data = self.data_map[target]
+                    styles = styles_map.get(target, None)
+                    if styles is None:
+                        styles = {}
+                    label = label_map.get(target, "")
+                    if draw_stats:
+                        if target in self.stat_configs:
+                            stat_configs = self.stat_configs[target]
+                        elif None in self.stat_configs:
+                            stat_configs = self.stat_configs[None]
+                        else:
+                            stat_configs = None
                     else:
                         stat_configs = None
-                else:
-                    stat_configs = None
-                handle, stat_handles = self.draw_single_data(ax, data, 
-                                                             xattrib=xattrib,
-                                                             yattrib=yattrib,
-                                                             yerrloattrib=yerrloattrib,
-                                                             yerrhiattrib=yerrhiattrib,
-                                                             stat_configs=stat_configs,
-                                                             styles=styles,
-                                                             label=label)
-                handles[target] = handle
-                if stat_handles is not None:
-                    for i, stat_handle in enumerate(stat_handles):
-                        if handle_has_label(stat_handle):
-                            handle_name = f"{target}_stat_handle_{i}"
-                            handles[handle_name] = stat_handle
+                    if ('color' not in styles):
+                        styles['color'] = next(self.color_cycle)
+                    handle, stat_handles = self.draw_single_data(ax, data, 
+                                                                 xattrib=xattrib,
+                                                                 yattrib=yattrib,
+                                                                 yerrloattrib=yerrloattrib,
+                                                                 yerrhiattrib=yerrhiattrib,
+                                                                 stat_configs=stat_configs,
+                                                                 styles=styles,
+                                                                 label=label)
+                    handles[target] = handle
+                    if stat_handles is not None:
+                        for i, stat_handle in enumerate(stat_handles):
+                            if handle_has_label(stat_handle):
+                                handle_name = f"{target}_stat_handle_{i}"
+                                handles[handle_name] = stat_handle
             legend_order.extend(handles.keys())
             self.update_legend_handles(handles)
         else:
             raise ValueError("invalid data format")
             
         self.legend_order = legend_order
-        self.draw_legend(ax)
+        handles, labels = self.get_legend_handles_labels()
+        ax1.legend(handles, labels, **self.styles['legend'])
         
-        self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
-        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)
+        tmp_styles = combine_dict(self.styles)
+        self.styles['axis']['y_axis_styles']['left'] = True
+        self.styles['axis']['y_axis_styles']['labelleft'] = True
+        self.styles['axis']['y_axis_styles']['right'] = False
+        self.styles['axis']['y_axis_styles']['labelright'] = False
+        self.draw_axis_components(ax1, xlabel=xlabel, ylabel=ylabel_first)
+        self.styles['axis']['y_axis_styles']['left'] = False
+        self.styles['axis']['y_axis_styles']['labelleft'] = False
+        self.styles['axis']['y_axis_styles']['right'] = True
+        self.styles['axis']['y_axis_styles']['labelright'] = True
+        self.draw_axis_components(ax2, xlabel=xlabel, ylabel=ylabel_second)
+        self.styles = tmp_styles
+        self.set_axis_range(ax1, xmin=xmin, xmax=xmax, ymin=ymin_first, ymax=ymax_first, ypad=ypad_first)
+        self.set_axis_range(ax2, xmin=xmin, xmax=xmax, ymin=ymin_second, ymax=ymax_second, ypad=ypad_second)
         
-        return ax
+        return ax1, ax2
```

### Comparing `quickstats-0.7.0.5/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.7.0.5.1/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/collective_data_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/color_schemes.py` & `quickstats-0.7.0.5.1/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/core.py` & `quickstats-0.7.0.5.1/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/correlation_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/general_1D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/general_2D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/general_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/general_distribution_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/np_ranking_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/sample_purity_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/score_distribution_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/stat_plot_config.py` & `quickstats-0.7.0.5.1/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/template.py` & `quickstats-0.7.0.5.1/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/two_panel_1D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/two_panel_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.7.0.5.1/quickstats/plots/variable_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/root_checker.py` & `quickstats-0.7.0.5.1/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/common_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/data_conversion.py` & `quickstats-0.7.0.5.1/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/hep_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/path_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/py_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/roofit_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/roostats_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/root_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/string_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/sys_utils.py` & `quickstats-0.7.0.5.1/quickstats/utils/sys_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats/utils/xml_tools.py` & `quickstats-0.7.0.5.1/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.5/quickstats.egg-info/PKG-INFO` & `quickstats-0.7.0.5.1/quickstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.5
+Version: 0.7.0.5.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.5/quickstats.egg-info/SOURCES.txt` & `quickstats-0.7.0.5.1/quickstats.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
 quickstats/maths/symbolics.py
 quickstats/parsers/__init__.py
 quickstats/parsers/config_parser.py
 quickstats/parsers/param_parser.py
 quickstats/parsers/roo_param_setup_parser.py
 quickstats/plots/__init__.py
 quickstats/plots/abstract_plot.py
-quickstats/plots/bar_chart.py
 quickstats/plots/bidirectional_bar_chart.py
 quickstats/plots/collective_data_plot.py
 quickstats/plots/color_schemes.py
 quickstats/plots/core.py
 quickstats/plots/correlation_plot.py
 quickstats/plots/general_1D_plot.py
 quickstats/plots/general_2D_plot.py
```

### Comparing `quickstats-0.7.0.5/setup.py` & `quickstats-0.7.0.5.1/setup.py`

 * *Files identical despite different names*

