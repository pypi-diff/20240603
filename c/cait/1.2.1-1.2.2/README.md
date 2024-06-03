# Comparing `tmp/cait-1.2.1-py3-none-any.whl.zip` & `tmp/cait-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,115 +1,166 @@
-Zip file size: 326849 bytes, number of entries: 113
--rw-r--r--  2.0 unx      746 b- defN 23-Dec-20 10:36 cait/__init__.py
--rw-r--r--  2.0 unx    60936 b- defN 24-Jan-22 11:19 cait/data_handler.py
--rw-r--r--  2.0 unx   119663 b- defN 23-Sep-12 14:17 cait/evaluation_tools.py
--rw-r--r--  2.0 unx    47532 b- defN 23-Sep-12 14:17 cait/event_interface.py
--rw-r--r--  2.0 unx    36117 b- defN 24-Jan-22 11:19 cait/viztool.py
+Zip file size: 375852 bytes, number of entries: 164
+-rw-r--r--  2.0 unx      781 b- defN 24-Apr-03 09:29 cait/__init__.py
+-rw-r--r--  2.0 unx       49 b- defN 24-Jun-03 10:56 cait/_version.py
+-rw-r--r--  2.0 unx    61506 b- defN 24-May-21 09:54 cait/data_handler.py
+-rw-r--r--  2.0 unx   119663 b- defN 24-Feb-09 15:37 cait/evaluation_tools.py
+-rw-r--r--  2.0 unx    47532 b- defN 24-Feb-09 15:37 cait/event_interface.py
+-rw-r--r--  2.0 unx    36117 b- defN 24-May-21 09:54 cait/viztool.py
 -rw-r--r--  2.0 unx      439 b- defN 23-Mar-02 11:40 cait/augment/__init__.py
--rw-r--r--  2.0 unx    48244 b- defN 23-Sep-12 14:17 cait/augment/_cryoaug.py
+-rw-r--r--  2.0 unx    48244 b- defN 24-Feb-09 15:37 cait/augment/_cryoaug.py
 -rw-r--r--  2.0 unx      236 b- defN 23-Mar-02 11:40 cait/calibration/__init__.py
--rw-r--r--  2.0 unx     4317 b- defN 23-Sep-12 14:17 cait/calibration/_energy_calibration.py
--rw-r--r--  2.0 unx     5870 b- defN 23-Sep-12 14:17 cait/calibration/_energy_calibration_linear.py
--rw-r--r--  2.0 unx     5353 b- defN 23-Sep-12 14:17 cait/calibration/_energy_calibration_tree.py
--rw-r--r--  2.0 unx    33166 b- defN 24-Jan-22 11:19 cait/calibration/_pulser_model.py
+-rw-r--r--  2.0 unx     4317 b- defN 24-Feb-09 15:37 cait/calibration/_energy_calibration.py
+-rw-r--r--  2.0 unx     5870 b- defN 24-Feb-09 15:37 cait/calibration/_energy_calibration_linear.py
+-rw-r--r--  2.0 unx     5353 b- defN 24-Feb-09 15:37 cait/calibration/_energy_calibration_tree.py
+-rw-r--r--  2.0 unx    33166 b- defN 24-Feb-09 15:37 cait/calibration/_pulser_model.py
 -rw-r--r--  2.0 unx      236 b- defN 23-Mar-02 11:40 cait/cuts/__init__.py
--rw-r--r--  2.0 unx     3724 b- defN 23-Sep-12 14:17 cait/cuts/_cut_class.py
+-rw-r--r--  2.0 unx     3724 b- defN 24-Feb-09 15:37 cait/cuts/_cut_class.py
 -rw-r--r--  2.0 unx     1666 b- defN 23-Mar-02 11:40 cait/cuts/_logical.py
--rw-r--r--  2.0 unx     6527 b- defN 23-Sep-12 14:17 cait/cuts/_rate_cut.py
--rw-r--r--  2.0 unx    11313 b- defN 23-Sep-12 14:17 cait/cuts/_stability_cut.py
+-rw-r--r--  2.0 unx     6527 b- defN 24-Feb-09 15:37 cait/cuts/_rate_cut.py
+-rw-r--r--  2.0 unx    11313 b- defN 24-Feb-09 15:37 cait/cuts/_stability_cut.py
 -rw-r--r--  2.0 unx      577 b- defN 23-Mar-02 11:40 cait/data/__init__.py
--rw-r--r--  2.0 unx     7671 b- defN 23-Sep-12 14:17 cait/data/_baselines.py
--rw-r--r--  2.0 unx     2223 b- defN 23-Sep-12 14:17 cait/data/_converter.py
--rw-r--r--  2.0 unx    16373 b- defN 23-Sep-12 14:17 cait/data/_gen_h5.py
--rw-r--r--  2.0 unx    13450 b- defN 23-Sep-12 14:17 cait/data/_gen_h5_memsafe.py
--rw-r--r--  2.0 unx    14048 b- defN 23-Sep-12 14:17 cait/data/_merge_h5.py
--rw-r--r--  2.0 unx     9005 b- defN 23-Sep-12 14:17 cait/data/_raw.py
--rw-r--r--  2.0 unx     2625 b- defN 23-Sep-12 14:17 cait/data/_shrink_h5.py
--rw-r--r--  2.0 unx    25394 b- defN 23-Sep-13 14:11 cait/data/_test_data.py
--rw-r--r--  2.0 unx     2268 b- defN 23-Sep-12 14:17 cait/data/_xy_file.py
+-rw-r--r--  2.0 unx     7671 b- defN 24-Feb-09 15:37 cait/data/_baselines.py
+-rw-r--r--  2.0 unx     2223 b- defN 24-Feb-09 15:37 cait/data/_converter.py
+-rw-r--r--  2.0 unx    16373 b- defN 24-Feb-09 15:37 cait/data/_gen_h5.py
+-rw-r--r--  2.0 unx    13450 b- defN 24-Feb-09 15:37 cait/data/_gen_h5_memsafe.py
+-rw-r--r--  2.0 unx    14048 b- defN 24-Feb-09 15:37 cait/data/_merge_h5.py
+-rw-r--r--  2.0 unx     9005 b- defN 24-Feb-09 15:37 cait/data/_raw.py
+-rw-r--r--  2.0 unx     2625 b- defN 24-Feb-09 15:37 cait/data/_shrink_h5.py
+-rw-r--r--  2.0 unx    25089 b- defN 24-Apr-03 09:29 cait/data/_test_data.py
+-rw-r--r--  2.0 unx     2268 b- defN 24-Feb-09 15:37 cait/data/_xy_file.py
 -rw-r--r--  2.0 unx      376 b- defN 23-Mar-02 11:40 cait/datasets/__init__.py
--rw-r--r--  2.0 unx      974 b- defN 23-Sep-12 14:17 cait/datasets/_pt_dataloader.py
--rw-r--r--  2.0 unx     9373 b- defN 23-Sep-12 14:17 cait/datasets/_pt_datamodule.py
--rw-r--r--  2.0 unx     7137 b- defN 23-Sep-12 14:17 cait/datasets/_pt_dataset.py
--rw-r--r--  2.0 unx     1764 b- defN 23-Sep-12 14:17 cait/datasets/_pt_sampler.py
--rw-r--r--  2.0 unx     6478 b- defN 23-Sep-12 14:17 cait/datasets/_pt_transforms.py
+-rw-r--r--  2.0 unx      974 b- defN 24-Feb-09 15:37 cait/datasets/_pt_dataloader.py
+-rw-r--r--  2.0 unx     9373 b- defN 24-Feb-09 15:37 cait/datasets/_pt_datamodule.py
+-rw-r--r--  2.0 unx     7137 b- defN 24-Feb-09 15:37 cait/datasets/_pt_dataset.py
+-rw-r--r--  2.0 unx     1764 b- defN 24-Feb-09 15:37 cait/datasets/_pt_sampler.py
+-rw-r--r--  2.0 unx     6478 b- defN 24-Feb-09 15:37 cait/datasets/_pt_transforms.py
 -rw-r--r--  2.0 unx       90 b- defN 23-Mar-02 11:40 cait/evaluation/__init__.py
 -rw-r--r--  2.0 unx    23111 b- defN 23-Mar-02 11:40 cait/evaluation/_color.py
--rw-r--r--  2.0 unx      456 b- defN 23-Sep-12 14:17 cait/evaluation/_make_features.py
+-rw-r--r--  2.0 unx      456 b- defN 24-Feb-09 15:37 cait/evaluation/_make_features.py
 -rw-r--r--  2.0 unx      503 b- defN 23-Mar-02 11:40 cait/evaluation/_pgf_config.py
--rw-r--r--  2.0 unx     2047 b- defN 23-Sep-12 14:17 cait/evaluation/_plot_event.py
+-rw-r--r--  2.0 unx     2047 b- defN 24-Feb-09 15:37 cait/evaluation/_plot_event.py
 -rw-r--r--  2.0 unx      326 b- defN 23-Mar-02 11:40 cait/features/__init__.py
--rw-r--r--  2.0 unx     4711 b- defN 23-Sep-12 14:17 cait/features/_fem.py
--rw-r--r--  2.0 unx    16259 b- defN 23-Sep-12 14:17 cait/features/_mp.py
--rw-r--r--  2.0 unx     1907 b- defN 23-Sep-12 14:17 cait/features/_ph_corr.py
+-rw-r--r--  2.0 unx     4711 b- defN 24-Feb-09 15:37 cait/features/_fem.py
+-rw-r--r--  2.0 unx    16259 b- defN 24-Feb-09 15:37 cait/features/_mp.py
+-rw-r--r--  2.0 unx     1907 b- defN 24-Feb-09 15:37 cait/features/_ph_corr.py
 -rw-r--r--  2.0 unx      339 b- defN 23-Mar-02 11:40 cait/filter/__init__.py
 -rw-r--r--  2.0 unx     1936 b- defN 23-Mar-02 11:40 cait/filter/_extend.py
--rw-r--r--  2.0 unx     2836 b- defN 23-Sep-12 14:17 cait/filter/_ma.py
--rw-r--r--  2.0 unx     8455 b- defN 24-Jan-22 11:19 cait/filter/_of.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-Feb-09 15:37 cait/filter/_ma.py
+-rw-r--r--  2.0 unx    10404 b- defN 24-Mar-10 09:33 cait/filter/_of.py
 -rw-r--r--  2.0 unx      725 b- defN 23-Mar-02 11:40 cait/fit/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 23-Sep-12 14:17 cait/fit/_bl_fit.py
--rw-r--r--  2.0 unx    32126 b- defN 23-Sep-12 14:17 cait/fit/_noise.py
--rw-r--r--  2.0 unx     8510 b- defN 23-Sep-12 14:17 cait/fit/_numerical_fit.py
--rw-r--r--  2.0 unx     5583 b- defN 23-Oct-24 11:09 cait/fit/_pm_fit.py
--rw-r--r--  2.0 unx     4220 b- defN 23-Sep-12 14:17 cait/fit/_saturation.py
--rw-r--r--  2.0 unx     6340 b- defN 23-Sep-12 14:17 cait/fit/_sev.py
--rw-r--r--  2.0 unx    21319 b- defN 24-Jan-22 11:19 cait/fit/_templates.py
--rw-r--r--  2.0 unx     4056 b- defN 23-Sep-12 14:17 cait/fit/_threshold.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Feb-09 15:37 cait/fit/_bl_fit.py
+-rw-r--r--  2.0 unx    32126 b- defN 24-Feb-09 15:37 cait/fit/_noise.py
+-rw-r--r--  2.0 unx     8510 b- defN 24-Feb-09 15:37 cait/fit/_numerical_fit.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-Feb-09 15:37 cait/fit/_pm_fit.py
+-rw-r--r--  2.0 unx     4220 b- defN 24-Feb-09 15:37 cait/fit/_saturation.py
+-rw-r--r--  2.0 unx     6340 b- defN 24-Feb-09 15:37 cait/fit/_sev.py
+-rw-r--r--  2.0 unx    21319 b- defN 24-Feb-09 15:37 cait/fit/_templates.py
+-rw-r--r--  2.0 unx     4056 b- defN 24-Feb-09 15:37 cait/fit/_threshold.py
 -rw-r--r--  2.0 unx      132 b- defN 23-Mar-02 11:40 cait/limit/__init__.py
--rw-r--r--  2.0 unx    15422 b- defN 23-Sep-12 14:17 cait/limit/_yellin.py
+-rw-r--r--  2.0 unx    15426 b- defN 24-Apr-03 09:29 cait/limit/_yellin.py
 -rw-r--r--  2.0 unx      545 b- defN 23-Mar-02 11:40 cait/mixins/__init__.py
--rw-r--r--  2.0 unx    38128 b- defN 23-Sep-13 14:04 cait/mixins/_data_handler_analysis.py
--rw-r--r--  2.0 unx    39093 b- defN 23-Sep-13 14:05 cait/mixins/_data_handler_bin.py
--rw-r--r--  2.0 unx    52517 b- defN 23-Sep-13 14:19 cait/mixins/_data_handler_csmpl.py
--rw-r--r--  2.0 unx    50903 b- defN 24-Jan-22 11:19 cait/mixins/_data_handler_features.py
--rw-r--r--  2.0 unx    29713 b- defN 24-Jan-22 11:19 cait/mixins/_data_handler_fit.py
--rw-r--r--  2.0 unx     5174 b- defN 23-Sep-12 14:17 cait/mixins/_data_handler_ml.py
--rw-r--r--  2.0 unx    43848 b- defN 23-Sep-12 14:17 cait/mixins/_data_handler_plot.py
--rw-r--r--  2.0 unx    34773 b- defN 23-Sep-13 14:08 cait/mixins/_data_handler_rdt.py
--rw-r--r--  2.0 unx    22729 b- defN 23-Sep-12 14:17 cait/mixins/_data_handler_simulate.py
+-rw-r--r--  2.0 unx    38128 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_analysis.py
+-rw-r--r--  2.0 unx    39093 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_bin.py
+-rw-r--r--  2.0 unx    52517 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_csmpl.py
+-rw-r--r--  2.0 unx    53667 b- defN 24-Mar-10 09:33 cait/mixins/_data_handler_features.py
+-rw-r--r--  2.0 unx    29713 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_fit.py
+-rw-r--r--  2.0 unx     5174 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_ml.py
+-rw-r--r--  2.0 unx    43848 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_plot.py
+-rw-r--r--  2.0 unx    34773 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_rdt.py
+-rw-r--r--  2.0 unx    22729 b- defN 24-Feb-09 15:37 cait/mixins/_data_handler_simulate.py
 -rw-r--r--  2.0 unx      396 b- defN 23-Mar-02 11:40 cait/models/__init__.py
--rw-r--r--  2.0 unx     7867 b- defN 24-Jan-22 11:19 cait/models/_cnn_model.py
--rw-r--r--  2.0 unx    10828 b- defN 23-Sep-12 14:17 cait/models/_lstm_model.py
--rw-r--r--  2.0 unx     3434 b- defN 23-Sep-12 14:17 cait/models/_model_handler.py
--rw-r--r--  2.0 unx    10869 b- defN 23-Sep-12 14:17 cait/models/_predict.py
--rw-r--r--  2.0 unx     8386 b- defN 23-Sep-12 14:17 cait/models/_rnn_model.py
--rw-r--r--  2.0 unx     8565 b- defN 23-Sep-12 14:17 cait/models/_separation_lstm.py
--rw-r--r--  2.0 unx    12115 b- defN 23-Sep-12 14:17 cait/models/_transformer_model.py
+-rw-r--r--  2.0 unx     7867 b- defN 24-Feb-09 15:37 cait/models/_cnn_model.py
+-rw-r--r--  2.0 unx    10828 b- defN 24-Feb-09 15:37 cait/models/_lstm_model.py
+-rw-r--r--  2.0 unx     3434 b- defN 24-Feb-09 15:37 cait/models/_model_handler.py
+-rw-r--r--  2.0 unx    10869 b- defN 24-Feb-09 15:37 cait/models/_predict.py
+-rw-r--r--  2.0 unx     8386 b- defN 24-Feb-09 15:37 cait/models/_rnn_model.py
+-rw-r--r--  2.0 unx     8565 b- defN 24-Feb-09 15:37 cait/models/_separation_lstm.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-Feb-09 15:37 cait/models/_transformer_model.py
 -rw-r--r--  2.0 unx      130 b- defN 23-Mar-02 11:40 cait/resources/__init__.py
 -rw-r--r--  2.0 unx     1915 b- defN 23-Mar-02 11:40 cait/resources/_resources.py
 -rw-r--r--  2.0 unx      177 b- defN 23-Mar-02 11:40 cait/simulate/__init__.py
--rw-r--r--  2.0 unx     2217 b- defN 23-Sep-12 14:17 cait/simulate/_generate_pm_par.py
--rw-r--r--  2.0 unx     4225 b- defN 23-Sep-12 14:17 cait/simulate/_sim_bl.py
--rw-r--r--  2.0 unx    13035 b- defN 23-Sep-12 14:17 cait/simulate/_sim_pulses.py
--rw-r--r--  2.0 unx      119 b- defN 23-Sep-12 14:17 cait/styles/__init__.py
--rw-r--r--  2.0 unx     3946 b- defN 24-Jan-22 11:19 cait/styles/_plt_styles.py
--rw-r--r--  2.0 unx     1852 b- defN 23-Jun-05 10:37 cait/styles/_print_styles.py
+-rw-r--r--  2.0 unx     2217 b- defN 24-Feb-09 15:37 cait/simulate/_generate_pm_par.py
+-rw-r--r--  2.0 unx     4225 b- defN 24-Feb-09 15:37 cait/simulate/_sim_bl.py
+-rw-r--r--  2.0 unx    13035 b- defN 24-Feb-09 15:37 cait/simulate/_sim_pulses.py
+-rw-r--r--  2.0 unx      119 b- defN 24-Feb-09 15:37 cait/styles/__init__.py
+-rw-r--r--  2.0 unx     3946 b- defN 24-Feb-09 15:37 cait/styles/_plt_styles.py
+-rw-r--r--  2.0 unx     1852 b- defN 24-Feb-27 14:16 cait/styles/_print_styles.py
 -rw-r--r--  2.0 unx      597 b- defN 23-Mar-02 11:40 cait/trigger/__init__.py
--rw-r--r--  2.0 unx    13292 b- defN 23-Sep-13 14:01 cait/trigger/_bin.py
--rw-r--r--  2.0 unx    26263 b- defN 23-Sep-13 14:03 cait/trigger/_csmpl.py
--rw-r--r--  2.0 unx     3454 b- defN 23-Sep-13 14:03 cait/trigger/_ma_trigger.py
+-rw-r--r--  2.0 unx    13292 b- defN 24-May-16 12:14 cait/trigger/_bin.py
+-rw-r--r--  2.0 unx    26263 b- defN 24-May-16 12:14 cait/trigger/_csmpl.py
+-rw-r--r--  2.0 unx     3454 b- defN 24-Feb-09 15:37 cait/trigger/_ma_trigger.py
 -rw-r--r--  2.0 unx     6437 b- defN 23-Mar-02 11:40 cait/trigger/_peakdet.py
--rw-r--r--  2.0 unx      426 b- defN 24-Jan-22 11:19 cait/versatile/__init__.py
--rw-r--r--  2.0 unx    14372 b- defN 23-Sep-07 12:05 cait/versatile/file.py
--rw-r--r--  2.0 unx    26537 b- defN 24-Jan-22 11:19 cait/versatile/iterators.py
--rw-r--r--  2.0 unx    19329 b- defN 24-Jan-22 11:19 cait/versatile/rdt.py
--rw-r--r--  2.0 unx     9456 b- defN 24-Jan-22 11:19 cait/versatile/utils.py
--rw-r--r--  2.0 unx      144 b- defN 24-Jan-22 11:19 cait/versatile/analysis/__init__.py
--rw-r--r--  2.0 unx    25410 b- defN 24-Jan-22 11:19 cait/versatile/analysis/arrays_with_benefits.py
--rw-r--r--  2.0 unx     9354 b- defN 24-Jan-22 11:19 cait/versatile/analysis/energy_calibration.py
--rw-r--r--  2.0 unx      454 b- defN 24-Jan-22 11:19 cait/versatile/functions/__init__.py
--rw-r--r--  2.0 unx     1744 b- defN 24-Jan-22 11:19 cait/versatile/functions/abstract_functions.py
--rw-r--r--  2.0 unx     9892 b- defN 24-Jan-22 11:19 cait/versatile/functions/event_functions.py
--rw-r--r--  2.0 unx     7785 b- defN 24-Jan-22 11:19 cait/versatile/functions/fit_functions.py
--rw-r--r--  2.0 unx     6163 b- defN 24-Jan-22 11:19 cait/versatile/functions/scalar_functions.py
--rw-r--r--  2.0 unx      180 b- defN 24-Jan-22 11:19 cait/versatile/plot/__init__.py
--rw-r--r--  2.0 unx    34070 b- defN 24-Jan-22 11:19 cait/versatile/plot/plot.py
--rw-r--r--  2.0 unx    26769 b- defN 24-Jan-22 11:19 cait/versatile/plot/plot_backends.py
--rw-r--r--  2.0 unx       98 b- defN 24-Jan-22 11:19 cait/versatile/stream/__init__.py
--rw-r--r--  2.0 unx    23160 b- defN 24-Jan-22 11:19 cait/versatile/stream/stream.py
--rw-r--r--  2.0 unx     7654 b- defN 24-Jan-22 11:19 cait/versatile/stream/trigger.py
--rw-r--r--  2.0 unx    35149 b- defN 24-Jan-22 11:20 cait-1.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5529 b- defN 24-Jan-22 11:20 cait-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-22 11:20 cait-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Jan-22 11:20 cait-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9474 b- defN 24-Jan-22 11:20 cait-1.2.1.dist-info/RECORD
-113 files, 1398855 bytes uncompressed, 312077 bytes compressed:  77.7%
+-rw-r--r--  2.0 unx      132 b- defN 24-Apr-26 19:01 cait/versatile/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 24-Mar-23 15:07 cait/versatile/analysisobjects/__init__.py
+-rw-r--r--  2.0 unx     1518 b- defN 24-Mar-23 15:07 cait/versatile/analysisobjects/arraywithbenefits.py
+-rw-r--r--  2.0 unx     9354 b- defN 24-Mar-23 15:07 cait/versatile/analysisobjects/energy_calibration.py
+-rw-r--r--  2.0 unx     7711 b- defN 24-Apr-09 07:13 cait/versatile/analysisobjects/nps.py
+-rw-r--r--  2.0 unx    10118 b- defN 24-Apr-22 08:58 cait/versatile/analysisobjects/of.py
+-rw-r--r--  2.0 unx     8446 b- defN 24-Apr-09 07:14 cait/versatile/analysisobjects/sev.py
+-rw-r--r--  2.0 unx      159 b- defN 24-Mar-23 15:07 cait/versatile/datasources/__init__.py
+-rw-r--r--  2.0 unx      338 b- defN 24-May-21 09:54 cait/versatile/datasources/datasourcebase.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/datasources/hardwaretriggered/__init__.py
+-rw-r--r--  2.0 unx     3430 b- defN 24-May-16 12:14 cait/versatile/datasources/hardwaretriggered/par_file.py
+-rw-r--r--  2.0 unx    18219 b- defN 24-May-21 09:54 cait/versatile/datasources/hardwaretriggered/rdt_file.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/datasources/simulation/__init__.py
+-rw-r--r--  2.0 unx     1004 b- defN 24-Mar-23 15:07 cait/versatile/datasources/simulation/ebl_pulse_sim.py
+-rw-r--r--  2.0 unx     4601 b- defN 24-May-21 09:54 cait/versatile/datasources/simulation/mock.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/datasources/stream/__init__.py
+-rw-r--r--  2.0 unx     3180 b- defN 24-May-21 09:54 cait/versatile/datasources/stream/factory.py
+-rw-r--r--  2.0 unx     3714 b- defN 24-May-21 09:54 cait/versatile/datasources/stream/impl_cresst.py
+-rw-r--r--  2.0 unx     2862 b- defN 24-May-21 09:54 cait/versatile/datasources/stream/impl_sum.py
+-rw-r--r--  2.0 unx     3578 b- defN 24-May-28 13:16 cait/versatile/datasources/stream/impl_vdaq2.py
+-rw-r--r--  2.0 unx     3857 b- defN 24-May-21 09:54 cait/versatile/datasources/stream/impl_vdaq3.py
+-rw-r--r--  2.0 unx    10486 b- defN 24-May-21 09:54 cait/versatile/datasources/stream/streambase.py
+-rw-r--r--  2.0 unx      391 b- defN 24-Apr-24 08:03 cait/versatile/eventfunctions/__init__.py
+-rw-r--r--  2.0 unx     2151 b- defN 24-Mar-28 10:30 cait/versatile/eventfunctions/functionbase.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/eventfunctions/processing/__init__.py
+-rw-r--r--  2.0 unx     1290 b- defN 24-Mar-28 10:30 cait/versatile/eventfunctions/processing/align.py
+-rw-r--r--  2.0 unx     1962 b- defN 24-Apr-03 14:03 cait/versatile/eventfunctions/processing/boxcarsmoothing.py
+-rw-r--r--  2.0 unx     1821 b- defN 24-Apr-03 14:03 cait/versatile/eventfunctions/processing/downsample.py
+-rw-r--r--  2.0 unx     1544 b- defN 24-Mar-28 10:30 cait/versatile/eventfunctions/processing/helper.py
+-rw-r--r--  2.0 unx     1762 b- defN 24-Apr-03 13:50 cait/versatile/eventfunctions/processing/optimumfiltering.py
+-rw-r--r--  2.0 unx     2403 b- defN 24-Apr-03 14:03 cait/versatile/eventfunctions/processing/removebaseline.py
+-rw-r--r--  2.0 unx     1525 b- defN 24-Apr-03 13:53 cait/versatile/eventfunctions/processing/tukey.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/eventfunctions/scalarfunctions/__init__.py
+-rw-r--r--  2.0 unx     8208 b- defN 24-Apr-03 14:13 cait/versatile/eventfunctions/scalarfunctions/calcmp.py
+-rw-r--r--  2.0 unx     3419 b- defN 24-Mar-28 10:30 cait/versatile/eventfunctions/scalarfunctions/classify.py
+-rw-r--r--  2.0 unx     7642 b- defN 24-Apr-03 14:06 cait/versatile/eventfunctions/scalarfunctions/fitbaseline.py
+-rw-r--r--  2.0 unx      206 b- defN 24-May-28 13:16 cait/versatile/functions/__init__.py
+-rw-r--r--  2.0 unx     4009 b- defN 24-May-28 13:16 cait/versatile/functions/apply.py
+-rw-r--r--  2.0 unx    14373 b- defN 24-Mar-23 15:07 cait/versatile/functions/file.py
+-rw-r--r--  2.0 unx     9456 b- defN 24-Mar-23 15:07 cait/versatile/functions/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/functions/trigger/__init__.py
+-rw-r--r--  2.0 unx     7924 b- defN 24-May-28 13:16 cait/versatile/functions/trigger/trigger.py
+-rw-r--r--  2.0 unx     3845 b- defN 24-May-28 13:16 cait/versatile/functions/trigger/trigger_of.py
+-rw-r--r--  2.0 unx     4234 b- defN 24-May-28 13:16 cait/versatile/functions/trigger/trigger_zscore.py
+-rw-r--r--  2.0 unx     6199 b- defN 24-May-28 13:16 cait/versatile/functions/trigger/triggerbase.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/iterators/__init__.py
+-rw-r--r--  2.0 unx     3582 b- defN 24-Mar-28 10:30 cait/versatile/iterators/batchresolver.py
+-rw-r--r--  2.0 unx     6608 b- defN 24-May-21 09:54 cait/versatile/iterators/impl_h5.py
+-rw-r--r--  2.0 unx     3012 b- defN 24-May-21 09:54 cait/versatile/iterators/impl_mock.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-Mar-23 15:07 cait/versatile/iterators/impl_pulsesim.py
+-rw-r--r--  2.0 unx     3753 b- defN 24-May-21 09:54 cait/versatile/iterators/impl_rdt.py
+-rw-r--r--  2.0 unx     4543 b- defN 24-May-21 09:54 cait/versatile/iterators/impl_stream.py
+-rw-r--r--  2.0 unx    15289 b- defN 24-May-21 09:54 cait/versatile/iterators/iteratorbase.py
+-rw-r--r--  2.0 unx      270 b- defN 24-May-28 13:23 cait/versatile/plot/__init__.py
+-rw-r--r--  2.0 unx    13093 b- defN 24-Jun-03 12:30 cait/versatile/plot/viewer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/plot/backends/__init__.py
+-rw-r--r--  2.0 unx     1819 b- defN 24-Mar-23 15:07 cait/versatile/plot/backends/backendbase.py
+-rw-r--r--  2.0 unx      726 b- defN 24-Mar-23 15:07 cait/versatile/plot/backends/helper.py
+-rw-r--r--  2.0 unx    14605 b- defN 24-Mar-28 10:30 cait/versatile/plot/backends/impl_matplotlib.py
+-rw-r--r--  2.0 unx    13269 b- defN 24-Jun-03 10:56 cait/versatile/plot/backends/impl_plotly.py
+-rw-r--r--  2.0 unx    11921 b- defN 24-Mar-23 15:07 cait/versatile/plot/backends/impl_uniplot.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/plot/basic/__init__.py
+-rw-r--r--  2.0 unx     1861 b- defN 24-Jun-03 12:30 cait/versatile/plot/basic/histogram.py
+-rw-r--r--  2.0 unx     1919 b- defN 24-Jun-03 12:30 cait/versatile/plot/basic/line.py
+-rw-r--r--  2.0 unx     1963 b- defN 24-Jun-03 12:30 cait/versatile/plot/basic/scatter.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 09:29 cait/versatile/plot/highlevel/__init__.py
+-rw-r--r--  2.0 unx     2731 b- defN 24-Mar-28 10:30 cait/versatile/plot/highlevel/preview.py
+-rw-r--r--  2.0 unx     5975 b- defN 24-May-28 13:45 cait/versatile/plot/highlevel/scatterpreview.py
+-rw-r--r--  2.0 unx     7821 b- defN 24-May-28 13:19 cait/versatile/plot/highlevel/streamviewer.py
+-rw-r--r--  2.0 unx    35149 b- defN 24-Jun-03 12:53 cait-1.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6156 b- defN 24-Jun-03 12:53 cait-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 12:53 cait-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Jun-03 12:53 cait-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    14768 b- defN 24-Jun-03 12:53 cait-1.2.2.dist-info/RECORD
+164 files, 1480600 bytes uncompressed, 352366 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: cait/__init__.py
 Comment: 
 
+Filename: cait/_version.py
+Comment: 
+
 Filename: cait/data_handler.py
 Comment: 
 
 Filename: cait/evaluation_tools.py
 Comment: 
 
 Filename: cait/event_interface.py
@@ -264,77 +267,227 @@
 
 Filename: cait/trigger/_peakdet.py
 Comment: 
 
 Filename: cait/versatile/__init__.py
 Comment: 
 
-Filename: cait/versatile/file.py
+Filename: cait/versatile/analysisobjects/__init__.py
+Comment: 
+
+Filename: cait/versatile/analysisobjects/arraywithbenefits.py
+Comment: 
+
+Filename: cait/versatile/analysisobjects/energy_calibration.py
+Comment: 
+
+Filename: cait/versatile/analysisobjects/nps.py
+Comment: 
+
+Filename: cait/versatile/analysisobjects/of.py
+Comment: 
+
+Filename: cait/versatile/analysisobjects/sev.py
+Comment: 
+
+Filename: cait/versatile/datasources/__init__.py
+Comment: 
+
+Filename: cait/versatile/datasources/datasourcebase.py
+Comment: 
+
+Filename: cait/versatile/datasources/hardwaretriggered/__init__.py
+Comment: 
+
+Filename: cait/versatile/datasources/hardwaretriggered/par_file.py
+Comment: 
+
+Filename: cait/versatile/datasources/hardwaretriggered/rdt_file.py
+Comment: 
+
+Filename: cait/versatile/datasources/simulation/__init__.py
+Comment: 
+
+Filename: cait/versatile/datasources/simulation/ebl_pulse_sim.py
+Comment: 
+
+Filename: cait/versatile/datasources/simulation/mock.py
+Comment: 
+
+Filename: cait/versatile/datasources/stream/__init__.py
+Comment: 
+
+Filename: cait/versatile/datasources/stream/factory.py
+Comment: 
+
+Filename: cait/versatile/datasources/stream/impl_cresst.py
+Comment: 
+
+Filename: cait/versatile/datasources/stream/impl_sum.py
+Comment: 
+
+Filename: cait/versatile/datasources/stream/impl_vdaq2.py
+Comment: 
+
+Filename: cait/versatile/datasources/stream/impl_vdaq3.py
+Comment: 
+
+Filename: cait/versatile/datasources/stream/streambase.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/__init__.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/functionbase.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/processing/__init__.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/processing/align.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/processing/boxcarsmoothing.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/processing/downsample.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/processing/helper.py
+Comment: 
+
+Filename: cait/versatile/eventfunctions/processing/optimumfiltering.py
 Comment: 
 
-Filename: cait/versatile/iterators.py
+Filename: cait/versatile/eventfunctions/processing/removebaseline.py
 Comment: 
 
-Filename: cait/versatile/rdt.py
+Filename: cait/versatile/eventfunctions/processing/tukey.py
 Comment: 
 
-Filename: cait/versatile/utils.py
+Filename: cait/versatile/eventfunctions/scalarfunctions/__init__.py
 Comment: 
 
-Filename: cait/versatile/analysis/__init__.py
+Filename: cait/versatile/eventfunctions/scalarfunctions/calcmp.py
 Comment: 
 
-Filename: cait/versatile/analysis/arrays_with_benefits.py
+Filename: cait/versatile/eventfunctions/scalarfunctions/classify.py
 Comment: 
 
-Filename: cait/versatile/analysis/energy_calibration.py
+Filename: cait/versatile/eventfunctions/scalarfunctions/fitbaseline.py
 Comment: 
 
 Filename: cait/versatile/functions/__init__.py
 Comment: 
 
-Filename: cait/versatile/functions/abstract_functions.py
+Filename: cait/versatile/functions/apply.py
+Comment: 
+
+Filename: cait/versatile/functions/file.py
+Comment: 
+
+Filename: cait/versatile/functions/utils.py
+Comment: 
+
+Filename: cait/versatile/functions/trigger/__init__.py
 Comment: 
 
-Filename: cait/versatile/functions/event_functions.py
+Filename: cait/versatile/functions/trigger/trigger.py
 Comment: 
 
-Filename: cait/versatile/functions/fit_functions.py
+Filename: cait/versatile/functions/trigger/trigger_of.py
 Comment: 
 
-Filename: cait/versatile/functions/scalar_functions.py
+Filename: cait/versatile/functions/trigger/trigger_zscore.py
+Comment: 
+
+Filename: cait/versatile/functions/trigger/triggerbase.py
+Comment: 
+
+Filename: cait/versatile/iterators/__init__.py
+Comment: 
+
+Filename: cait/versatile/iterators/batchresolver.py
+Comment: 
+
+Filename: cait/versatile/iterators/impl_h5.py
+Comment: 
+
+Filename: cait/versatile/iterators/impl_mock.py
+Comment: 
+
+Filename: cait/versatile/iterators/impl_pulsesim.py
+Comment: 
+
+Filename: cait/versatile/iterators/impl_rdt.py
+Comment: 
+
+Filename: cait/versatile/iterators/impl_stream.py
+Comment: 
+
+Filename: cait/versatile/iterators/iteratorbase.py
 Comment: 
 
 Filename: cait/versatile/plot/__init__.py
 Comment: 
 
-Filename: cait/versatile/plot/plot.py
+Filename: cait/versatile/plot/viewer.py
+Comment: 
+
+Filename: cait/versatile/plot/backends/__init__.py
+Comment: 
+
+Filename: cait/versatile/plot/backends/backendbase.py
+Comment: 
+
+Filename: cait/versatile/plot/backends/helper.py
+Comment: 
+
+Filename: cait/versatile/plot/backends/impl_matplotlib.py
+Comment: 
+
+Filename: cait/versatile/plot/backends/impl_plotly.py
+Comment: 
+
+Filename: cait/versatile/plot/backends/impl_uniplot.py
+Comment: 
+
+Filename: cait/versatile/plot/basic/__init__.py
+Comment: 
+
+Filename: cait/versatile/plot/basic/histogram.py
+Comment: 
+
+Filename: cait/versatile/plot/basic/line.py
+Comment: 
+
+Filename: cait/versatile/plot/basic/scatter.py
 Comment: 
 
-Filename: cait/versatile/plot/plot_backends.py
+Filename: cait/versatile/plot/highlevel/__init__.py
 Comment: 
 
-Filename: cait/versatile/stream/__init__.py
+Filename: cait/versatile/plot/highlevel/preview.py
 Comment: 
 
-Filename: cait/versatile/stream/stream.py
+Filename: cait/versatile/plot/highlevel/scatterpreview.py
 Comment: 
 
-Filename: cait/versatile/stream/trigger.py
+Filename: cait/versatile/plot/highlevel/streamviewer.py
 Comment: 
 
-Filename: cait-1.2.1.dist-info/LICENSE
+Filename: cait-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: cait-1.2.1.dist-info/METADATA
+Filename: cait-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: cait-1.2.1.dist-info/WHEEL
+Filename: cait-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: cait-1.2.1.dist-info/top_level.txt
+Filename: cait-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cait-1.2.1.dist-info/RECORD
+Filename: cait-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cait/__init__.py

```diff
@@ -2,14 +2,16 @@
 from .data_handler import DataHandler
 from .models._model_handler import ModelHandler
 from .evaluation_tools import EvaluationTools
 from .viztool import VizTool
 from .limit import *
 from .resources import *
 
+from ._version import __version__
+
 __all__ = ['EventInterface',
            'DataHandler',
            'ModelHandler',
            'EvaluationTools',
            'VizTool',
            'data',
            'datasets',
```

## cait/data_handler.py

```diff
@@ -14,16 +14,17 @@
 from .mixins._data_handler_features import FeaturesMixin
 from .mixins._data_handler_analysis import AnalysisMixin
 from .mixins._data_handler_fit import FitMixin
 from .mixins._data_handler_csmpl import CsmplMixin
 from .mixins._data_handler_ml import MachineLearningMixin
 from .mixins._data_handler_bin import BinMixin
 from .styles._print_styles import fmt_gr, fmt_ds, fmt_virt, sizeof_fmt, txt_fmt, datetime_fmt
-from .versatile.file import ds_source_available
-from .versatile.iterators import H5Iterator, IteratorBaseClass
+from .versatile.functions.file import ds_source_available
+from .versatile.iterators.impl_h5 import H5Iterator
+from .versatile.iterators.iteratorbase import IteratorBaseClass
 
 MAINPAR = ['pulse_height', 'onset', 'rise_time', 'decay_time', 'slope']
 ADD_MAINPAR = ['array_max', 'array_min', 'var_first_eight', 
                'mean_first_eight', 'var_last_eight', 'mean_last_eight', 
                'var', 'mean', 'skewness', 'max_derivative',
                'ind_max_derivative', 'min_derivative', 'ind_min_derivative', 
                'max_filtered', 'ind_max_filtered', 'skewness_filtered_peak']
@@ -316,19 +317,19 @@
         with h5py.File(self.get_filepath(), 'r') as f:
             n_events = f[group]["event"].shape[1]
             
         inds = np.arange(n_events)
 
         if flag is not None: inds = inds[flag]
 
-        return H5Iterator(path_h5=self.get_filepath(), group=group, dataset="event", channels=channel, inds=inds, batch_size=batch_size)
+        return H5Iterator(self, group=group, channels=channel, inds=inds, batch_size=batch_size)
     
     def include_event_iterator(self, group: str, it: IteratorBaseClass, dtype: str = 'float32'):
         """
-        Includes the events returned by an iterator into dataset 'event' of a specified group. 
+        Includes the events returned by an iterator into dataset 'event' of a specified group. The timestamps of the iterator are saved in datasets 'time_s' and 'time_mus' of the same group, in alignment with the convention of cait.
 
         :param group: The target group in the HDF5 file.
         :type group: str
         :param it: The iterator whose events we want to include.
         :type it: IteratorBaseClass
         :param dtype: The datatype which the events should be stored as. Either 'float32' or 'float64'. Some `cait` methods expect 'float32' event datasets. Defaults to 'float32'
         :type dtype: str, optional
@@ -375,14 +376,22 @@
                         if it.n_channels > 1:
                             ev = np.transpose(ev, axes=[1,0,2])
                     else:
                         step, sl = 1, ind
 
                     hdf5ds[:, sl, :] = ev
                     ind += step
+
+        # Include timestamps
+        sec = (it.timestamps//1e6).astype(np.int32)
+        mus = (it.timestamps%1e6).astype(np.int32)
+        hours = (sec.astype(np.int64)*int(1e6) + mus.astype(np.int64) - it.ds_start_us)/1e6/3600
+        
+        self.set(group, overwrite_existing=True, time_s=sec, time_mus=mus, dtype=np.int32)
+        self.set(group, overwrite_existing=True, hours=hours, dtype=np.float64)
     
     def import_labels(self,
                       path_labels: str,
                       type: str = 'events',
                       path_h5=None):
         """
         Include the `*.csv` file with the labels into the HDF5 File.
```

## cait/data/_test_data.py

```diff
@@ -305,34 +305,30 @@
         tpas = np.zeros(self.nmbr_events * self.nmbr_channels)
 
         for e in range(self.nmbr_events):
             for c in range(self.nmbr_channels):
                 idx = int(e * self.nmbr_channels + c)
                 recs['detector_nmbr'][idx] = self.channels[c]
                 recs['pulse_height'][idx] = self._saturation_curve(
-                    self.all_tpas[e] * self.ph_deviations[e] + np.random.normal(loc=self.offset[c],
-                                                                                scale=
-                                                                                self.baseline_resolution[
-                                                                                    c], size=1),
+                    self.all_tpas[e] * self.ph_deviations[e] + np.random.normal(loc=self.offset[c], scale=self.baseline_resolution[c]),
                     slope=self.slopes[c],
-                    scale=self.scales[c]) * np.random.normal(loc=1,
-                                                             scale=0.05, size=1)
+                    scale=self.scales[c]
+                    ) * np.random.normal(loc=1, scale=0.05)
                 recs['time_stamp_low'][idx] = int((((e + 1) * self.pulser_interval) * 1e7) % (2 ** 32))
                 recs['time_stamp_high'][idx] = int(((e + 1) * self.pulser_interval) * 1e7 / (2 ** 32))
                 recs['dead_time'][idx] = 0
                 recs['mus_since_last_tp'][idx] = 0
                 tpas[idx] = self.all_tpas[e]
 
         recs = recs[tpas > 10]
 
         # write the array to file
-        f = open(self.filepath + ".con", "bw")
-        np.zeros(3, dtype=np.int32).tofile(f)
-        recs.tofile(f)
-        f.close()
+        with open(self.filepath + ".con", "bw") as f:
+            np.zeros(3, dtype=np.int32).tofile(f)
+            recs.tofile(f)
 
         print('Con file written.')
 
     def _generate_par_file(self, start_offset: float = 0):
         """
         Generate a par file from the measurement.
```

## cait/filter/_of.py

```diff
@@ -86,15 +86,16 @@
     event_filtered = irfft(event_filtered)  # fft back to time space
 
     return event_filtered
 
 
 def get_amplitudes(events_array, stdevent, nps, hard_restrict=False, down=1, window=False,
                    peakpos=None, return_peakpos=False, flexibility=20,
-                   baseline_model='constant', pretrigger_samples=500, transfer_function=None):
+                   baseline_model='constant', pretrigger_samples=500, transfer_function=None,
+                   calc_rms=False):
     """
     This function determines the amplitudes of several events with optimal sig-noise-ratio.
 
     :param events_array: 2D array (nmbr_events, rec_length), the events to determine ph
     :param stdevent: 1D array, the standardevent
     :param nps: 1D array, length N/2 + 1, the noise power spectrum
     :param hard_restrict: bool, The maximum search is restricted to 20-30% of the record window.
@@ -104,14 +105,15 @@
     :param return_peakpos: bool, if true a second array is returned, namely the peak positions within the arrays
     :param flexibility: int, in case a peak position is provided, the maximum search can still deviate by this
         amount of samples
     :param baseline_model: str, which baseline model to use, either "constant", "linear" or "exponential"
     :param pretrigger_samples: int, the number of samples from the start of the record window to evaluate the baseline
     :param transition_function: 2D complex float numpy array, use this transfer function instead of calculating it
         again from the stdevent and nps
+    :param calc_rms: bool, if true tmr RMS of the filtered peak is also calculated
     :return: 1D array size (nmbr_events), the phs after of filtering; if return_peakpos is true, this is instead
         a 2-tuple of the of_ph and the maximum positions
     """
 
     length = events_array.shape[1]
     rem_off(events_array, baseline_model=baseline_model, pretrigger_samples=pretrigger_samples)
 
@@ -124,32 +126,68 @@
         nps = np.concatenate(([nps_offset], nps))
 
     # calc transition function
     if transfer_function is None:
         transfer_function = optimal_transfer_function(stdevent, nps, window=window)
     # filter events
     events_filtered = np.array([filter_event(event, transfer_function, window=window) for event in events_array])
+    # filter standard event
+    if calc_rms:
+        stdevent_filtered = filter_event(np.copy(stdevent), transfer_function, window=window)
     # get maximal heights of filtered events
     if peakpos is not None:
         amplitudes = np.array(
             [np.max(events_filtered[i, int(p - flexibility):int(p + flexibility)]) for i, p in enumerate(peakpos)])
     elif not hard_restrict:
+        peakpos = np.argmax(events_filtered[:, int(length / 8):-int(length / 8)], axis=1)
+        peakpos += int(length / 8)
         if return_peakpos:
-            peakpos = np.argmax(events_filtered[:, int(length / 8):-int(length / 8)], axis=1)
-            peakpos += int(length / 8)
             amplitudes = np.array(
                 [np.max(events_filtered[i, int(p - flexibility):int(p + flexibility)]) for i, p in enumerate(peakpos)])
         else:
             amplitudes = np.max(events_filtered[:, int(length / 8):-int(length / 8)], axis=1)
     else:
+        peakpos = np.argmax(events_filtered[:, int(length * 20 / 100):int(length * 30 / 100)], axis=1)
+        peakpos += int(length * 20 / 100)
         if return_peakpos:
-            peakpos = np.argmax(events_filtered[:, int(length * 20 / 100):int(length * 30 / 100)], axis=1)
-            peakpos += int(length * 20 / 100)
             amplitudes = np.array(
                 [np.max(events_filtered[i, int(p - flexibility):int(p + flexibility)]) for i, p in enumerate(peakpos)])
         else:
             amplitudes = np.max(events_filtered[:, int(length * 20 / 100):int(length * 30 / 100)], axis=1)
 
-    if return_peakpos:
+    if calc_rms:
+        rms = get_of_rms(events_filtered,stdevent_filtered,peakpos,amplitudes,around_peak=False)
+        rms_peak = get_of_rms(events_filtered,stdevent_filtered,peakpos,amplitudes,around_peak=True)
+
+    if return_peakpos and calc_rms:
+        return amplitudes, peakpos, rms, rms_peak
+    elif return_peakpos and not calc_rms:
         return amplitudes, peakpos
+    elif not return_peakpos and calc_rms:
+        return amplitudes, rms, rms_peak
     else:
         return amplitudes
+
+def get_of_rms(events_filtered,stdevent_filtered,peakpos,amplitudes,around_peak=False):
+    """
+    This function calculates the rms between the filtered events and the filtered standard event.
+
+    :param events_filtered: 2D array (nmbr_events, rec_length), the filtered events
+    :param stdevent_filtered: 1D array (rec_length), the filtered standard event
+    :param peakpos: 1D array (nmbr_events), the positions of the maxima of the filtered events
+    :param amplitudes: 1D array (nmbr_events), the of amplitude of the events
+    :param around_peak: bool, calculate the rms only around the peak 
+    :return: 1D array (nmbr_events) of rms values
+    """
+    length = events_filtered.shape[1]
+    stdevent_peakpos = np.argmax(stdevent_filtered)
+    rms = np.zeros_like(amplitudes)
+    for i,ev in enumerate(events_filtered):
+        this_stdevent = np.roll(stdevent_filtered*amplitudes[i],int(peakpos[i]-stdevent_peakpos))
+        if around_peak: this_stdevent = this_stdevent[stdevent_peakpos-int(length/32):stdevent_peakpos+int(length/32)]
+        if around_peak:
+            this_ev = ev[int(peakpos[i]-int(length/32)):int(peakpos[i]+int(length/32))]
+            rms[i] = np.mean((this_ev-this_stdevent) ** 2)
+        else:
+            rms[i] = np.mean((ev-this_stdevent) ** 2)
+
+    return rms
```

## cait/limit/_yellin.py

```diff
@@ -315,16 +315,16 @@
             print('Plot the limit.')
             plt.close()
             use_cait_style()
             plt.plot(x, y)
             make_grid()
             plt.xscale('log')
             plt.yscale('log')
-            plt.xlabel("$m_\chi$ [GeV c${^-2}$]")
-            plt.ylabel("$\sigma_0$ [cm$^{-2}$]")
+            plt.xlabel(r"$m_\chi$ [GeV c${^-2}$]")
+            plt.ylabel(r"$\sigma_0$ [cm$^{-2}$]")
             plt.show()
 
         self.x = x
         self.limit = y
 
         return x, y
 
@@ -339,15 +339,15 @@
         :param wimp_masses: list of float, the wimp masses for that we want to do the plot
         """
         plt.close()
         use_cait_style()
         x = np.linspace(.1, 5., 100)
         for i, m in enumerate(wimp_masses):
             y = [expected_interaction_rate(e, m, 16) for e in x]
-            plt.plot(x, y, label="$m_\chi$ = {} GeV".format(m), zorder=10 + 2*i)
+            plt.plot(x, y, label=r"$m_\chi$ = {} GeV".format(m), zorder=10 + 2*i)
         make_grid()
         plt.xlabel("Recoil Energy (keV)")
         plt.ylabel("dR/dE (kg$^{-1}$ d$^{-1}$ keV$^{-1}$)")
         plt.legend()
         plt.show()
 
     def plot_recoil_distribution(self,
@@ -365,15 +365,15 @@
         for i, m in enumerate(wimp_masses):
             y = [expected_recoil_rate(e,
                                       m,
                                       self.component_mass,
                                       self.component_nucleons,
                                       self.component_efficiencies,
                                       self.exposure) for e in x]
-            plt.plot(x, y, label="$m_\chi$ = {:.1} GeV".format(m), zorder=10 + 2*i)
+            plt.plot(x, y, label=r"$m_\chi$ = {:.1} GeV".format(m), zorder=10 + 2*i)
         make_grid()
         plt.xlabel("Recoil Energy (keV)")
         plt.ylabel("dN/dE (keV$^{-1}$)")
         plt.legend()
         plt.show()
 
     def plot_observations(self,
```

## cait/mixins/_data_handler_features.py

```diff
@@ -410,15 +410,15 @@
 
             print('OF updated.')
 
     # apply the optimum filter
     def apply_of(self, type='events', name_appendix_group: str = '', name_appendix_set: str = '',
                  chunk_size=10000, hard_restrict=False, down=1, window=True, first_channel_dominant=False,
                  baseline_model='constant', pretrigger_samples=500, onset_to_dominant_channel=None,
-                 flexibility=1):
+                 flexibility=1, calc_rms=False):
         """
         Calculates the height of events or testpulses after applying the optimum filter.
 
         :param type: The group name in the HDF5 set, either events of testpulses.
         :type type: string
         :param name_appendix_group: A string that is appended to the stdevent group in the HDF5 set.
         :type name_appendix_group: string
@@ -443,17 +443,22 @@
             trigger region.
         :type pretrigger_samples: int
         :param onset_to_dominant_channel: The difference in the onset value to the dominant channel. If e.g. the second
             channel has a typical max_pos value of 4000, but the first of 4100, then the onset for this would be -100.
         :type onset_to_dominant_channel: list of ints
         :param flexibility: In case a peak position is provided, the maximum search can still deviate by this amount of samples.
         :type flexibility: int
+        :param calc_rms: If true, calculated also the rms of the filtered pulses.
+        :type calc_rms: bool
         """
 
-        print('Calculating OF Heights.')
+        if calc_rms:
+            print('Calculating OF Heights and RMS.')
+        else:
+            print('Calculating OF Heights.')
 
         if onset_to_dominant_channel is None:
             onset_to_dominant_channel = np.zeros(self.nmbr_channels)
         assert len(onset_to_dominant_channel) == self.nmbr_channels, \
             'onset_to_dominant_channel must have length nmbr_channels!'
 
         with h5py.File(self.path_h5, 'r+') as f:
@@ -468,73 +473,121 @@
 
             if 'of_ph' + name_appendix_set in f[type]:
                 del f[type]['of_ph' + name_appendix_set]
 
             f[type].require_dataset(name='of_ph' + name_appendix_set,
                                     shape=(self.nmbr_channels, len(events[0])),
                                     dtype='float')
+            if calc_rms:
+                if 'of_rms' + name_appendix_set in f[type]:
+                    del f[type]['of_rms' + name_appendix_set]
+                if 'of_rms_peak' + name_appendix_set in f[type]:
+                    del f[type]['of_rms_peak' + name_appendix_set]
+                f[type].require_dataset(name='of_rms' + name_appendix_set,
+                                shape=(self.nmbr_channels, len(events[0])),
+                                dtype='float')
+                f[type].require_dataset(name='of_rms_peak' + name_appendix_set,
+                                shape=(self.nmbr_channels, len(events[0])),
+                                dtype='float')
 
             nmbr_events = len(events[0])
             counter = 0
 
             # we do the calculation in batches, so that memory does not overflow
             while counter + chunk_size < nmbr_events:
                 for c in range(self.nmbr_channels):
                     if first_channel_dominant and c == 0:
-                        of_ph, peakpos = get_amplitudes(events[c, counter:counter + chunk_size], sev[c], nps[c],
+                        results = get_amplitudes(events[c, counter:counter + chunk_size], sev[c], nps[c],
                                                         hard_restrict=hard_restrict, down=down, window=window,
                                                         return_peakpos=True,
                                                         baseline_model=baseline_model,
                                                         pretrigger_samples=pretrigger_samples,
                                                         transfer_function=transfer_function[c],
-                                                        flexibility=flexibility)
+                                                        flexibility=flexibility,
+                                                        calc_rms=calc_rms)
+                        if calc_rms:
+                            of_ph, peakpos, of_rms, of_rms_peak = results
+                        else:
+                            of_ph, peakpos = results
                     elif first_channel_dominant:
-                        of_ph = get_amplitudes(events[c, counter:counter + chunk_size], sev[c], nps[c],
+                        results = get_amplitudes(events[c, counter:counter + chunk_size], sev[c], nps[c],
                                                hard_restrict=hard_restrict, down=down, window=window,
                                                peakpos=peakpos + onset_to_dominant_channel[c],
                                                return_peakpos=False,
                                                baseline_model=baseline_model, pretrigger_samples=pretrigger_samples,
                                                transfer_function=transfer_function[c],
-                                                        flexibility=flexibility)
+                                               flexibility=flexibility,
+                                               calc_rms=calc_rms)
+                        if calc_rms:
+                            of_ph, of_rms, of_rms_peak = results
+                        else:
+                            of_ph = results
                     else:
-                        of_ph = get_amplitudes(events[c, counter:counter + chunk_size], sev[c], nps[c],
+                        results = get_amplitudes(events[c, counter:counter + chunk_size], sev[c], nps[c],
                                                hard_restrict=hard_restrict, down=down, window=window,
                                                return_peakpos=False,
                                                baseline_model=baseline_model, pretrigger_samples=pretrigger_samples,
                                                transfer_function=transfer_function[c],
-                                                        flexibility=flexibility)
+                                               flexibility=flexibility,
+                                               calc_rms=calc_rms)
+                        if calc_rms:
+                            of_ph, of_rms, of_rms_peak = results
+                        else:
+                            of_ph = results
 
                     f[type]['of_ph' + name_appendix_set][c, counter:counter + chunk_size] = of_ph
+                    if calc_rms:
+                        f[type]['of_rms' + name_appendix_set][c, counter:counter + chunk_size] = of_rms
+                        f[type]['of_rms_peak' + name_appendix_set][c, counter:counter + chunk_size] = of_rms_peak
                 counter += chunk_size
 
             # calc rest that is smaller than a batch
             for c in range(self.nmbr_channels):
                 if first_channel_dominant and c == 0:
-                    of_ph, peakpos = get_amplitudes(events[c, counter:nmbr_events], sev[c], nps[c],
+                    results = get_amplitudes(events[c, counter:nmbr_events], sev[c], nps[c],
                                                     hard_restrict=hard_restrict, down=down, window=window,
                                                     return_peakpos=True,
                                                     baseline_model=baseline_model,
                                                     pretrigger_samples=pretrigger_samples,
                                                     transfer_function=transfer_function[c],
-                                                        flexibility=flexibility)
+                                                    flexibility=flexibility,
+                                                    calc_rms=calc_rms)
+                    if calc_rms:
+                        of_ph, peakpos, of_rms, of_rms_peak = results
+                    else:
+                        of_ph, peakpos = results
                 elif first_channel_dominant:
-                    of_ph = get_amplitudes(events[c, counter:nmbr_events], sev[c], nps[c],
+                    results = get_amplitudes(events[c, counter:nmbr_events], sev[c], nps[c],
                                            hard_restrict=hard_restrict, down=down, window=window,
                                            peakpos=peakpos + onset_to_dominant_channel[c], return_peakpos=False,
                                            baseline_model=baseline_model, pretrigger_samples=pretrigger_samples,
                                            transfer_function=transfer_function[c],
-                                                        flexibility=flexibility)
+                                           flexibility=flexibility,
+                                           calc_rms=calc_rms)
+                    if calc_rms:
+                        of_ph, of_rms, of_rms_peak = results
+                    else:
+                        of_ph = results
                 else:
-                    of_ph = get_amplitudes(events[c, counter:nmbr_events], sev[c], nps[c],
+                    results = get_amplitudes(events[c, counter:nmbr_events], sev[c], nps[c],
                                            hard_restrict=hard_restrict, down=down, window=window,
                                            return_peakpos=False,
                                            baseline_model=baseline_model, pretrigger_samples=pretrigger_samples,
                                            transfer_function=transfer_function[c],
-                                                        flexibility=flexibility)
+                                           flexibility=flexibility,
+                                           calc_rms=calc_rms)
+                    if calc_rms:
+                        of_ph, of_rms, of_rms_peak = results
+                    else:
+                        of_ph = results
                 f[type]['of_ph' + name_appendix_set][c, counter:nmbr_events] = of_ph
+                if calc_rms:
+                    f[type]['of_rms' + name_appendix_set][c, counter:nmbr_events] = of_rms
+                    f[type]['of_rms_peak' + name_appendix_set][c, counter:nmbr_events] = of_rms_peak
+
 
     # calc stdevent carrier
     def calc_exceptional_sev(self,
                              naming,
                              channel=0,
                              type='events',
                              use_prediction_instead_label=False,
```

## cait/versatile/__init__.py

```diff
@@ -1,19 +1,5 @@
-from .file import combine, merge
-from .iterators import apply
-from .utils import timestamp_coincidence, sample_noise
-# from .utils import timestamps_to_timedict
-from .analysis import *
-from .stream import *
-from .plot import *
+from .datasources import *
+from .analysisobjects import *
+from .eventfunctions import *
 from .functions import *
-from .rdt import RDTFile
-
-__all__ = [
-    'apply',
-    'combine',
-    'merge',
-    'RDTFile',
-    'sample_noise',
-    'timestamp_coincidence',
-#    'timestamps_to_timedict'
-]
+from .plot import *
```

## cait/versatile/functions/__init__.py

```diff
@@ -1,17 +1,5 @@
-from .event_functions import Unity, Downsample, RemoveBaseline, BoxCarSmoothing, TukeyFiltering, OptimumFiltering, Align, Lags
-from .fit_functions import FitBaseline
-# from .scalar_functions import AIClassifyBool, AIClassifyProb
-
-__all__ = [
-#    'AIClassifyBool',
-#    'AIClassifyProb',
-    'Align',
-    'BoxCarSmoothing',
-    'Downsample',
-    'FitBaseline',
-    'Lags',
-    'OptimumFiltering',
-    'RemoveBaseline',
-    'TukeyFiltering',
-    'Unity'
-]
+from .file import combine, merge
+from .apply import apply
+from .trigger.trigger_zscore import trigger_zscore
+from .trigger.trigger_of import trigger_of
+from .utils import timestamp_coincidence, sample_noise
```

## cait/versatile/plot/__init__.py

```diff
@@ -1,10 +1,7 @@
-from .plot import Viewer, Line, Scatter, Histogram, StreamViewer, Preview
-
-__all__ = [
-    'Viewer',
-    'Line',
-    'Scatter',
-    'Histogram',
-    'StreamViewer',
-    'Preview'
-]
+from .viewer import Viewer
+from .basic.line import Line
+from .basic.scatter import Scatter
+from .basic.histogram import Histogram
+from .highlevel.preview import Preview
+from .highlevel.streamviewer import StreamViewer
+from .highlevel.scatterpreview import ScatterPreview
```

## Comparing `cait/versatile/file.py` & `cait/versatile/functions/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import h5py
 from typing import List
 
-from ..styles._print_styles import sizeof_fmt
+from ...styles._print_styles import sizeof_fmt
 
 def ds_source_available(file: h5py.File, group: str, dataset: str):
     """
     Checks whether the sources of a virtual dataset 'dataset' in the group 'group' are still available to the file 'file'. For regular datasets (not virtual) this method returns True.
     This method DOES NOT check for the existence of the dataset!
 
     :param file: Open file stream to the HDF5 file.
```

## Comparing `cait/versatile/rdt.py` & `cait/versatile/datasources/hardwaretriggered/rdt_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,131 +1,49 @@
 import os
-import re
+
 from typing import Union
 
 import numpy as np
 import cait as ai
 
-from .iterators import RDTIterator
-
-# Would be cool to input parameters manually in case we don't have a PAR file. 
-# This should go directly into this class so that higher level classes don't have to handle it.
-class PARFile:
-    def __init__(self, arg: Union[str, dict]):
-        # if isinstance(arg, str):
-        if not arg.endswith(".par"):
-            raise ValueError("Unrecognized file extension. Please input a *.par file.")
-        
-        with open(arg, "r") as f:
-            s = f.read()
-
-        match = re.findall("Timeofday at start\s*\[s\].*Timeofday at start\s*\[us\].*Timeofday at stop\s*\[s\].*Timeofday at stop\s*\[us\].*Measuring time\s*\[h\].*Integers in header.*Unsigned longs in header.*Reals in header.*DVM channels.*Record length.*Time base\s*\[us\]", s, re.DOTALL)
-        if not match:
-            raise ValueError("Unable to extract data from file.")
-        
-        self.s = s
-        # elif isinstance(arg, dict):
-        #     if not all([['start_s', 
-        #                  'start_us', 
-        #                  'stop_s', 
-        #                  'stop_us', 
-        #                  'measuring_time_h', 
-        #                  'ints_in_header', 
-        #                  'uslongs_in_header',
-        #                  'reals_in_header',
-        #                  'dvm_channels',
-        #                  'record_length',
-        #                  'records_written',
-        #                  'time_base_us']])
-        # else:
-        #     raise NotImplementedError(f"Unrecognized input type '{type(arg)}'.")
-
-    @property
-    def start_s(self):
-        return int(re.findall("Timeofday at start\s*\[s\]\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def start_us(self):
-        return int(re.findall("Timeofday at start\s*\[us\]\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def stop_s(self):
-        return int(re.findall("Timeofday at stop\s*\[s\]\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def stop_us(self):
-        return int(re.findall("Timeofday at stop\s*\[us\]\s*:\s+(\d+)", self.s)[0])
-    
-    @property
-    def measuring_time_h(self):
-        return float(re.findall("Measuring time\s*\[h\]\s*:\s+([0-9]*[.]?[0-9]+)", self.s)[0])
-
-    @property
-    def ints_in_header(self):
-        return int(re.findall("Integers in header\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def uslongs_in_header(self):
-        return int(re.findall("Unsigned longs in header\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def reals_in_header(self):
-        return int(re.findall("Reals in header\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def dvm_channels(self):
-        return int(re.findall("DVM channels\s*:\s+(\d+)", self.s)[0])
+from .par_file import PARFile
+from ..datasourcebase import DataSourceBaseClass
+from ...iterators.impl_rdt import RDTIterator
 
-    @property
-    def record_length(self):
-        return int(re.findall("Record length\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def records_written(self):
-        return int(re.findall("Records written\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def time_base_us(self):
-        return int(re.findall("Time base\s*\[us\]\s*:\s+(\d+)", self.s)[0])
-
-    @property
-    def has_channel_names(self):
-        return bool(self.channel_names)
-    
-    @property
-    def channel_names(self):
-        return {int(i[0])-1: i[1] for i in re.findall("ch(\d+): (.+)", self.s)}
-    
 class RDTFile:
     """
-    Class for interfacing hardware triggered files (file extension `.rdt`). This class automatically infers the available channels and the available correlated channels. Those can be retrieved by indexing the RDTFile object. In a second step, testpulse amplitudes, timestamps, and event iterators can be constructed from a selected channel.
+    Class for interfacing hardware triggered files (file extension `.rdt`). This class automatically infers the available channels and the available correlated channels. Those can be retrieved by indexing the RDTFile object with channel indices/names or tuples thereof, the result of the indexing is a :class:`RDTChannel` object which provides testpulse amplitudes, timestamps, and event iterators for (the) selected channel(s) (see documentation for :class:`RDTChannel`).
 
     :param path: The full path (including the file extension `.rdt`) to the file of interest.
     :type path: str
     :param path_par: The full path (including the file extension `.par`) to the file which contains the necessary parameters to read the `.rdt` file. If None is given, it is assumed that a `.par` file with identical name/path as `path` is available. Defaults to None.
     :type path_par: str, optional
 
     :return: Object interfacing an `.rdt` file.
     :rtype: RDTFile
 
-    >>> import cait.versatile as vai
-    >>> f = vai.RDTFile('path/to/file.rdt')
-    >>> # Check available channels
-    >>> print(f.keys)
-    >>> # Choose channel(s) to iterate over, get testpulse amplitudes, ...,  by slicing RDTFile
-    >>> channels = f[(0,1)]
-    >>> it = channels.get_event_iterator()
-    >>> # You can now further slice this iterator (like any other iterator in cait.versatile):
-    >>> it_testpulses = it[:, channels.tpas > 0]
-    >>> it_events = it[:, channels.tpas == 0]
-    >>> it_noise = it[:, channels.tpas == -1]
-    >>> # Remove baselines:
-    >>> it_testpulses.add_processing(vai.RemoveBaseline())
-    >>> # Have a look:
-    >>> vai.Preview(it_testpulses)
+    **Example:**
+    ::
+        import cait.versatile as vai
+
+        f = vai.RDTFile('path/to/file.rdt')
+
+        # Check available channels
+        print(f.keys)
+        # Choose channel(s) to iterate over, get testpulse amplitudes, ...,  by slicing RDTFile
+        channels = f[(0,1)] # if interested in only one channel: channel0 = f[0]
+        it = channels.get_event_iterator()
+
+        # You can now further slice this iterator (like any other iterator in cait.versatile):
+        it_testpulses = it[:, channels.tpas > 0]
+        it_events = it[:, channels.tpas == 0]
+        it_noise = it[:, channels.tpas == -1]
+
+        # Have a look (after removing the baseline):
+        vai.Preview(it_testpulses.with_processing(vai.RemoveBaseline()))
     """
     def __init__(self, path: str, path_par: str = None):
         if not path.endswith(".rdt"):
             raise ValueError("Unrecognized file extension for 'path'. Please input an *.rdt file.")
         
         if path_par is None:
             path_par = os.path.splitext(path)[0] + '.par'
@@ -152,69 +70,82 @@
                        ('dac_output', 'f4'),
                        ('dvm_channels', 'f4', self._par.dvm_channels),
                        ('samples', 'i2', self._par.record_length),
                        ])
         
         self._raw_file = np.memmap(path, dtype=self._dtype, mode='r')
 
-        self._available_channels = list(set(self._raw_file["detector_nmbr"]))
+        # Copy the relevant data to memory so that we don't have to go through
+        # the memory mapped file all the time (this should only need a few MB of RAM)
+        meta_copy = np.array(self._raw_file[["detector_nmbr", "trig_count"]])
+
+        self._available_channels = np.unique(meta_copy["detector_nmbr"]).tolist()
 
+        # I'M STILL NOT SURE IF I WANT A DEFAULT CHANNELS BEHAVIOR OR NOT 
         # If no channels are requested by the user (through __getitem__), the default behavior is such
         # that all quantities (iterators, timestamps, tpas) are returned for all channels.
         # Notice that this might fail (when not all are correlated). 
         # In the case that, e.g., only two channels are present and correlated, this provides a shortcut
         # when accessing the important stuff
-        if len(self._available_channels) > 1:
-            self._default_channels = tuple(self._available_channels)
-        else:
-            self._default_channels = int(self._available_channels[0])
+        # if len(self._available_channels) > 1:
+        #     self._default_channels = tuple(self._available_channels)
+        # else:
+        #     self._default_channels = int(self._available_channels[0])
 
         self._inds = dict()
         # DETERMINE INDICES FOR SINGLE CHANNELS:
         for c in self._available_channels:
-            self._inds[c] = np.nonzero(self._raw_file["detector_nmbr"] == c)[0]
+            self._inds[c] = np.nonzero(meta_copy["detector_nmbr"] == c)[0]
 
         # DETERMINE INDICES FOR CORRELATED CHANNELS (have same trig_count):
-        vals, idx_start, count = np.unique(np.array(self._raw_file["trig_count"]), return_counts=True, return_index=True)
+        vals, idx_start, count = np.unique(meta_copy["trig_count"], return_counts=True, return_index=True)
         
         # We are only interested in trigger counts that appear more than once
         flag_corr = count > 1
         if np.sum(flag_corr) > 0:
 
             # Split trigger count array according to the first occurences
             # (note: the first entry is discarded)
-            s = np.split(self._raw_file["trig_count"], idx_start)[1:]
+            s = np.split(meta_copy["trig_count"], idx_start)[1:]
         
             # Now restrict to those cases which include more than one occurrence 
             # (note that this has to be done AFTER the splitting above)
             vals = vals[flag_corr]
             idx_start = idx_start[flag_corr]
             count = count[flag_corr]
 
             # Furthermore, we are only interested in identical trigger counts that
             # are adjacent in the file (ensure that only correctly written records
             # are included)
             # (The next line just checks if the pieces in s all include the same value, i.e. are consecutive)
-            flag_adj = [len(set(x))==1 for x in s if len(x)>1]
+            flag_adj = [len(np.unique(x))==1 for x in s if len(x)>1]
             
             # Restrict to adjacent
             vals = vals[flag_adj]
             idx_start = idx_start[flag_adj]
             count = count[flag_adj]
 
-            lst = list()
-            for i, l in zip(idx_start, count):
-                lst.append(tuple(self._raw_file[i:(i+l)]["detector_nmbr"]))
-
-            for tup in list(set(lst)):
-                tup_inds = np.array([i for i, x in enumerate(lst) if x == tup])
-                self._inds[tup] = idx_start[tup_inds]
+            # Create and populate a dictionary whose keys are the unique 
+            # channel combinations and whose values are the corresponding 
+            # data indices
+            unique_tuples = dict()
+            for n, (i, l) in enumerate(zip(idx_start, count)):
+                tup = tuple(meta_copy["detector_nmbr"][i:(i+l)])
+                if not (tup in unique_tuples.keys()): 
+                    unique_tuples[tup] = []
+                unique_tuples[tup].append(n)
+                
+            # Add tuples and corresponding indices to self._inds dictionary
+            for k, v in unique_tuples.items():
+                tup_inds = np.array(v)
+                self._inds[k] = idx_start[tup_inds]
         
     def __repr__(self):
-        return f'{self.__class__.__name__}(keys={self.keys}, record_length={self.record_length}, dt_us={self.time_base_us}, measuring_time_h={self.measuring_time_h}, default_channel={self[self._default_channels]})'
+        k = self.keys.keys() if isinstance(self.keys, dict) else self.keys
+        return f'{self.__class__.__name__}(keys={k}, record_length={self.record_length}, dt_us={self.dt_us}, measuring_time_h={self.measuring_time_h:.2f})'
 
     def __getitem__(self, channels: Union[int, str, tuple]):
         """
         Choose a single channel (integer) or correlated channels (tuple of integers) from this RDTFile for further investigations. 
         The available keys are found via `RDTFile.keys`. If the channels have names (successfully extracted from the `*.par` file), you can also use those for indexing.
 
         :param channels: Channel index (potentially name) or tuple thereof.
@@ -259,15 +190,15 @@
     
     @property
     def record_length(self):
         """The record length (number of samples per event) of the events in the corresponding `*.rdt` file."""
         return self._par.record_length
     
     @property
-    def time_base_us(self):
+    def dt_us(self):
         """The time base in microseconds (time between two samples) of the events in the corresponding `*.rdt` file."""
         return self._par.time_base_us
     
     @property
     def sample_frequency(self):
         """The sample frequency in Hz of the events in the corresponding `*.rdt` file."""
         return int(np.round(1e6/self._par.time_base_us))
@@ -275,103 +206,105 @@
     @property
     def measuring_time_h(self):
         """The total measuring time in hours of the corresponding `*.rdt` file."""
         return self._par.measuring_time_h
     
     @property
     def keys(self):
+        """The channel keys that can be used to index this RDTFile instance. If available, the channel names (corresponding to the indices) are shown as well."""
         if self._par.has_channel_names:
             d = dict()
             for k in self._inds.keys():
                 if isinstance(k, tuple):
                     d[k] = tuple([self._par.channel_names[i] for i in k])
                 else: # then int
                     d[k] = self._par.channel_names[k]
                     
             return d
         else:
             return list(self._inds.keys())
         
-    @property
-    def default_channels(self):
-        """
-        This RDTFile's default channel(s). 
-        Those are used if `tpas`, `unique_tpas`, `timestamps` and `get_event_iterator` are called on this RDTFile instance.
-        """
-        return self._default_channels
-        
     def get_voltage_trace(self, inds: Union[int, list]):
         """
         Return the voltage traces of events in this RDTFile for given indices.
         
         :param inds: The indices for which to return the voltage traces.
         :type inds: Union[int, list]
 
         :return: Array of as many voltage traces as given `inds`.
         :rtype: numpy.array
         """
         return ai.data.convert_to_V(self._file["samples"][inds], bits=16, min=-10, max=10)
-    
-    @property
-    def timestamps(self):
-        """The microsecond timestamps of the events in this RDTFile's default channel(s)."""
-        # Create an RDTChannel instance for the default channels and return its timestamps
-        return self[self._default_channels].timestamps
-    
-    @property
-    def tpas(self):
-        """The testpulse amplitudes of the events in this RDTFile's default channel(s)."""
-        # Create an RDTChannel instance for the default channels and return its tpas
-        return self[self._default_channels].tpas
-    
-    @property
-    def unique_tpas(self):
-        """The unique testpulse amplitudes of the events in this RDTFile's default channel(s)."""
-        # Create an RDTChannel instance for the default channels and return its unique_tpas
-        return self[self._default_channels].unique_tpas
-    
-    def get_event_iterator(self):
-        """
-        Get an iterator over the events of this RDTFile's default channel(s). 
-        Note that this is merely a shortcut to first choosing the channel of interest and then constructing the iterator, and that the recommended way is to NOT use this shortcut unless you are certain that you want to use the default channel.
-
-        :return: Iterable object
-        :rtype: RDTIterator
 
-        >>> import cait.versatile as vai
-        >>> f = vai.RDTFile('path/to/file.rdt')
-        >>> # Check what default channel is:
-        >>> print(f.default_channel)
-        >>> # If you're happy with the default channel, use f.get_event_iterator()
-        >>> # If you'd rather choose another channel, you can do so by slicing, 
-        >>> # e.g., f[0] for the channel number 0
-        >>> it = f.get_event_iterator()
-        >>> # You can now further slice this iterator (like any other iterator in cait.versatile):
-        >>> it_testpulses = it[:, f.tpas > 0]
-        >>> it_events = it[:, f.tpas == 0]
-        >>> it_noise = it[:, f.tpas == -1]
-        >>> # Remove baselines:
-        >>> it_testpulses.add_processing(vai.RemoveBaseline())
-        >>> # Have a look:
-        >>> vai.Preview(it_testpulses)
-        """
-        # Create an RDTChannel instance for the default channels and return its event_iterator
-        return self[self._default_channels].get_event_iterator()
+    # I'M STILL NOT SURE IF I WANT A DEFAULT CHANNELS BEHAVIOR OR NOT     
+    # @property
+    # def default_channels(self):
+    #     """
+    #     This RDTFile's default channel(s). 
+    #     Those are used if `tpas`, `unique_tpas`, `timestamps` and `get_event_iterator` are called on this RDTFile instance.
+    #     """
+    #     return self._default_channels
+    
+    # @property
+    # def timestamps(self):
+    #     """The microsecond timestamps of the events in this RDTFile's default channel(s)."""
+    #     # Create an RDTChannel instance for the default channels and return its timestamps
+    #     return self[self._default_channels].timestamps
+    
+    # @property
+    # def tpas(self):
+    #     """The testpulse amplitudes of the events in this RDTFile's default channel(s)."""
+    #     # Create an RDTChannel instance for the default channels and return its tpas
+    #     return self[self._default_channels].tpas
+    
+    # @property
+    # def unique_tpas(self):
+    #     """The unique testpulse amplitudes of the events in this RDTFile's default channel(s)."""
+    #     # Create an RDTChannel instance for the default channels and return its unique_tpas
+    #     return self[self._default_channels].unique_tpas
+    
+    # def get_event_iterator(self):
+    #     """
+    #     Get an iterator over the events of this RDTFile's default channel(s). 
+    #     Note that this is merely a shortcut to first choosing the channel of interest and then constructing the iterator, and that the recommended way is to NOT use this shortcut unless you are certain that you want to use the default channel.
+
+    #     :return: Iterable object
+    #     :rtype: RDTIterator
+
+    #     >>> import cait.versatile as vai
+    #     >>> f = vai.RDTFile('path/to/file.rdt')
+    #     >>> # Check what default channel is:
+    #     >>> print(f.default_channel)
+    #     >>> # If you're happy with the default channel, use f.get_event_iterator()
+    #     >>> # If you'd rather choose another channel, you can do so by slicing, 
+    #     >>> # e.g., f[0] for the channel number 0
+    #     >>> it = f.get_event_iterator()
+    #     >>> # You can now further slice this iterator (like any other iterator in cait.versatile):
+    #     >>> it_testpulses = it[:, f.tpas > 0]
+    #     >>> it_events = it[:, f.tpas == 0]
+    #     >>> it_noise = it[:, f.tpas == -1]
+    #     >>> # Remove baselines:
+    #     >>> it_testpulses.add_processing(vai.RemoveBaseline())
+    #     >>> # Have a look:
+    #     >>> vai.Preview(it_testpulses)
+    #     """
+    #     # Create an RDTChannel instance for the default channels and return its event_iterator
+    #     return self[self._default_channels].get_event_iterator()
         
-class RDTChannel:
+class RDTChannel(DataSourceBaseClass):
     """
     Object representing a coherent part of an RDTFile (i.e. either a single channel or correlated channels). Usually this is not created as a standalone but the result of slicing an RDTFile.
 
     :param rdt_file: An RDTFile instance.
     :type rdt_file: RDTFile
     :param key: The key which selects the single channel or correlated channels. Either of `rdt_file.keys`.
     :type key: Union[int, tuple]
 
-    :return: Iterable object
-    :rtype: RDTIterator
+    :return: Specified channels of an RDTFile
+    :rtype: RDTChannel
     """
     def __init__(self, rdt_file: RDTFile, key: Union[int, tuple]):
 
         inds = rdt_file._inds[key]
         self._n_channels = len(key) if isinstance(key, tuple) else 1
 
         # Build index array for all channels, first dimension is channel index (also existent if only one
@@ -386,27 +319,40 @@
         return f"{self.__class__.__name__}(key={self._key}, n_events={len(self)}, n_channels={self._n_channels}, unique_tpas={self.unique_tpas})"
     
     def __len__(self):
         return self._inds.shape[-1]
     
     def __getitem__(self, val):
         """Return voltage traces of events. Any numpy indexing can be used as if it was an array of shape (n_channels, n_events)."""
-        return self._rdt_file.get_voltage_trace(self._inds[val])
+        if isinstance(val, tuple):
+            if len(val) != 2: 
+                raise ValueError("Indexing only supports up to two arguments.")
+            requested_events = self._inds[val[0]][...,val[1]].T
+        else:
+            requested_events = self._inds[..., val].T
+
+        return self._rdt_file.get_voltage_trace(requested_events)
     
     @property
     def key(self):
         """The RDTFile key that this RDTChannel corresponds to."""
         return self._key
     
     @property
     def n_channels(self):
         """The number of channels this RDTChannel corresponds to."""
         return self._n_channels
     
     @property
+    def start_us(self):
+        s = self._rdt_file._par.start_s
+        mus = self._rdt_file._par.start_us
+        return s*int(1e6) + mus
+    
+    @property
     def timestamps(self):
         """The microsecond timestamps of the events in this RDTChannel."""
         secs = np.array(self._rdt_file._file["abs_time_s"][self._inds[0]], dtype=np.int64)
         msecs = np.array(self._rdt_file._file["abs_time_mus"][self._inds[0]], dtype=np.int64)
 
         return secs*int(1e6) + msecs
     
@@ -416,29 +362,38 @@
         return self._rdt_file._file["test_pulse_amplitude"][self._inds[0]]
     
     @property
     def unique_tpas(self):
         """The unique testpulse amplitudes of the events in this RDTChannel."""
         return sorted(list(set(self.tpas)))
     
-    def get_event_iterator(self):
+    def get_event_iterator(self, batch_size: int = None):
         """
         Get an iterator over the events present in this RDTChannel instance. 
 
+        :param batch_size: The number of events to be returned at once (these are all read together). There will be a trade-off: large batch_sizes cause faster read speed but increase the memory usage.
+        :type batch_size: int
+
         :return: Iterable object
         :rtype: RDTIterator
 
-        >>> import cait.versatile as vai
-        >>> f = vai.RDTFile('path/to/file.rdt')
-        >>> # Choose channel(s) to iterate over by slicing RDTFile
-        >>> channels = f[(0,1)]
-        >>> it = channels.get_event_iterator()
-        >>> # You can now further slice this iterator (like any other iterator in cait.versatile):
-        >>> it_testpulses = it[:, channels.tpas > 0]
-        >>> it_events = it[:, channels.tpas == 0]
-        >>> it_noise = it[:, channels.tpas == -1]
-        >>> # Remove baselines:
-        >>> it_testpulses.add_processing(vai.RemoveBaseline())
-        >>> # Have a look:
-        >>> vai.Preview(it_testpulses)
+        **Example:**
+        ::
+            import cait.versatile as vai
+
+            f = vai.RDTFile('path/to/file.rdt')
+
+            # Choose channel(s) to iterate over by slicing RDTFile
+            channels = f[(0,1)]
+            it = channels.get_event_iterator()
+
+            # You can now further slice this iterator (like any other iterator in cait.versatile):
+            it_testpulses = it[:, channels.tpas > 0]
+            it_events = it[:, channels.tpas == 0]
+            it_noise = it[:, channels.tpas == -1]
+            # Remove baselines:
+            it_testpulses.add_processing(vai.RemoveBaseline())
+            
+            # Have a look:
+            vai.Preview(it_testpulses)
         """
-        return RDTIterator(self)
+        return RDTIterator(self, batch_size=batch_size)
```

## Comparing `cait/versatile/utils.py` & `cait/versatile/functions/utils.py`

 * *Files identical despite different names*

## Comparing `cait/versatile/analysis/energy_calibration.py` & `cait/versatile/analysisobjects/energy_calibration.py`

 * *Files identical despite different names*

## Comparing `cait/versatile/functions/abstract_functions.py` & `cait/versatile/eventfunctions/functionbase.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,24 @@
         p = ", ".join([f"{k}={getattr(self, '_'+k)}" 
                        for k in params if hasattr(self, '_'+k)])
         return f"{self.__class__.__name__}({p})"
     
     @abstractmethod
     def __call__(self, event):
         ...
+
+    @property
+    @abstractmethod
+    def batch_support(self):
+        """
+        Returns 'trivial' if function can process all given event traces at a time in an uncorrelated manner, i.e. different channels are treated equally.
+        Returns 'full' if batches (possibly with multiple channels, too) can be processed at once.
+        Returns 'none' if batches are not supported.
+        """
+        ...
     
     def preview(self, event) -> dict:
         raise NotImplementedError(f"{self.__class__.__name__} does not support preview.")
         
 class FitFncBaseClass(FncBaseClass):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

## Comparing `cait/versatile/functions/fit_functions.py` & `cait/versatile/eventfunctions/scalarfunctions/fitbaseline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import List, Union
+from typing import Union, List
 import warnings
 
 import numpy as np
 from scipy.optimize import curve_fit
 
-from .abstract_functions import FitFncBaseClass
+from ..functionbase import FitFncBaseClass
 
 # We do not use scipy's parameter error estimation anyways so we can suppress this warning
 warnings.filterwarnings("ignore", "Covariance of the parameters could not be estimated")
 
 def exponential_decay(x, a, b, c):
     return a*np.exp(-b*x) + c
 
@@ -17,19 +17,35 @@
     Fit voltage traces with a polynomial or decaying exponential and return the fit parameters as well as the RMS.
     Also works for multiple channels simultaneously.
 
     :param model: Order of the polynomial or 'exponential'/'exp', defaults to 0, i.e. a constant baseline.
     :type model: Union[int, str]
     :param where: Specifies a subset of data points to be used in the fit: Either a boolean flag of the same length of the voltage traces, a slice object (e.g. slice(0,50) for using the first 50 data points), or a float. If a float `where` is passed, the first `int(where)*record_length` samples are used (e.g. if `where=1/8`, the first 1/8th of the record window is used). Defaults to `slice(None, None, None).  
     :type where: Union[List[bool], slice, int]
-    :param xdata: x-data to use for the fit (has no effect for `order=0`). Specifying x-data is not necessary in general but if you want your fit parameters to have physical units (e.g. time constants) instead of just samples, you may use this option. Defaults to `None`.
+    :param xdata: x-data to use for the fit (has no effect for `order=0`). Specifying xdata is not necessary in general but if you want your fit parameters to have physical units (e.g. time constants) instead of just samples, you may use this option. Defaults to `None`, in which case `xdata=np.linspace(0,1,record_length)`.
     :type xdata: List[float]
 
     :return: Fit parameter(s) and RMS as a tuple.
     :rtype: Tuple[Union[float, numpy.ndarray], float]
+
+    **Example:**
+    ::
+        import cait.versatile as vai
+
+        # Construct mock data (which provides event iterator)
+        md = vai.MockData()
+        it = md.get_event_iterator()[0]
+
+        # View effect of fitting baseline on events
+        # We specify that for the fit, 1/8th of the record window should be used,
+        # that we fit with a degree-0-polynomial (i.e. constant)
+        # Specifying the xdata is not necessary, but it lets us plot in terms of time
+        vai.Preview(it, vai.FitBaseline(where=1/8, model=0, xdata=it.t), xlabel="Time (ms)")
+
+    .. image:: media/FitBaseline_preview.png
     """
     def __init__(self, model: Union[int, str] = 0, where: Union[List[bool], slice, float] = slice(None, None, None), xdata: List[float] = None):
         if type(model) not in [str, int]:
             raise NotImplementedError(f"Unsupported type '{type(model)}' for input 'order'.")
         elif type(model) is str and model not in ['exponential', 'exp']:
             raise NotImplementedError(f"Unrecognized baseline model '{model}'.")
         elif type(model) is int and model < 0:
@@ -48,15 +64,15 @@
         # Shortcut for constant baseline model
         if self._model == 0:
             self._fitpar =  np.mean(event[..., self._where], axis=-1)
             self._rms = np.std(event[..., self._where], axis=-1)
         else:
             # ATTENTION: This is only set once, i.e. data has to have same length 
             if self._xdata is None: 
-                self._xdata = np.arange(np.array(event).shape[-1])
+                self._xdata = np.linspace(0, 1, np.array(event).shape[-1])
 
             # Exponential fit
             if self._model in ['exponential', 'exp']:
                 if np.array(event).ndim > 1:
                     self._fitpar = np.array(
                         [
                           curve_fit(exponential_decay, 
@@ -89,14 +105,18 @@
 
                 par, err, *_ = np.linalg.lstsq(self._A, event[..., self._where].T, rcond=None)
                 self._fitpar = par.T
                 self._rms = np.sqrt(err)
 
         return self._fitpar, self._rms
     
+    @property
+    def batch_support(self):
+        return 'trivial'
+    
     def model(self, x: List, par: List):
         """
         
         """
         par = np.array(par)
         
         if self._model in ['exponential', 'exp']:
@@ -133,61 +153,15 @@
         # Reconstruct fit function
         fit = self.model(self._xdata, par)
                 
         if np.ndim(event) > 1:
             d = dict()
             for i in range(np.ndim(event)):
                 d[f'channel {i}'] = [self._xdata, event[i]]
-                d[f'fit channel {i}'] = [self._xdata, fit[i]]
+                d[f'baseline fit channel {i}'] = [self._xdata, fit[i]]
         else:
             
         
             d = {'event': [self._xdata, event],
-                 'fit': [self._xdata, fit]}
+                 'baseline fit': [self._xdata, fit]}
             
-        return dict(line = d)
-    
-class ArrayFit(FitFncBaseClass):
-    """
-    
-    """
-    def __init__(self, sev: np.ndarray):
-        raise NotImplementedError
-        self._sev = np.array(sev)
-
-    def __call__(self, event):
-        self._fitted_sev = None
-        self._height = None
-        self._rms = None
-
-        return self._height, self._rms
-    
-    def model(self, x: List, par: List):
-        """
-        
-        """
-        ...
-    
-    def preview(self, event):
-        self(event)
-        return dict(line={'event': [None, event],
-                          'fitted sev': [None, self._fitted_sev]
-                          })
-
-class SEVFit(FitFncBaseClass):
-    """
-    
-    """
-    def __init__(self):
-        raise NotImplementedError
-
-    def __call__(self, event):
-        ...
-    
-    def model(self, x: List, par: List):
-        """
-        
-        """
-        ...
-    
-    def preview(self, event):
-        ...
+        return dict(line = d)
```

## Comparing `cait/versatile/stream/trigger.py` & `cait/versatile/functions/trigger/trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from typing import Union, List, Callable
 
 import numpy as np
 from tqdm.auto import tqdm
 
-from ..functions import RemoveBaseline
-from .stream import StreamBaseClass
+from ...eventfunctions.processing.removebaseline import RemoveBaseline
+from ...datasources.stream.streambase import StreamBaseClass
 
 ####################################################
 ### FUNCTIONS IN THIS FILE HAVE NO TESTCASES YET ###
 ####################################################
 
+####################################################
+### THIS IS (A VARIANT) OF THE TRIGGER USED BY   ###
+### EXISTING CAIT ROUTINES.                      ###
+####################################################
+
 def trigger(stream, 
             key: str, 
             threshold: float,
             record_length: int,
             overlap_fraction: float = 1/8,
             trigger_block: int = None,
             n_triggers: int = None,
```

## Comparing `cait-1.2.1.dist-info/LICENSE` & `cait-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cait-1.2.1.dist-info/METADATA` & `cait-1.2.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: cait
-Version: 1.2.1
+Version: 1.2.2
 Summary: Cryogenic Artificial Intelligence Tools - A Python Package for the Data Analysis of Rare Event Search Experiments with Machine Learning.
-Home-page: https://github.com/fewagner/cait
-Author: Philipp Schreiner, Felix Wagner
-Author-email: felix.wagner@oeaw.ac.at
-License: GPLv3
-Platform: UNKNOWN
+Author-email: Philipp Schreiner <philipp.schreiner@oeaw.ac.at>, Felix Wagner <felix.wagner@oeaw.ac.at>
+Project-URL: Repository, https://github.com/fewagner/cait
+Project-URL: Documentation, https://cait.readthedocs.io/en/latest/index.html
+Project-URL: Changelog, https://cait.readthedocs.io/en/latest/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: numpy <1.25
+Requires-Dist: numpy >=1.22
 Requires-Dist: scipy >=1.6
 Requires-Dist: pandas >=1.1
 Requires-Dist: h5py >=3.2
 Requires-Dist: uproot >=4.1
 Requires-Dist: ipywidgets >=7.5
 Requires-Dist: dash >=2.0
 Requires-Dist: matplotlib >=3.4
 Requires-Dist: numba >=0.54
 Requires-Dist: tqdm >=4.62
 Requires-Dist: scikit-learn >=0.24
 Requires-Dist: deprecation
+Provides-Extra: clplot
+Requires-Dist: uniplot >=0.12.2 ; extra == 'clplot'
+Provides-Extra: nn
+Requires-Dist: pytorch-lightning ==1.9.4 ; extra == 'nn'
+Requires-Dist: torch >=1.8 ; extra == 'nn'
+Provides-Extra: test
+Requires-Dist: pytest ; extra == 'test'
 
 .. -*- mode: rst -*-
 
 |PyPi|_ |DOI|_
 
 .. |PyPi| image:: https://badge.fury.io/py/cait.svg
 .. _PyPi: https://badge.fury.io/py/cait
@@ -64,23 +70,27 @@
 
 You can now import the library in Python, e.g.
 
 .. code:: python
 
     import cait as ai
 
-**Important Note for JupyterHub on computing clusters:**
+.. note::
+  **Important Note for JupyterHub on computing clusters**
 
-In the past, many users experienced issues with our interactive plotting tools which are based on plotly and ipywidgets. These problems were due to version mismatches between the plotly/ipywidgets packages and their corresponding JupyterLab extensions (which are automatically installed alongside the packages). 
+  In the past, many users experienced issues with our interactive plotting tools which are based on plotly and ipywidgets. These problems were due to version mismatches between the plotly/ipywidgets packages and their corresponding JupyterLab extensions (which are automatically installed alongside the packages). 
 
-To not run into such issues in the first place, we recommend one of the following approaches:
-- Install cait in the base environment of your computing cluster's JupyterLab. 
-- Install it in a virtual environment (because you want or have to) is also possible but you will have to make sure that the same plotly/ipywidgets versions (which are installed as dependencies of cait) are also present in the base environment. A good practice to ensure this is to always pip-upgrade plotly/ipywidgets to the latest version in both environments. Note that you will potentially have to match these versions every time you upgrade cait.
+  To not run into such issues in the first place, we recommend one of the following approaches:
 
-Lastly, remember to **restart JupyterHub completely** (not just the kernel) for the changes to take effect.
+  * Install cait in the base environment of your computing cluster's JupyterLab. 
+  * Install it in a virtual environment (because you want or have to) is also possible but you will have to make sure that the same plotly/ipywidgets versions (which are installed as dependencies of cait) are also present in the base environment. A good practice to ensure this is to always pip-upgrade plotly/ipywidgets to the latest version in both environments. Note that you will potentially have to match these versions every time you upgrade cait.
+
+  Lastly, remember to **restart JupyterHub completely** (not just the kernel) for the changes to take effect.
+
+  To learn how to add a virtual environment as a kernel to jupyterlab, refer to `this great reference <https://janakiev.com/blog/jupyter-virtual-envs/>`_.
 
 Version History
 ===============
 
 Master branch is on the latest release version and stable.
 
 Previous versions are hosted on the accordingly named Git branch.
@@ -111,8 +121,7 @@
 
 We want you ...
 ===============
 
 ... to contribute! We are always happy about any contributions to our software. To coordinate
 efforts, please get in touch with felix.wagner(at)oeaw.ac.at such that we can include your
 features in the upcoming release. If you have any troubles with the current release, please open an issue in the Bug Report.
-
```

