# Comparing `tmp/qiclib-1.0.0.tar.gz` & `tmp/qiclib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiclib-1.0.0.tar", last modified: Wed Nov 29 13:43:48 2023, max compression
+gzip compressed data, was "qiclib-1.1.0.tar", last modified: Tue May  7 08:58:03 2024, max compression
```

## Comparing `qiclib-1.0.0.tar` & `qiclib-1.1.0.tar`

### file list

```diff
@@ -1,195 +1,203 @@
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.939891 qiclib-1.0.0/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    35149 2023-11-24 10:40:17.000000 qiclib-1.0.0/COPYING
--rw-r--r--   0 lukas     (1000) lukas     (1000)    11466 2023-11-29 13:43:48.939891 qiclib-1.0.0/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    10625 2023-11-29 13:42:21.000000 qiclib-1.0.0/README.md
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1422 2023-11-27 13:32:09.000000 qiclib-1.0.0/pyproject.toml
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      942 2023-11-29 13:43:48.939891 qiclib-1.0.0/setup.cfg
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      838 2023-11-27 13:32:09.000000 qiclib-1.0.0/setup.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.919890 qiclib-1.0.0/src/
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.919890 qiclib-1.0.0/src/qiclib/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1922 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/__init__.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.923891 qiclib-1.0.0/src/qiclib/code/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1585 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/__init__.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.923891 qiclib-1.0.0/src/qiclib/code/analysis/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      769 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/analysis/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    30667 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/analysis/qi_insert_mem_parameters.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    20924 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_dataflow.py
--rwxrwxr-x   0 lukas     (1000) lukas     (1000)    68094 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_jobs.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    50598 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_prog_builder.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    10215 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_pulse.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    24960 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_seq_instructions.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    46162 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_sequencer.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5319 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_simulate.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    19615 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_types.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2415 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_util.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    21122 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_var_definitions.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    18669 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/code/qi_visitor.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.923891 qiclib-1.0.0/src/qiclib/coding/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      769 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/coding/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    25881 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/coding/sequencercode.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.927891 qiclib-1.0.0/src/qiclib/experiment/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2938 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/SecondToneSweepR5.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1108 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4732 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/active_cooling_t1.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2437 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/active_reset_t1.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    13178 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/autoconf_readout.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    41508 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/base.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6181 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/benchmarking.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2770 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/collection.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3559 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/correlation_calibration.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4820 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/correlation_conv_all.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3248 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/g1_correlation.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2824 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/g1_correlation_conv.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6423 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/g1_meas_setuptest.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3388 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/g2_correlation.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2923 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/g2_correlation_conv.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     7039 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/gx_correlation_base.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2073 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/inverted_t1.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3600 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/iq_clouds.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2316 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/iq_clouds_multi_qfb.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2330 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/iq_clouds_qfb.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1999 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/iq_clouds_qfb_decay.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1993 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/iq_clouds_ramsey.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2773 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/iq_clouds_ringup.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3726 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/multi_pi.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2599 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/multi_pi_t1.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.927891 qiclib-1.0.0/src/qiclib/experiment/qicode/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    23736 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/base.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9994 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/collection.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9674 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/data_handler.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4083 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/data_provider.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    18751 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/init_readout.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8703 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/qubit_times.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    11192 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qicode/qubit_times_qkit.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    25138 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qkit_virtual_awg.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4871 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/quantum_jumps.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3523 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/quantum_jumps_long.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8236 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qubit_times.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9347 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/qubit_times_qkit.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3798 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rabi.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3137 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rabi_R5PG.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3623 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rabi_drag.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5101 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rabi_short.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3179 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/ramsey.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5351 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/readout.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3526 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/readout_spectr.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3988 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/resonator_ringup.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3008 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/resonator_ringup_window.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.931891 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1420 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2406 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/active_cooling.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3238 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/average_trace.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3308 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/base_experiment_task.c
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.931891 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6113 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/calibration.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    14925 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/correlation_conv.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5601 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     7305 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation_conv.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5131 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g1_meas_setuptest.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6995 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8194 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation_conv.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4960 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/interleaved.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5801 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/interleaved_multi.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1867 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/iq_clouds.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2868 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/optimize_rec_offset.c
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.931891 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5374 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/averaging.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4446 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/iq_collect.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4300 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/state_collect.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4038 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/state_count.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5343 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/timetrace.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2181 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/quantum_jumps.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5405 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_multi.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3368 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_new.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2895 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qubit_freq_sweep_task.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2823 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/rabi_r5.c
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.931891 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3609 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/copy_test.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      845 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/empty.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1701 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/shift_test.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1896 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/stream_test.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1312 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/test_databox.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    17797 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/time_test_code.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    11557 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/timing_test.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3425 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/timing_test_axi.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1937 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/timing_test_single.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    12932 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/trace_fft.c
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6431 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/single_pulse.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5311 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/spinecho.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2482 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/stream_test.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2928 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/t1.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3942 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/experiment/test_two_pulse.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.935891 qiclib-1.0.0/src/qiclib/hardware/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4253 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    25878 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/controller.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5284 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/pimc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5631 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/platform_component.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    30077 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/pulsegen.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    41187 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/recording.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    10026 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/rfdc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8781 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/sequencer.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2543 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/servicehub.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9750 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/storage.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    13241 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/taskrunner.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    14780 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/hardware/unitcell.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.935891 qiclib-1.0.0/src/qiclib/measurement/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/measurement/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    17134 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/measurement/iq_fit.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    23748 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/measurement/iq_plot.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5521 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/measurement/measure_iq.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.935891 qiclib-1.0.0/src/qiclib/packages/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1414 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/constants.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.935891 qiclib-1.0.0/src/qiclib/packages/grpc/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1380 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6999 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/pimc_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    33412 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/pimc_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9414 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/pulsegen_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    31355 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/pulsegen_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    12627 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/qic_storage_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    30398 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/qic_storage_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    16399 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/qic_unitcell_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    31245 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/qic_unitcell_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    18662 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/recording_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    66761 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/recording_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    14007 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/rfdc_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    38283 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/rfdc_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9010 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/sequencer_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    27991 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/sequencer_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9343 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/servicehubcontrol_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    22470 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/servicehubcontrol_pb2_grpc.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    10686 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/taskrunner_pb2.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    28789 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/grpc/taskrunner_pb2_grpc.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.935891 qiclib-1.0.0/src/qiclib/packages/qiskit/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    15607 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/qiskit/QiController_backend.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3642 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/qiskit/QiController_job.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2525 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/qiskit/QiController_provider.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9420 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/qiskit/QiGates.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/qiskit/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4417 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/qkit_polyfill.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3261 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/servicehub.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     7447 2023-11-24 10:54:49.000000 qiclib-1.0.0/src/qiclib/packages/utility.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        0 2023-11-24 10:40:17.000000 qiclib-1.0.0/src/qiclib/py.typed
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.939891 qiclib-1.0.0/src/qiclib.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)    11466 2023-11-29 13:43:48.000000 qiclib-1.0.0/src/qiclib.egg-info/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     7014 2023-11-29 13:43:48.000000 qiclib-1.0.0/src/qiclib.egg-info/SOURCES.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2023-11-29 13:43:48.000000 qiclib-1.0.0/src/qiclib.egg-info/dependency_links.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      141 2023-11-29 13:43:48.000000 qiclib-1.0.0/src/qiclib.egg-info/requires.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        7 2023-11-29 13:43:48.000000 qiclib-1.0.0/src/qiclib.egg-info/top_level.txt
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-11-29 13:43:48.939891 qiclib-1.0.0/tests/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2980 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_experiments.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4092 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_iq_fit.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    26473 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_insert_mem_parameters.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    41742 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_jobs.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)   102061 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_prog_builder.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4424 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_pulse.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4459 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_seq_instructions.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    33921 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_sequencer.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    13416 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_types.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2305 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_util.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1228 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_var_definitions.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    10648 2023-11-27 13:32:09.000000 qiclib-1.0.0/tests/test_qi_visitor.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.771277 qiclib-1.1.0/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    35149 2024-05-07 08:35:46.000000 qiclib-1.1.0/COPYING
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    11466 2024-05-07 08:58:03.771277 qiclib-1.1.0/PKG-INFO
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    10625 2024-05-07 08:35:46.000000 qiclib-1.1.0/README.md
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1422 2024-05-07 08:35:46.000000 qiclib-1.1.0/pyproject.toml
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      942 2024-05-07 08:58:03.771277 qiclib-1.1.0/setup.cfg
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      838 2024-05-07 08:35:46.000000 qiclib-1.1.0/setup.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.751277 qiclib-1.1.0/src/
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.751277 qiclib-1.1.0/src/qiclib/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1922 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/__init__.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.755277 qiclib-1.1.0/src/qiclib/code/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1650 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/__init__.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.755277 qiclib-1.1.0/src/qiclib/code/analysis/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      769 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/analysis/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    30667 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/analysis/qi_insert_mem_parameters.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    20924 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_dataflow.py
+-rwxrwxr-x   0 lukas     (1000) lukas     (1000)    74325 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_jobs.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    51287 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_prog_builder.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    10215 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_pulse.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    25019 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_seq_instructions.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    46850 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_sequencer.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5319 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_simulate.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    19615 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_types.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2415 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_util.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    21122 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_var_definitions.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    18669 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/code/qi_visitor.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.755277 qiclib-1.1.0/src/qiclib/coding/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      769 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/coding/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    27701 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/coding/sequencercode.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.759277 qiclib-1.1.0/src/qiclib/experiment/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2938 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/SecondToneSweepR5.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1108 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4732 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/active_cooling_t1.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2437 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/active_reset_t1.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    13178 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/autoconf_readout.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    41692 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/base.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     6181 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/benchmarking.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2770 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/collection.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3559 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/correlation_calibration.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4820 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/correlation_conv_all.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3248 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/g1_correlation.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2824 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/g1_correlation_conv.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     6423 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/g1_meas_setuptest.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3388 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/g2_correlation.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2923 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/g2_correlation_conv.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     7039 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/gx_correlation_base.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2073 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/inverted_t1.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3600 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/iq_clouds.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2316 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/iq_clouds_multi_qfb.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2330 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/iq_clouds_qfb.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1999 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/iq_clouds_qfb_decay.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1993 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/iq_clouds_ramsey.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2773 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/iq_clouds_ringup.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3726 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/multi_pi.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2599 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/multi_pi_t1.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.759277 qiclib-1.1.0/src/qiclib/experiment/qicode/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    25002 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/base.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     9994 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/collection.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     9674 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/data_handler.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4083 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/data_provider.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    18751 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/init_readout.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     8703 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/qubit_times.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    11192 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qicode/qubit_times_qkit.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    25138 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qkit_virtual_awg.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4871 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/quantum_jumps.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3523 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/quantum_jumps_long.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     8236 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qubit_times.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     9347 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/qubit_times_qkit.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3798 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rabi.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3137 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rabi_R5PG.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3623 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rabi_drag.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5101 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rabi_short.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3179 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/ramsey.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5351 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/readout.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3526 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/readout_spectr.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3988 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/resonator_ringup.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3008 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/resonator_ringup_window.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.763277 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1420 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2406 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/active_cooling.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3238 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/average_trace.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3308 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/base_experiment_task.c
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.763277 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     6113 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/calibration.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    14925 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/correlation_conv.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5601 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     7305 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation_conv.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5131 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g1_meas_setuptest.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     6995 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     8194 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation_conv.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4960 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/interleaved.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5801 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/interleaved_multi.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1867 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/iq_clouds.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2868 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/optimize_rec_offset.c
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.763277 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5374 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/averaging.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4446 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/iq_collect.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4300 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/state_collect.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4038 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/state_count.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5343 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/timetrace.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2181 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/quantum_jumps.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5405 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_multi.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3368 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_new.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2895 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qubit_freq_sweep_task.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2823 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/rabi_r5.c
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.763277 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3609 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/copy_test.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      845 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/empty.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1701 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/shift_test.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1896 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/stream_test.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1312 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/test_databox.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    17797 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/time_test_code.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    11557 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/timing_test.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3425 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/timing_test_axi.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1937 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/timing_test_single.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    12932 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/trace_fft.c
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     6431 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/single_pulse.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5311 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/spinecho.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2482 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/stream_test.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2928 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/t1.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3942 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/experiment/test_two_pulse.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.767277 qiclib-1.1.0/src/qiclib/hardware/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4252 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    26791 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/controller.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5910 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/digital_trigger.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5277 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/pimc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5636 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/platform_component.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4956 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/pulse_player.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    30138 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/pulsegen.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    41232 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/recording.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    11265 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/rfdc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     8801 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/sequencer.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2962 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/servicehub.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     9795 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/storage.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    13253 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/taskrunner.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    15315 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/hardware/unitcell.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.767277 qiclib-1.1.0/src/qiclib/measurement/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/measurement/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    17134 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/measurement/iq_fit.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    23748 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/measurement/iq_plot.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5521 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/measurement/measure_iq.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.767277 qiclib-1.1.0/src/qiclib/packages/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1414 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/constants.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.771277 qiclib-1.1.0/src/qiclib/packages/grpc/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1380 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     9829 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/datatypes_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      158 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/datatypes_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5810 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/digital_trigger_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    12316 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/digital_trigger_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5015 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/pimc_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    33650 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/pimc_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3250 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/pulse_player_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    10519 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/pulse_player_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     7918 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/pulsegen_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    30784 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/pulsegen_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    11065 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/qic_storage_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    29569 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/qic_storage_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    14421 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/qic_unitcell_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    30308 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/qic_unitcell_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    17273 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/recording_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    66067 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/recording_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    13059 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/rfdc_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    37814 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/rfdc_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     7102 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/sequencer_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    27297 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/sequencer_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     8206 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/servicehubcontrol_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    21554 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/servicehubcontrol_pb2_grpc.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     9655 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/taskrunner_pb2.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    28044 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/grpc/taskrunner_pb2_grpc.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.771277 qiclib-1.1.0/src/qiclib/packages/qiskit/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    15607 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/qiskit/QiController_backend.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3642 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/qiskit/QiController_job.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2525 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/qiskit/QiController_provider.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     9420 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/qiskit/QiGates.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      768 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/qiskit/__init__.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4417 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/qkit_polyfill.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3261 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/servicehub.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     7447 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/packages/utility.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:35:46.000000 qiclib-1.1.0/src/qiclib/py.typed
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.771277 qiclib-1.1.0/src/qiclib.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    11466 2024-05-07 08:58:03.000000 qiclib-1.1.0/src/qiclib.egg-info/PKG-INFO
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     7374 2024-05-07 08:58:03.000000 qiclib-1.1.0/src/qiclib.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2024-05-07 08:58:03.000000 qiclib-1.1.0/src/qiclib.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      141 2024-05-07 08:58:03.000000 qiclib-1.1.0/src/qiclib.egg-info/requires.txt
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)        7 2024-05-07 08:58:03.000000 qiclib-1.1.0/src/qiclib.egg-info/top_level.txt
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2024-05-07 08:58:03.771277 qiclib-1.1.0/tests/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3022 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_experiments.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4092 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_iq_fit.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    26473 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_insert_mem_parameters.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    41742 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_jobs.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)   102061 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_prog_builder.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4424 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_pulse.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     4404 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_seq_instructions.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    34215 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_sequencer.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    13416 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_types.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2305 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_util.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1228 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_var_definitions.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    10648 2024-05-07 08:35:46.000000 qiclib-1.1.0/tests/test_qi_visitor.py
```

### Comparing `qiclib-1.0.0/COPYING` & `qiclib-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/PKG-INFO` & `qiclib-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiclib
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library to connect to Quantum Interface's QiController.
 Home-page: https://github.com/quantuminterface/qiclib
 Author: Quantum Interface
 Author-email: quantuminterface@ipe.kit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `qiclib-1.0.0/README.md` & `qiclib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/pyproject.toml` & `qiclib-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/setup.cfg` & `qiclib-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qiclib
-version = 1.0.0
+version = 1.1.0
 author = Quantum Interface
 author_email = quantuminterface@ipe.kit.edu
 description = Library to connect to Quantum Interface's QiController.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/quantuminterface/qiclib
 classifiers =
```

### Comparing `qiclib-1.0.0/setup.py` & `qiclib-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/__init__.py` & `qiclib-1.1.0/src/qiclib/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/__init__.py` & `qiclib-1.1.0/src/qiclib/code/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,24 +30,28 @@
 from .qi_jobs import (
     QiTimeVariable,
     QiVariable,
     QiStateVariable,
     QiResult,
     Play,
     PlayReadout,
+    PlayFlux,
     RotateFrame,
     QiJob,
     QiCells,
     QiCell,
+    QiCoupler,
+    QiCouplers,
     QiSample,
     Recording,
     Wait,
     Assign,
     Sync,
     If,
     Else,
     ForRange,
     Parallel,
     QiGate,
+    DigitalTrigger,
 )
 from .qi_pulse import ShapeLib, QiPulse
 from . import qi_seq_instructions
```

### Comparing `qiclib-1.0.0/src/qiclib/code/analysis/__init__.py` & `qiclib-1.1.0/src/qiclib/code/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/analysis/qi_insert_mem_parameters.py` & `qiclib-1.1.0/src/qiclib/code/analysis/qi_insert_mem_parameters.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_dataflow.py` & `qiclib-1.1.0/src/qiclib/code/qi_dataflow.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_jobs.py` & `qiclib-1.1.0/src/qiclib/code/qi_jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,42 +17,54 @@
 """
 This is the main module of QiCode.
 Here, all important commands write QiPrograms are defined.
 """
 import os
 from abc import abstractmethod
 import json
-from typing import Dict, List, Callable, Optional, Union, Set, Any, Type
+from typing import (
+    Dict,
+    List,
+    Callable,
+    Optional,
+    Union,
+    Set,
+    Any,
+    Type,
+    Iterable,
+)
+from typing_extensions import Protocol
 import functools
 import warnings
 
 import numpy as np
 
 import qiclib.packages.utility as util
-from ..hardware.taskrunner import TaskRunner
-from ..experiment.qicode.data_provider import DataProvider
-from ..experiment.qicode.data_handler import DataHandler
-from .qi_seq_instructions import SequencerInstruction
-from .qi_var_definitions import (
+from qiclib.hardware import digital_trigger
+from qiclib.hardware.taskrunner import TaskRunner
+from qiclib.experiment.qicode.data_provider import DataProvider
+from qiclib.experiment.qicode.data_handler import DataHandler
+from qiclib.code.qi_seq_instructions import SequencerInstruction
+from qiclib.code.qi_var_definitions import (
     _QiVariableBase,
     _QiCalcBase,
     _QiConstValue,
     QiCellProperty,
     QiExpression,
     QiVariableSet,
     QiCondition,
 )
-from .qi_pulse import QiPulse
-from .qi_visitor import (
+from qiclib.code.qi_pulse import QiPulse
+from qiclib.code.qi_visitor import (
     QiCMContainedCellVisitor,
     QiResultCollector,
     QiVarInForRange,
 )
-from .qi_prog_builder import QiProgramBuilder
-from .qi_types import (
+from qiclib.code.qi_prog_builder import QiProgramBuilder
+from qiclib.code.qi_types import (
     QiType,
     QiPostTypecheckVisitor,
     QiTypeFallbackVisitor,
     _TypeDefiningUse,
 )
 
 
@@ -180,14 +192,15 @@
 
     def __init__(self, cellID: int):
         if not isinstance(_QiJobReference, QiJob):
             raise RuntimeError("QiCell can't be used outside of QiJob.")
 
         self.cellID = cellID
         self.manipulation_pulses: List[QiPulse] = []
+        self.digital_trigger_sets: List[digital_trigger.TriggerSet] = []
         self.flux_pulses: List[QiPulse] = []
         self.readout_pulses: List[QiPulse] = []
         self._result_container: Dict[str, QiResult] = {}
         # The order in which recorded values are assigned to which result container
         self._result_recording_order: List[QiResult] = []
         self._unresolved_property: Set[QiCellProperty] = set()
         self._job_ref = _QiJobReference
@@ -232,14 +245,25 @@
             self.manipulation_pulses.append(pulse)
 
         if len(self.manipulation_pulses) > 13:
             raise RuntimeError("Too many pulses in use")
 
         return self.manipulation_pulses.index(pulse) + 1  # index 0 and 15 are reserved
 
+    def add_digital_trigger(self, trig_set: digital_trigger.TriggerSet):
+        if trig_set not in self.digital_trigger_sets:
+            self.digital_trigger_sets.append(trig_set)
+
+        if len(self.digital_trigger_sets) > 3:
+            raise RuntimeError(
+                "Too many digital trigger sets in use (Only three sets are available)"
+            )
+
+        return self.digital_trigger_sets.index(trig_set) + 1  # index 0 is reserved
+
     @property
     def initial_manipulation_frequency(self):
         if self._initial_manip_freq is None:
             if len(self.manipulation_pulses) > 0:
                 warnings.warn(
                     "Manipulation pulses without frequency given, using 90 MHz."
                 )
@@ -329,15 +353,15 @@
         """
         Returns the data after running an experiment.
 
         When calling this function without a name, i.e., calling :python:`cell.data()`,
         returns a dictionary containing the results as numpy arrays.
 
         When calling this function with a name, i.e., calling :python:`cell.data("result_name")`,
-        returns the whole dictionary.
+        returns the result referenced by :python:`name`
 
         :param name: The name of the data
         :return: A single result, or a dictionary of result names mapped to results.
         """
         if name is None:
             result_dict = {}
             for key, container in self._result_container.items():
@@ -405,19 +429,71 @@
     def __getitem__(self, key):
         return self.cells[key]
 
     def __len__(self):
         return len(self.cells)
 
 
+class QiCoupler:
+    def __init__(self, associated_unit_cell: QiCell, coupling_index: int):
+        self.associated_unit_cell = associated_unit_cell
+        self.coupling_index = coupling_index
+        self.coupling_pulses: List[QiPulse] = []
+
+    def add_pulse(self, pulse: QiPulse):
+        self.coupling_pulses.append(pulse)
+        return len(self.coupling_pulses)
+
+
+class QiCouplers:
+    """
+    Declares :py:`count` couplers.
+
+    Couplers are capable of playing flux pulses.
+    In the context of QiCode, flux Pulses are longer but do not have Digital Up-Conversion.
+
+    You can instantiate up to twice the amount of digital Unit Cells.
+
+    .. warning::
+        You must first instantiate Digital Unit Cells before you can instantiate Couplers.
+
+    .. code-block:: python
+
+        with QiJob() as job:
+            q = QiCells(6)
+            c = QiCouplers(12)
+    """
+
+    def __init__(self, count: int):
+        if not isinstance(_QiJobReference, QiJob):
+            raise RuntimeError("QiCouplers can only be used within QiJob description.")
+
+        if len(_QiJobReference.cells) == 0:
+            raise RuntimeError(
+                "No cells in the QiJob found."
+                "Note that couplers must be instantiated after cells."
+            )
+
+        self._couplers = [
+            QiCoupler(_QiJobReference.cells[i // 2], i % 2) for i in range(count)
+        ]
+        _QiJobReference._register_couplers(self._couplers)
+
+    def __getitem__(self, key):
+        return self._couplers[key]
+
+    def __len__(self):
+        return len(self._couplers)
+
+
 class QiSampleCell:
     """QiSampleCell is the representation of a single qubit/cell and its properties.
 
     All necessary parameters to perform experiments can be stored here. For this
-    purpose, the QiSampleCell can be utilized as a dictionary with user-defined keys.
+    purpose, the QiSampleCell can be used as a dictionary with user-defined keys.
     """
 
     def __init__(self, cellID: int, cells_ref: "QiSample"):
         self.cellID = cellID
         self._cells_ref = cells_ref
         self._relevant_vars: Set[_QiVariableBase] = set()
 
@@ -648,14 +724,39 @@
         super().__init__()
         self.var = var
 
     def accept(self, visitor, *input):
         return visitor.visit_variable_command(self, *input)
 
 
+class QiTriggerCommand(Protocol):
+    """
+    Common interface for all commands that can cause a trigger.
+    """
+
+    trigger_index: int
+
+
+class cQiDigitalTrigger(QiCellCommand, QiTriggerCommand):
+    """Command generated by :meth:`DigitalTrigger`"""
+
+    def __init__(self, cell: QiCell, outputs: List[int], length: float):
+        super().__init__(cell)
+        self.cell = cell
+        self.trigger_index = cell.add_digital_trigger(
+            digital_trigger.TriggerSet(
+                duration=length, outputs=outputs, continuous=False
+            )
+        )
+        self.length = length
+
+    def _stringify(self) -> str:
+        return f"DigitalTrigger({self.cell}, {self.trigger_index}, {self.length})"
+
+
 class cQiWait(QiCellCommand):
     """Command generated by :meth:`Wait`"""
 
     def __init__(self, cell, length: Union[QiExpression, QiCellProperty]):
         from .qi_types import _TypeDefiningUse
 
         super().__init__(cell)
@@ -676,15 +777,15 @@
             self._length() if isinstance(self._length, QiCellProperty) else self._length
         )
 
     def _stringify(self) -> str:
         return f"Wait({self.cell}, {self._length})"
 
 
-class _cQiPlay_base(QiCellCommand):
+class _cQiPlay_base(QiCellCommand, QiTriggerCommand):
     """Base class of Play commands.
     Saves pulses, trigger_index and adds pulse variables to associated variable set
     """
 
     def __init__(self, cell, pulse: QiPulse):
         super().__init__(cell)
         self.pulse = pulse
@@ -721,15 +822,23 @@
         self.trigger_index = cell.add_pulse(pulse)
 
     def _stringify(self) -> str:
         return f"Play({self.cell}, {self.pulse._stringify()})"
 
 
 class cQiPlayFlux(_cQiPlay_base):
-    pass
+    """Command generated by PlayFlux()"""
+
+    def __init__(self, coupler: QiCoupler, pulse: QiPulse) -> None:
+        super().__init__(coupler.associated_unit_cell, pulse)
+        self.coupler = coupler
+        self.trigger_index = coupler.add_pulse(pulse)
+
+    def _stringify(self) -> str:
+        return f"PlayFlux({self.coupler}, {self.pulse._stringify()})"
 
 
 class cQiPlayReadout(_cQiPlay_base):
     """Command generated by :meth:`PlayReadout`"""
 
     def __init__(self, cell, pulse) -> None:
         super().__init__(cell, pulse)
@@ -1157,25 +1266,28 @@
                 (
                     cQiPlay,
                     cQiPlayReadout,
                     cQiPlayFlux,
                     cQiRotateFrame,
                     cQiRecording,
                     cQiWait,
+                    cQiDigitalTrigger,
                 ),
             ):
                 raise TypeError("Type not allowed inside Parallel()", command)
             if (
                 isinstance(command, (cQiRecording, cQiPlayReadout))
                 and command.uses_state
             ):
                 raise RuntimeError("Can not save to state variable inside Parallel")
 
             try:
-                if isinstance(command.length, _QiVariableBase):
+                if hasattr(command, "length") and isinstance(
+                    command.length, _QiVariableBase
+                ):
                     self._associated_variable_set.add(command.length)
             except KeyError:
                 pass  # length was QiCellProperty
             command.accept(containing_cells)
 
         self._relevant_cells.update(containing_cells.contained_cells)
 
@@ -1534,14 +1646,15 @@
     def __init__(
         self,
         skip_nco_sync=False,
         nco_sync_length=0,
     ):
         self.qi_results: List[QiResult] = []
         self.cells = []
+        self.couplers = []
         self.skip_nco_sync = skip_nco_sync
         self.nco_sync_length = nco_sync_length
 
         self._description = _JobDescription()
 
         # Build
         self._performed_analyses = False
@@ -1588,14 +1701,20 @@
 
     def _register_cells(self, cells: List[QiCell]):
         if len(self.cells) > 0:
             raise RuntimeError("Can only register one set of cells at a QiJob.")
 
         self.cells = cells
 
+    def _register_couplers(self, couplers: List[QiCoupler]):
+        if len(self.couplers) > 0:
+            raise RuntimeError("Can only register one set of couplers at a QiJob.")
+
+        self.couplers = couplers
+
     def _run_analyses(self):
         """
         Executes needed (dataflow) analyses.
         These mutate the commands in QiJob by inserting additional instructions, therefore
         they should only run once, in order to avoid duplicate instructions.
         """
         from .analysis.qi_insert_mem_parameters import (
@@ -1692,22 +1811,29 @@
 
     def create_experiment(
         self,
         controller,
         sample: Optional[QiSample] = None,
         averages: int = 1,
         cell_map: Optional[List[int]] = None,
+        coupling_map: Optional[List[int]] = None,
         data_collection=None,
         use_taskrunner=False,
     ):
         from ..experiment.qicode.base import QiCodeExperiment
 
         exp = QiCodeExperiment(
             *self._prepare_experiment_params(
-                controller, sample, averages, cell_map, data_collection, use_taskrunner
+                controller,
+                sample,
+                averages,
+                cell_map,
+                coupling_map,
+                data_collection,
+                use_taskrunner,
             )
         )
 
         if data_collection is None:
             if self._custom_processing is not None:
                 exp._taskrunner.update(self._custom_processing)
             if self._custom_data_handler is not None:
@@ -1725,14 +1851,15 @@
 
     def _prepare_experiment_params(
         self,
         controller,
         sample: Optional[QiSample] = None,
         averages: int = 1,
         cell_map: Optional[List[int]] = None,
+        coupling_map: Optional[List[int]] = None,
         data_collection=None,
         use_taskrunner=False,
     ):
         if len(self.cells) > len(controller.cell):
             raise IndexError(
                 f"This job requires {len(self.cells)} cells but only "
                 f"{len(controller.cell)} are available in the QiController."
@@ -1768,14 +1895,17 @@
                 raise ValueError("Duplicate values not allowed in cell_map!")
             if any(m < 0 or m >= len(sample) for m in cell_map):
                 raise IndexError(
                     "cell_map values can only point to valid indices within the passed"
                     f" QiSample object, i.e. values between 0 and {len(sample) - 1}."
                 )
 
+        if coupling_map is None:
+            coupling_map = list(range(len(self.couplers)))
+
         # Translate cell_map from sample cells ("cells") to QiController cells
         cell_map = [sample.cell_map[c] for c in cell_map]
 
         if any(c < 0 or c >= len(controller.cell) for c in cell_map):
             raise ValueError(
                 "The QiSample cell_map can only reference available QiController "
                 f"cells, i.e. between 0 and {len(controller.cell) - 1}."
@@ -1787,45 +1917,55 @@
 
         for cell in self.cells:
             for_range_list.append(self.cell_seq_dict[cell]._for_range_list)
 
         return (
             controller,
             self.cells,
+            self.couplers,
             self._get_sequencer_codes(),
             averages,
             for_range_list,
             cell_map,
+            coupling_map,
             self._var_reg_map,
             data_collection,
             use_taskrunner,
         )
 
     def run(
         self,
         controller,
         sample: Optional[QiSample] = None,
         averages: int = 1,
         cell_map: Optional[List[int]] = None,
+        coupling_map: Optional[List[int]] = None,
         data_collection=None,
         use_taskrunner=False,
     ):
         """executes the job and returns the results
 
         :param controller: the QiController on which the job should be executed
         :param sample: the QiSample object used for execution of pulses and extracts parameters for the experiment
         :param averages: the number of executions that should be averaged, by default 1
         :param cell_map: A list containing the indices of the cells
+        :param cell_map: A list containing the indices of the couplers
         :param data_collection: the data_collection mode for the result, by default "average"
         :param use_taskrunner: if the execution should be handled by the Taskrunner
             Some advanced schemes and data_collection modes are currently only supported
             by the Taskrunner and not yet by a native control flow.
         """
         exp = self.create_experiment(
-            controller, sample, averages, cell_map, data_collection, use_taskrunner
+            controller,
+            sample,
+            averages,
+            cell_map,
+            coupling_map,
+            data_collection,
+            use_taskrunner,
         )
         exp.run()
 
     def run_with_data_callback(self, on_new_data: Callable[[dict], None]):
         pass
 
     def run_streamed(self):
@@ -1912,14 +2052,24 @@
 
     :param cell: the cell that plays the readout
     :param pulse: the readout to play
     """
     _add_cmd_to_job(cQiPlayReadout(cell, pulse))
 
 
+def PlayFlux(coupler: QiCoupler, pulse: QiPulse):
+    """
+    Add Flux Pulse command to cell
+
+    :param coupler: The coupler that plays the pulse
+    :param pulse: The pulse to play
+    """
+    _add_cmd_to_job(cQiPlayFlux(coupler, pulse))
+
+
 def RotateFrame(cell: QiCell, angle: float):
     """Rotates the reference frame of the manipulation pulses played with :python:`Play()`.
     This corresponds to an instantaneous, virtual Z rotation on the Bloch sphere.
 
     :param cell: the cell for the rotation
     :param angle: the angle of the rotation
     """
@@ -1953,14 +2103,61 @@
         toggleContinuous=toggleContinuous,
     )
     # When True, cQiRecording is added to the readout command
     if rec.follows_readout is False:
         _add_cmd_to_job(rec)
 
 
+def DigitalTrigger(
+    cell: QiCell,
+    length: float,
+    outputs: Iterable[int],
+):
+    """
+    Adds a digital trigger command to the cell.
+
+    Digital triggers are visible at auxiliary outputs and can be used, for example, to trigger external electronics
+    simultaneously to outputting a pulse.
+    The time resolution of digital triggers is 4 ns.
+
+    =======
+    Example
+    =======
+
+    The following QiJob Generates a 12 ns long pulse at digital outputs 3 and 6:
+
+    .. code-block:: python
+
+        with QiJob() as job:
+            q = QiCells(1)
+            DigitalTrigger(q[0], length=12e-9, outputs=(3, 6))
+
+    ===================================================
+    Combining the output of multiple Digital Unit Cells
+    ===================================================
+
+    Each Digital Unit Cell can trigger each output.
+    To combine multiple outputs to multiple inputs, all digital outputs are combined using a logical OR operation.
+
+    ================
+    Delaying outputs
+    ================
+
+    A static delay can be added to each output using
+    :python:`QiController.digital_trigger.set_delay(output_number, delay_in_seconds)`.
+    To add a variable amount of time, use :python:`Wait(cell, duration)` before calling :python:`DigitalTrigger`
+
+    :param cell: The cell that is responsible for the outputting the digital trigger
+    :param length: The duration of the pulse in seconds. Should be a multiple of four ns
+    :param outputs: The outputs to trigger. This can also be an expression like :python:`range(0, 8)`
+        to trigger all outputs.
+    """
+    _add_cmd_to_job(cQiDigitalTrigger(cell, list(outputs), length))
+
+
 def Wait(cell: QiCell, delay: Union[int, float, _QiVariableBase, QiCellProperty]):
     """Add Wait command to cell. delay can be int or QiVariable
 
     :param cell: the QiCell that should wait
     :param delay: the time to wait in seconds
     """
     _add_cmd_to_job(cQiWait(cell, delay))
```

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_prog_builder.py` & `qiclib-1.1.0/src/qiclib/code/qi_prog_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,16 +380,18 @@
             self.cell_seq[cell].exit_for_range()
 
     def visit_cell_command(self, cell_cmd):
         from .qi_jobs import (
             cQiWait,
             cQiPlay,
             cQiPlayReadout,
+            cQiPlayFlux,
             cQiRotateFrame,
             cQiRecording,
+            cQiDigitalTrigger,
         )
 
         relevant_cells = self.get_relevant_cells(cell_cmd)
 
         for cell in relevant_cells:
             if isinstance(cell_cmd, cQiWait):
                 # Ignore Wait command if it is of length less than a cycle.
@@ -409,16 +411,27 @@
             elif isinstance(cell_cmd, cQiPlayReadout):
                 # cell_cmd.combine_recording is either None or cQiRecording
                 self.cell_seq[cell].add_trigger_cmd(
                     readout=cell_cmd,
                     recording=cell_cmd.recording,
                     var_single_cycle=cell_cmd._var_single_cycle_trigger,
                 )
+            elif isinstance(cell_cmd, cQiPlayFlux):
+                if cell_cmd.coupler.coupling_index == 0:
+                    self.cell_seq[cell].add_trigger_cmd(coupling0=cell_cmd)
+                elif cell_cmd.coupler.coupling_index == 1:
+                    self.cell_seq[cell].add_trigger_cmd(coupling1=cell_cmd)
+                else:
+                    raise RuntimeError(
+                        f"Illegal coupling index {cell_cmd.coupler.coupling_index} (must be 0 or 1)"
+                    )
             elif isinstance(cell_cmd, cQiRecording):
                 self.cell_seq[cell].add_trigger_cmd(recording=cell_cmd)
+            elif isinstance(cell_cmd, cQiDigitalTrigger):
+                self.cell_seq[cell].add_trigger_cmd(digital=cell_cmd)
 
     def visit_context_manager(self, context_manager):
         """Context managers are evaluated in respective visit"""
 
     def visit_if(self, if_cm):
         """Visits If command and builds sequencer instructions.
         Tries synchronizing if multiple cells are used."""
```

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_pulse.py` & `qiclib-1.1.0/src/qiclib/code/qi_pulse.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_seq_instructions.py` & `qiclib-1.1.0/src/qiclib/code/qi_seq_instructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 This module defines the customized RISC-V instruction set used by the sequencers
 and how to encode the instruction into their binary format.
 """
 
 from abc import abstractmethod
 from typing import Tuple, Union
 from enum import Enum
-import numpy as np
 from .qi_var_definitions import QiOp, QiOpCond
 
 
 class SeqOpCode(Enum):
     """Enumeration containing Opcodes of Sequencer instructions"""
 
     JUMP = 0b1101111
@@ -679,27 +678,29 @@
     def __init__(
         self,
         module0: int = 0,
         module1: int = 0,
         module2: int = 0,
         module3: int = 0,
         module4: int = 0,
+        module5: int = 0,
         sync=False,
         reset=False,
     ) -> None:
-        self._trig_indices = [module0, module1, module2, module3, module4]
+        self._trig_indices = [module0, module1, module2, module3, module4, module5]
 
         immediate = 0
         immediate |= (reset & 0x1) << 12
         immediate |= (sync & 0x1) << 14
         immediate |= (module0 & 0xF) << 16
         immediate |= (module1 & 0xF) << 20
         immediate |= (module2 & 0xF) << 22
-        immediate |= (module3 & 0xF) << 26
-        immediate |= (module4 & 0xF) << 30
+        immediate |= (module3 & 0x3) << 26
+        immediate |= (module4 & 0x3) << 28
+        immediate |= (module5 & 0x3) << 30
         super().__init__(OpCode=SeqOpCode.TRIGGER, immediate=immediate)
 
     def __str__(self) -> str:
         return (
             f"Op: {self.op.name}, mod0: {hex(self._trig_indices[0])}, mod1: {hex(self._trig_indices[1])}"
             f", mod2: {hex(self._trig_indices[2])}, mod3: {hex(self._trig_indices[3])},  mod4: {hex(self._trig_indices[4])}\n"
         )
```

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_sequencer.py` & `qiclib-1.1.0/src/qiclib/code/qi_sequencer.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 from qiclib.code.qi_jobs import (
     ForRange,
     If,
     Parallel,
     cQiRecording,
     cQiSync,
+    cQiDigitalTrigger,
+    cQiPlay,
+    cQiPlayReadout,
+    QiTriggerCommand,
+    cQiPlayFlux,
 )
 import qiclib.packages.utility as util
 from .qi_var_definitions import (
     QiCellProperty,
     QiVariableSet,
     _QiCalcBase,
     _QiVariableBase,
@@ -279,22 +284,14 @@
         """Set externally when ForRange is used."""
         self._prog_cycles.cycles = x
 
     @property
     def recording_delay(self):
         return util.conv_cycles_to_time(self.RECORDING_MODULE_DELAY_CYCLES)
 
-    @property
-    def readout_active(self):
-        return self._trigger_mods.is_readout_active
-
-    @property
-    def manipulation_active(self):
-        return self._trigger_mods.is_manipulation_active
-
     def add_variable(self, var):
         """Adds variable to sequencer, reserving a register for it"""
         reg = self.request_register()
         self._var_reg_dict[var.id] = reg
         # Named variables can be initialized externally
         if var.name is not None:
             reg.valid = False
@@ -618,15 +615,15 @@
         TODO check register value, if it is smaller than other pulses play other lengths
         """
         from .qi_var_definitions import _QiVariableBase
         from .qi_jobs import _cQiPlay_base
 
         var_set = QiVariableSet()
         for pulse_cmd in pulses:
-            if isinstance(pulse_cmd, _cQiPlay_base):
+            if hasattr(pulse_cmd, "length"):
                 if isinstance(pulse_cmd.length, _QiVariableBase):
                     var_set.add(pulse_cmd.length)
 
         if len(var_set) > 1:
             raise RuntimeError(
                 "Concurrent pulses with different variable length not supported"
             )
@@ -661,24 +658,19 @@
             self._wait_cycles(
                 length - 1
             )  # -1 cycle, because trigger already takes up one cycle
 
     def trigger_choke_pulse(self):
         """Adds trigger command choking still running pulse generators."""
         trigger_values = self._trigger_mods.get_trigger_val()
-        choke_pulse = SeqTrigger(
-            trigger_values[0],  # readout
-            trigger_values[1],  # recording
-            trigger_values[2],  # manipulation
-            trigger_values[3],
-        )  # external
+        choke_pulse = SeqTrigger(*trigger_values)
 
         self.add_instruction_to_list(choke_pulse)
 
-    def _check_recording_state(self, recording=None, external=None) -> bool:
+    def _check_recording_state(self, recording=None) -> bool:
         """If recording saves to state variable, add command to save to the defined variable.
         Returns True if saving to state, else returns False"""
         if recording is not None and recording.uses_state:
             reg = self.get_var_register(recording.var)
             self.add_instruction_to_list(
                 SeqAwaitQubitState(dst=reg.adr, cell=self.cell_index)
             )
@@ -687,42 +679,37 @@
 
             return True
 
         return False
 
     def add_trigger_cmd(
         self,
-        manipulation=None,
-        readout=None,
-        recording=None,
-        external=None,
-        recording_delay=True,
-        var_single_cycle=False,
+        manipulation: Optional[cQiPlay] = None,
+        readout: Optional[cQiPlayReadout] = None,
+        recording: Optional[cQiRecording] = None,
+        coupling0: Optional[cQiPlayFlux] = None,
+        coupling1: Optional[cQiPlayFlux] = None,
+        digital: Optional[cQiDigitalTrigger] = None,
+        recording_delay: bool = True,
+        var_single_cycle: bool = False,
     ):
         """Adds trigger command to sequencer, depending on the specified pulses.
         The sequencer keeps track of still running pulse generators. If a pulse generator is not choked yet,
         the index of the choke pulse or the index of the new pulse to be played is used to choke the running pulse.
         Recording_delay defines, if the delay cycles of the recording module are added to the trigger length, this can be turned
         off, because Parallel bodies already implement this duration in the sequence generation.
         """
         trigger_values = self._trigger_mods.get_trigger_val(
-            readout, recording, manipulation, external
+            readout, recording, manipulation, coupling0, coupling1, digital
         )
 
-        self.add_instruction_to_list(
-            SeqTrigger(
-                trigger_values[0],  # readout
-                trigger_values[1],  # recording
-                trigger_values[2],  # manipulation
-                trigger_values[3],
-            )
-        )  # external
+        self.add_instruction_to_list(SeqTrigger(*trigger_values))
 
         length = self._get_length_of_trigger(
-            manipulation, readout, recording, recording_delay=recording_delay
+            manipulation, readout, recording, digital, recording_delay=recording_delay
         )
 
         if isinstance(length, _Register) or var_single_cycle:  # is any pulse variable?
             if var_single_cycle is False:
                 if length.value is None:
                     raise RuntimeError(
                         f"Variable at Register {length.adr} has not been properly initialised"
@@ -730,21 +717,21 @@
 
                 self.add_instruction_to_list(
                     SeqTriggerWaitRegister(length.adr), length.value - 1, length.valid
                 )
             self._trigger_mods.set_active(readout, None, manipulation, None)
 
             self._check_recording_state(
-                recording, external
+                recording
             )  # add possible state save; var pulse is stopped before saving operation
 
         elif (
             length > 1
             and (recording is None or recording.toggleContinuous is None)
-            and not self._check_recording_state(recording, external)
+            and not self._check_recording_state(recording)
         ):
             self._wait_cycles(
                 length - 1
             )  # -1 cycle, because trigger already takes up one cycle
 
     def end_of_command_body(self):
         """Called when body of commands ended; adds choke command for active pulses"""
@@ -1145,66 +1132,91 @@
             # CONTINUOUS toggles (second trigger turns continuous recoding off)
             return _RecordingTrigger.CONTINUOUS.value
         if recording.save_to is None:
             return _RecordingTrigger.ONESHOT.value
         return _RecordingTrigger.SINGLE.value
 
 
+def _get_trigger_index(
+    pulse: Optional[QiTriggerCommand], active_trigger: Union[bool, int]
+) -> int:
+    if pulse is None and active_trigger is False:
+        return 0
+    elif pulse is None and active_trigger:
+        return Sequencer.CHOKE_PULSE_INDEX
+    else:
+        return pulse.trigger_index
+
+
 class _TriggerModules:
     """Class of Sequencer to keep track of running pulse generators."""
 
     READOUT = 0
     RECORDING = 1
     MANIPULATION = 2
-    EXTERNAL = 3
+    COUPLING0 = 3
+    COUPLING1 = 4
+    DIGITAL = 5
 
     def __init__(self) -> None:
         self.reset()
 
     def reset(self):
-        self._trigger_modules_active: List[bool] = [False, False, False, False]
+        self._trigger_modules_active: List[Union[bool, int]] = [False] * 6
 
     @property
-    def is_pulse_active(self):
+    def is_pulse_active(self) -> bool:
         """Return True if any pulse generator is active/running"""
         return any(self._trigger_modules_active)
 
-    @property
-    def is_readout_active(self):
-        return self._trigger_modules_active[_TriggerModules.READOUT]
-
-    @property
-    def is_manipulation_active(self):
-        return self._trigger_modules_active[_TriggerModules.MANIPULATION]
-
-    def set_active(self, readout=None, rec=None, manipulation=None, ext=None):
+    def set_active(
+        self,
+        readout: Optional[Any] = None,
+        rec: Optional[Any] = None,
+        manipulation: Optional[Any] = None,
+        coupling0: Optional[Any] = None,
+        coupling1: Optional[Any] = None,
+        digital: Optional[Any] = None,
+    ):
         """Marks pulse generators of defined pulses as active/running"""
         self._trigger_modules_active[_TriggerModules.READOUT] = readout is not None
         self._trigger_modules_active[_TriggerModules.RECORDING] = rec is not None
         self._trigger_modules_active[_TriggerModules.MANIPULATION] = (
             manipulation is not None
         )
-        self._trigger_modules_active[_TriggerModules.EXTERNAL] = ext is not None
+        self._trigger_modules_active[_TriggerModules.COUPLING0] = coupling0 is not None
+        self._trigger_modules_active[_TriggerModules.COUPLING0] = coupling1 is not None
+        self._trigger_modules_active[_TriggerModules.DIGITAL] = digital is not None
 
-    def _evaluate_pulse(self, pulse, _active_trigger) -> int:
-        if pulse is None and _active_trigger is False:
-            return 0
-        elif pulse is None and _active_trigger:
-            return Sequencer.CHOKE_PULSE_INDEX
-        else:
-            return pulse.trigger_index
-
-    def get_trigger_val(self, readout=None, rec=None, manipulation=None, ext=None):
-        """Returns trigger values for defined pulses. If a pulse is not defined but it's module is marked active/running,
+    def get_trigger_val(
+        self,
+        readout: Optional[cQiPlayReadout] = None,
+        rec: Optional[cQiRecording] = None,
+        manipulation: Optional[cQiPlay] = None,
+        coupling0: Optional[cQiPlay] = None,
+        coupling1: Optional[cQiPlay] = None,
+        digital: Optional[cQiDigitalTrigger] = None,
+    ) -> List[int]:
+        """Returns trigger values for defined pulses.
+        If a pulse is not defined, but its module is marked active/running,
         the index of the choke pulse is returned.
-        After calling the function all pulse generators are marked as inactive/off."""
-        pulse_values = [0, 0, 0, 0]
-        pulse_values[_TriggerModules.READOUT] = self._evaluate_pulse(
-            readout, self._trigger_modules_active[0]
+        After calling the function, all pulse generators are marked as inactive/off."""
+        pulse_values = [0] * 6
+        pulse_values[_TriggerModules.READOUT] = _get_trigger_index(
+            readout, self._trigger_modules_active[_TriggerModules.READOUT]
         )
         pulse_values[_TriggerModules.RECORDING] = _RecordingTrigger.from_recording(rec)
-        pulse_values[_TriggerModules.MANIPULATION] = self._evaluate_pulse(
-            manipulation, self._trigger_modules_active[2]
+        pulse_values[_TriggerModules.MANIPULATION] = _get_trigger_index(
+            manipulation, self._trigger_modules_active[_TriggerModules.MANIPULATION]
+        )
+        pulse_values[_TriggerModules.COUPLING0] = _get_trigger_index(
+            coupling0, self._trigger_modules_active[_TriggerModules.COUPLING0]
+        )
+        pulse_values[_TriggerModules.COUPLING1] = _get_trigger_index(
+            coupling1, self._trigger_modules_active[_TriggerModules.COUPLING1]
+        )
+        pulse_values[_TriggerModules.DIGITAL] = _get_trigger_index(
+            digital, self._trigger_modules_active[_TriggerModules.DIGITAL]
         )
 
         self.reset()  # active pulses are now choked
         return pulse_values
```

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_simulate.py` & `qiclib-1.1.0/src/qiclib/code/qi_simulate.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_types.py` & `qiclib-1.1.0/src/qiclib/code/qi_types.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_util.py` & `qiclib-1.1.0/src/qiclib/code/qi_util.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_var_definitions.py` & `qiclib-1.1.0/src/qiclib/code/qi_var_definitions.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/code/qi_visitor.py` & `qiclib-1.1.0/src/qiclib/code/qi_visitor.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/coding/__init__.py` & `qiclib-1.1.0/src/qiclib/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/coding/sequencercode.py` & `qiclib-1.1.0/src/qiclib/coding/sequencercode.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,58 +36,63 @@
     def __init__(self, pc_dict=None):
         self.assembler = []
         self.binary = bytearray()
         self._instruction_values = []  # type: List[int]
         self.program_counter = 0
         self.pc_dict = pc_dict
 
-    def tr(self, mod0=0, mod1=0, mod2=0, mod3=0, mod4=0, reset=False, sync=False):
+    def tr(
+        self, mod0=0, mod1=0, mod2=0, mod3=0, mod4=0, mod5=0, reset=False, sync=False
+    ):
         """
         Triggers the modules with the given codes.
         Additionally, global triggers can be issued (reset and sync).
 
         TR = Trigger
         """
 
         self._check_trigger(mod0, "mod0")
         self._check_trigger(mod1, "mod1")
         self._check_trigger(mod2, "mod2")
         self._check_trigger(mod3, "mod3")
         self._check_trigger(mod4, "mod4")
+        self._check_trigger(mod5, "mod5")
 
         if not isinstance(reset, bool) or not isinstance(sync, bool):
             raise ValueError("reset and sync parameter need to be boolean.")
 
-        # Assembler: TR mod0, mod1, mod2, mod3, reset, sync
+        # Assembler: TR mod0, mod1, mod2, mod3, mod4, mod5, reset, sync
         self.assembler.append(
-            f"tr {mod0}, {mod1}, {mod2}, {mod3}, {mod4}, {reset*1}, {sync*1}\n"
+            f"tr {mod0}, {mod1}, {mod2}, {mod3}, {mod4}, {mod5}, {reset*1}, {sync*1}\n"
         )
 
         # Binary:
         #   0-6 OpCode (TRIGGER = 0x2)
         #   7-11 Rd (Unused)
         #   12-15 Global Trigger
         #       12 Reset
         #       13 Start Marker (Will only be issued by the sequencer itself)
         #       14 Sync
         #       15 (Unused)
         #   16-19 Mod0 Trigger
         #   20-21 Mod1 Trigger
         #   22-25 Mod2 Trigger
-        #   25-29 Mod3 Trigger
-        #   30-31 Mod4 Trigger
+        #   26-27 Mod3 Trigger
+        #   28-29 Mod4 Trigger
+        #   30-31 Mod5 Trigger
         self._add_command_value(
             0b0000010  # opcode TRIGGER
             + (reset << 12)
             + (sync << 14)
             + (mod0 << 16)
             + (mod1 << 20)
             + (mod2 << 22)
             + (mod3 << 26)
-            + (mod4 << 30)
+            + (mod4 << 28)
+            + (mod5 << 30)
         )
 
         return self
 
     def wti(self, clock_cycles=0):
         """
         Waits the given number of `clock_cycles` before continuing.
@@ -152,35 +157,35 @@
         # Binary:
         #   0-6 OpCode (TRIG_WAIT_REG = 0xA)
         #   7-11 Rd: Register Address
         self._add_command_value(0b0001010 + (register << 7))  # opcode TRIG_WAIT_REG
 
         return self
 
-    def tri(self, clock_cycles=1, mod0=0, mod1=0, mod2=0, mod3=0):
+    def tri(self, clock_cycles=1, mod0=0, mod1=0, mod2=0, mod3=0, mod4=0, mod5=0):
         """Triggers the modules with the given codes.
         Then waits the given number of `clock_cycles`.
 
         .. deprecated:: 0.0.2
             New sequencer has two separate commands for trigger (TR) and wait (WTI/WTR).
         """
-        self.tr(mod0, mod1, mod2, mod3)
+        self.tr(mod0, mod1, mod2, mod3, mod4, mod5)
         if clock_cycles > 1:
             self.wti(clock_cycles - 1)
         return self
 
-    def trr(self, reg=1, mod0=0, mod1=0, mod2=0, mod3=0):
+    def trr(self, reg=1, mod0=0, mod1=0, mod2=0, mod3=0, mod4=0, mod5=0):
         """Triggers the modules with the given codes.
         Then waits as long as the delay in the specified register `reg` states, decremented by 1,
         to account for trigger instruction duration.
 
         .. deprecated:: 0.0.2
             New sequencer has two separate commands for trigger (TR) and wait (WTI/WTR).
         """
-        self.tr(mod0, mod1, mod2, mod3)
+        self.tr(mod0, mod1, mod2, mod3, mod4, mod5)
         self.twr(reg)
         return self
 
     def sts(self, save_register, mod0=False, mod1=False, mod2=False, mod3=False):
         """
         Waits for a trigger response from the triggerbus of the specified modules
         and stores it into the register `save_register`.
@@ -512,88 +517,132 @@
         return str(hex(number))[2:] + "h"
 
 
 class SequencerCode(SequencerCodeBase):
     """Class to easily generate code for the QiController sequencer in an object-oriented manner."""
 
     def trigger_immediate(
-        self, delay=0, manipulation=0, readout=0, recording=0, external=0
+        self,
+        delay=0,
+        manipulation=0,
+        readout=0,
+        recording=0,
+        coupling0=0,
+        coupling1=0,
+        digital=0,
     ):
         """Triggers the modules with the given codes. Then waits for *delay* seconds.
 
         :param delay: The delay in seconds to wait before the next command is executed.
         :param manipulation: The code passed to the manipulation pulse generation module.
         :param readout: The code passed to the readout pulse generation module.
         :param recording: The code passed to the recording module.
-        :param external: The code triggering an optional external module.
+        :param coupling0: The code triggering the associated first coupling module.
+        :param coupling1: The code triggering the associated second coupling module.
+        :param digital: The code for digital output triggers.
         """
         # We always ceil so we get no accidental overlap
         clock_cycles_to_wait = util.conv_time_to_cycles(delay, "ceil")
 
         if clock_cycles_to_wait >= (1 << 12):
             raise ValueError(
                 "delay must be smaller than 2^12 clock cycles. Try TRR instead."
             )
+        if register < 0 or register >= (1 << 4):
+            raise ValueError("register has to be between 0 and 15.")
         if manipulation < 0 or manipulation >= (1 << 4):
             raise ValueError("manipulation has to be between 0 and 15.")
         if readout < 0 or readout >= (1 << 4):
             raise ValueError("readout has to be between 0 and 15.")
         if recording < 0 or recording >= (1 << 4):
             raise ValueError("recording has to be between 0 and 15.")
-        if external < 0 or external >= (1 << 4):
-            raise ValueError("external has to be between 0 and 15.")
+        if coupling0 < 0 or coupling0 >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
+        if coupling1 < 0 or coupling1 >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
+        if digital < 0 or digital >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
 
         return self.tri(
-            clock_cycles_to_wait, readout, recording, manipulation, external
+            clock_cycles_to_wait, readout, recording, manipulation, coupling0, coupling1
         )
 
     def trigger_registered(
-        self, register, manipulation=0, readout=0, recording=0, external=0
+        self,
+        register,
+        manipulation=0,
+        readout=0,
+        recording=0,
+        coupling0=0,
+        coupling1=0,
+        digital=0,
     ):
         """Triggers the modules with the given codes.
         Then waits as long as the delay in the specified *register* states.
 
         :param register: The register containing the delay to wait before continuing with the next command.
         :param manipulation: The code passed to the manipulation pulse generation module.
         :param readout: The code passed to the readout pulse generation module.
         :param recording: The code passed to the recording module.
-        :param external: The code triggering an optional external module.
+        :param coupling0: The code triggering the associated first coupling module.
+        :param coupling1: The code triggering the associated second coupling module.
+        :param digital: The code for digital output triggers.
         """
         if register < 0 or register >= (1 << 4):
             raise ValueError("register has to be between 0 and 15.")
         if manipulation < 0 or manipulation >= (1 << 4):
             raise ValueError("manipulation has to be between 0 and 15.")
         if readout < 0 or readout >= (1 << 4):
             raise ValueError("readout has to be between 0 and 15.")
         if recording < 0 or recording >= (1 << 4):
             raise ValueError("recording has to be between 0 and 15.")
-        if external < 0 or external >= (1 << 4):
-            raise ValueError("external has to be between 0 and 15.")
-
-        return self.trr(register, readout, recording, manipulation, external)
-
-    def trigger(self, manipulation=0, readout=0, recording=0, external=0):
+        if coupling0 < 0 or coupling0 >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
+        if coupling1 < 0 or coupling1 >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
+        if digital < 0 or digital >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
+
+        return self.trr(
+            register, readout, recording, manipulation, coupling0, coupling1, digital
+        )
+
+    def trigger(
+        self,
+        manipulation=0,
+        readout=0,
+        recording=0,
+        coupling0=0,
+        coupling1=0,
+        digital=0,
+    ):
         """Triggers the modules with the given codes.
         Then immediately continues with the next instruction (no delay / only 1 cycle).
 
         :param manipulation: The code passed to the manipulation pulse generation module.
         :param readout: The code passed to the readout pulse generation module.
         :param recording: The code passed to the recording module.
-        :param external: The code triggering an optional external module.
+        :param coupling0: The code triggering the associated first coupling module.
+        :param coupling1: The code triggering the associated second coupling module.
+        :param digital: The code for digital output triggers.
         """
         if manipulation < 0 or manipulation >= (1 << 4):
             raise ValueError("manipulation has to be between 0 and 15.")
         if readout < 0 or readout >= (1 << 4):
             raise ValueError("readout has to be between 0 and 15.")
         if recording < 0 or recording >= (1 << 4):
             raise ValueError("recording has to be between 0 and 15.")
-        if external < 0 or external >= (1 << 4):
-            raise ValueError("external has to be between 0 and 15.")
+        if coupling0 < 0 or coupling0 >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
+        if coupling1 < 0 or coupling1 >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
+        if digital < 0 or digital >= (1 << 2):
+            raise ValueError("external has to be between 0 and 3.")
 
-        return self.tr(readout, recording, manipulation, external)
+        return self.tr(readout, recording, manipulation, coupling0, coupling1, digital)
 
     def conditional_jump(self, address, state=None):
         """Waits for a previous readout to return its result.
         Then jumps to the given *address* if the determined state is *state*,
         otherwise program continues with the next command.
 
         If no *state* is given, the jump will always be performed.
```

### Comparing `qiclib-1.0.0/src/qiclib/experiment/SecondToneSweepR5.py` & `qiclib-1.1.0/src/qiclib/experiment/SecondToneSweepR5.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/__init__.py` & `qiclib-1.1.0/src/qiclib/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/active_cooling_t1.py` & `qiclib-1.1.0/src/qiclib/experiment/active_cooling_t1.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/active_reset_t1.py` & `qiclib-1.1.0/src/qiclib/experiment/active_reset_t1.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/autoconf_readout.py` & `qiclib-1.1.0/src/qiclib/experiment/autoconf_readout.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/base.py` & `qiclib-1.1.0/src/qiclib/experiment/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,16 @@
         self._configure_called = True
 
         # All methods can be overwritten depending on the needs of the actual experiments
         self._configure_readout()
         self._configure_drive_pulses()
         self._configure_sequences()
         self._configure_taskrunner()
+        self._configure_digital_triggers()
+        self._configure_couplers()
 
     def record(self):
         """Starts the experiment recording and returns the result.
 
         .. note::
             This method does not configure the QiController. It expects that
             :meth:`BaseExperiment.configure` has been called in advance. If you are
@@ -558,14 +560,20 @@
 
         Method _build_code_from_sequences() can be used here.
         """
         self._built_code_from_sequences(
             {"default": lambda code: None}  # Everything will be added by wrapper
         )
 
+    def _configure_digital_triggers(self):
+        pass
+
+    def _configure_couplers(self):
+        pass
+
     def _configure_taskrunner(self):
         """This method configures the taskrunner for the experiment.
 
         In it's default configuration, a versatile standard task to use with `use_taskrunner=True` is loaded.
         """
         if self.use_taskrunner:
             if self.qic.taskrunner is not None:
```

### Comparing `qiclib-1.0.0/src/qiclib/experiment/benchmarking.py` & `qiclib-1.1.0/src/qiclib/experiment/benchmarking.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/collection.py` & `qiclib-1.1.0/src/qiclib/experiment/collection.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/correlation_calibration.py` & `qiclib-1.1.0/src/qiclib/experiment/correlation_calibration.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/correlation_conv_all.py` & `qiclib-1.1.0/src/qiclib/experiment/correlation_conv_all.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/g1_correlation.py` & `qiclib-1.1.0/src/qiclib/experiment/g1_correlation.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/g1_correlation_conv.py` & `qiclib-1.1.0/src/qiclib/experiment/g1_correlation_conv.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/g1_meas_setuptest.py` & `qiclib-1.1.0/src/qiclib/experiment/g1_meas_setuptest.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/g2_correlation.py` & `qiclib-1.1.0/src/qiclib/experiment/g2_correlation.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/g2_correlation_conv.py` & `qiclib-1.1.0/src/qiclib/experiment/g2_correlation_conv.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/gx_correlation_base.py` & `qiclib-1.1.0/src/qiclib/experiment/gx_correlation_base.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/inverted_t1.py` & `qiclib-1.1.0/src/qiclib/experiment/inverted_t1.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/iq_clouds.py` & `qiclib-1.1.0/src/qiclib/experiment/iq_clouds.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/iq_clouds_multi_qfb.py` & `qiclib-1.1.0/src/qiclib/experiment/iq_clouds_multi_qfb.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/iq_clouds_qfb.py` & `qiclib-1.1.0/src/qiclib/experiment/iq_clouds_qfb.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/iq_clouds_qfb_decay.py` & `qiclib-1.1.0/src/qiclib/experiment/iq_clouds_qfb_decay.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/iq_clouds_ramsey.py` & `qiclib-1.1.0/src/qiclib/experiment/iq_clouds_ramsey.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/iq_clouds_ringup.py` & `qiclib-1.1.0/src/qiclib/experiment/iq_clouds_ringup.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/multi_pi.py` & `qiclib-1.1.0/src/qiclib/experiment/multi_pi.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/multi_pi_t1.py` & `qiclib-1.1.0/src/qiclib/experiment/multi_pi_t1.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/__init__.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/base.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .data_handler import DataHandler
 from ...code.qi_types import QiType
 from ...hardware.pulsegen import TriggerSet
 from ...hardware.taskrunner import TaskRunner
 from ...experiment.base import BaseExperiment, ExperimentReadout
 from ...packages.constants import CONTROLLER_SAMPLE_FREQUENCY_IN_HZ as samplerate
 from ...packages import utility as util
-from ...code.qi_jobs import QiCell
+from ...code.qi_jobs import QiCell, QiCoupler
 from ...code.qi_sequencer import ForRangeEntry, Sequencer
 from ...code.qi_pulse import QiPulse
 from ...code.qi_var_definitions import _QiVariableBase
 
 from ...packages.qkit_polyfill import SampleObject
 
 
@@ -61,29 +61,33 @@
     :raises Exception: If more than 16 parameterized pulses are present
     """
 
     def __init__(
         self,
         controller,
         cell_list: List[QiCell],
+        couplers: List[QiCoupler],
         sequencer_codes,
         averages: int = 1,
         for_range_list=[],
         cell_map: Optional[List[int]] = None,
+        coupler_map: Optional[List[int]] = None,
         var_reg_map: Dict[_QiVariableBase, Dict[QiCell, int]] = {},
         data_collection="average",
         use_taskrunner=False,
     ):
         self.cell_list = cell_list
+        self.couplers = couplers
         # The Variables for calculating a parametrized Pulse.
         super().__init__(controller)
         self._seq_instructions = sequencer_codes
         self.averages = averages
         self.for_range_list = for_range_list
         self.cell_map = cell_map
+        self.coupler_map = coupler_map
         self._var_reg_map = var_reg_map
         self._data_collection = data_collection
         self.use_taskrunner = use_taskrunner
         self._data_handler_factory: Optional[
             Callable[[DataProvider, List[QiCell], int], DataHandler]
         ] = None
 
@@ -192,14 +196,18 @@
                 f"Invalid data collection option: '{self._data_collection}' (possible settings: {options})"
             )
 
     def cell_iterator(self):
         for idx, sample_cell in enumerate(self.cell_list):
             yield idx, sample_cell, self.qic.cell[self.cell_map[idx]]
 
+    def coupling_iterator(self):
+        for idx, coupler in enumerate(self.couplers):
+            yield coupler, self.qic.pulse_players[self.coupler_map[idx]]
+
     def _configure_readout(self, no_warn=False):
         """Overwrites the _configure_readout method of BaseExperiment class.
         Loads readout pulses of a sequence in successive readout triggersets.
 
         :param no_warn: currently not used here
 
         :raises Exception: if one uses more than 13 different readout pulses within the sequence.
@@ -259,14 +267,29 @@
                     )
 
             try:
                 qic_cell.manipulation.if_frequency = cell.initial_manipulation_frequency
             except AttributeError:
                 pass  # No manipulation pulses present -> just leave the current setting
 
+    def _configure_digital_triggers(self):
+        for _, cell, qic_cell in self.cell_iterator():
+            qic_cell.digital_trigger.clear_trigger_sets()
+            for index, trig_set in enumerate(cell.digital_trigger_sets):
+                # In the array, triggers are indexed starting from 0. However, index 0 is reserved and cannot be used.
+                # Therefore, we start at index # 1. This is also accounted for in QiCell.add_digital_trigger()
+                qic_cell.digital_trigger.set_trigger_set(index + 1, trig_set)
+
+    def _configure_couplers(self):
+        for coupler, pulse_player in self.coupling_iterator():
+            pulse_player.reset()
+            for index, pulse in enumerate(coupler.coupling_pulses):
+                # In the array, triggers are indexed starting from 0. However, index 0 is reserved and cannot be used.
+                pulse_player.pulses[index + 1] = pulse(pulse_player.sample_rate)
+
     def _configure_sequences(self):
         """Overwrites the _configure_sequences method of BaseExperiment class.
         This function generates the assembler code for the sequencer and loads it on the platform.
         """
         for index, _, qic_cell in self.cell_iterator():
             qic_cell.sequencer.load_program_code(self._seq_instructions[index])
```

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/collection.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/collection.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/data_handler.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/data_handler.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/data_provider.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/data_provider.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/init_readout.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/init_readout.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/qubit_times.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/qubit_times.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qicode/qubit_times_qkit.py` & `qiclib-1.1.0/src/qiclib/experiment/qicode/qubit_times_qkit.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qkit_virtual_awg.py` & `qiclib-1.1.0/src/qiclib/experiment/qkit_virtual_awg.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/quantum_jumps.py` & `qiclib-1.1.0/src/qiclib/experiment/quantum_jumps.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/quantum_jumps_long.py` & `qiclib-1.1.0/src/qiclib/experiment/quantum_jumps_long.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qubit_times.py` & `qiclib-1.1.0/src/qiclib/experiment/qubit_times.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/qubit_times_qkit.py` & `qiclib-1.1.0/src/qiclib/experiment/qubit_times_qkit.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rabi.py` & `qiclib-1.1.0/src/qiclib/experiment/rabi.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rabi_R5PG.py` & `qiclib-1.1.0/src/qiclib/experiment/rabi_R5PG.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rabi_drag.py` & `qiclib-1.1.0/src/qiclib/experiment/rabi_drag.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rabi_short.py` & `qiclib-1.1.0/src/qiclib/experiment/rabi_short.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/ramsey.py` & `qiclib-1.1.0/src/qiclib/experiment/ramsey.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/readout.py` & `qiclib-1.1.0/src/qiclib/experiment/readout.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/readout_spectr.py` & `qiclib-1.1.0/src/qiclib/experiment/readout_spectr.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/resonator_ringup.py` & `qiclib-1.1.0/src/qiclib/experiment/resonator_ringup.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/resonator_ringup_window.py` & `qiclib-1.1.0/src/qiclib/experiment/resonator_ringup_window.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/__init__.py` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/active_cooling.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/active_cooling.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/average_trace.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/average_trace.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/base_experiment_task.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/base_experiment_task.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/__init__.py` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/calibration.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/calibration.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/correlation_conv.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/correlation_conv.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation_conv.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g1_correlation_conv.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g1_meas_setuptest.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g1_meas_setuptest.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation_conv.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/correlation/g2_correlation_conv.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/interleaved.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/interleaved.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/interleaved_multi.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/interleaved_multi.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/iq_clouds.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/iq_clouds.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/optimize_rec_offset.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/optimize_rec_offset.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/__init__.py` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/averaging.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/averaging.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/iq_collect.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/iq_collect.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/state_collect.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/state_collect.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/state_count.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/state_count.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qicode/timetrace.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qicode/timetrace.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/quantum_jumps.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/quantum_jumps.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_multi.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_multi.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_new.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/quantum_jumps_new.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/qubit_freq_sweep_task.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/qubit_freq_sweep_task.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/rabi_r5.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/rabi_r5.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/__init__.py` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/copy_test.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/copy_test.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/empty.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/empty.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/shift_test.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/shift_test.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/stream_test.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/stream_test.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/test_databox.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/test_databox.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/time_test_code.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/time_test_code.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/timing_test.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/timing_test.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/timing_test_axi.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/timing_test_axi.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/test/timing_test_single.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/test/timing_test_single.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/rtos_tasks/trace_fft.c` & `qiclib-1.1.0/src/qiclib/experiment/rtos_tasks/trace_fft.c`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/single_pulse.py` & `qiclib-1.1.0/src/qiclib/experiment/single_pulse.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/spinecho.py` & `qiclib-1.1.0/src/qiclib/experiment/spinecho.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/stream_test.py` & `qiclib-1.1.0/src/qiclib/experiment/stream_test.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/t1.py` & `qiclib-1.1.0/src/qiclib/experiment/t1.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/experiment/test_two_pulse.py` & `qiclib-1.1.0/src/qiclib/experiment/test_two_pulse.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/hardware/__init__.py` & `qiclib-1.1.0/src/qiclib/hardware/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,32 +23,34 @@
 controlled and configured to obtain the desired output and functionality.
 In the following the architecture of the QiController is introduced in more detail.
 
 .. todo:: Add architecture image (overview of the QiController architecture)
 
 .. image:: platform.png
 
-Tasks which require nanosecond accuracy are handled within the FPGA.
-There, the main functionality is provided by digital unit cells (see `qiclib.hardware.unitcell`).
-They generate digital microwave pulses which are flexibly routed (i.e. combined and distributed) to the available DAC channels.
-Likewise, returning digitized microwave signals from the ADCs are distributed and split up onto the belonging cells.
-The cells are synchronized using a special cell coordinator which also facilitates data exchange between the cells.
-On the processing system, online data processing and advanced control is implemented by the Taskrunner on a dedicated real-time processor.
-A modular communication server called ServiceHub provides a user interface to interact with the platform via Ethernet.
-This python driver encapsulates the remote procedure calls exposed by the ServiceHub (using the gRPC framework).
+Tasks which require nanosecond accuracy are handled within the FPGA. There, the main functionality is provided by
+digital unit cells (see `qiclib.hardware.unitcell`). They generate digital microwave pulses which are flexibly routed
+(i.e. combined and distributed) to the available DAC channels. Likewise, returning digitized microwave signals from
+the ADCs are distributed and split up onto the belonging cells. The cells are synchronized using a special cell
+coordinator which also facilitates data exchange between the cells. On the processing system, online data processing
+and advanced control is implemented by the Taskrunner on a dedicated real-time processor. A modular communication
+server called ServiceHub provides a user interface to interact with the platform via Ethernet. This python driver
+encapsulates the remote procedure calls exposed by the ServiceHub (using the gRPC framework).
 
-Experiments running on the QiController are normally all partitioned in a similar way.
-Pulse generation, detection, sequencing and result storage, as well as simple parameter variations, happen with nanosecond precision in the digital unit cells in the FPGA.
-Their execution is synchronized by the cell coordinator which is triggered by the Taskrunner.
-The Taskrunner controls the execution of the FPGA, performs more complex parameter variations between multiple executions and collects the result data that is generated within the digital unit cells.
-Also, further data aggregation, sorting or online evaluation are possible, depending on the requirements of the experiment.
-This includes, but is not limited to, averaging of data, collection of individual qubit states or single measurement values, as well as counting different qubit state outcomes.
-You can also define your own C program to perform custom data processing and aggregation (see `qiclib.hardware.taskrunner`).
-The resulting data is then sent via the ServiceHub to the user client where you can either persist or further process the data offline.
-During the experiment, in principle, no connection between client and QiController is required.
-However, you can monitor the progress of the execution and, depending on the experiment, stream some result data already before the execution finished.
+Experiments running on the QiController are normally all partitioned in a similar way. Pulse generation, detection,
+sequencing and result storage, as well as simple parameter variations, happen with nanosecond precision in the
+digital unit cells in the FPGA. Their execution is synchronized by the cell coordinator which is triggered by the
+Taskrunner. The Taskrunner controls the execution of the FPGA, performs more complex parameter variations between
+multiple executions and collects the result data that is generated within the digital unit cells. Also, further data
+aggregation, sorting or online evaluation are possible, depending on the requirements of the experiment. This
+includes, but is not limited to, averaging of data, collection of individual qubit states or single measurement
+values, as well as counting different qubit state outcomes. You can also define your own C program to perform custom
+data processing and aggregation (see `qiclib.hardware.taskrunner`). The resulting data is then sent via the
+ServiceHub to the user client where you can either persist or further process the data offline. During the
+experiment, in principle, no connection between client and QiController is required. However, you can monitor the
+progress of the execution and, depending on the experiment, stream some result data already before the execution
+finished.
 
-For more details on how to interact with the QiController, see `qiclib.hardware.controller`.
-Details concerning the high-level experiment description language QiCode can be found in `qiclib.code`.
-The functionalities covered by the digital unit cells within the FPGA are covered in `qiclib.hardware.unitcell`.
-For more background regarding the online data processing and aggregation within the Taskrunner, refer to `qiclib.hardware.taskrunner`.
-"""
+For more details on how to interact with the QiController, see `qiclib.hardware.controller`. Details concerning the
+high-level experiment description language QiCode can be found in `qiclib.code`. The functionalities covered by the
+digital unit cells within the FPGA are covered in `qiclib.hardware.unitcell`. For more background regarding the
+online data processing and aggregation within the Taskrunner, refer to `qiclib.hardware.taskrunner`."""
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/controller.py` & `qiclib-1.1.0/src/qiclib/hardware/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 import warnings
 
 from qiclib.hardware.platform_component import (
     PlatformComponent,
     platform_attribute,
     platform_attribute_collector,
 )
+from qiclib.hardware.pulse_player import PulsePlayer
 from qiclib.hardware.pulsegen import PulseGen
 from qiclib.hardware.recording import Recording
 from qiclib.hardware.rfdc import RFDataConverter
 from qiclib.hardware.sequencer import Sequencer
 from qiclib.hardware.servicehub import ServiceHub
 from qiclib.hardware.storage import Storage
 from qiclib.hardware.taskrunner import TaskRunner
@@ -122,19 +123,30 @@
             self._taskrunner = TaskRunner("Taskrunner", connection, self)
         else:
             self._taskrunner = None
 
         self._rfdc = RFDataConverter("RF Data Converter", connection, self)
         self._cell = UnitCells("UnitCells", connection, self, qkit_instrument=False)
         self._print(f"Firmware with {self.cell.count} digital unit cells detected.")
+
         if self.cell.count == 0:
             raise NotImplementedError(
                 "No digital unit cells found on QiController! "
                 "Please update the board firmware."
             )
+        self._pulse_players = []
+        for endpoint in self._servicehub.get_endpoints_of_plugin("PulsePlayerPlugin"):
+            index = self._servicehub.get_endpoint_index_from_plugin(
+                "PulsePlayerPlugin", endpoint
+            )
+            self._pulse_players.append(
+                PulsePlayer(
+                    "Pulse Player", connection, self, index, qkit_instrument=False
+                )
+            )
 
         # TODO Deprecated, remove in next major version
         # Preconfigure some standard values
         warnings.filterwarnings("ignore", category=FutureWarning)
         self._sample = SampleObject()
         self._init_sample_object()
         self.update_modules()
@@ -211,14 +223,15 @@
                 "by this driver version"
             )
 
         self._platform_name = {
             0x23: "ZCU111",
             0x38: "ZRF8",
             0x41: "ZCU216",
+            0x51: "ZCU208",
         }.get(self.platform_id)
 
         if self.platform_name is None:
             raise RuntimeError(
                 f"Board ID {self.platform_id} ({self.platform_name}) is not supported "
                 "by this driver version"
             )
@@ -254,14 +267,25 @@
 
         This component provides configuration access to the data converters of the board
         and can be used to query status information like overvoltage conditions.
         """
         return self._rfdc
 
     @property
+    def pulse_players(self) -> List[PulsePlayer]:
+        """
+        The pulse players of the platform.
+
+        Each :class:`qiclib.hardware.pulse_player.PulsePlayer`
+        is similar to the `qiclib.hardware.pulse_player.PulseGen` component,
+        however, pulse players do not have digital upconversion but instead  more memory.
+        """
+        return self._pulse_players
+
+    @property
     def taskrunner(self) -> Optional[TaskRunner]:
         """The Taskrunner framework of the QiController.
 
         This subsystem can be used to run arbitrary C code on a processor of the
         QiController to perform custom online data processing and aggregation.
 
         More information can be found here: :class:`qiclib.hardware.taskrunner`
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/pimc.py` & `qiclib-1.1.0/src/qiclib/hardware/pimc.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 A ready flag tells the user if the platform is fully initialized and ready to use.
 This includes a check if all clocks are configured and running correctly, and if the
 connection to the converters is established and working.
 """
 from qiclib.hardware.platform_component import PlatformComponent
 
 from qiclib.packages.servicehub import ServiceHubCall
-import qiclib.packages.grpc.pimc_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.pimc_pb2_grpc as grpc_stub
 
 
 class PIMC(PlatformComponent):
     """Platform Information and Management Core/Controller (PIMC)
 
     This core provides information about the loaded project and the hardware used.
@@ -60,15 +60,15 @@
             )
 
     @ServiceHubCall(
         errormsg="Could not read board information. "
         "Please make sure the board is connected."
     )
     def _get_info(self):
-        return self._stub.GetInfo(proto.Empty())
+        return self._stub.GetInfo(dt.Empty())
 
     @property
     def core_version(self) -> int:
         """The version of the PIMC component."""
         return self._info.pimcVersion
 
     @property
@@ -113,15 +113,15 @@
             * rst_done: bool
                 If a software reset was already called (necessary for some initializations)
             * ready: bool
                 If the Platform is ready to use.
             * busy: bool
                 If the Platform is currently busy.
         """
-        return self._stub.GetStatus(proto.Empty())
+        return self._stub.GetStatus(dt.Empty())
 
     @property
     def is_ready(self):
         """If the Platform is ready to use."""
         return self.status.ready
 
     @property
@@ -133,8 +133,8 @@
     def reset_done_flag(self):
         """If a software reset was already called (necessary for some initializations)."""
         return self.status.rst_done
 
     @ServiceHubCall(errormsg="Error resetting the Platform")
     def reset(self):
         """Resets the hardware part of the Platform."""
-        self._stub.SetReset(proto.Empty())
+        self._stub.SetReset(dt.Empty())
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/platform_component.py` & `qiclib-1.1.0/src/qiclib/hardware/platform_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """This module contains the base class for all QiController platform components.
 
 All modules representing a part of the QiController should be derived from it. It also
 includes automatic integration of the component into the Qkit framework.
 """
-from typing import TYPE_CHECKING, Dict, Any, Set
+import abc
+from typing import Dict, Any, Set
 
 from qiclib.packages.qkit_polyfill import QKIT_ENABLED, Instrument, qkit
 from qiclib.packages.servicehub import Connection
 
 
-class PlatformComponent:
+class PlatformComponent(abc.ABC):
     """Base class for components on the QiController.
 
     All QiController platform components share a common constructor
     (`qiclib.hardware.platform_component.PlatformComponent`).
 
     The user does not create this class directly.
     Instead, existing instances of it can be accessed using the `qiclib.hardware.controller.QiController`
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/pulsegen.py` & `qiclib-1.1.0/src/qiclib/hardware/pulsegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     PlatformComponent,
     platform_attribute,
     platform_attribute_collector,
 )
 import qiclib.packages.utility as util
 from qiclib.packages.servicehub import ServiceHubCall
 import qiclib.packages.grpc.pulsegen_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.pulsegen_pb2_grpc as grpc_stub
 
 
 @platform_attribute_collector
 class PulseGen(PlatformComponent):
     """A signal generator within a digital unit cell of the QiController.
 
@@ -120,15 +121,15 @@
 
     def __init__(
         self, name: str, connection, controller, qkit_instrument=True, index=0
     ):
         super().__init__(name, connection, controller, qkit_instrument)
         self._stub = grpc_stub.PulseGenServiceStub(self._conn.channel)
         self._index = index
-        self._component = proto.EndpointIndex(value=self._index)
+        self._component = dt.EndpointIndex(value=self._index)
 
         # TODO Numbers to appropriate constants
         self._triggerset: List[Optional["TriggerSet"]] = [None]
         self._triggerset.extend(
             TriggerSet(
                 f"{self.name} Trigger {i:02d}",
                 self._conn,
@@ -413,15 +414,15 @@
 
     @ServiceHubCall(errormsg="Error resetting the signal generator status flags")
     def reset_status_flags(self):
         """Resets the status flags of the signal generator."""
         self._stub.ResetStatusFlags(self._component)
 
     @ServiceHubCall(errormsg="Error obtaining the signal generator status flags")
-    def get_status_flags(self) -> proto.StatusFlags:
+    def get_status_flags(self) -> proto.StatusFlags:  # type: ignore
         """Obtains the status flags of the signal generator.
 
         The following flags will be returned as object properties:
 
         - ``saturation``: If the amplitude calibration resulted in signal saturation at
             signal generator output (output was compressed/clipped).
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/recording.py` & `qiclib-1.1.0/src/qiclib/hardware/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     PlatformComponent,
     platform_attribute,
     platform_attribute_collector,
 )
 
 from qiclib.packages.servicehub import ServiceHubCall
 import qiclib.packages.grpc.recording_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.recording_pb2_grpc as grpc_stub
 
 
 class RecordingTrigger(Enum):
     """The available trigger commands of the signal recorder.
 
     They distinguish different operation modes.
@@ -168,15 +169,15 @@
 
     def __init__(
         self, name: str, connection, controller, qkit_instrument=True, index: int = 0
     ):
         super().__init__(name, connection, controller, qkit_instrument)
         self._stub = grpc_stub.RecordingStub(self._conn.channel)
         self._index = index
-        self._component = proto.EndpointIndex(value=self._index)
+        self._component = dt.EndpointIndex(value=self._index)
 
     def load_configuration(self, sample, no_warn: bool = False):
         """Load the recording module configuration from a (legacy) sample object.
 
         .. deprecated::
             `sample` will be removed in future. Therefore, this method becomes obsolete.
             Please use the new QiCode syntax (see `qiclib.code`) instead.
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/rfdc.py` & `qiclib-1.1.0/src/qiclib/hardware/rfdc.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,34 +22,31 @@
 While not usually the case, the sampling frequency `Fs` can be different based on any given converter.
 It can be obtained using the :python:`sampling_frequency` field in the objects returned by the
 :meth:`RFDataConverter.adc_block_status` and :meth:`RFDataConverter.dac_block_status` methods.
 
 Mixing Capabilities
 ===================
 
-ADCs and DACs contain a fine-tunable mixer that is implemented using a 48-bit NCO.
+ADCs and DACs contain a fine-tunable mixer implemented using a 48-bit NCO.
 Obtain the current frequency of the NCO via the :meth:`RFDataConverter.get_mixer_frequency` method.
 Using the :meth:`RFDataConverter.set_mixer_frequency`, the sampling frequency of a mixer can be changed.
 The Frequency range is -Fs/2 to Fs/2.
 """
 import sys
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from enum import Enum
 
 from qiclib.hardware.platform_component import PlatformComponent
 
 from qiclib.packages.servicehub import ServiceHubCall
 import qiclib.packages.grpc.rfdc_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.rfdc_pb2_grpc as grpc_stub
 
-from enum import Enum
-
-from typing_extensions import Literal
-
-ConverterType = Literal["adc", "dac"]
-
 
 class MixerMode(Enum):
     """
     Represents possible mixer modes.
     """
 
     OFF = 0
@@ -67,28 +64,37 @@
     REAL_TO_COMPLEX = 3
     """
     The mixer is in real-to-complex mode, i.e. mixes real signals to IQ signals
     """
 
 
 class InvSincFilterState(Enum):
+    """
+    Normally, the output spectrum of the RF-DAC used in the RFdc has a sin(x)/x characteristic.
+    If a flat-output response is desired, the inverse sinc filter can be enabled.
+    See more at the `official documentation <https://docs.xilinx.com/r/en-US/pg269-rf-data-converter/RF-DAC-Inverse-Sinc-Filter>`_
+    """
+
     DISABLED = 0
     """
     No inverse sinc filter is implemented
     """
     FIRST_NYQUIST = 1
     """
     The inverse sinc filter is active for the first nyquist zone
     """
     SECOND_NYQUIST = 2
     """
     The inverse sinc filter is active for the second nyquist zone.
     Note that this is only available for Gen3 / DFE devices (i.e. only for the ZCU216 platform)
     """
 
+    def is_on(self) -> bool:
+        return self != InvSincFilterState.DISABLED
+
 
 class DecoderMode(Enum):
     """
     Inside the RFdc, a trade-off can be chosen between maximizing the SNR or the linearity.
     """
 
     UNSET = 0
@@ -138,14 +144,142 @@
     adder_status: int
     mixer_mode: MixerMode
     data_path_clocks_enabled: bool
     fifo_flags_enabled: bool
     fifo_flags_asserted: bool
 
 
+class DataConverter(ABC):
+    def __init__(self, stub: grpc_stub.RFdcServiceStub, block: int, tile: int):
+        self._stub = stub
+        self.block = block
+        self.tile = tile
+
+    @abstractmethod
+    def _endpoint_index(self) -> proto.ConverterIndex:  # type: ignore
+        pass
+
+    @property
+    def mixer_frequency(self) -> float:
+        """
+        Get the internal mixer frequency.
+
+        :return:
+            The mixer frequency at that DAC or ADC in Hz
+
+        """
+        return self._stub.GetMixerFrequency(self._endpoint_index()).value
+
+    @mixer_frequency.setter
+    def mixer_frequency(self, frequency: float):
+        """
+        Set the mixer frequency.
+        The mixer frequency must be in the range `-Fs/2` to `Fs/2` where `Fs` is the sampling frequency.
+
+        :param frequency:
+            The frequency in Hz
+
+        :return: The mixer frequency of the DAC or ADC
+
+        """
+        self._stub.SetMixerFrequency(
+            proto.Frequency(value=frequency, index=self._endpoint_index())
+        )
+
+    @property
+    def mixer_phase(self) -> float:
+        """
+        Get the phase of the mixer
+
+        :return:
+            The mixer's phase in ?
+        """
+        return self._stub.GetPhase(self._endpoint_index()).value
+
+    @mixer_phase.setter
+    def mixer_phase(self, phase: float):
+        """
+        Set the phase of the mixer
+
+        :param phase:
+            The mixer's phase in ?
+        """
+        self._stub.SetPhase(proto.Phase(value=phase, index=self._endpoint_index()))
+
+
+class DAC(DataConverter):
+    def _endpoint_index(self) -> proto.ConverterIndex:  # type: ignore
+        return proto.ConverterIndex(
+            tile=self.tile, block=self.block, converter_type=proto.ConverterType.DAC
+        )
+
+    @property
+    def status(self) -> DACBlockStatus:
+        """
+        reports the status of a DAC
+
+        :return:
+            All relevant status information
+        """
+        status = self._stub.GetBlockStatus(self._endpoint_index())
+        return DACBlockStatus(
+            sampling_frequency=status.frequency,
+            inv_sinc_status=InvSincFilterState(status.analogstatus & 0xF),
+            decoder_mode=DecoderMode((status.analogstatus & 0x0F) >> 4),
+            fifo_status=(status.digitalstatus & 0xF),
+            interpolation_factor=(status.digitalstatus & 0x0F) >> 4,
+            adder_status=(status.digitalstatus & 0x00F) >> 12,
+            mixer_mode=MixerMode((status.digitalstatus & 0xF000) >> 12),
+            data_path_clocks_enabled=bool(status.clockstatus),
+            fifo_flags_enabled=bool(status.fifoflagsenabled),
+            fifo_flags_asserted=bool(status.fifoflagsasserted),
+        )
+
+    @property
+    def inv_sinc_filter(self) -> InvSincFilterState:
+        proto_state = self._stub.GetInvSincFIR(
+            proto.InvSincFIR(index=self._endpoint_index())
+        ).value
+        if proto_state == proto.InvSincFIR_Enum.DISABLED:
+            return InvSincFilterState.DISABLED
+        elif proto_state == proto.InvSincFIR_Enum.FIRST_NYQUIST:
+            return InvSincFilterState.FIRST_NYQUIST
+        elif proto_state == proto.InvSincFIR_Enum.SECOND_NYQUIST:
+            return InvSincFilterState.SECOND_NYQUIST
+        else:
+            raise ValueError(f"Illegal state {proto_state} returned from protobuf call")
+
+
+class ADC(DataConverter):
+    def _endpoint_index(self) -> proto.ConverterIndex:  # type: ignore
+        return proto.ConverterIndex(
+            tile=self.tile, block=self.block, converter_type=proto.ConverterType.ADC
+        )
+
+    @property
+    def status(self) -> ADCBlockStatus:
+        """
+        reports the status of this ADC
+
+        :return:
+            All relevant status information
+        """
+        status = self._stub.GetBlockStatus(self._endpoint_index())
+        return ADCBlockStatus(
+            sampling_frequency=status.frequency,
+            enabled=bool(status.analogstatus & 0x1),
+            fifo_status=status.digitalstatus & 0xF,
+            decimation_factor=(status.digitalstatus & 0x0F) >> 4,
+            mixer_mode=MixerMode((status.digitalstatus & 0xF00) >> 8),
+            data_path_clocks_enabled=bool(status.clockstatus),
+            fifo_flags_enabled=bool(status.fifoflagsenabled),
+            fifo_flags_asserted=bool(status.fifoflagsasserted),
+        )
+
+
 class RFDataConverter(PlatformComponent):
     """
     Driver to interface with the RF data converters (ADCs/DACs) on the QiController.
 
     The ADCs and DACs are organized in tiles and blocks. Most functions accept that tile and block as argument.
     """
 
@@ -155,34 +289,39 @@
         connection,
         controller,
         qkit_instrument=True,
     ):
         super().__init__(name, connection, controller, qkit_instrument)
         self._stub = grpc_stub.RFdcServiceStub(self._conn.channel)
 
-    def _endpoint_index(self, converter_type: ConverterType, tile: int, block: int):
-        if converter_type == "adc":
-            proto_converter_type = proto.ConverterType.ADC
-        elif converter_type == "dac":
-            proto_converter_type = proto.ConverterType.DAC
-        else:
-            raise ValueError(
-                f"Illegal converter choice {converter_type}. Must be 'dac' or 'adc'"
-            )
-        return proto.ConverterIndex(
-            tile=tile, block=block, converter_type=proto_converter_type
-        )
+    def dac(self, block: int, tile: int) -> DAC:
+        """
+        Get a reference to a DAC at a certain tile and block index.
+
+        Using the returned object, properties of the corresponding DAC can be set
+        that will be updated on the QiController.
+        """
+        return DAC(self._stub, block, tile)
+
+    def adc(self, block: int, tile: int) -> ADC:
+        """
+        Get a reference to an ADC ar a certain tile and block index.
+
+        Using the returned object, properties of the corresponding ADC can be set
+        that will be updated on the QiController.
+        """
+        return ADC(self._stub, block, tile)
 
     @ServiceHubCall(errormsg="Could not reset RF data converter status")
     def reset_status(self):
         """Reset the status of the RF data converters.
 
         This is especially the ADC over voltage conditions.
         """
-        self._stub.ResetStatus(proto.Empty())
+        self._stub.ResetStatus(dt.Empty())
 
     @ServiceHubCall(errormsg="Could not check RF data converter status")
     def check_status(self, raise_exceptions: bool = True) -> bool:
         """Check if a converter reported an error and if so, forward it to the user.
 
         .. warning::
             Currently, this is not working as reliable as the information provided by the
@@ -191,118 +330,20 @@
         :param raise_exceptions:
             if assigned status flags will result in an exception or just in a warning
             output
 
         :return:
             if everything is fine and no status flags have been raised.
         """
-        response = self._stub.ReportStatus(proto.Empty())
+        response = self._stub.ReportStatus(dt.Empty())
         status_report = response.report
 
         if response.failure:
             self.reset_status()
             status_report = (
                 "The data converters reported the following issue(s):\n" + status_report
             )
             if raise_exceptions:
                 raise Warning(status_report)
             sys.stderr.write(status_report)
 
         return not response.failure
-
-    @ServiceHubCall(errormsg="Could not obtain ADC block status")
-    def adc_block_status(self, tile, block) -> ADCBlockStatus:
-        """
-        reports the status of an ADC
-
-        :param tile:
-            The tile of the ADC
-        :param block:
-            The block of the ADC
-
-        :return:
-            All relevant status information
-        """
-        index = self._endpoint_index("adc", tile, block)
-        status = self._stub.GetBlockStatus(index)
-        return ADCBlockStatus(
-            sampling_frequency=status.frequency,
-            enabled=bool(status.analogstatus & 0x1),
-            fifo_status=status.digitalstatus & 0xF,
-            decimation_factor=(status.digitalstatus & 0x0F) >> 4,
-            mixer_mode=MixerMode((status.digitalstatus & 0x00F) >> 8),
-            data_path_clocks_enabled=bool(status.clockstatus),
-            fifo_flags_enabled=bool(status.fifoflagsenabled),
-            fifo_flags_asserted=bool(status.fifoflagsasserted),
-        )
-
-    @ServiceHubCall(errormsg="Could not obtain DAC block status")
-    def dac_block_status(self, tile, block) -> DACBlockStatus:
-        """
-        reports the status of a DAC
-
-        :param tile:
-            The tile of the DAC
-        :param block:
-            The block of the DAC
-
-        :return:
-            All relevant status information
-        """
-        index = self._endpoint_index("dac", tile, block)
-        status = self._stub.GetBlockStatus(index)
-        return DACBlockStatus(
-            sampling_frequency=status.frequency,
-            inv_sinc_status=InvSincFilterState(status.analogstatus & 0xF),
-            decoder_mode=DecoderMode((status.analogstatus & 0x0F) >> 4),
-            fifo_status=(status.digitalstatus & 0xF),
-            interpolation_factor=(status.digitalstatus & 0x0F) >> 4,
-            adder_status=(status.digitalstatus & 0x00F) >> 8,
-            mixer_mode=MixerMode((status.digitalstatus & 0x000F) >> 12),
-            data_path_clocks_enabled=bool(status.clockstatus),
-            fifo_flags_enabled=bool(status.fifoflagsenabled),
-            fifo_flags_asserted=bool(status.fifoflagsasserted),
-        )
-
-    @ServiceHubCall(errormsg="Could not obtain mixer frequency")
-    def get_mixer_frequency(
-        self, converter_type: ConverterType, tile: int, block: int
-    ) -> float:
-        """
-        Get the internal mixer frequency.
-
-        :param converter_type:
-            The type; either "adc" or "dac"
-        :param tile:
-            The tile of the converter
-        :param block:
-            The block of the converter
-
-        :return:
-            The mixer frequency at that DAC or ADC in Hz
-
-        """
-        index = self._endpoint_index(converter_type, tile, block)
-        return self._stub.GetMixerFrequency(index).value
-
-    @ServiceHubCall(errormsg="Could not set mixer frequency")
-    def set_mixer_frequency(
-        self, converter_type: ConverterType, tile: int, block: int, frequency: float
-    ):
-        """
-        Set the mixer frequency.
-        The mixer frequency must be in the range `-Fs/2` to `Fs/2` where `Fs` is the sampling frequency.
-
-        :param converter_type:
-            The type; either "adc" or "dac"
-        :param tile:
-            The tile of the converter
-        :param block:
-            The block of the converter
-        :param frequency:
-            The frequency in Hz
-
-        :return: The mixer frequency of the DAC or ADC
-
-        """
-        index = self._endpoint_index(converter_type, tile, block)
-        self._stub.SetMixerFrequency(proto.Frequency(value=frequency, index=index))
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/sequencer.py` & `qiclib-1.1.0/src/qiclib/hardware/sequencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,29 @@
     platform_attribute,
     platform_attribute_collector,
 )
 
 from qiclib.packages.servicehub import ServiceHubCall
 
 import qiclib.packages.grpc.sequencer_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.sequencer_pb2_grpc as grpc_stub
 
 
 from qiclib.coding.sequencercode import SequencerCodeBase
 
 
 class _SequencerRegisters:
     def __init__(self, endpoint: int, stub: grpc_stub.SequencerServiceStub):
         self._endpoint = endpoint
         self._stub = stub
 
     def get_all(self):
         """Returns a list with all 32bit unsigned int register values."""
-        return self._stub.GetAllRegisters(
-            proto.EndpointIndex(value=self._endpoint)
-        ).list
+        return self._stub.GetAllRegisters(dt.EndpointIndex(value=self._endpoint)).list
 
     def __getitem__(self, index):
         self._check_index(index)
         register_index = proto.RegisterIndex(endpoint=self._endpoint, index=index)
         return self._stub.GetRegister(register_index).value
 
     def __setitem__(self, index, value):
@@ -69,15 +68,15 @@
 
     def __init__(
         self, name: str, connection, controller, qkit_instrument=True, index=0
     ):
         super().__init__(name, connection, controller, qkit_instrument)
         self._stub = grpc_stub.SequencerServiceStub(self._conn.channel)
         self._index = index
-        self._component = proto.EndpointIndex(value=self._index)
+        self._component = dt.EndpointIndex(value=self._index)
         self._registers = _SequencerRegisters(self._index, self._stub)
         self._program_description = "Nothing loaded"
 
     @property
     def register(self):
         """The 32 registers of the Sequencer."""
         return self._registers
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/servicehub.py` & `qiclib-1.1.0/src/qiclib/hardware/servicehub.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 The ServiceHub Control Interface is a standardized interface to query which
 functionalities are available within the current platform.
 """
 from typing import List
 from qiclib.hardware.platform_component import PlatformComponent
 
 from qiclib.packages.servicehub import ServiceHubCall
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.servicehubcontrol_pb2 as proto
 import qiclib.packages.grpc.servicehubcontrol_pb2_grpc as grpc_stub
 
 
 class ServiceHub(PlatformComponent):
     """ServiceHub Control Interface
 
@@ -45,23 +46,31 @@
         self._info = self._get_version()
 
     @ServiceHubCall(
         errormsg="Could not read ServiceHub information. "
         "Please make sure that your connection is working!"
     )
     def _get_version(self):
-        return self._stub.GetServiceHubVersion(proto.Empty())
+        return self._stub.GetServiceHubVersion(dt.Empty())
 
     @property
     @ServiceHubCall(errormsg="Could not get list of loaded ServiceHub plugins")
     def plugin_list(self) -> List[str]:
         """A list of all loaded ServiceHub plugins."""
-        return self._stub.GetPluginList(proto.Empty()).str
+        return self._stub.GetPluginList(dt.Empty()).str
 
     @property
     def taskrunner_available(self) -> bool:
         """If the Taskrunner is available on the connected platform."""
         return "TaskRunnerPlugin" in self.plugin_list
 
     def reboot(self):
         """Reboots the whole platform."""
-        self._stub.Reboot(proto.Empty())
+        self._stub.Reboot(dt.Empty())
+
+    def get_endpoints_of_plugin(self, plugin: str) -> List[str]:
+        return list(self._stub.GetEndpointsOfPlugin(proto.String(str=plugin)).str)
+
+    def get_endpoint_index_from_plugin(self, plugin: str, endpoint: str) -> int:
+        return self._stub.GetEndpointIndexOfPlugin(
+            proto.EndpointIndexRequest(plugin_name=plugin, endpoint_name=endpoint)
+        ).val
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/storage.py` & `qiclib-1.1.0/src/qiclib/hardware/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Contains the Driver to control a Storage Module on the Hardware Platform.."""
 from qiclib.hardware.platform_component import PlatformComponent
 
 from qiclib.packages.servicehub import ServiceHubCall
 import qiclib.packages.grpc.qic_storage_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.qic_storage_pb2_grpc as grpc_stub
 
 
 class Storage(PlatformComponent):
     """Driver to control a Storage Module on the Hardware Platform."""
 
     def __init__(
@@ -31,15 +32,15 @@
         controller,
         qkit_instrument=True,
         index=0,
     ):
         super().__init__(name, connection, controller, qkit_instrument)
         self._stub = grpc_stub.StorageStub(self._conn.channel)
         self._index = index
-        self._component = proto.EndpointIndex(value=self._index)
+        self._component = dt.EndpointIndex(value=self._index)
 
         self._bram = [
             _StorageBRAM(
                 f"{self.name} Memory #{i}",
                 self._conn,
                 self._qip,
                 qkit_instrument=False,
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/taskrunner.py` & `qiclib-1.1.0/src/qiclib/hardware/taskrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     platform_attribute,
     platform_attribute_collector,
 )
 from qiclib.experiment.rtos_tasks import get_task_source
 
 from qiclib.packages.servicehub import ServiceHubCall
 import qiclib.packages.grpc.taskrunner_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.taskrunner_pb2_grpc as grpc_stub
 
 
 @platform_attribute_collector
 class TaskRunner(PlatformComponent):
     """Driver to control the Taskrunner on the Hardware Platform."""
 
@@ -48,76 +49,76 @@
     @property
     @platform_attribute
     @ServiceHubCall(
         errormsg="Could not fetch the current firmware hash of the Taskrunner"
     )
     def firmware_hash(self):
         """The hash of the current firmware running on the realtime core."""
-        return self._stub.GetStatus(proto.Empty()).firmware_hash
+        return self._stub.GetStatus(dt.Empty()).firmware_hash
 
     @property
     @platform_attribute
     @ServiceHubCall(
         errormsg="Could not determine the build date of the Taskrunner firmware"
     )
     def firmware_build_date(self):
         """Returns the build date of the Taskrunner firmware."""
-        return self._stub.GetStatus(proto.Empty()).build_date
+        return self._stub.GetStatus(dt.Empty()).build_date
 
     @property
     @platform_attribute
     @ServiceHubCall(
         errormsg="Could not determine the build commit of the Taskrunner firmware"
     )
     def firmware_build_commit(self):
         """Returns the build commit hash of the Taskrunner firmware."""
-        return self._stub.GetStatus(proto.Empty()).build_commit
+        return self._stub.GetStatus(dt.Empty()).build_commit
 
     @property
     @platform_attribute
     @ServiceHubCall(errormsg="Could not determine the status of the taskrunner")
     def loaded_task(self):
         """The name of the currently loaded task."""
-        return self._stub.GetStatus(proto.Empty()).task_name
+        return self._stub.GetStatus(dt.Empty()).task_name
 
     @property
     @ServiceHubCall(errormsg="Could not determine the progress of the task")
     def task_progress(self):
         """Returns the progress of the task"""
-        return self._stub.GetStatus(proto.Empty()).task_progress
+        return self._stub.GetStatus(dt.Empty()).task_progress
 
     @property
     @ServiceHubCall(errormsg="Could not determine number of available databoxes")
     def databoxes_available(self):
         """Returns the number of available databoxes."""
-        return self._stub.GetStatus(proto.Empty()).databoxes_available
+        return self._stub.GetStatus(dt.Empty()).databoxes_available
 
     @property
     @ServiceHubCall(errormsg="Could not determine state of the taskrunner")
     def busy(self):
         """Returns if the taskrunner is currently busy."""
-        return self._stub.GetTaskState(proto.Empty()).busy
+        return self._stub.GetTaskState(dt.Empty()).busy
 
     @property
     @ServiceHubCall(errormsg="Could not determine if task has finished")
     def task_done(self):
         """Returns if the task has finished."""
-        return self._stub.GetTaskState(proto.Empty()).done
+        return self._stub.GetTaskState(dt.Empty()).done
 
     @property
     @ServiceHubCall(errormsg="Could not determine if task has error messages")
     def task_errormsg_available(self):
         """Returns if task has error messages."""
-        return self._stub.GetTaskState(proto.Empty()).error_msg_available
+        return self._stub.GetTaskState(dt.Empty()).error_msg_available
 
     @property
     @ServiceHubCall(errormsg="Could not determine if error message queue is full")
     def task_errormsg_queue_full(self):
         """Returns if if error message queue is full."""
-        return self._stub.GetTaskState(proto.Empty()).error_msg_queue_full
+        return self._stub.GetTaskState(dt.Empty()).error_msg_queue_full
 
     @ServiceHubCall(errormsg="Failed to start task")
     def start_task(self, loop=False, overwrite=False):
         """Starts the execution of a previously loaded task.
 
         :param loop: bool, optional
             if the task should be executed in a loop, by default False
@@ -234,15 +235,15 @@
             TaskRunner.DataMode.UINT64: self._stub.GetDataboxesUINT64,
         }.get(mode, None)
         if method_call is None:
             raise ValueError("Data mode is unknown! Only use DataMode Enum values.")
 
         databoxes: List[List[Any]] = []
         last_index = -1
-        for databox_reply in method_call(proto.Empty()):
+        for databox_reply in method_call(dt.Empty()):
             # print databox_reply.index, databox_reply.data[:]
             if last_index != databox_reply.index:
                 # Create new (empty) databox in list
                 databoxes.append([])
                 last_index = databox_reply.index
             # Fill the latest databox with content
             databoxes[-1].extend(databox_reply.data[:])
@@ -316,15 +317,15 @@
         Data is interpreted as 64bit unsigned integer values which are returned as array.
         """
         return self.get_databoxes_with_mode(TaskRunner.DataMode.UINT64, require_done)
 
     @ServiceHubCall
     def get_error_messages(self):
         """Retrieves all error messages from the task"""
-        reply = self._stub.GetTaskErrorMessages(proto.Empty())
+        reply = self._stub.GetTaskErrorMessages(dt.Empty())
         return reply.message[:]
 
     def check_task_errors(self):
         errors = self.get_error_messages()
         if errors:
             raise RuntimeError(
                 "The following error messages were retrieved "
```

### Comparing `qiclib-1.0.0/src/qiclib/hardware/unitcell.py` & `qiclib-1.1.0/src/qiclib/hardware/unitcell.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,20 +60,22 @@
 
 import numpy as np
 
 from qiclib.hardware.platform_component import PlatformComponent
 
 from qiclib.packages.servicehub import ServiceHubCall
 import qiclib.packages.grpc.qic_unitcell_pb2 as proto
+import qiclib.packages.grpc.datatypes_pb2 as dt
 import qiclib.packages.grpc.qic_unitcell_pb2_grpc as grpc_stub
 
 from qiclib.hardware.sequencer import Sequencer
 from qiclib.hardware.pulsegen import PulseGen
 from qiclib.hardware.recording import Recording
 from qiclib.hardware.storage import Storage
+from qiclib.hardware.digital_trigger import DigitalTrigger
 
 if TYPE_CHECKING:
     from qiclib.hardware.controller import QiController
 
 
 class UnitCell:
     """A single digital unit cell containing its internal modules as properties.
@@ -89,15 +91,15 @@
 
         qic = QiController("ip-address")
         qic.cell[5].busy # if the 6th digital unit cell in the QiController is busy
         qic.cell[3].sequencer.start_at(0) # start the sequencer in the 4th cell
 
     """
 
-    def __init__(self, index: int, cells: "UnitCells", info: proto.CellInfo):
+    def __init__(self, index: int, cells: "UnitCells", info: proto.CellInfo):  # type: ignore
         self._index = index
         self._cells = cells
         controller: QiController = cells._qip
         connection = controller._conn
 
         self._sequencer = Sequencer(
             f"Cell {index} Sequencer", connection, controller, index=info.sequencer
@@ -111,14 +113,20 @@
         )
         self._recording = Recording(
             f"Cell {index} Recording", connection, controller, index=info.recording
         )
         self._storage = Storage(
             f"Cell {index} Storage", connection, controller, index=info.storage
         )
+        self._digital_trigger = DigitalTrigger(
+            f"Cell {index} Digital Trigger",
+            connection,
+            controller,
+            index=info.digital_trigger,
+        )
 
     @property
     def sequencer(self) -> Sequencer:
         """Sequencer of this digital unit cell.
 
         It controls and orchestrates the execution of the other modules within the cell
         with nanosecond precision.
@@ -154,14 +162,22 @@
         """Data storage of this digital unit cell.
 
         It contains the data which was obtained and persisted during an experiment.
         """
         return self._storage
 
     @property
+    def digital_trigger(self) -> DigitalTrigger:
+        """Digital trigger capabilities of this digital unit cell.
+
+        Enables manual trigger and trigger-set overrides.
+        """
+        return self._digital_trigger
+
+    @property
     def busy(self) -> bool:
         """If the cell is currently busy.
 
         This returns true if any of the internal modules is currently busy.
         """
         return self._index in self._cells.busy_cells
 
@@ -191,15 +207,15 @@
         super().__init__(name, connection, controller, qkit_instrument)
         self._stub = grpc_stub.UnitCellServiceStub(self._conn.channel)
         self._cells: List[UnitCell] = []
         self._update_cells()
 
     @ServiceHubCall(errormsg="Could not obtain digital unit cell information.")
     def _update_cells(self):
-        info = self._stub.GetAllCellInfo(proto.Empty())
+        info = self._stub.GetAllCellInfo(dt.Empty())
         self._cells = []
         for i, cell in enumerate(info.cells):
             self._cells.append(UnitCell(i, self, cell))
 
     def __getitem__(self, key):
         return self._cells[int(key)]
 
@@ -261,26 +277,26 @@
         for cell in self._cells:
             cell.sequencer.stop()
 
     @property
     @ServiceHubCall
     def busy(self) -> bool:
         """If any of the digital unit cells is currently busy."""
-        return self._stub.GetBusyCells(proto.Empty()).busy
+        return self._stub.GetBusyCells(dt.Empty()).busy
 
     @property
     @ServiceHubCall
     def busy_cells(self) -> List[int]:
         """A list with the indices of all digital unit cells that are currently busy."""
-        return self._stub.GetBusyCells(proto.Empty()).cells
+        return self._stub.GetBusyCells(dt.Empty()).cells
 
     @ServiceHubCall
     def check_status(self, raise_exceptions=True):
         """Check if a converter reported an error and if so, forward it to the user."""
-        response = self._stub.GetConverterStatus(proto.Empty())
+        response = self._stub.GetConverterStatus(dt.Empty())
         status_report = response.report
         status_ok = not response.error
 
         if not status_ok:
             self.clear_status_report()
             status_report = (
                 "The converters reported the following issue(s):\n" + status_report
@@ -290,20 +306,20 @@
             sys.stderr.write(status_report)
 
         return status_ok
 
     @ServiceHubCall
     def get_status_report(self) -> str:
         """Retrieve a status report from the converters."""
-        return self._stub.GetConverterStatus(proto.Empty()).report
+        return self._stub.GetConverterStatus(dt.Empty()).report
 
     @ServiceHubCall
     def clear_status_report(self):
         """Resets the status report so old error messages will be discarded."""
-        self._stub.ClearConverterStatus(proto.Empty())
+        self._stub.ClearConverterStatus(dt.Empty())
 
     @ServiceHubCall
     def run_experiment(
         self,
         averages: int,
         cells: List[int],
         recordings: List[int],
```

### Comparing `qiclib-1.0.0/src/qiclib/measurement/__init__.py` & `qiclib-1.1.0/src/qiclib/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/measurement/iq_fit.py` & `qiclib-1.1.0/src/qiclib/measurement/iq_fit.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/measurement/iq_plot.py` & `qiclib-1.1.0/src/qiclib/measurement/iq_plot.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/measurement/measure_iq.py` & `qiclib-1.1.0/src/qiclib/measurement/measure_iq.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/__init__.py` & `qiclib-1.1.0/src/qiclib/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/constants.py` & `qiclib-1.1.0/src/qiclib/packages/constants.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/__init__.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/pimc_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/sequencer_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,142 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: pimc.proto
+# source: sequencer.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\npimc.proto\x12\x04pimc"N\n\tBoardInfo\x12\x0e\n\x06\x63oreId\x18\x01 \x01(\r\x12\x1e\n\x07project\x18\x02 \x01(\x0b\x32\r.pimc.Project\x12\x11\n\tbuildTime\x18\x03 \x01(\t"G\n\x07Project\x12\x11\n\tprojectId\x18\x01 \x01(\r\x12\x12\n\nplatformId\x18\x02 \x01(\r\x12\x15\n\rbuildRevision\x18\x03 \x01(\r";\n\nPIMCStatus\x12\x10\n\x08rst_done\x18\x01 \x01(\x08\x12\r\n\x05ready\x18\x02 \x01(\x08\x12\x0c\n\x04\x62usy\x18\x03 \x01(\x08"\xbc\x01\n\x04Info\x12\x0e\n\x06pimcId\x18\x01 \x01(\r\x12\x13\n\x0bpimcVersion\x18\x02 \x01(\r\x12\x11\n\tprojectId\x18\x03 \x01(\r\x12\x12\n\nplatformId\x18\x04 \x01(\r\x12\x15\n\rbuildRevision\x18\x05 \x01(\r\x12\x11\n\tbuildTime\x18\x06 \x01(\t\x12\x13\n\x0bprojectName\x18\x07 \x01(\t\x12\x14\n\x0cplatformName\x18\x08 \x01(\t\x12\x13\n\x0b\x62uildCommit\x18\t \x01(\t"\x15\n\x04\x42ool\x12\r\n\x05value\x18\x01 \x01(\x08"\x15\n\x04UInt\x12\r\n\x05value\x18\x01 \x01(\r"\x17\n\x06String\x12\r\n\x05value\x18\x01 \x01(\t"\x07\n\x05\x45mpty2\x80\x07\n\x0bPIMCService\x12&\n\x08SetReset\x12\x0b.pimc.Empty\x1a\x0b.pimc.Empty"\x00\x12$\n\x07GetBusy\x12\x0b.pimc.Empty\x1a\n.pimc.Bool"\x00\x12%\n\x08GetReady\x12\x0b.pimc.Empty\x1a\n.pimc.Bool"\x00\x12(\n\nSetSWReady\x12\x0b.pimc.Empty\x1a\x0b.pimc.Empty"\x00\x12\'\n\nGetSWReady\x12\x0b.pimc.Empty\x1a\n.pimc.Bool"\x00\x12*\n\x0cSetResetDone\x12\x0b.pimc.Empty\x1a\x0b.pimc.Empty"\x00\x12)\n\x0cGetResetDone\x12\x0b.pimc.Empty\x1a\n.pimc.Bool"\x00\x12+\n\x0eGetChipVersion\x12\x0b.pimc.Empty\x1a\n.pimc.UInt"\x00\x12\x31\n\x14GetModuleChipVersion\x12\x0b.pimc.Empty\x1a\n.pimc.UInt"\x00\x12$\n\x07GetInfo\x12\x0b.pimc.Empty\x1a\n.pimc.Info"\x00\x12,\n\rGetInfoString\x12\x0b.pimc.Empty\x1a\x0c.pimc.String"\x00\x12.\n\x11GetAllClocksValid\x12\x0b.pimc.Empty\x1a\n.pimc.Bool"\x00\x12,\n\rGetClocksInfo\x12\x0b.pimc.Empty\x1a\x0c.pimc.String"\x00\x12.\n\x0fGetStatusInputs\x12\x0b.pimc.Empty\x1a\x0c.pimc.String"\x00\x12+\n\x0cGetReadyMask\x12\x0b.pimc.Empty\x1a\x0c.pimc.String"\x00\x12,\n\rGetReadyState\x12\x0b.pimc.Empty\x1a\x0c.pimc.String"\x00\x12,\n\tGetStatus\x12\x0b.pimc.Empty\x1a\x10.pimc.PIMCStatus"\x00\x12*\n\nGetProject\x12\x0b.pimc.Empty\x1a\r.pimc.Project"\x00\x12+\n\x0cGetBuildTime\x12\x0b.pimc.Empty\x1a\x0c.pimc.String"\x00\x12.\n\x0cGetBoardInfo\x12\x0b.pimc.Empty\x1a\x0f.pimc.BoardInfo"\x00\x62\x06proto3'
+    b'\n\x0fsequencer.proto\x12\tsequencer\x1a\x0f\x64\x61tatypes.proto"E\n\x07\x41verage\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"N\n\rRegisterIndex\x12.\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05index\x18\x02 \x01(\r"B\n\x08Register\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.sequencer.RegisterIndex\x12\r\n\x05value\x18\x02 \x01(\r"\x1c\n\x0cRegisterList\x12\x0c\n\x04list\x18\x01 \x03(\r"L\n\x0eProgramCounter\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"_\n\x05\x44\x65lay\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x0b\n\x03reg\x18\x02 \x01(\r\x12\x0c\n\x04time\x18\x03 \x01(\x01\x12\x0e\n\x06\x63ycles\x18\x04 \x01(\r"a\n\x07Program\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x14\n\x0cprogram_data\x18\x02 \x03(\r\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t"d\n\x0cStatusReport\x12\x0c\n\x04\x62usy\x18\x01 \x01(\x08\x12\x0f\n\x07relaxed\x18\x02 \x01(\x08\x12\x14\n\x0cwait_on_sync\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\t\x12\x10\n\x08warnings\x18\x05 \x03(\t2\xf4\x08\n\x10SequencerService\x12>\n\x07GetBusy\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x13.sdr.datatypes.Bool"\x00\x12\x41\n\nGetRelaxed\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x13.sdr.datatypes.Bool"\x00\x12\x41\n\x0bGetAverages\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x12.sequencer.Average"\x00\x12\x39\n\x0bSetAverages\x12\x12.sequencer.Average\x1a\x14.sdr.datatypes.Empty"\x00\x12N\n\x11GetProgramCounter\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x19.sequencer.ProgramCounter"\x00\x12>\n\x0bGetRegister\x12\x18.sequencer.RegisterIndex\x1a\x13.sequencer.Register"\x00\x12:\n\x0bSetRegister\x12\x13.sequencer.Register\x1a\x14.sdr.datatypes.Empty"\x00\x12J\n\x0fGetAllRegisters\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x17.sequencer.RegisterList"\x00\x12\x34\n\x08SetDelay\x12\x10.sequencer.Delay\x1a\x14.sdr.datatypes.Empty"\x00\x12\x39\n\x0bLoadProgram\x12\x12.sequencer.Program\x1a\x14.sdr.datatypes.Empty"\x00\x12<\n\x07StartAt\x12\x19.sequencer.ProgramCounter\x1a\x14.sdr.datatypes.Empty"\x00\x12L\n\x0fGetStartAddress\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x19.sequencer.ProgramCounter"\x00\x12\x44\n\x0fSetStartAddress\x12\x19.sequencer.ProgramCounter\x1a\x14.sdr.datatypes.Empty"\x00\x12>\n\x06Resume\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12=\n\x05Reset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12<\n\x04Stop\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12G\n\x0cReportStatus\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x17.sequencer.StatusReport"\x00\x62\x06proto3'
 )
 
 
-_BOARDINFO = DESCRIPTOR.message_types_by_name["BoardInfo"]
-_PROJECT = DESCRIPTOR.message_types_by_name["Project"]
-_PIMCSTATUS = DESCRIPTOR.message_types_by_name["PIMCStatus"]
-_INFO = DESCRIPTOR.message_types_by_name["Info"]
-_BOOL = DESCRIPTOR.message_types_by_name["Bool"]
-_UINT = DESCRIPTOR.message_types_by_name["UInt"]
-_STRING = DESCRIPTOR.message_types_by_name["String"]
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
-BoardInfo = _reflection.GeneratedProtocolMessageType(
-    "BoardInfo",
+_AVERAGE = DESCRIPTOR.message_types_by_name["Average"]
+_REGISTERINDEX = DESCRIPTOR.message_types_by_name["RegisterIndex"]
+_REGISTER = DESCRIPTOR.message_types_by_name["Register"]
+_REGISTERLIST = DESCRIPTOR.message_types_by_name["RegisterList"]
+_PROGRAMCOUNTER = DESCRIPTOR.message_types_by_name["ProgramCounter"]
+_DELAY = DESCRIPTOR.message_types_by_name["Delay"]
+_PROGRAM = DESCRIPTOR.message_types_by_name["Program"]
+_STATUSREPORT = DESCRIPTOR.message_types_by_name["StatusReport"]
+Average = _reflection.GeneratedProtocolMessageType(
+    "Average",
     (_message.Message,),
     {
-        "DESCRIPTOR": _BOARDINFO,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.BoardInfo)
+        "DESCRIPTOR": _AVERAGE,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.Average)
     },
 )
-_sym_db.RegisterMessage(BoardInfo)
+_sym_db.RegisterMessage(Average)
 
-Project = _reflection.GeneratedProtocolMessageType(
-    "Project",
+RegisterIndex = _reflection.GeneratedProtocolMessageType(
+    "RegisterIndex",
     (_message.Message,),
     {
-        "DESCRIPTOR": _PROJECT,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.Project)
+        "DESCRIPTOR": _REGISTERINDEX,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.RegisterIndex)
     },
 )
-_sym_db.RegisterMessage(Project)
+_sym_db.RegisterMessage(RegisterIndex)
 
-PIMCStatus = _reflection.GeneratedProtocolMessageType(
-    "PIMCStatus",
+Register = _reflection.GeneratedProtocolMessageType(
+    "Register",
     (_message.Message,),
     {
-        "DESCRIPTOR": _PIMCSTATUS,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.PIMCStatus)
+        "DESCRIPTOR": _REGISTER,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.Register)
     },
 )
-_sym_db.RegisterMessage(PIMCStatus)
+_sym_db.RegisterMessage(Register)
 
-Info = _reflection.GeneratedProtocolMessageType(
-    "Info",
+RegisterList = _reflection.GeneratedProtocolMessageType(
+    "RegisterList",
     (_message.Message,),
     {
-        "DESCRIPTOR": _INFO,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.Info)
+        "DESCRIPTOR": _REGISTERLIST,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.RegisterList)
     },
 )
-_sym_db.RegisterMessage(Info)
+_sym_db.RegisterMessage(RegisterList)
 
-Bool = _reflection.GeneratedProtocolMessageType(
-    "Bool",
+ProgramCounter = _reflection.GeneratedProtocolMessageType(
+    "ProgramCounter",
     (_message.Message,),
     {
-        "DESCRIPTOR": _BOOL,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.Bool)
+        "DESCRIPTOR": _PROGRAMCOUNTER,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.ProgramCounter)
     },
 )
-_sym_db.RegisterMessage(Bool)
+_sym_db.RegisterMessage(ProgramCounter)
 
-UInt = _reflection.GeneratedProtocolMessageType(
-    "UInt",
+Delay = _reflection.GeneratedProtocolMessageType(
+    "Delay",
     (_message.Message,),
     {
-        "DESCRIPTOR": _UINT,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.UInt)
+        "DESCRIPTOR": _DELAY,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.Delay)
     },
 )
-_sym_db.RegisterMessage(UInt)
+_sym_db.RegisterMessage(Delay)
 
-String = _reflection.GeneratedProtocolMessageType(
-    "String",
+Program = _reflection.GeneratedProtocolMessageType(
+    "Program",
     (_message.Message,),
     {
-        "DESCRIPTOR": _STRING,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.String)
+        "DESCRIPTOR": _PROGRAM,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.Program)
     },
 )
-_sym_db.RegisterMessage(String)
+_sym_db.RegisterMessage(Program)
 
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
+StatusReport = _reflection.GeneratedProtocolMessageType(
+    "StatusReport",
     (_message.Message,),
     {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "pimc_pb2"
-        # @@protoc_insertion_point(class_scope:pimc.Empty)
+        "DESCRIPTOR": _STATUSREPORT,
+        "__module__": "sequencer_pb2"
+        # @@protoc_insertion_point(class_scope:sequencer.StatusReport)
     },
 )
-_sym_db.RegisterMessage(Empty)
+_sym_db.RegisterMessage(StatusReport)
 
-_PIMCSERVICE = DESCRIPTOR.services_by_name["PIMCService"]
+_SEQUENCERSERVICE = DESCRIPTOR.services_by_name["SequencerService"]
 if _descriptor._USE_C_DESCRIPTORS == False:
+
     DESCRIPTOR._options = None
-    _BOARDINFO._serialized_start = 20
-    _BOARDINFO._serialized_end = 98
-    _PROJECT._serialized_start = 100
-    _PROJECT._serialized_end = 171
-    _PIMCSTATUS._serialized_start = 173
-    _PIMCSTATUS._serialized_end = 232
-    _INFO._serialized_start = 235
-    _INFO._serialized_end = 423
-    _BOOL._serialized_start = 425
-    _BOOL._serialized_end = 446
-    _UINT._serialized_start = 448
-    _UINT._serialized_end = 469
-    _STRING._serialized_start = 471
-    _STRING._serialized_end = 494
-    _EMPTY._serialized_start = 496
-    _EMPTY._serialized_end = 503
-    _PIMCSERVICE._serialized_start = 506
-    _PIMCSERVICE._serialized_end = 1402
+    _AVERAGE._serialized_start = 47
+    _AVERAGE._serialized_end = 116
+    _REGISTERINDEX._serialized_start = 118
+    _REGISTERINDEX._serialized_end = 196
+    _REGISTER._serialized_start = 198
+    _REGISTER._serialized_end = 264
+    _REGISTERLIST._serialized_start = 266
+    _REGISTERLIST._serialized_end = 294
+    _PROGRAMCOUNTER._serialized_start = 296
+    _PROGRAMCOUNTER._serialized_end = 372
+    _DELAY._serialized_start = 374
+    _DELAY._serialized_end = 469
+    _PROGRAM._serialized_start = 471
+    _PROGRAM._serialized_end = 568
+    _STATUSREPORT._serialized_start = 570
+    _STATUSREPORT._serialized_end = 670
+    _SEQUENCERSERVICE._serialized_start = 673
+    _SEQUENCERSERVICE._serialized_end = 1813
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/pimc_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/pulsegen_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1069 +1,888 @@
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import pimc_pb2 as pimc__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.pulsegen_pb2 as pulsegen__pb2
 
 
-class PIMCServiceStub(object):
+class PulseGenServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.SetReset = channel.unary_unary(
-            "/pimc.PIMCService/SetReset",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Empty.FromString,
-        )
-        self.GetBusy = channel.unary_unary(
-            "/pimc.PIMCService/GetBusy",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Bool.FromString,
-        )
-        self.GetReady = channel.unary_unary(
-            "/pimc.PIMCService/GetReady",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Bool.FromString,
-        )
-        self.SetSWReady = channel.unary_unary(
-            "/pimc.PIMCService/SetSWReady",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Empty.FromString,
-        )
-        self.GetSWReady = channel.unary_unary(
-            "/pimc.PIMCService/GetSWReady",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Bool.FromString,
-        )
-        self.SetResetDone = channel.unary_unary(
-            "/pimc.PIMCService/SetResetDone",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Empty.FromString,
-        )
-        self.GetResetDone = channel.unary_unary(
-            "/pimc.PIMCService/GetResetDone",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Bool.FromString,
-        )
-        self.GetChipVersion = channel.unary_unary(
-            "/pimc.PIMCService/GetChipVersion",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.UInt.FromString,
-        )
-        self.GetModuleChipVersion = channel.unary_unary(
-            "/pimc.PIMCService/GetModuleChipVersion",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.UInt.FromString,
-        )
-        self.GetInfo = channel.unary_unary(
-            "/pimc.PIMCService/GetInfo",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Info.FromString,
-        )
-        self.GetInfoString = channel.unary_unary(
-            "/pimc.PIMCService/GetInfoString",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.String.FromString,
-        )
-        self.GetAllClocksValid = channel.unary_unary(
-            "/pimc.PIMCService/GetAllClocksValid",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Bool.FromString,
-        )
-        self.GetClocksInfo = channel.unary_unary(
-            "/pimc.PIMCService/GetClocksInfo",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.String.FromString,
-        )
-        self.GetStatusInputs = channel.unary_unary(
-            "/pimc.PIMCService/GetStatusInputs",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.String.FromString,
-        )
-        self.GetReadyMask = channel.unary_unary(
-            "/pimc.PIMCService/GetReadyMask",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.String.FromString,
-        )
-        self.GetReadyState = channel.unary_unary(
-            "/pimc.PIMCService/GetReadyState",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.String.FromString,
-        )
-        self.GetStatus = channel.unary_unary(
-            "/pimc.PIMCService/GetStatus",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.PIMCStatus.FromString,
-        )
-        self.GetProject = channel.unary_unary(
-            "/pimc.PIMCService/GetProject",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.Project.FromString,
-        )
-        self.GetBuildTime = channel.unary_unary(
-            "/pimc.PIMCService/GetBuildTime",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.String.FromString,
-        )
-        self.GetBoardInfo = channel.unary_unary(
-            "/pimc.PIMCService/GetBoardInfo",
-            request_serializer=pimc__pb2.Empty.SerializeToString,
-            response_deserializer=pimc__pb2.BoardInfo.FromString,
+        self.GetNCOFrequency = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetNCOFrequency",
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=pulsegen__pb2.Frequency.FromString,
+        )
+        self.SetNCOFrequency = channel.unary_unary(
+            "/pulsegen.PulseGenService/SetNCOFrequency",
+            request_serializer=pulsegen__pb2.Frequency.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.Reset = channel.unary_unary(
+            "/pulsegen.PulseGenService/Reset",
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.ResetEnvelopeMemory = channel.unary_unary(
+            "/pulsegen.PulseGenService/ResetEnvelopeMemory",
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetAmplitudeCalibration = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetAmplitudeCalibration",
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=pulsegen__pb2.AmplitudeCalibration.FromString,
+        )
+        self.SetAmplitudeCalibration = channel.unary_unary(
+            "/pulsegen.PulseGenService/SetAmplitudeCalibration",
+            request_serializer=pulsegen__pb2.AmplitudeCalibration.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetPhaseOffset = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetPhaseOffset",
+            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
+            response_deserializer=pulsegen__pb2.PhaseOffset.FromString,
+        )
+        self.SetPhaseOffset = channel.unary_unary(
+            "/pulsegen.PulseGenService/SetPhaseOffset",
+            request_serializer=pulsegen__pb2.PhaseOffset.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetGlobalPhase = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetGlobalPhase",
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=pulsegen__pb2.PhaseOffset.FromString,
+        )
+        self.GetDuration = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetDuration",
+            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
+            response_deserializer=pulsegen__pb2.Duration.FromString,
+        )
+        self.SetDuration = channel.unary_unary(
+            "/pulsegen.PulseGenService/SetDuration",
+            request_serializer=pulsegen__pb2.Duration.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetStartAddressI = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetStartAddressI",
+            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
+            response_deserializer=pulsegen__pb2.Address.FromString,
+        )
+        self.SetStartAddressI = channel.unary_unary(
+            "/pulsegen.PulseGenService/SetStartAddressI",
+            request_serializer=pulsegen__pb2.Address.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetStartAddressQ = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetStartAddressQ",
+            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
+            response_deserializer=pulsegen__pb2.Address.FromString,
+        )
+        self.SetStartAddressQ = channel.unary_unary(
+            "/pulsegen.PulseGenService/SetStartAddressQ",
+            request_serializer=pulsegen__pb2.Address.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.TriggerManually = channel.unary_unary(
+            "/pulsegen.PulseGenService/TriggerManually",
+            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.LoadPulse = channel.unary_unary(
+            "/pulsegen.PulseGenService/LoadPulse",
+            request_serializer=pulsegen__pb2.Pulse.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetStatusFlags = channel.unary_unary(
+            "/pulsegen.PulseGenService/GetStatusFlags",
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=pulsegen__pb2.StatusFlags.FromString,
+        )
+        self.ResetStatusFlags = channel.unary_unary(
+            "/pulsegen.PulseGenService/ResetStatusFlags",
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
 
 
-class PIMCServiceServicer(object):
+class PulseGenServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def SetReset(self, request, context):
-        """*
-        @brief Issue reset in the firmware.
-
-        This reset is given to the IP cores within the FPGA side.
-        The cores need to be connected to PIMC rst out.
-        Some cores will go in an async state to its userspace/kernel driver
-        if the reset is issued. Thus not working as expected.
-
-        @param Empty
-        @return Empty
-        """
+    def GetNCOFrequency(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetBusy(self, request, context):
-        """*
-        @brief Read if system is busy.
-
-        @param Empty
-        @return Bool
-        """
+    def SetNCOFrequency(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetReady(self, request, context):
-        """*
-        @brief Read if the system is fully initialized and ready to be operated.
-
-        @param Empty
-        @return Bool
-        """
+    def Reset(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetSWReady(self, request, context):
-        """*
-        @brief Set the software ready flag of the platform.
-
-        @param Empty
-        @return Empty
-        """
+    def ResetEnvelopeMemory(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetSWReady(self, request, context):
-        """*
-        @brief Read the software ready flag from the platform.
-
-        @param Empty
-        @return Bool
-        """
+    def GetAmplitudeCalibration(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetResetDone(self, request, context):
-        """*
-        @brief Set the reset done flag of the platform.
-
-        @param Empty
-        @return Empty
-        """
+    def SetAmplitudeCalibration(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetResetDone(self, request, context):
-        """*
-        @brief Read the reset done flag from the platform.
-
-        @param Empty
-        @return Bool
-        """
+    def GetPhaseOffset(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetChipVersion(self, request, context):
-        """*
-        @brief Returns Chip version of PIMC core.
-
-        The ID Should be 0xFFFF, the version is iterated
-        if major things are changed.
-
-        @param Empty
-        @return UInt
-        """
+    def SetPhaseOffset(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetModuleChipVersion(self, request, context):
-        """*
-        @brief Returns version of the core module from the platform.
-
-        @param Empty
-        @return UInt
-        """
+    def GetGlobalPhase(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetInfo(self, request, context):
-        """*
-        @brief Returns struct containing pimcID, pimcVersion, projectID,
-        platformID, buildRevision and buildTime.
-
-        @param Empty
-        @return Info
-        """
+    def GetDuration(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetInfoString(self, request, context):
-        """*
-        @brief Returns all Info data.
-
-        @param Empty
-        @return String
-        """
+    def SetDuration(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetAllClocksValid(self, request, context):
-        """*
-        @brief Returns true if all clocks are in valid frequency range.
-
-        @param Empty
-        @return Bool
-        """
+    def GetStartAddressI(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetClocksInfo(self, request, context):
-        """*
-        @brief Returns String containing information about connected clocks.
-
-        @param Empty
-        @return String
-        """
+    def SetStartAddressI(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetStatusInputs(self, request, context):
-        """*
-        @brief Returns String representing 16bit StatusInputs.
-
-        @param Empty
-        @return String
-        """
+    def GetStartAddressQ(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetReadyMask(self, request, context):
-        """*
-        @brief Returns String representing 16bit ReadyMask.
-
-        @param Empty
-        @return String
-        """
+    def SetStartAddressQ(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetReadyState(self, request, context):
-        """*
-        @brief Returns String representing 16bit ReadyState.
-
-        @param Empty
-        @return String
-        """
+    def TriggerManually(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetStatus(self, request, context):
-        """*
-        @brief Returns the status of the platform.
-
-        The user can check if the platform is ready by reading the flag.
-        The ready state is defined within the PIMC core.
-
-        @param Empty
-        @return PIMCStatus
-        """
+    def LoadPulse(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetProject(self, request, context):
-        """*
-        @brief \deprecated Returns Project containing projectId, platformId and
-        buildRevision.
-
-        With this function one can test if the correct/expected
-        FPGA firmware is running on the device. Using the device
-        with a different image will cause unexpected behavior or even
-        damage the board.
-
-        @param Empty
-        @return Project
-        """
+    def GetStatusFlags(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetBuildTime(self, request, context):
-        """*
-        @brief \deprecated Returns buildTime in string format.
-
-        The returned build time tells when the synthesis was started.
-        This is only related to the FPGA firmware.
-
-        @param Empty
-        @return string
-        """
+    def ResetStatusFlags(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetBoardInfo(self, request, context):
-        """*
-        @brief \deprecated Returns BoardInfo containing coreId, the Project and
-        BuildTime.
-
-        @param Empty
-        @return BoardInfo
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
 
-
-def add_PIMCServiceServicer_to_server(servicer, server):
+def add_PulseGenServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "SetReset": grpc.unary_unary_rpc_method_handler(
-            servicer.SetReset,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Empty.SerializeToString,
-        ),
-        "GetBusy": grpc.unary_unary_rpc_method_handler(
-            servicer.GetBusy,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Bool.SerializeToString,
-        ),
-        "GetReady": grpc.unary_unary_rpc_method_handler(
-            servicer.GetReady,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Bool.SerializeToString,
-        ),
-        "SetSWReady": grpc.unary_unary_rpc_method_handler(
-            servicer.SetSWReady,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Empty.SerializeToString,
-        ),
-        "GetSWReady": grpc.unary_unary_rpc_method_handler(
-            servicer.GetSWReady,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Bool.SerializeToString,
-        ),
-        "SetResetDone": grpc.unary_unary_rpc_method_handler(
-            servicer.SetResetDone,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Empty.SerializeToString,
-        ),
-        "GetResetDone": grpc.unary_unary_rpc_method_handler(
-            servicer.GetResetDone,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Bool.SerializeToString,
-        ),
-        "GetChipVersion": grpc.unary_unary_rpc_method_handler(
-            servicer.GetChipVersion,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.UInt.SerializeToString,
-        ),
-        "GetModuleChipVersion": grpc.unary_unary_rpc_method_handler(
-            servicer.GetModuleChipVersion,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.UInt.SerializeToString,
-        ),
-        "GetInfo": grpc.unary_unary_rpc_method_handler(
-            servicer.GetInfo,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Info.SerializeToString,
-        ),
-        "GetInfoString": grpc.unary_unary_rpc_method_handler(
-            servicer.GetInfoString,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.String.SerializeToString,
-        ),
-        "GetAllClocksValid": grpc.unary_unary_rpc_method_handler(
-            servicer.GetAllClocksValid,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Bool.SerializeToString,
-        ),
-        "GetClocksInfo": grpc.unary_unary_rpc_method_handler(
-            servicer.GetClocksInfo,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.String.SerializeToString,
-        ),
-        "GetStatusInputs": grpc.unary_unary_rpc_method_handler(
-            servicer.GetStatusInputs,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.String.SerializeToString,
-        ),
-        "GetReadyMask": grpc.unary_unary_rpc_method_handler(
-            servicer.GetReadyMask,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.String.SerializeToString,
-        ),
-        "GetReadyState": grpc.unary_unary_rpc_method_handler(
-            servicer.GetReadyState,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.String.SerializeToString,
-        ),
-        "GetStatus": grpc.unary_unary_rpc_method_handler(
-            servicer.GetStatus,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.PIMCStatus.SerializeToString,
-        ),
-        "GetProject": grpc.unary_unary_rpc_method_handler(
-            servicer.GetProject,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.Project.SerializeToString,
-        ),
-        "GetBuildTime": grpc.unary_unary_rpc_method_handler(
-            servicer.GetBuildTime,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.String.SerializeToString,
-        ),
-        "GetBoardInfo": grpc.unary_unary_rpc_method_handler(
-            servicer.GetBoardInfo,
-            request_deserializer=pimc__pb2.Empty.FromString,
-            response_serializer=pimc__pb2.BoardInfo.SerializeToString,
+        "GetNCOFrequency": grpc.unary_unary_rpc_method_handler(
+            servicer.GetNCOFrequency,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=pulsegen__pb2.Frequency.SerializeToString,
+        ),
+        "SetNCOFrequency": grpc.unary_unary_rpc_method_handler(
+            servicer.SetNCOFrequency,
+            request_deserializer=pulsegen__pb2.Frequency.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "Reset": grpc.unary_unary_rpc_method_handler(
+            servicer.Reset,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "ResetEnvelopeMemory": grpc.unary_unary_rpc_method_handler(
+            servicer.ResetEnvelopeMemory,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetAmplitudeCalibration": grpc.unary_unary_rpc_method_handler(
+            servicer.GetAmplitudeCalibration,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=pulsegen__pb2.AmplitudeCalibration.SerializeToString,
+        ),
+        "SetAmplitudeCalibration": grpc.unary_unary_rpc_method_handler(
+            servicer.SetAmplitudeCalibration,
+            request_deserializer=pulsegen__pb2.AmplitudeCalibration.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetPhaseOffset": grpc.unary_unary_rpc_method_handler(
+            servicer.GetPhaseOffset,
+            request_deserializer=pulsegen__pb2.IndexSet.FromString,
+            response_serializer=pulsegen__pb2.PhaseOffset.SerializeToString,
+        ),
+        "SetPhaseOffset": grpc.unary_unary_rpc_method_handler(
+            servicer.SetPhaseOffset,
+            request_deserializer=pulsegen__pb2.PhaseOffset.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetGlobalPhase": grpc.unary_unary_rpc_method_handler(
+            servicer.GetGlobalPhase,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=pulsegen__pb2.PhaseOffset.SerializeToString,
+        ),
+        "GetDuration": grpc.unary_unary_rpc_method_handler(
+            servicer.GetDuration,
+            request_deserializer=pulsegen__pb2.IndexSet.FromString,
+            response_serializer=pulsegen__pb2.Duration.SerializeToString,
+        ),
+        "SetDuration": grpc.unary_unary_rpc_method_handler(
+            servicer.SetDuration,
+            request_deserializer=pulsegen__pb2.Duration.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetStartAddressI": grpc.unary_unary_rpc_method_handler(
+            servicer.GetStartAddressI,
+            request_deserializer=pulsegen__pb2.IndexSet.FromString,
+            response_serializer=pulsegen__pb2.Address.SerializeToString,
+        ),
+        "SetStartAddressI": grpc.unary_unary_rpc_method_handler(
+            servicer.SetStartAddressI,
+            request_deserializer=pulsegen__pb2.Address.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetStartAddressQ": grpc.unary_unary_rpc_method_handler(
+            servicer.GetStartAddressQ,
+            request_deserializer=pulsegen__pb2.IndexSet.FromString,
+            response_serializer=pulsegen__pb2.Address.SerializeToString,
+        ),
+        "SetStartAddressQ": grpc.unary_unary_rpc_method_handler(
+            servicer.SetStartAddressQ,
+            request_deserializer=pulsegen__pb2.Address.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "TriggerManually": grpc.unary_unary_rpc_method_handler(
+            servicer.TriggerManually,
+            request_deserializer=pulsegen__pb2.IndexSet.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "LoadPulse": grpc.unary_unary_rpc_method_handler(
+            servicer.LoadPulse,
+            request_deserializer=pulsegen__pb2.Pulse.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetStatusFlags": grpc.unary_unary_rpc_method_handler(
+            servicer.GetStatusFlags,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=pulsegen__pb2.StatusFlags.SerializeToString,
+        ),
+        "ResetStatusFlags": grpc.unary_unary_rpc_method_handler(
+            servicer.ResetStatusFlags,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pimc.PIMCService", rpc_method_handlers
+        "pulsegen.PulseGenService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class PIMCService(object):
+class PulseGenService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def SetReset(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            "/pimc.PIMCService/SetReset",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Empty.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def GetBusy(
+    def GetNCOFrequency(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetBusy",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Bool.FromString,
+            "/pulsegen.PulseGenService/GetNCOFrequency",
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            pulsegen__pb2.Frequency.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetReady(
+    def SetNCOFrequency(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetReady",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Bool.FromString,
+            "/pulsegen.PulseGenService/SetNCOFrequency",
+            pulsegen__pb2.Frequency.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetSWReady(
+    def Reset(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/SetSWReady",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Empty.FromString,
+            "/pulsegen.PulseGenService/Reset",
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetSWReady(
+    def ResetEnvelopeMemory(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetSWReady",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Bool.FromString,
+            "/pulsegen.PulseGenService/ResetEnvelopeMemory",
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetResetDone(
+    def GetAmplitudeCalibration(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/SetResetDone",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Empty.FromString,
+            "/pulsegen.PulseGenService/GetAmplitudeCalibration",
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            pulsegen__pb2.AmplitudeCalibration.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetResetDone(
+    def SetAmplitudeCalibration(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetResetDone",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Bool.FromString,
+            "/pulsegen.PulseGenService/SetAmplitudeCalibration",
+            pulsegen__pb2.AmplitudeCalibration.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetChipVersion(
+    def GetPhaseOffset(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetChipVersion",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.UInt.FromString,
+            "/pulsegen.PulseGenService/GetPhaseOffset",
+            pulsegen__pb2.IndexSet.SerializeToString,
+            pulsegen__pb2.PhaseOffset.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetModuleChipVersion(
+    def SetPhaseOffset(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetModuleChipVersion",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.UInt.FromString,
+            "/pulsegen.PulseGenService/SetPhaseOffset",
+            pulsegen__pb2.PhaseOffset.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetInfo(
+    def GetGlobalPhase(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetInfo",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Info.FromString,
+            "/pulsegen.PulseGenService/GetGlobalPhase",
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            pulsegen__pb2.PhaseOffset.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetInfoString(
+    def GetDuration(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetInfoString",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.String.FromString,
+            "/pulsegen.PulseGenService/GetDuration",
+            pulsegen__pb2.IndexSet.SerializeToString,
+            pulsegen__pb2.Duration.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetAllClocksValid(
+    def SetDuration(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetAllClocksValid",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Bool.FromString,
+            "/pulsegen.PulseGenService/SetDuration",
+            pulsegen__pb2.Duration.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetClocksInfo(
+    def GetStartAddressI(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetClocksInfo",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.String.FromString,
+            "/pulsegen.PulseGenService/GetStartAddressI",
+            pulsegen__pb2.IndexSet.SerializeToString,
+            pulsegen__pb2.Address.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetStatusInputs(
+    def SetStartAddressI(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetStatusInputs",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.String.FromString,
+            "/pulsegen.PulseGenService/SetStartAddressI",
+            pulsegen__pb2.Address.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetReadyMask(
+    def GetStartAddressQ(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetReadyMask",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.String.FromString,
+            "/pulsegen.PulseGenService/GetStartAddressQ",
+            pulsegen__pb2.IndexSet.SerializeToString,
+            pulsegen__pb2.Address.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetReadyState(
+    def SetStartAddressQ(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetReadyState",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.String.FromString,
+            "/pulsegen.PulseGenService/SetStartAddressQ",
+            pulsegen__pb2.Address.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetStatus(
+    def TriggerManually(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetStatus",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.PIMCStatus.FromString,
+            "/pulsegen.PulseGenService/TriggerManually",
+            pulsegen__pb2.IndexSet.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetProject(
+    def LoadPulse(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetProject",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.Project.FromString,
+            "/pulsegen.PulseGenService/LoadPulse",
+            pulsegen__pb2.Pulse.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetBuildTime(
+    def GetStatusFlags(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetBuildTime",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.String.FromString,
+            "/pulsegen.PulseGenService/GetStatusFlags",
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            pulsegen__pb2.StatusFlags.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetBoardInfo(
+    def ResetStatusFlags(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pimc.PIMCService/GetBoardInfo",
-            pimc__pb2.Empty.SerializeToString,
-            pimc__pb2.BoardInfo.FromString,
+            "/pulsegen.PulseGenService/ResetStatusFlags",
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/pulsegen_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/pimc_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,902 +1,1055 @@
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import pulsegen_pb2 as pulsegen__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.pimc_pb2 as pimc__pb2
 
 
-class PulseGenServiceStub(object):
-    """import "MultiModuleCommon.proto";"""
+class PIMCServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.GetNCOFrequency = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetNCOFrequency",
-            request_serializer=pulsegen__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=pulsegen__pb2.Frequency.FromString,
-        )
-        self.SetNCOFrequency = channel.unary_unary(
-            "/pulsegen.PulseGenService/SetNCOFrequency",
-            request_serializer=pulsegen__pb2.Frequency.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.Reset = channel.unary_unary(
-            "/pulsegen.PulseGenService/Reset",
-            request_serializer=pulsegen__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.ResetEnvelopeMemory = channel.unary_unary(
-            "/pulsegen.PulseGenService/ResetEnvelopeMemory",
-            request_serializer=pulsegen__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.GetAmplitudeCalibration = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetAmplitudeCalibration",
-            request_serializer=pulsegen__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=pulsegen__pb2.AmplitudeCalibration.FromString,
-        )
-        self.SetAmplitudeCalibration = channel.unary_unary(
-            "/pulsegen.PulseGenService/SetAmplitudeCalibration",
-            request_serializer=pulsegen__pb2.AmplitudeCalibration.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.GetPhaseOffset = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetPhaseOffset",
-            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
-            response_deserializer=pulsegen__pb2.PhaseOffset.FromString,
-        )
-        self.SetPhaseOffset = channel.unary_unary(
-            "/pulsegen.PulseGenService/SetPhaseOffset",
-            request_serializer=pulsegen__pb2.PhaseOffset.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.GetGlobalPhase = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetGlobalPhase",
-            request_serializer=pulsegen__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=pulsegen__pb2.PhaseOffset.FromString,
-        )
-        self.GetDuration = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetDuration",
-            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
-            response_deserializer=pulsegen__pb2.Duration.FromString,
-        )
-        self.SetDuration = channel.unary_unary(
-            "/pulsegen.PulseGenService/SetDuration",
-            request_serializer=pulsegen__pb2.Duration.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.GetStartAddressI = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetStartAddressI",
-            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
-            response_deserializer=pulsegen__pb2.Address.FromString,
-        )
-        self.SetStartAddressI = channel.unary_unary(
-            "/pulsegen.PulseGenService/SetStartAddressI",
-            request_serializer=pulsegen__pb2.Address.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.GetStartAddressQ = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetStartAddressQ",
-            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
-            response_deserializer=pulsegen__pb2.Address.FromString,
-        )
-        self.SetStartAddressQ = channel.unary_unary(
-            "/pulsegen.PulseGenService/SetStartAddressQ",
-            request_serializer=pulsegen__pb2.Address.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.TriggerManually = channel.unary_unary(
-            "/pulsegen.PulseGenService/TriggerManually",
-            request_serializer=pulsegen__pb2.IndexSet.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.LoadPulse = channel.unary_unary(
-            "/pulsegen.PulseGenService/LoadPulse",
-            request_serializer=pulsegen__pb2.Pulse.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
-        self.GetStatusFlags = channel.unary_unary(
-            "/pulsegen.PulseGenService/GetStatusFlags",
-            request_serializer=pulsegen__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=pulsegen__pb2.StatusFlags.FromString,
-        )
-        self.ResetStatusFlags = channel.unary_unary(
-            "/pulsegen.PulseGenService/ResetStatusFlags",
-            request_serializer=pulsegen__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=pulsegen__pb2.Empty.FromString,
-        )
+        self.SetReset = channel.unary_unary(
+            "/pimc.PIMCService/SetReset",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetBusy = channel.unary_unary(
+            "/pimc.PIMCService/GetBusy",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Bool.FromString,
+        )
+        self.GetReady = channel.unary_unary(
+            "/pimc.PIMCService/GetReady",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Bool.FromString,
+        )
+        self.SetSWReady = channel.unary_unary(
+            "/pimc.PIMCService/SetSWReady",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetSWReady = channel.unary_unary(
+            "/pimc.PIMCService/GetSWReady",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Bool.FromString,
+        )
+        self.SetResetDone = channel.unary_unary(
+            "/pimc.PIMCService/SetResetDone",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
+        )
+        self.GetResetDone = channel.unary_unary(
+            "/pimc.PIMCService/GetResetDone",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Bool.FromString,
+        )
+        self.GetChipVersion = channel.unary_unary(
+            "/pimc.PIMCService/GetChipVersion",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.UInt.FromString,
+        )
+        self.GetModuleChipVersion = channel.unary_unary(
+            "/pimc.PIMCService/GetModuleChipVersion",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.UInt.FromString,
+        )
+        self.GetInfo = channel.unary_unary(
+            "/pimc.PIMCService/GetInfo",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=pimc__pb2.Info.FromString,
+        )
+        self.GetInfoString = channel.unary_unary(
+            "/pimc.PIMCService/GetInfoString",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.String.FromString,
+        )
+        self.GetAllClocksValid = channel.unary_unary(
+            "/pimc.PIMCService/GetAllClocksValid",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Bool.FromString,
+        )
+        self.GetClocksInfo = channel.unary_unary(
+            "/pimc.PIMCService/GetClocksInfo",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.String.FromString,
+        )
+        self.GetStatusInputs = channel.unary_unary(
+            "/pimc.PIMCService/GetStatusInputs",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.String.FromString,
+        )
+        self.GetReadyMask = channel.unary_unary(
+            "/pimc.PIMCService/GetReadyMask",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.String.FromString,
+        )
+        self.GetReadyState = channel.unary_unary(
+            "/pimc.PIMCService/GetReadyState",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.String.FromString,
+        )
+        self.GetStatus = channel.unary_unary(
+            "/pimc.PIMCService/GetStatus",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=pimc__pb2.PIMCStatus.FromString,
+        )
+        self.GetProject = channel.unary_unary(
+            "/pimc.PIMCService/GetProject",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=pimc__pb2.Project.FromString,
+        )
+        self.GetBuildTime = channel.unary_unary(
+            "/pimc.PIMCService/GetBuildTime",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.String.FromString,
+        )
+        self.GetBoardInfo = channel.unary_unary(
+            "/pimc.PIMCService/GetBoardInfo",
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=pimc__pb2.BoardInfo.FromString,
+        )
+
+
+class PIMCServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def SetReset(self, request, context):
+        """*
+        @brief Issue reset in the firmware.
+
+        This reset is given to the IP cores within the FPGA side.
+        The cores need to be connected to PIMC rst out.
+        Some cores will go in an async state to its userspace/kernel driver
+        if the reset is issued. Thus not working as expected.
 
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Empty
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
-class PulseGenServiceServicer(object):
-    """import "MultiModuleCommon.proto";"""
+    def GetBusy(self, request, context):
+        """*
+        @brief Read if system is busy.
 
-    def GetNCOFrequency(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Bool
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetNCOFrequency(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetReady(self, request, context):
+        """*
+        @brief Read if the system is fully initialized and ready to be operated.
+
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Bool
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def Reset(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def SetSWReady(self, request, context):
+        """*
+        @brief Set the software ready flag of the platform.
+
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Empty
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def ResetEnvelopeMemory(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetSWReady(self, request, context):
+        """*
+        @brief Read the software ready flag from the platform.
+
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Bool
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetAmplitudeCalibration(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def SetResetDone(self, request, context):
+        """*
+        @brief Set the reset done flag of the platform.
+
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Empty
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetAmplitudeCalibration(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetResetDone(self, request, context):
+        """*
+        @brief Read the reset done flag from the platform.
+
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Bool
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetPhaseOffset(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetChipVersion(self, request, context):
+        """*
+        @brief Returns Chip version of PIMC core.
+
+        The ID Should be 0xFFFF, the version is iterated
+        if major things are changed.
+
+        @param sdr.datatypes.Empty
+        @return UInt
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetPhaseOffset(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetModuleChipVersion(self, request, context):
+        """*
+        @brief Returns version of the core module from the platform.
+
+        @param sdr.datatypes.Empty
+        @return UInt
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetGlobalPhase(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetInfo(self, request, context):
+        """*
+        @brief Returns struct containing pimcID, pimcVersion, projectID,
+        platformID, buildRevision and buildTime.
+
+        @param sdr.datatypes.Empty
+        @return Info
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetDuration(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetInfoString(self, request, context):
+        """*
+        @brief Returns all Info data.
+
+        @param sdr.datatypes.Empty
+        @return String
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetDuration(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetAllClocksValid(self, request, context):
+        """*
+        @brief Returns true if all clocks are in valid frequency range.
+
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Bool
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetStartAddressI(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetClocksInfo(self, request, context):
+        """*
+        @brief Returns String containing information about connected clocks.
+
+        @param sdr.datatypes.Empty
+        @return String
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetStartAddressI(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetStatusInputs(self, request, context):
+        """*
+        @brief Returns String representing 16bit StatusInputs.
+
+        @param sdr.datatypes.Empty
+        @return String
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetStartAddressQ(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetReadyMask(self, request, context):
+        """*
+        @brief Returns String representing 16bit ReadyMask.
+
+        @param sdr.datatypes.Empty
+        @return String
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SetStartAddressQ(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetReadyState(self, request, context):
+        """*
+        @brief Returns String representing 16bit ReadyState.
+
+        @param sdr.datatypes.Empty
+        @return String
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def TriggerManually(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetStatus(self, request, context):
+        """*
+        @brief Returns the status of the platform.
+
+        The user can check if the platform is ready by reading the flag.
+        The ready state is defined within the PIMC core.
+
+        @param sdr.datatypes.Empty
+        @return PIMCStatus
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def LoadPulse(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetProject(self, request, context):
+        """*
+        @brief \deprecated Returns Project containing projectId, platformId and
+        buildRevision.
+
+        With this function one can test if the correct/expected
+        FPGA firmware is running on the device. Using the device
+        with a different image will cause unexpected behavior or even
+        damage the board.
+
+        @param sdr.datatypes.Empty
+        @return Project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def GetStatusFlags(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetBuildTime(self, request, context):
+        """*
+        @brief \deprecated Returns buildTime in string format.
+
+        The returned build time tells when the synthesis was started.
+        This is only related to the FPGA firmware.
+
+        @param sdr.datatypes.Empty
+        @return string
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def ResetStatusFlags(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetBoardInfo(self, request, context):
+        """*
+        @brief \deprecated Returns BoardInfo containing coreId, the Project and
+        BuildTime.
+
+        @param sdr.datatypes.Empty
+        @return BoardInfo
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_PulseGenServiceServicer_to_server(servicer, server):
+def add_PIMCServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "GetNCOFrequency": grpc.unary_unary_rpc_method_handler(
-            servicer.GetNCOFrequency,
-            request_deserializer=pulsegen__pb2.EndpointIndex.FromString,
-            response_serializer=pulsegen__pb2.Frequency.SerializeToString,
-        ),
-        "SetNCOFrequency": grpc.unary_unary_rpc_method_handler(
-            servicer.SetNCOFrequency,
-            request_deserializer=pulsegen__pb2.Frequency.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "Reset": grpc.unary_unary_rpc_method_handler(
-            servicer.Reset,
-            request_deserializer=pulsegen__pb2.EndpointIndex.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "ResetEnvelopeMemory": grpc.unary_unary_rpc_method_handler(
-            servicer.ResetEnvelopeMemory,
-            request_deserializer=pulsegen__pb2.EndpointIndex.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "GetAmplitudeCalibration": grpc.unary_unary_rpc_method_handler(
-            servicer.GetAmplitudeCalibration,
-            request_deserializer=pulsegen__pb2.EndpointIndex.FromString,
-            response_serializer=pulsegen__pb2.AmplitudeCalibration.SerializeToString,
-        ),
-        "SetAmplitudeCalibration": grpc.unary_unary_rpc_method_handler(
-            servicer.SetAmplitudeCalibration,
-            request_deserializer=pulsegen__pb2.AmplitudeCalibration.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "GetPhaseOffset": grpc.unary_unary_rpc_method_handler(
-            servicer.GetPhaseOffset,
-            request_deserializer=pulsegen__pb2.IndexSet.FromString,
-            response_serializer=pulsegen__pb2.PhaseOffset.SerializeToString,
-        ),
-        "SetPhaseOffset": grpc.unary_unary_rpc_method_handler(
-            servicer.SetPhaseOffset,
-            request_deserializer=pulsegen__pb2.PhaseOffset.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "GetGlobalPhase": grpc.unary_unary_rpc_method_handler(
-            servicer.GetGlobalPhase,
-            request_deserializer=pulsegen__pb2.EndpointIndex.FromString,
-            response_serializer=pulsegen__pb2.PhaseOffset.SerializeToString,
-        ),
-        "GetDuration": grpc.unary_unary_rpc_method_handler(
-            servicer.GetDuration,
-            request_deserializer=pulsegen__pb2.IndexSet.FromString,
-            response_serializer=pulsegen__pb2.Duration.SerializeToString,
-        ),
-        "SetDuration": grpc.unary_unary_rpc_method_handler(
-            servicer.SetDuration,
-            request_deserializer=pulsegen__pb2.Duration.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "GetStartAddressI": grpc.unary_unary_rpc_method_handler(
-            servicer.GetStartAddressI,
-            request_deserializer=pulsegen__pb2.IndexSet.FromString,
-            response_serializer=pulsegen__pb2.Address.SerializeToString,
-        ),
-        "SetStartAddressI": grpc.unary_unary_rpc_method_handler(
-            servicer.SetStartAddressI,
-            request_deserializer=pulsegen__pb2.Address.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "GetStartAddressQ": grpc.unary_unary_rpc_method_handler(
-            servicer.GetStartAddressQ,
-            request_deserializer=pulsegen__pb2.IndexSet.FromString,
-            response_serializer=pulsegen__pb2.Address.SerializeToString,
-        ),
-        "SetStartAddressQ": grpc.unary_unary_rpc_method_handler(
-            servicer.SetStartAddressQ,
-            request_deserializer=pulsegen__pb2.Address.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "TriggerManually": grpc.unary_unary_rpc_method_handler(
-            servicer.TriggerManually,
-            request_deserializer=pulsegen__pb2.IndexSet.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "LoadPulse": grpc.unary_unary_rpc_method_handler(
-            servicer.LoadPulse,
-            request_deserializer=pulsegen__pb2.Pulse.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
-        ),
-        "GetStatusFlags": grpc.unary_unary_rpc_method_handler(
-            servicer.GetStatusFlags,
-            request_deserializer=pulsegen__pb2.EndpointIndex.FromString,
-            response_serializer=pulsegen__pb2.StatusFlags.SerializeToString,
-        ),
-        "ResetStatusFlags": grpc.unary_unary_rpc_method_handler(
-            servicer.ResetStatusFlags,
-            request_deserializer=pulsegen__pb2.EndpointIndex.FromString,
-            response_serializer=pulsegen__pb2.Empty.SerializeToString,
+        "SetReset": grpc.unary_unary_rpc_method_handler(
+            servicer.SetReset,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetBusy": grpc.unary_unary_rpc_method_handler(
+            servicer.GetBusy,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Bool.SerializeToString,
+        ),
+        "GetReady": grpc.unary_unary_rpc_method_handler(
+            servicer.GetReady,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Bool.SerializeToString,
+        ),
+        "SetSWReady": grpc.unary_unary_rpc_method_handler(
+            servicer.SetSWReady,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetSWReady": grpc.unary_unary_rpc_method_handler(
+            servicer.GetSWReady,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Bool.SerializeToString,
+        ),
+        "SetResetDone": grpc.unary_unary_rpc_method_handler(
+            servicer.SetResetDone,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
+        ),
+        "GetResetDone": grpc.unary_unary_rpc_method_handler(
+            servicer.GetResetDone,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Bool.SerializeToString,
+        ),
+        "GetChipVersion": grpc.unary_unary_rpc_method_handler(
+            servicer.GetChipVersion,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.UInt.SerializeToString,
+        ),
+        "GetModuleChipVersion": grpc.unary_unary_rpc_method_handler(
+            servicer.GetModuleChipVersion,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.UInt.SerializeToString,
+        ),
+        "GetInfo": grpc.unary_unary_rpc_method_handler(
+            servicer.GetInfo,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=pimc__pb2.Info.SerializeToString,
+        ),
+        "GetInfoString": grpc.unary_unary_rpc_method_handler(
+            servicer.GetInfoString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.String.SerializeToString,
+        ),
+        "GetAllClocksValid": grpc.unary_unary_rpc_method_handler(
+            servicer.GetAllClocksValid,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Bool.SerializeToString,
+        ),
+        "GetClocksInfo": grpc.unary_unary_rpc_method_handler(
+            servicer.GetClocksInfo,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.String.SerializeToString,
+        ),
+        "GetStatusInputs": grpc.unary_unary_rpc_method_handler(
+            servicer.GetStatusInputs,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.String.SerializeToString,
+        ),
+        "GetReadyMask": grpc.unary_unary_rpc_method_handler(
+            servicer.GetReadyMask,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.String.SerializeToString,
+        ),
+        "GetReadyState": grpc.unary_unary_rpc_method_handler(
+            servicer.GetReadyState,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.String.SerializeToString,
+        ),
+        "GetStatus": grpc.unary_unary_rpc_method_handler(
+            servicer.GetStatus,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=pimc__pb2.PIMCStatus.SerializeToString,
+        ),
+        "GetProject": grpc.unary_unary_rpc_method_handler(
+            servicer.GetProject,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=pimc__pb2.Project.SerializeToString,
+        ),
+        "GetBuildTime": grpc.unary_unary_rpc_method_handler(
+            servicer.GetBuildTime,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.String.SerializeToString,
+        ),
+        "GetBoardInfo": grpc.unary_unary_rpc_method_handler(
+            servicer.GetBoardInfo,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=pimc__pb2.BoardInfo.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pulsegen.PulseGenService", rpc_method_handlers
+        "pimc.PIMCService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class PulseGenService(object):
-    """import "MultiModuleCommon.proto";"""
+class PIMCService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def SetReset(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/pimc.PIMCService/SetReset",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
 
     @staticmethod
-    def GetNCOFrequency(
+    def GetBusy(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetNCOFrequency",
-            pulsegen__pb2.EndpointIndex.SerializeToString,
-            pulsegen__pb2.Frequency.FromString,
+            "/pimc.PIMCService/GetBusy",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Bool.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetNCOFrequency(
+    def GetReady(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/SetNCOFrequency",
-            pulsegen__pb2.Frequency.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetReady",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Bool.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def Reset(
+    def SetSWReady(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/Reset",
-            pulsegen__pb2.EndpointIndex.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/SetSWReady",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def ResetEnvelopeMemory(
+    def GetSWReady(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/ResetEnvelopeMemory",
-            pulsegen__pb2.EndpointIndex.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetSWReady",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Bool.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetAmplitudeCalibration(
+    def SetResetDone(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetAmplitudeCalibration",
-            pulsegen__pb2.EndpointIndex.SerializeToString,
-            pulsegen__pb2.AmplitudeCalibration.FromString,
+            "/pimc.PIMCService/SetResetDone",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetAmplitudeCalibration(
+    def GetResetDone(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/SetAmplitudeCalibration",
-            pulsegen__pb2.AmplitudeCalibration.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetResetDone",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Bool.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetPhaseOffset(
+    def GetChipVersion(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetPhaseOffset",
-            pulsegen__pb2.IndexSet.SerializeToString,
-            pulsegen__pb2.PhaseOffset.FromString,
+            "/pimc.PIMCService/GetChipVersion",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.UInt.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetPhaseOffset(
+    def GetModuleChipVersion(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/SetPhaseOffset",
-            pulsegen__pb2.PhaseOffset.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetModuleChipVersion",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.UInt.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetGlobalPhase(
+    def GetInfo(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetGlobalPhase",
-            pulsegen__pb2.EndpointIndex.SerializeToString,
-            pulsegen__pb2.PhaseOffset.FromString,
+            "/pimc.PIMCService/GetInfo",
+            datatypes__pb2.Empty.SerializeToString,
+            pimc__pb2.Info.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetDuration(
+    def GetInfoString(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetDuration",
-            pulsegen__pb2.IndexSet.SerializeToString,
-            pulsegen__pb2.Duration.FromString,
+            "/pimc.PIMCService/GetInfoString",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.String.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetDuration(
+    def GetAllClocksValid(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/SetDuration",
-            pulsegen__pb2.Duration.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetAllClocksValid",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Bool.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetStartAddressI(
+    def GetClocksInfo(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetStartAddressI",
-            pulsegen__pb2.IndexSet.SerializeToString,
-            pulsegen__pb2.Address.FromString,
+            "/pimc.PIMCService/GetClocksInfo",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.String.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetStartAddressI(
+    def GetStatusInputs(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/SetStartAddressI",
-            pulsegen__pb2.Address.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetStatusInputs",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.String.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetStartAddressQ(
+    def GetReadyMask(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetStartAddressQ",
-            pulsegen__pb2.IndexSet.SerializeToString,
-            pulsegen__pb2.Address.FromString,
+            "/pimc.PIMCService/GetReadyMask",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.String.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SetStartAddressQ(
+    def GetReadyState(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/SetStartAddressQ",
-            pulsegen__pb2.Address.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetReadyState",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.String.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def TriggerManually(
+    def GetStatus(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/TriggerManually",
-            pulsegen__pb2.IndexSet.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetStatus",
+            datatypes__pb2.Empty.SerializeToString,
+            pimc__pb2.PIMCStatus.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def LoadPulse(
+    def GetProject(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/LoadPulse",
-            pulsegen__pb2.Pulse.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetProject",
+            datatypes__pb2.Empty.SerializeToString,
+            pimc__pb2.Project.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def GetStatusFlags(
+    def GetBuildTime(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/GetStatusFlags",
-            pulsegen__pb2.EndpointIndex.SerializeToString,
-            pulsegen__pb2.StatusFlags.FromString,
+            "/pimc.PIMCService/GetBuildTime",
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.String.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def ResetStatusFlags(
+    def GetBoardInfo(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pulsegen.PulseGenService/ResetStatusFlags",
-            pulsegen__pb2.EndpointIndex.SerializeToString,
-            pulsegen__pb2.Empty.FromString,
+            "/pimc.PIMCService/GetBoardInfo",
+            datatypes__pb2.Empty.SerializeToString,
+            pimc__pb2.BoardInfo.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/qic_storage_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/qic_storage_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,44 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: qic_storage.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x11qic_storage.proto\x12\x0bqic_storage"\x1e\n\rEndpointIndex\x12\r\n\x05value\x18\x01 \x01(\r"\x86\x01\n\rStateHandling\x12)\n\x05index\x18\x01 \x01(\x0b\x32\x1a.qic_storage.EndpointIndex\x12\r\n\x05store\x18\x02 \x01(\x08\x12\x12\n\naccumulate\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65stination\x18\x04 \x01(\r\x12\x12\n\ndense_mode\x18\x05 \x01(\x08">\n\x11StateAccumulation\x12\x13\n\x0b\x61\x63\x63u_states\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63u_counter\x18\x02 \x01(\r"_\n\x0eResultHandling\x12)\n\x05index\x18\x01 \x01(\x0b\x32\x1a.qic_storage.EndpointIndex\x12\r\n\x05store\x18\x02 \x01(\x08\x12\x13\n\x0b\x64\x65stination\x18\x03 \x01(\r"a\n\x10\x41veragedHandling\x12)\n\x05index\x18\x01 \x01(\x0b\x32\x1a.qic_storage.EndpointIndex\x12\r\n\x05store\x18\x02 \x01(\x08\x12\x13\n\x0b\x64\x65stination\x18\x03 \x01(\r"c\n\x0b\x42ramControl\x12)\n\x05index\x18\x01 \x01(\x0b\x32\x1a.qic_storage.EndpointIndex\x12\r\n\x05reset\x18\x02 \x01(\x08\x12\x0c\n\x04wrap\x18\x03 \x01(\x08\x12\x0c\n\x04\x62ram\x18\x04 \x01(\r"Q\n\nBramStatus\x12\x0c\n\x04\x66ull\x18\x01 \x01(\x08\x12\r\n\x05\x65mpty\x18\x02 \x01(\x08\x12\x10\n\x08overflow\x18\x03 \x01(\x08\x12\x14\n\x0cnext_address\x18\x04 \x01(\r"D\n\tBramIndex\x12)\n\x05index\x18\x01 \x01(\x0b\x32\x1a.qic_storage.EndpointIndex\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"0\n\nResultData\x12\x10\n\x08result_i\x18\x01 \x03(\x05\x12\x10\n\x08result_q\x18\x02 \x03(\x05" \n\x0c\x41veragedData\x12\x10\n\x08\x61veraged\x18\x01 \x03(\x05"\x1a\n\tStateData\x12\r\n\x05state\x18\x01 \x03(\r",\n\x0e\x42ramDataUInt32\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\r\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"+\n\rBramDataInt32\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x05\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"(\n\nLatestData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x05\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"\x7f\n\x08\x44\x61taLost\x12\x15\n\rsingle_result\x18\x01 \x01(\x08\x12\x1a\n\x12state_accumulation\x18\x02 \x01(\x08\x12\x13\n\x0bqubit_state\x18\x03 \x01(\x08\x12\x17\n\x0f\x61veraged_result\x18\x04 \x01(\x08\x12\x12\n\nbram_input\x18\x05 \x01(\x08"\x07\n\x05\x45mpty2\xb2\n\n\x07Storage\x12\x39\n\x05Reset\x12\x1a.qic_storage.EndpointIndex\x1a\x12.qic_storage.Empty"\x00\x12\x44\n\x10SetStateHandling\x12\x1a.qic_storage.StateHandling\x1a\x12.qic_storage.Empty"\x00\x12L\n\x10GetStateHandling\x12\x1a.qic_storage.EndpointIndex\x1a\x1a.qic_storage.StateHandling"\x00\x12T\n\x14GetStateAccumulation\x12\x1a.qic_storage.EndpointIndex\x1a\x1e.qic_storage.StateAccumulation"\x00\x12\x46\n\x11SetResultHandling\x12\x1b.qic_storage.ResultHandling\x1a\x12.qic_storage.Empty"\x00\x12N\n\x11GetResultHandling\x12\x1a.qic_storage.EndpointIndex\x1a\x1b.qic_storage.ResultHandling"\x00\x12J\n\x13SetAveragedHandling\x12\x1d.qic_storage.AveragedHandling\x1a\x12.qic_storage.Empty"\x00\x12R\n\x13GetAveragedHandling\x12\x1a.qic_storage.EndpointIndex\x1a\x1d.qic_storage.AveragedHandling"\x00\x12@\n\x0eSetBramControl\x12\x18.qic_storage.BramControl\x1a\x12.qic_storage.Empty"\x00\x12\x42\n\rGetBramStatus\x12\x16.qic_storage.BramIndex\x1a\x17.qic_storage.BramStatus"\x00\x12=\n\rResetBramData\x12\x16.qic_storage.BramIndex\x1a\x12.qic_storage.Empty"\x00\x12J\n\x11GetBramResultData\x12\x1a.qic_storage.EndpointIndex\x1a\x17.qic_storage.ResultData"\x00\x12N\n\x13GetBramAveragedData\x12\x1a.qic_storage.EndpointIndex\x1a\x19.qic_storage.AveragedData"\x00\x12H\n\x10GetBramStateData\x12\x1a.qic_storage.EndpointIndex\x1a\x16.qic_storage.StateData"\x00\x12J\n\x11GetBramDataUInt32\x12\x16.qic_storage.BramIndex\x1a\x1b.qic_storage.BramDataUInt32"\x00\x12H\n\x10GetBramDataInt32\x12\x16.qic_storage.BramIndex\x1a\x1a.qic_storage.BramDataInt32"\x00\x12\x46\n\x11GetBramLatestData\x12\x16.qic_storage.BramIndex\x1a\x17.qic_storage.LatestData"\x00\x12\x41\n\nIsDataLost\x12\x1a.qic_storage.EndpointIndex\x1a\x15.qic_storage.DataLost"\x00\x62\x06proto3'
+    b'\n\x11qic_storage.proto\x12\x0bqic_storage\x1a\x0f\x64\x61tatypes.proto"\x88\x01\n\rStateHandling\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05store\x18\x02 \x01(\x08\x12\x12\n\naccumulate\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65stination\x18\x04 \x01(\r\x12\x12\n\ndense_mode\x18\x05 \x01(\x08">\n\x11StateAccumulation\x12\x13\n\x0b\x61\x63\x63u_states\x18\x01 \x01(\r\x12\x14\n\x0c\x61\x63\x63u_counter\x18\x02 \x01(\r"a\n\x0eResultHandling\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05store\x18\x02 \x01(\x08\x12\x13\n\x0b\x64\x65stination\x18\x03 \x01(\r"c\n\x10\x41veragedHandling\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05store\x18\x02 \x01(\x08\x12\x13\n\x0b\x64\x65stination\x18\x03 \x01(\r"e\n\x0b\x42ramControl\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05reset\x18\x02 \x01(\x08\x12\x0c\n\x04wrap\x18\x03 \x01(\x08\x12\x0c\n\x04\x62ram\x18\x04 \x01(\r"Q\n\nBramStatus\x12\x0c\n\x04\x66ull\x18\x01 \x01(\x08\x12\r\n\x05\x65mpty\x18\x02 \x01(\x08\x12\x10\n\x08overflow\x18\x03 \x01(\x08\x12\x14\n\x0cnext_address\x18\x04 \x01(\r"F\n\tBramIndex\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"0\n\nResultData\x12\x10\n\x08result_i\x18\x01 \x03(\x05\x12\x10\n\x08result_q\x18\x02 \x03(\x05" \n\x0c\x41veragedData\x12\x10\n\x08\x61veraged\x18\x01 \x03(\x05"\x1a\n\tStateData\x12\r\n\x05state\x18\x01 \x03(\r",\n\x0e\x42ramDataUInt32\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\r\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"+\n\rBramDataInt32\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x05\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"(\n\nLatestData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x05\x12\x0c\n\x04\x62ram\x18\x02 \x01(\r"\x7f\n\x08\x44\x61taLost\x12\x15\n\rsingle_result\x18\x01 \x01(\x08\x12\x1a\n\x12state_accumulation\x18\x02 \x01(\x08\x12\x13\n\x0bqubit_state\x18\x03 \x01(\x08\x12\x17\n\x0f\x61veraged_result\x18\x04 \x01(\x08\x12\x12\n\nbram_input\x18\x05 \x01(\x08\x32\xd0\n\n\x07Storage\x12=\n\x05Reset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12\x46\n\x10SetStateHandling\x12\x1a.qic_storage.StateHandling\x1a\x14.sdr.datatypes.Empty"\x00\x12N\n\x10GetStateHandling\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1a.qic_storage.StateHandling"\x00\x12V\n\x14GetStateAccumulation\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1e.qic_storage.StateAccumulation"\x00\x12H\n\x11SetResultHandling\x12\x1b.qic_storage.ResultHandling\x1a\x14.sdr.datatypes.Empty"\x00\x12P\n\x11GetResultHandling\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1b.qic_storage.ResultHandling"\x00\x12L\n\x13SetAveragedHandling\x12\x1d.qic_storage.AveragedHandling\x1a\x14.sdr.datatypes.Empty"\x00\x12T\n\x13GetAveragedHandling\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1d.qic_storage.AveragedHandling"\x00\x12\x42\n\x0eSetBramControl\x12\x18.qic_storage.BramControl\x1a\x14.sdr.datatypes.Empty"\x00\x12\x42\n\rGetBramStatus\x12\x16.qic_storage.BramIndex\x1a\x17.qic_storage.BramStatus"\x00\x12?\n\rResetBramData\x12\x16.qic_storage.BramIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12L\n\x11GetBramResultData\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x17.qic_storage.ResultData"\x00\x12P\n\x13GetBramAveragedData\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x19.qic_storage.AveragedData"\x00\x12J\n\x10GetBramStateData\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x16.qic_storage.StateData"\x00\x12J\n\x11GetBramDataUInt32\x12\x16.qic_storage.BramIndex\x1a\x1b.qic_storage.BramDataUInt32"\x00\x12H\n\x10GetBramDataInt32\x12\x16.qic_storage.BramIndex\x1a\x1a.qic_storage.BramDataInt32"\x00\x12\x46\n\x11GetBramLatestData\x12\x16.qic_storage.BramIndex\x1a\x17.qic_storage.LatestData"\x00\x12\x43\n\nIsDataLost\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x15.qic_storage.DataLost"\x00\x62\x06proto3'
 )
 
 
-_ENDPOINTINDEX = DESCRIPTOR.message_types_by_name["EndpointIndex"]
 _STATEHANDLING = DESCRIPTOR.message_types_by_name["StateHandling"]
 _STATEACCUMULATION = DESCRIPTOR.message_types_by_name["StateAccumulation"]
 _RESULTHANDLING = DESCRIPTOR.message_types_by_name["ResultHandling"]
 _AVERAGEDHANDLING = DESCRIPTOR.message_types_by_name["AveragedHandling"]
 _BRAMCONTROL = DESCRIPTOR.message_types_by_name["BramControl"]
 _BRAMSTATUS = DESCRIPTOR.message_types_by_name["BramStatus"]
 _BRAMINDEX = DESCRIPTOR.message_types_by_name["BramIndex"]
 _RESULTDATA = DESCRIPTOR.message_types_by_name["ResultData"]
 _AVERAGEDDATA = DESCRIPTOR.message_types_by_name["AveragedData"]
 _STATEDATA = DESCRIPTOR.message_types_by_name["StateData"]
 _BRAMDATAUINT32 = DESCRIPTOR.message_types_by_name["BramDataUInt32"]
 _BRAMDATAINT32 = DESCRIPTOR.message_types_by_name["BramDataInt32"]
 _LATESTDATA = DESCRIPTOR.message_types_by_name["LatestData"]
 _DATALOST = DESCRIPTOR.message_types_by_name["DataLost"]
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
-EndpointIndex = _reflection.GeneratedProtocolMessageType(
-    "EndpointIndex",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _ENDPOINTINDEX,
-        "__module__": "qic_storage_pb2"
-        # @@protoc_insertion_point(class_scope:qic_storage.EndpointIndex)
-    },
-)
-_sym_db.RegisterMessage(EndpointIndex)
-
 StateHandling = _reflection.GeneratedProtocolMessageType(
     "StateHandling",
     (_message.Message,),
     {
         "DESCRIPTOR": _STATEHANDLING,
         "__module__": "qic_storage_pb2"
         # @@protoc_insertion_point(class_scope:qic_storage.StateHandling)
@@ -210,56 +185,42 @@
         "DESCRIPTOR": _DATALOST,
         "__module__": "qic_storage_pb2"
         # @@protoc_insertion_point(class_scope:qic_storage.DataLost)
     },
 )
 _sym_db.RegisterMessage(DataLost)
 
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "qic_storage_pb2"
-        # @@protoc_insertion_point(class_scope:qic_storage.Empty)
-    },
-)
-_sym_db.RegisterMessage(Empty)
-
 _STORAGE = DESCRIPTOR.services_by_name["Storage"]
 if _descriptor._USE_C_DESCRIPTORS == False:
+
     DESCRIPTOR._options = None
-    _ENDPOINTINDEX._serialized_start = 34
-    _ENDPOINTINDEX._serialized_end = 64
-    _STATEHANDLING._serialized_start = 67
-    _STATEHANDLING._serialized_end = 201
-    _STATEACCUMULATION._serialized_start = 203
-    _STATEACCUMULATION._serialized_end = 265
-    _RESULTHANDLING._serialized_start = 267
-    _RESULTHANDLING._serialized_end = 362
-    _AVERAGEDHANDLING._serialized_start = 364
-    _AVERAGEDHANDLING._serialized_end = 461
-    _BRAMCONTROL._serialized_start = 463
-    _BRAMCONTROL._serialized_end = 562
-    _BRAMSTATUS._serialized_start = 564
-    _BRAMSTATUS._serialized_end = 645
-    _BRAMINDEX._serialized_start = 647
-    _BRAMINDEX._serialized_end = 715
-    _RESULTDATA._serialized_start = 717
-    _RESULTDATA._serialized_end = 765
-    _AVERAGEDDATA._serialized_start = 767
-    _AVERAGEDDATA._serialized_end = 799
-    _STATEDATA._serialized_start = 801
-    _STATEDATA._serialized_end = 827
-    _BRAMDATAUINT32._serialized_start = 829
-    _BRAMDATAUINT32._serialized_end = 873
-    _BRAMDATAINT32._serialized_start = 875
-    _BRAMDATAINT32._serialized_end = 918
-    _LATESTDATA._serialized_start = 920
-    _LATESTDATA._serialized_end = 960
-    _DATALOST._serialized_start = 962
-    _DATALOST._serialized_end = 1089
-    _EMPTY._serialized_start = 1091
-    _EMPTY._serialized_end = 1098
-    _STORAGE._serialized_start = 1101
-    _STORAGE._serialized_end = 2431
+    _STATEHANDLING._serialized_start = 52
+    _STATEHANDLING._serialized_end = 188
+    _STATEACCUMULATION._serialized_start = 190
+    _STATEACCUMULATION._serialized_end = 252
+    _RESULTHANDLING._serialized_start = 254
+    _RESULTHANDLING._serialized_end = 351
+    _AVERAGEDHANDLING._serialized_start = 353
+    _AVERAGEDHANDLING._serialized_end = 452
+    _BRAMCONTROL._serialized_start = 454
+    _BRAMCONTROL._serialized_end = 555
+    _BRAMSTATUS._serialized_start = 557
+    _BRAMSTATUS._serialized_end = 638
+    _BRAMINDEX._serialized_start = 640
+    _BRAMINDEX._serialized_end = 710
+    _RESULTDATA._serialized_start = 712
+    _RESULTDATA._serialized_end = 760
+    _AVERAGEDDATA._serialized_start = 762
+    _AVERAGEDDATA._serialized_end = 794
+    _STATEDATA._serialized_start = 796
+    _STATEDATA._serialized_end = 822
+    _BRAMDATAUINT32._serialized_start = 824
+    _BRAMDATAUINT32._serialized_end = 868
+    _BRAMDATAINT32._serialized_start = 870
+    _BRAMDATAINT32._serialized_end = 913
+    _LATESTDATA._serialized_start = 915
+    _LATESTDATA._serialized_end = 955
+    _DATALOST._serialized_start = 957
+    _DATALOST._serialized_end = 1084
+    _STORAGE._serialized_start = 1087
+    _STORAGE._serialized_end = 2447
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/qic_storage_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/qic_storage_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,92 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import qic_storage_pb2 as qic__storage__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.qic_storage_pb2 as qic__storage__pb2
 
 
 class StorageStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Reset = channel.unary_unary(
             "/qic_storage.Storage/Reset",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=qic__storage__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.SetStateHandling = channel.unary_unary(
             "/qic_storage.Storage/SetStateHandling",
             request_serializer=qic__storage__pb2.StateHandling.SerializeToString,
-            response_deserializer=qic__storage__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetStateHandling = channel.unary_unary(
             "/qic_storage.Storage/GetStateHandling",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.StateHandling.FromString,
         )
         self.GetStateAccumulation = channel.unary_unary(
             "/qic_storage.Storage/GetStateAccumulation",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.StateAccumulation.FromString,
         )
         self.SetResultHandling = channel.unary_unary(
             "/qic_storage.Storage/SetResultHandling",
             request_serializer=qic__storage__pb2.ResultHandling.SerializeToString,
-            response_deserializer=qic__storage__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetResultHandling = channel.unary_unary(
             "/qic_storage.Storage/GetResultHandling",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.ResultHandling.FromString,
         )
         self.SetAveragedHandling = channel.unary_unary(
             "/qic_storage.Storage/SetAveragedHandling",
             request_serializer=qic__storage__pb2.AveragedHandling.SerializeToString,
-            response_deserializer=qic__storage__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetAveragedHandling = channel.unary_unary(
             "/qic_storage.Storage/GetAveragedHandling",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.AveragedHandling.FromString,
         )
         self.SetBramControl = channel.unary_unary(
             "/qic_storage.Storage/SetBramControl",
             request_serializer=qic__storage__pb2.BramControl.SerializeToString,
-            response_deserializer=qic__storage__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetBramStatus = channel.unary_unary(
             "/qic_storage.Storage/GetBramStatus",
             request_serializer=qic__storage__pb2.BramIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.BramStatus.FromString,
         )
         self.ResetBramData = channel.unary_unary(
             "/qic_storage.Storage/ResetBramData",
             request_serializer=qic__storage__pb2.BramIndex.SerializeToString,
-            response_deserializer=qic__storage__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetBramResultData = channel.unary_unary(
             "/qic_storage.Storage/GetBramResultData",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.ResultData.FromString,
         )
         self.GetBramAveragedData = channel.unary_unary(
             "/qic_storage.Storage/GetBramAveragedData",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.AveragedData.FromString,
         )
         self.GetBramStateData = channel.unary_unary(
             "/qic_storage.Storage/GetBramStateData",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.StateData.FromString,
         )
         self.GetBramDataUInt32 = channel.unary_unary(
             "/qic_storage.Storage/GetBramDataUInt32",
             request_serializer=qic__storage__pb2.BramIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.BramDataUInt32.FromString,
         )
@@ -112,15 +98,15 @@
         self.GetBramLatestData = channel.unary_unary(
             "/qic_storage.Storage/GetBramLatestData",
             request_serializer=qic__storage__pb2.BramIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.LatestData.FromString,
         )
         self.IsDataLost = channel.unary_unary(
             "/qic_storage.Storage/IsDataLost",
-            request_serializer=qic__storage__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=qic__storage__pb2.DataLost.FromString,
         )
 
 
 class StorageServicer(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -233,80 +219,80 @@
         raise NotImplementedError("Method not implemented!")
 
 
 def add_StorageServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "Reset": grpc.unary_unary_rpc_method_handler(
             servicer.Reset,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
-            response_serializer=qic__storage__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "SetStateHandling": grpc.unary_unary_rpc_method_handler(
             servicer.SetStateHandling,
             request_deserializer=qic__storage__pb2.StateHandling.FromString,
-            response_serializer=qic__storage__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetStateHandling": grpc.unary_unary_rpc_method_handler(
             servicer.GetStateHandling,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.StateHandling.SerializeToString,
         ),
         "GetStateAccumulation": grpc.unary_unary_rpc_method_handler(
             servicer.GetStateAccumulation,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.StateAccumulation.SerializeToString,
         ),
         "SetResultHandling": grpc.unary_unary_rpc_method_handler(
             servicer.SetResultHandling,
             request_deserializer=qic__storage__pb2.ResultHandling.FromString,
-            response_serializer=qic__storage__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetResultHandling": grpc.unary_unary_rpc_method_handler(
             servicer.GetResultHandling,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.ResultHandling.SerializeToString,
         ),
         "SetAveragedHandling": grpc.unary_unary_rpc_method_handler(
             servicer.SetAveragedHandling,
             request_deserializer=qic__storage__pb2.AveragedHandling.FromString,
-            response_serializer=qic__storage__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetAveragedHandling": grpc.unary_unary_rpc_method_handler(
             servicer.GetAveragedHandling,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.AveragedHandling.SerializeToString,
         ),
         "SetBramControl": grpc.unary_unary_rpc_method_handler(
             servicer.SetBramControl,
             request_deserializer=qic__storage__pb2.BramControl.FromString,
-            response_serializer=qic__storage__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetBramStatus": grpc.unary_unary_rpc_method_handler(
             servicer.GetBramStatus,
             request_deserializer=qic__storage__pb2.BramIndex.FromString,
             response_serializer=qic__storage__pb2.BramStatus.SerializeToString,
         ),
         "ResetBramData": grpc.unary_unary_rpc_method_handler(
             servicer.ResetBramData,
             request_deserializer=qic__storage__pb2.BramIndex.FromString,
-            response_serializer=qic__storage__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetBramResultData": grpc.unary_unary_rpc_method_handler(
             servicer.GetBramResultData,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.ResultData.SerializeToString,
         ),
         "GetBramAveragedData": grpc.unary_unary_rpc_method_handler(
             servicer.GetBramAveragedData,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.AveragedData.SerializeToString,
         ),
         "GetBramStateData": grpc.unary_unary_rpc_method_handler(
             servicer.GetBramStateData,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.StateData.SerializeToString,
         ),
         "GetBramDataUInt32": grpc.unary_unary_rpc_method_handler(
             servicer.GetBramDataUInt32,
             request_deserializer=qic__storage__pb2.BramIndex.FromString,
             response_serializer=qic__storage__pb2.BramDataUInt32.SerializeToString,
         ),
@@ -318,15 +304,15 @@
         "GetBramLatestData": grpc.unary_unary_rpc_method_handler(
             servicer.GetBramLatestData,
             request_deserializer=qic__storage__pb2.BramIndex.FromString,
             response_serializer=qic__storage__pb2.LatestData.SerializeToString,
         ),
         "IsDataLost": grpc.unary_unary_rpc_method_handler(
             servicer.IsDataLost,
-            request_deserializer=qic__storage__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=qic__storage__pb2.DataLost.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "qic_storage.Storage", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
@@ -349,16 +335,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/Reset",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
-            qic__storage__pb2.Empty.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -379,15 +365,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/SetStateHandling",
             qic__storage__pb2.StateHandling.SerializeToString,
-            qic__storage__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -407,15 +393,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/GetStateHandling",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.StateHandling.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -436,15 +422,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/GetStateAccumulation",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.StateAccumulation.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -466,15 +452,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/SetResultHandling",
             qic__storage__pb2.ResultHandling.SerializeToString,
-            qic__storage__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -494,15 +480,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/GetResultHandling",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.ResultHandling.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -524,15 +510,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/SetAveragedHandling",
             qic__storage__pb2.AveragedHandling.SerializeToString,
-            qic__storage__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -552,15 +538,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/GetAveragedHandling",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.AveragedHandling.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -582,15 +568,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/SetBramControl",
             qic__storage__pb2.BramControl.SerializeToString,
-            qic__storage__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -640,15 +626,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/ResetBramData",
             qic__storage__pb2.BramIndex.SerializeToString,
-            qic__storage__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -668,15 +654,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/GetBramResultData",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.ResultData.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -697,15 +683,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/GetBramAveragedData",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.AveragedData.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -726,15 +712,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/GetBramStateData",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.StateData.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -842,15 +828,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_storage.Storage/IsDataLost",
-            qic__storage__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             qic__storage__pb2.DataLost.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/qic_unitcell_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/qic_unitcell_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,8 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: qic_unitcell.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
@@ -25,32 +10,33 @@
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x12qic_unitcell.proto\x12\x0cqic_unitcell"\x1a\n\tCellIndex\x12\r\n\x05value\x18\x01 \x01(\r"\x1c\n\x0b\x43\x65llIndexes\x12\r\n\x05\x63\x65lls\x18\x01 \x03(\r"\x19\n\x08Unsigned\x12\r\n\x05value\x18\x01 \x01(\r"z\n\x08\x43\x65llInfo\x12\x11\n\tsequencer\x18\x01 \x01(\r\x12\x11\n\trecording\x18\x02 \x01(\r\x12\x0f\n\x07readout\x18\x03 \x01(\r\x12\x14\n\x0cmanipulation\x18\x04 \x01(\r\x12\x10\n\x08\x63oupling\x18\x05 \x01(\r\x12\x0f\n\x07storage\x18\x06 \x01(\r"4\n\x0b\x41llCellInfo\x12%\n\x05\x63\x65lls\x18\x01 \x03(\x0b\x32\x16.qic_unitcell.CellInfo"1\n\rStartCellInfo\x12\x11\n\tall_cells\x18\x01 \x01(\x08\x12\r\n\x05\x63\x65lls\x18\x02 \x03(\r"+\n\x0c\x42usyCellInfo\x12\x0c\n\x04\x62usy\x18\x01 \x01(\x08\x12\r\n\x05\x63\x65lls\x18\x02 \x03(\r"$\n\x12QubitStateCellInfo\x12\x0e\n\x06states\x18\x01 \x01(\r"H\n\x0cPlatformInfo\x12\x12\n\ncell_count\x18\x01 \x01(\r\x12\x11\n\tdac_count\x18\x02 \x01(\r\x12\x11\n\tadc_count\x18\x03 \x01(\r",\n\tDACStatus\x12\r\n\x05ready\x18\x01 \x01(\x08\x12\x10\n\x08overflow\x18\x02 \x01(\x08"D\n\tADCStatus\x12\r\n\x05valid\x18\x01 \x01(\x08\x12\x14\n\x0cover_voltage\x18\x02 \x01(\x08\x12\x12\n\nover_range\x18\x03 \x01(\x08"~\n\x0f\x43onverterStatus\x12\r\n\x05\x65rror\x18\x01 \x01(\x08\x12\x0e\n\x06report\x18\x02 \x01(\t\x12%\n\x04\x64\x61\x63s\x18\x03 \x03(\x0b\x32\x17.qic_unitcell.DACStatus\x12%\n\x04\x61\x64\x63s\x18\x04 \x03(\x0b\x32\x17.qic_unitcell.ADCStatus"\x19\n\x08\x44\x41\x43Index\x12\r\n\x05value\x18\x01 \x01(\r"\x1f\n\x0e\x44\x41\x43SignalTypes\x12\r\n\x05types\x18\x01 \x03(\r"6\n\nDACRouting\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0b\n\x03\x64\x61\x63\x18\x02 \x01(\r\x12\r\n\x05\x63\x65lls\x18\x03 \x03(\r"\x1a\n\nADCIndexes\x12\x0c\n\x04\x61\x64\x63s\x18\x01 \x03(\r"6\n\nADCRouting\x12\x0b\n\x03\x61\x64\x63\x18\x01 \x01(\r\x12\r\n\x05\x63\x65lls\x18\x02 \x03(\r\x12\x0c\n\x04mode\x18\x03 \x01(\r"x\n\x14\x45xperimentParameters\x12.\n\x04mode\x18\x01 \x01(\x0e\x32 .qic_unitcell.DataCollectionMode\x12\r\n\x05shots\x18\x02 \x01(\r\x12\r\n\x05\x63\x65lls\x18\x03 \x03(\r\x12\x12\n\nrecordings\x18\x04 \x03(\r"\xc8\x02\n\x11\x45xperimentResults\x12\x10\n\x08progress\x18\x01 \x01(\r\x12\x14\n\x0cmax_progress\x18\x02 \x01(\r\x12\x10\n\x08\x66inished\x18\x03 \x01(\x08\x12.\n\x04mode\x18\x04 \x01(\x0e\x32 .qic_unitcell.DataCollectionMode\x12\x42\n\x07results\x18\x05 \x03(\x0b\x32\x31.qic_unitcell.ExperimentResults.SingleCellResults\x1a\x84\x01\n\x11SingleCellResults\x12\x15\n\rdata_double_1\x18\x01 \x03(\x01\x12\x15\n\rdata_double_2\x18\x02 \x03(\x01\x12\x15\n\rdata_sint32_1\x18\x03 \x03(\x11\x12\x15\n\rdata_sint32_2\x18\x04 \x03(\x11\x12\x13\n\x0b\x64\x61ta_uint32\x18\x05 \x03(\r"\x07\n\x05\x45mpty*}\n\x12\x44\x61taCollectionMode\x12\x0b\n\x07\x41VERAGE\x10\x00\x12\x13\n\x0f\x41MPLITUDE_PHASE\x10\x01\x12\x0b\n\x07IQCLOUD\x10\x02\x12\r\n\tRAW_TRACE\x10\x03\x12\n\n\x06STATES\x10\x04\x12\x0f\n\x0bSTATE_COUNT\x10\x05\x12\x0c\n\x08QM_JUMPS\x10\x06\x32\x96\n\n\x0fUnitCellService\x12=\n\x0cGetCellCount\x12\x13.qic_unitcell.Empty\x1a\x16.qic_unitcell.Unsigned"\x00\x12@\n\x0bGetCellInfo\x12\x17.qic_unitcell.CellIndex\x1a\x16.qic_unitcell.CellInfo"\x00\x12\x42\n\x0eGetAllCellInfo\x12\x13.qic_unitcell.Empty\x1a\x19.qic_unitcell.AllCellInfo"\x00\x12@\n\nStartCells\x12\x1b.qic_unitcell.StartCellInfo\x1a\x13.qic_unitcell.Empty"\x00\x12\x41\n\x0cGetBusyCells\x12\x13.qic_unitcell.Empty\x1a\x1a.qic_unitcell.BusyCellInfo"\x00\x12@\n\x0cGetSyncCells\x12\x13.qic_unitcell.Empty\x1a\x19.qic_unitcell.CellIndexes"\x00\x12\x44\n\x10GetDataSyncCells\x12\x13.qic_unitcell.Empty\x1a\x19.qic_unitcell.CellIndexes"\x00\x12I\n\x0eGetQubitStates\x12\x13.qic_unitcell.Empty\x1a .qic_unitcell.QubitStateCellInfo"\x00\x12\x44\n\x0fGetPlatformInfo\x12\x13.qic_unitcell.Empty\x1a\x1a.qic_unitcell.PlatformInfo"\x00\x12J\n\x12GetConverterStatus\x12\x13.qic_unitcell.Empty\x1a\x1d.qic_unitcell.ConverterStatus"\x00\x12\x42\n\x14\x43learConverterStatus\x12\x13.qic_unitcell.Empty\x1a\x13.qic_unitcell.Empty"\x00\x12H\n\x11GetDACSignalTypes\x12\x13.qic_unitcell.Empty\x1a\x1c.qic_unitcell.DACSignalTypes"\x00\x12J\n\x13GetDACRoutingSelect\x12\x16.qic_unitcell.DACIndex\x1a\x19.qic_unitcell.CellIndexes"\x00\x12\x46\n\x13SetDACRoutingSelect\x12\x18.qic_unitcell.DACRouting\x1a\x13.qic_unitcell.Empty"\x00\x12H\n\x14GetADCConnectedCells\x12\x13.qic_unitcell.Empty\x1a\x19.qic_unitcell.CellIndexes"\x00\x12\x46\n\x13GetADCRoutingSelect\x12\x13.qic_unitcell.Empty\x1a\x18.qic_unitcell.ADCIndexes"\x00\x12\x46\n\x13SetADCRoutingSelect\x12\x18.qic_unitcell.ADCRouting\x1a\x13.qic_unitcell.Empty"\x00\x12X\n\rRunExperiment\x12".qic_unitcell.ExperimentParameters\x1a\x1f.qic_unitcell.ExperimentResults"\x00\x30\x01\x62\x06proto3'
+    b'\n\x12qic_unitcell.proto\x12\x0cqic_unitcell\x1a\x0f\x64\x61tatypes.proto"\x1c\n\x0b\x43\x65llIndexes\x12\r\n\x05\x63\x65lls\x18\x01 \x03(\r"\x93\x01\n\x08\x43\x65llInfo\x12\x11\n\tsequencer\x18\x01 \x01(\r\x12\x11\n\trecording\x18\x02 \x01(\r\x12\x0f\n\x07readout\x18\x03 \x01(\r\x12\x14\n\x0cmanipulation\x18\x04 \x01(\r\x12\x10\n\x08\x63oupling\x18\x05 \x01(\r\x12\x0f\n\x07storage\x18\x06 \x01(\r\x12\x17\n\x0f\x64igital_trigger\x18\x07 \x01(\r"4\n\x0b\x41llCellInfo\x12%\n\x05\x63\x65lls\x18\x01 \x03(\x0b\x32\x16.qic_unitcell.CellInfo"1\n\rStartCellInfo\x12\x11\n\tall_cells\x18\x01 \x01(\x08\x12\r\n\x05\x63\x65lls\x18\x02 \x03(\r"+\n\x0c\x42usyCellInfo\x12\x0c\n\x04\x62usy\x18\x01 \x01(\x08\x12\r\n\x05\x63\x65lls\x18\x02 \x03(\r"$\n\x12QubitStateCellInfo\x12\x0e\n\x06states\x18\x01 \x01(\r"H\n\x0cPlatformInfo\x12\x12\n\ncell_count\x18\x01 \x01(\r\x12\x11\n\tdac_count\x18\x02 \x01(\r\x12\x11\n\tadc_count\x18\x03 \x01(\r",\n\tDACStatus\x12\r\n\x05ready\x18\x01 \x01(\x08\x12\x10\n\x08overflow\x18\x02 \x01(\x08"D\n\tADCStatus\x12\r\n\x05valid\x18\x01 \x01(\x08\x12\x14\n\x0cover_voltage\x18\x02 \x01(\x08\x12\x12\n\nover_range\x18\x03 \x01(\x08"~\n\x0f\x43onverterStatus\x12\r\n\x05\x65rror\x18\x01 \x01(\x08\x12\x0e\n\x06report\x18\x02 \x01(\t\x12%\n\x04\x64\x61\x63s\x18\x03 \x03(\x0b\x32\x17.qic_unitcell.DACStatus\x12%\n\x04\x61\x64\x63s\x18\x04 \x03(\x0b\x32\x17.qic_unitcell.ADCStatus"\x19\n\x08\x44\x41\x43Index\x12\r\n\x05value\x18\x01 \x01(\r"\x1f\n\x0e\x44\x41\x43SignalTypes\x12\r\n\x05types\x18\x01 \x03(\r"6\n\nDACRouting\x12\x0c\n\x04type\x18\x01 \x01(\r\x12\x0b\n\x03\x64\x61\x63\x18\x02 \x01(\r\x12\r\n\x05\x63\x65lls\x18\x03 \x03(\r"\x1a\n\nADCIndexes\x12\x0c\n\x04\x61\x64\x63s\x18\x01 \x03(\r"6\n\nADCRouting\x12\x0b\n\x03\x61\x64\x63\x18\x01 \x01(\r\x12\r\n\x05\x63\x65lls\x18\x02 \x03(\r\x12\x0c\n\x04mode\x18\x03 \x01(\r"x\n\x14\x45xperimentParameters\x12.\n\x04mode\x18\x01 \x01(\x0e\x32 .qic_unitcell.DataCollectionMode\x12\r\n\x05shots\x18\x02 \x01(\r\x12\r\n\x05\x63\x65lls\x18\x03 \x03(\r\x12\x12\n\nrecordings\x18\x04 \x03(\r"\xc8\x02\n\x11\x45xperimentResults\x12\x10\n\x08progress\x18\x01 \x01(\r\x12\x14\n\x0cmax_progress\x18\x02 \x01(\r\x12\x10\n\x08\x66inished\x18\x03 \x01(\x08\x12.\n\x04mode\x18\x04 \x01(\x0e\x32 .qic_unitcell.DataCollectionMode\x12\x42\n\x07results\x18\x05 \x03(\x0b\x32\x31.qic_unitcell.ExperimentResults.SingleCellResults\x1a\x84\x01\n\x11SingleCellResults\x12\x15\n\rdata_double_1\x18\x01 \x03(\x01\x12\x15\n\rdata_double_2\x18\x02 \x03(\x01\x12\x15\n\rdata_sint32_1\x18\x03 \x03(\x11\x12\x15\n\rdata_sint32_2\x18\x04 \x03(\x11\x12\x13\n\x0b\x64\x61ta_uint32\x18\x05 \x03(\r*}\n\x12\x44\x61taCollectionMode\x12\x0b\n\x07\x41VERAGE\x10\x00\x12\x13\n\x0f\x41MPLITUDE_PHASE\x10\x01\x12\x0b\n\x07IQCLOUD\x10\x02\x12\r\n\tRAW_TRACE\x10\x03\x12\n\n\x06STATES\x10\x04\x12\x0f\n\x0bSTATE_COUNT\x10\x05\x12\x0c\n\x08QM_JUMPS\x10\x06\x32\x9f\n\n\x0fUnitCellService\x12;\n\x0cGetCellCount\x12\x14.sdr.datatypes.Empty\x1a\x13.sdr.datatypes.UInt"\x00\x12<\n\x0bGetCellInfo\x12\x13.sdr.datatypes.UInt\x1a\x16.qic_unitcell.CellInfo"\x00\x12\x43\n\x0eGetAllCellInfo\x12\x14.sdr.datatypes.Empty\x1a\x19.qic_unitcell.AllCellInfo"\x00\x12\x41\n\nStartCells\x12\x1b.qic_unitcell.StartCellInfo\x1a\x14.sdr.datatypes.Empty"\x00\x12\x42\n\x0cGetBusyCells\x12\x14.sdr.datatypes.Empty\x1a\x1a.qic_unitcell.BusyCellInfo"\x00\x12\x41\n\x0cGetSyncCells\x12\x14.sdr.datatypes.Empty\x1a\x19.qic_unitcell.CellIndexes"\x00\x12\x45\n\x10GetDataSyncCells\x12\x14.sdr.datatypes.Empty\x1a\x19.qic_unitcell.CellIndexes"\x00\x12J\n\x0eGetQubitStates\x12\x14.sdr.datatypes.Empty\x1a .qic_unitcell.QubitStateCellInfo"\x00\x12\x45\n\x0fGetPlatformInfo\x12\x14.sdr.datatypes.Empty\x1a\x1a.qic_unitcell.PlatformInfo"\x00\x12K\n\x12GetConverterStatus\x12\x14.sdr.datatypes.Empty\x1a\x1d.qic_unitcell.ConverterStatus"\x00\x12\x44\n\x14\x43learConverterStatus\x12\x14.sdr.datatypes.Empty\x1a\x14.sdr.datatypes.Empty"\x00\x12I\n\x11GetDACSignalTypes\x12\x14.sdr.datatypes.Empty\x1a\x1c.qic_unitcell.DACSignalTypes"\x00\x12J\n\x13GetDACRoutingSelect\x12\x16.qic_unitcell.DACIndex\x1a\x19.qic_unitcell.CellIndexes"\x00\x12G\n\x13SetDACRoutingSelect\x12\x18.qic_unitcell.DACRouting\x1a\x14.sdr.datatypes.Empty"\x00\x12I\n\x14GetADCConnectedCells\x12\x14.sdr.datatypes.Empty\x1a\x19.qic_unitcell.CellIndexes"\x00\x12G\n\x13GetADCRoutingSelect\x12\x14.sdr.datatypes.Empty\x1a\x18.qic_unitcell.ADCIndexes"\x00\x12G\n\x13SetADCRoutingSelect\x12\x18.qic_unitcell.ADCRouting\x1a\x14.sdr.datatypes.Empty"\x00\x12X\n\rRunExperiment\x12".qic_unitcell.ExperimentParameters\x1a\x1f.qic_unitcell.ExperimentResults"\x00\x30\x01\x62\x06proto3'
 )
 
 _DATACOLLECTIONMODE = DESCRIPTOR.enum_types_by_name["DataCollectionMode"]
 DataCollectionMode = enum_type_wrapper.EnumTypeWrapper(_DATACOLLECTIONMODE)
 AVERAGE = 0
 AMPLITUDE_PHASE = 1
 IQCLOUD = 2
 RAW_TRACE = 3
 STATES = 4
 STATE_COUNT = 5
 QM_JUMPS = 6
 
 
-_CELLINDEX = DESCRIPTOR.message_types_by_name["CellIndex"]
 _CELLINDEXES = DESCRIPTOR.message_types_by_name["CellIndexes"]
-_UNSIGNED = DESCRIPTOR.message_types_by_name["Unsigned"]
 _CELLINFO = DESCRIPTOR.message_types_by_name["CellInfo"]
 _ALLCELLINFO = DESCRIPTOR.message_types_by_name["AllCellInfo"]
 _STARTCELLINFO = DESCRIPTOR.message_types_by_name["StartCellInfo"]
 _BUSYCELLINFO = DESCRIPTOR.message_types_by_name["BusyCellInfo"]
 _QUBITSTATECELLINFO = DESCRIPTOR.message_types_by_name["QubitStateCellInfo"]
 _PLATFORMINFO = DESCRIPTOR.message_types_by_name["PlatformInfo"]
 _DACSTATUS = DESCRIPTOR.message_types_by_name["DACStatus"]
@@ -62,48 +48,25 @@
 _ADCINDEXES = DESCRIPTOR.message_types_by_name["ADCIndexes"]
 _ADCROUTING = DESCRIPTOR.message_types_by_name["ADCRouting"]
 _EXPERIMENTPARAMETERS = DESCRIPTOR.message_types_by_name["ExperimentParameters"]
 _EXPERIMENTRESULTS = DESCRIPTOR.message_types_by_name["ExperimentResults"]
 _EXPERIMENTRESULTS_SINGLECELLRESULTS = _EXPERIMENTRESULTS.nested_types_by_name[
     "SingleCellResults"
 ]
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
-CellIndex = _reflection.GeneratedProtocolMessageType(
-    "CellIndex",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _CELLINDEX,
-        "__module__": "qic_unitcell_pb2"
-        # @@protoc_insertion_point(class_scope:qic_unitcell.CellIndex)
-    },
-)
-_sym_db.RegisterMessage(CellIndex)
-
 CellIndexes = _reflection.GeneratedProtocolMessageType(
     "CellIndexes",
     (_message.Message,),
     {
         "DESCRIPTOR": _CELLINDEXES,
         "__module__": "qic_unitcell_pb2"
         # @@protoc_insertion_point(class_scope:qic_unitcell.CellIndexes)
     },
 )
 _sym_db.RegisterMessage(CellIndexes)
 
-Unsigned = _reflection.GeneratedProtocolMessageType(
-    "Unsigned",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _UNSIGNED,
-        "__module__": "qic_unitcell_pb2"
-        # @@protoc_insertion_point(class_scope:qic_unitcell.Unsigned)
-    },
-)
-_sym_db.RegisterMessage(Unsigned)
-
 CellInfo = _reflection.GeneratedProtocolMessageType(
     "CellInfo",
     (_message.Message,),
     {
         "DESCRIPTOR": _CELLINFO,
         "__module__": "qic_unitcell_pb2"
         # @@protoc_insertion_point(class_scope:qic_unitcell.CellInfo)
@@ -282,69 +245,51 @@
         "__module__": "qic_unitcell_pb2"
         # @@protoc_insertion_point(class_scope:qic_unitcell.ExperimentResults)
     },
 )
 _sym_db.RegisterMessage(ExperimentResults)
 _sym_db.RegisterMessage(ExperimentResults.SingleCellResults)
 
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "qic_unitcell_pb2"
-        # @@protoc_insertion_point(class_scope:qic_unitcell.Empty)
-    },
-)
-_sym_db.RegisterMessage(Empty)
-
 _UNITCELLSERVICE = DESCRIPTOR.services_by_name["UnitCellService"]
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    _DATACOLLECTIONMODE._serialized_start = 1413
-    _DATACOLLECTIONMODE._serialized_end = 1538
-    _CELLINDEX._serialized_start = 36
-    _CELLINDEX._serialized_end = 62
-    _CELLINDEXES._serialized_start = 64
-    _CELLINDEXES._serialized_end = 92
-    _UNSIGNED._serialized_start = 94
-    _UNSIGNED._serialized_end = 119
-    _CELLINFO._serialized_start = 121
-    _CELLINFO._serialized_end = 243
-    _ALLCELLINFO._serialized_start = 245
-    _ALLCELLINFO._serialized_end = 297
-    _STARTCELLINFO._serialized_start = 299
-    _STARTCELLINFO._serialized_end = 348
-    _BUSYCELLINFO._serialized_start = 350
-    _BUSYCELLINFO._serialized_end = 393
-    _QUBITSTATECELLINFO._serialized_start = 395
-    _QUBITSTATECELLINFO._serialized_end = 431
-    _PLATFORMINFO._serialized_start = 433
-    _PLATFORMINFO._serialized_end = 505
-    _DACSTATUS._serialized_start = 507
-    _DACSTATUS._serialized_end = 551
-    _ADCSTATUS._serialized_start = 553
-    _ADCSTATUS._serialized_end = 621
-    _CONVERTERSTATUS._serialized_start = 623
-    _CONVERTERSTATUS._serialized_end = 749
-    _DACINDEX._serialized_start = 751
-    _DACINDEX._serialized_end = 776
-    _DACSIGNALTYPES._serialized_start = 778
-    _DACSIGNALTYPES._serialized_end = 809
-    _DACROUTING._serialized_start = 811
-    _DACROUTING._serialized_end = 865
-    _ADCINDEXES._serialized_start = 867
-    _ADCINDEXES._serialized_end = 893
-    _ADCROUTING._serialized_start = 895
-    _ADCROUTING._serialized_end = 949
-    _EXPERIMENTPARAMETERS._serialized_start = 951
-    _EXPERIMENTPARAMETERS._serialized_end = 1071
-    _EXPERIMENTRESULTS._serialized_start = 1074
-    _EXPERIMENTRESULTS._serialized_end = 1402
-    _EXPERIMENTRESULTS_SINGLECELLRESULTS._serialized_start = 1270
-    _EXPERIMENTRESULTS_SINGLECELLRESULTS._serialized_end = 1402
-    _EMPTY._serialized_start = 1404
-    _EMPTY._serialized_end = 1411
-    _UNITCELLSERVICE._serialized_start = 1541
-    _UNITCELLSERVICE._serialized_end = 2843
+    _DATACOLLECTIONMODE._serialized_start = 1392
+    _DATACOLLECTIONMODE._serialized_end = 1517
+    _CELLINDEXES._serialized_start = 53
+    _CELLINDEXES._serialized_end = 81
+    _CELLINFO._serialized_start = 84
+    _CELLINFO._serialized_end = 231
+    _ALLCELLINFO._serialized_start = 233
+    _ALLCELLINFO._serialized_end = 285
+    _STARTCELLINFO._serialized_start = 287
+    _STARTCELLINFO._serialized_end = 336
+    _BUSYCELLINFO._serialized_start = 338
+    _BUSYCELLINFO._serialized_end = 381
+    _QUBITSTATECELLINFO._serialized_start = 383
+    _QUBITSTATECELLINFO._serialized_end = 419
+    _PLATFORMINFO._serialized_start = 421
+    _PLATFORMINFO._serialized_end = 493
+    _DACSTATUS._serialized_start = 495
+    _DACSTATUS._serialized_end = 539
+    _ADCSTATUS._serialized_start = 541
+    _ADCSTATUS._serialized_end = 609
+    _CONVERTERSTATUS._serialized_start = 611
+    _CONVERTERSTATUS._serialized_end = 737
+    _DACINDEX._serialized_start = 739
+    _DACINDEX._serialized_end = 764
+    _DACSIGNALTYPES._serialized_start = 766
+    _DACSIGNALTYPES._serialized_end = 797
+    _DACROUTING._serialized_start = 799
+    _DACROUTING._serialized_end = 853
+    _ADCINDEXES._serialized_start = 855
+    _ADCINDEXES._serialized_end = 881
+    _ADCROUTING._serialized_start = 883
+    _ADCROUTING._serialized_end = 937
+    _EXPERIMENTPARAMETERS._serialized_start = 939
+    _EXPERIMENTPARAMETERS._serialized_end = 1059
+    _EXPERIMENTRESULTS._serialized_start = 1062
+    _EXPERIMENTRESULTS._serialized_end = 1390
+    _EXPERIMENTRESULTS_SINGLECELLRESULTS._serialized_start = 1258
+    _EXPERIMENTRESULTS_SINGLECELLRESULTS._serialized_end = 1390
+    _UNITCELLSERVICE._serialized_start = 1520
+    _UNITCELLSERVICE._serialized_end = 2831
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/qic_unitcell_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/qic_unitcell_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,108 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import qic_unitcell_pb2 as qic__unitcell__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.qic_unitcell_pb2 as qic__unitcell__pb2
 
 
 class UnitCellServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetCellCount = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetCellCount",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
-            response_deserializer=qic__unitcell__pb2.Unsigned.FromString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.UInt.FromString,
         )
         self.GetCellInfo = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetCellInfo",
-            request_serializer=qic__unitcell__pb2.CellIndex.SerializeToString,
+            request_serializer=datatypes__pb2.UInt.SerializeToString,
             response_deserializer=qic__unitcell__pb2.CellInfo.FromString,
         )
         self.GetAllCellInfo = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetAllCellInfo",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.AllCellInfo.FromString,
         )
         self.StartCells = channel.unary_unary(
             "/qic_unitcell.UnitCellService/StartCells",
             request_serializer=qic__unitcell__pb2.StartCellInfo.SerializeToString,
-            response_deserializer=qic__unitcell__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetBusyCells = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetBusyCells",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.BusyCellInfo.FromString,
         )
         self.GetSyncCells = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetSyncCells",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.CellIndexes.FromString,
         )
         self.GetDataSyncCells = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetDataSyncCells",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.CellIndexes.FromString,
         )
         self.GetQubitStates = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetQubitStates",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.QubitStateCellInfo.FromString,
         )
         self.GetPlatformInfo = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetPlatformInfo",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.PlatformInfo.FromString,
         )
         self.GetConverterStatus = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetConverterStatus",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.ConverterStatus.FromString,
         )
         self.ClearConverterStatus = channel.unary_unary(
             "/qic_unitcell.UnitCellService/ClearConverterStatus",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
-            response_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetDACSignalTypes = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetDACSignalTypes",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.DACSignalTypes.FromString,
         )
         self.GetDACRoutingSelect = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetDACRoutingSelect",
             request_serializer=qic__unitcell__pb2.DACIndex.SerializeToString,
             response_deserializer=qic__unitcell__pb2.CellIndexes.FromString,
         )
         self.SetDACRoutingSelect = channel.unary_unary(
             "/qic_unitcell.UnitCellService/SetDACRoutingSelect",
             request_serializer=qic__unitcell__pb2.DACRouting.SerializeToString,
-            response_deserializer=qic__unitcell__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetADCConnectedCells = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetADCConnectedCells",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.CellIndexes.FromString,
         )
         self.GetADCRoutingSelect = channel.unary_unary(
             "/qic_unitcell.UnitCellService/GetADCRoutingSelect",
-            request_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=qic__unitcell__pb2.ADCIndexes.FromString,
         )
         self.SetADCRoutingSelect = channel.unary_unary(
             "/qic_unitcell.UnitCellService/SetADCRoutingSelect",
             request_serializer=qic__unitcell__pb2.ADCRouting.SerializeToString,
-            response_deserializer=qic__unitcell__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.RunExperiment = channel.unary_stream(
             "/qic_unitcell.UnitCellService/RunExperiment",
             request_serializer=qic__unitcell__pb2.ExperimentParameters.SerializeToString,
             response_deserializer=qic__unitcell__pb2.ExperimentResults.FromString,
         )
 
@@ -258,96 +244,96 @@
         raise NotImplementedError("Method not implemented!")
 
 
 def add_UnitCellServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "GetCellCount": grpc.unary_unary_rpc_method_handler(
             servicer.GetCellCount,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
-            response_serializer=qic__unitcell__pb2.Unsigned.SerializeToString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.UInt.SerializeToString,
         ),
         "GetCellInfo": grpc.unary_unary_rpc_method_handler(
             servicer.GetCellInfo,
-            request_deserializer=qic__unitcell__pb2.CellIndex.FromString,
+            request_deserializer=datatypes__pb2.UInt.FromString,
             response_serializer=qic__unitcell__pb2.CellInfo.SerializeToString,
         ),
         "GetAllCellInfo": grpc.unary_unary_rpc_method_handler(
             servicer.GetAllCellInfo,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.AllCellInfo.SerializeToString,
         ),
         "StartCells": grpc.unary_unary_rpc_method_handler(
             servicer.StartCells,
             request_deserializer=qic__unitcell__pb2.StartCellInfo.FromString,
-            response_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetBusyCells": grpc.unary_unary_rpc_method_handler(
             servicer.GetBusyCells,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.BusyCellInfo.SerializeToString,
         ),
         "GetSyncCells": grpc.unary_unary_rpc_method_handler(
             servicer.GetSyncCells,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.CellIndexes.SerializeToString,
         ),
         "GetDataSyncCells": grpc.unary_unary_rpc_method_handler(
             servicer.GetDataSyncCells,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.CellIndexes.SerializeToString,
         ),
         "GetQubitStates": grpc.unary_unary_rpc_method_handler(
             servicer.GetQubitStates,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.QubitStateCellInfo.SerializeToString,
         ),
         "GetPlatformInfo": grpc.unary_unary_rpc_method_handler(
             servicer.GetPlatformInfo,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.PlatformInfo.SerializeToString,
         ),
         "GetConverterStatus": grpc.unary_unary_rpc_method_handler(
             servicer.GetConverterStatus,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.ConverterStatus.SerializeToString,
         ),
         "ClearConverterStatus": grpc.unary_unary_rpc_method_handler(
             servicer.ClearConverterStatus,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
-            response_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetDACSignalTypes": grpc.unary_unary_rpc_method_handler(
             servicer.GetDACSignalTypes,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.DACSignalTypes.SerializeToString,
         ),
         "GetDACRoutingSelect": grpc.unary_unary_rpc_method_handler(
             servicer.GetDACRoutingSelect,
             request_deserializer=qic__unitcell__pb2.DACIndex.FromString,
             response_serializer=qic__unitcell__pb2.CellIndexes.SerializeToString,
         ),
         "SetDACRoutingSelect": grpc.unary_unary_rpc_method_handler(
             servicer.SetDACRoutingSelect,
             request_deserializer=qic__unitcell__pb2.DACRouting.FromString,
-            response_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetADCConnectedCells": grpc.unary_unary_rpc_method_handler(
             servicer.GetADCConnectedCells,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.CellIndexes.SerializeToString,
         ),
         "GetADCRoutingSelect": grpc.unary_unary_rpc_method_handler(
             servicer.GetADCRoutingSelect,
-            request_deserializer=qic__unitcell__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=qic__unitcell__pb2.ADCIndexes.SerializeToString,
         ),
         "SetADCRoutingSelect": grpc.unary_unary_rpc_method_handler(
             servicer.SetADCRoutingSelect,
             request_deserializer=qic__unitcell__pb2.ADCRouting.FromString,
-            response_serializer=qic__unitcell__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "RunExperiment": grpc.unary_stream_rpc_method_handler(
             servicer.RunExperiment,
             request_deserializer=qic__unitcell__pb2.ExperimentParameters.FromString,
             response_serializer=qic__unitcell__pb2.ExperimentResults.SerializeToString,
         ),
     }
@@ -374,16 +360,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetCellCount",
-            qic__unitcell__pb2.Empty.SerializeToString,
-            qic__unitcell__pb2.Unsigned.FromString,
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.UInt.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -403,15 +389,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetCellInfo",
-            qic__unitcell__pb2.CellIndex.SerializeToString,
+            datatypes__pb2.UInt.SerializeToString,
             qic__unitcell__pb2.CellInfo.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -432,15 +418,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetAllCellInfo",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.AllCellInfo.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -462,15 +448,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/StartCells",
             qic__unitcell__pb2.StartCellInfo.SerializeToString,
-            qic__unitcell__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -490,15 +476,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetBusyCells",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.BusyCellInfo.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -519,15 +505,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetSyncCells",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.CellIndexes.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -548,15 +534,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetDataSyncCells",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.CellIndexes.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -577,15 +563,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetQubitStates",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.QubitStateCellInfo.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -606,15 +592,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetPlatformInfo",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.PlatformInfo.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -635,15 +621,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetConverterStatus",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.ConverterStatus.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -664,16 +650,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/ClearConverterStatus",
-            qic__unitcell__pb2.Empty.SerializeToString,
-            qic__unitcell__pb2.Empty.FromString,
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -693,15 +679,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetDACSignalTypes",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.DACSignalTypes.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -752,15 +738,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/SetDACRoutingSelect",
             qic__unitcell__pb2.DACRouting.SerializeToString,
-            qic__unitcell__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -780,15 +766,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetADCConnectedCells",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.CellIndexes.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -809,15 +795,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/GetADCRoutingSelect",
-            qic__unitcell__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             qic__unitcell__pb2.ADCIndexes.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -839,15 +825,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/qic_unitcell.UnitCellService/SetADCRoutingSelect",
             qic__unitcell__pb2.ADCRouting.SerializeToString,
-            qic__unitcell__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/recording_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/recording_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,30 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: recording.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0frecording.proto\x12\trecording"\x1e\n\rEndpointIndex\x12\r\n\x05value\x18\x01 \x01(\r"/\n\x0cStatusReport\x12\x0e\n\x06report\x18\x01 \x01(\t\x12\x0f\n\x07\x66\x61ilure\x18\x02 \x01(\x08"X\n\x12InterferometerMode\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\x19\n\x11is_interferometer\x18\x02 \x01(\x08"P\n\x0e\x43ontinuousMode\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\x15\n\ris_continuous\x18\x02 \x01(\x08"\xd9\x01\n\x07Trigger\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12.\n\x05value\x18\x02 \x01(\x0e\x32\x1f.recording.Trigger.TriggerValue"u\n\x0cTriggerValue\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06SINGLE\x10\x01\x12\x0b\n\x07ONESHOT\x10\x02\x12\x14\n\x10START_CONTINUOUS\x10\x06\x12\x13\n\x0fSTOP_CONTINUOUS\x10\x07\x12\t\n\x05RESET\x10\x0e\x12\x0c\n\x08NCO_SYNC\x10\x0f"G\n\rTriggerOffset\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"K\n\x11RecordingDuration\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"D\n\nValueShift\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"J\n\x10ValueShiftOffset\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x05"F\n\x0c\x41verageShift\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"C\n\tFrequency\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"E\n\x0bPhaseOffset\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"H\n\x0eReferenceDelay\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"k\n\x0bStateConfig\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\x10\n\x08value_ai\x18\x02 \x01(\x05\x12\x10\n\x08value_aq\x18\x03 \x01(\x05\x12\x0f\n\x07value_b\x18\x04 \x01(\x05",\n\x08IQResult\x12\x0f\n\x07i_value\x18\x01 \x01(\x05\x12\x0f\n\x07q_value\x18\x02 \x01(\x05"C\n\nMemorySize\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\x0c\n\x04size\x18\x02 \x01(\r"t\n\x0cMemoryStatus\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\x0c\n\x04size\x18\x02 \x01(\r\x12\r\n\x05\x65mpty\x18\x03 \x01(\x08\x12\x0c\n\x04\x66ull\x18\x04 \x01(\x08\x12\x10\n\x08overflow\x18\x05 \x01(\x08"2\n\x0cResultMemory\x12\x10\n\x08result_i\x18\x01 \x03(\x05\x12\x10\n\x08result_q\x18\x02 \x03(\x05")\n\tRawMemory\x12\r\n\x05raw_i\x18\x01 \x03(\x05\x12\r\n\x05raw_q\x18\x02 \x03(\x05"m\n\x12\x43onditioningMatrix\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\n\n\x02ii\x18\x02 \x01(\x01\x12\n\n\x02iq\x18\x03 \x01(\x01\x12\n\n\x02qi\x18\x04 \x01(\x01\x12\n\n\x02qq\x18\x05 \x01(\x01"S\n\x12\x43onditioningOffset\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.recording.EndpointIndex\x12\t\n\x01i\x18\x02 \x01(\x05\x12\t\n\x01q\x18\x03 \x01(\x05"\x07\n\x05\x45mpty2\xe2\x16\n\tRecording\x12\x35\n\x05Reset\x12\x18.recording.EndpointIndex\x1a\x10.recording.Empty"\x00\x12\x43\n\x0cReportStatus\x12\x18.recording.EndpointIndex\x1a\x17.recording.StatusReport"\x00\x12;\n\x0bResetStatus\x12\x18.recording.EndpointIndex\x1a\x10.recording.Empty"\x00\x12\x36\n\x0eResetStatusAll\x12\x10.recording.Empty\x1a\x10.recording.Empty"\x00\x12Q\n\x14IsInterferometerMode\x12\x18.recording.EndpointIndex\x1a\x1d.recording.InterferometerMode"\x00\x12J\n\x15SetInterferometerMode\x12\x1d.recording.InterferometerMode\x1a\x10.recording.Empty"\x00\x12I\n\x10IsContinuousMode\x12\x18.recording.EndpointIndex\x1a\x19.recording.ContinuousMode"\x00\x12\x42\n\x11SetContinuousMode\x12\x19.recording.ContinuousMode\x1a\x10.recording.Empty"\x00\x12@\n\x0eGetLastTrigger\x12\x18.recording.EndpointIndex\x1a\x12.recording.Trigger"\x00\x12\x39\n\x0fTriggerManually\x12\x12.recording.Trigger\x1a\x10.recording.Empty"\x00\x12H\n\x10GetTriggerOffset\x12\x18.recording.EndpointIndex\x1a\x18.recording.TriggerOffset"\x00\x12@\n\x10SetTriggerOffset\x12\x18.recording.TriggerOffset\x1a\x10.recording.Empty"\x00\x12P\n\x14GetRecordingDuration\x12\x18.recording.EndpointIndex\x1a\x1c.recording.RecordingDuration"\x00\x12H\n\x14SetRecordingDuration\x12\x1c.recording.RecordingDuration\x1a\x10.recording.Empty"\x00\x12\x42\n\rGetValueShift\x12\x18.recording.EndpointIndex\x1a\x15.recording.ValueShift"\x00\x12:\n\rSetValueShift\x12\x15.recording.ValueShift\x1a\x10.recording.Empty"\x00\x12I\n\x14GetValueShiftInitial\x12\x18.recording.EndpointIndex\x1a\x15.recording.ValueShift"\x00\x12N\n\x13GetValueShiftOffset\x12\x18.recording.EndpointIndex\x1a\x1b.recording.ValueShiftOffset"\x00\x12\x46\n\x13SetValueShiftOffset\x12\x1b.recording.ValueShiftOffset\x1a\x10.recording.Empty"\x00\x12\x46\n\x0fGetAverageShift\x12\x18.recording.EndpointIndex\x1a\x17.recording.AverageShift"\x00\x12>\n\x0fSetAverageShift\x12\x17.recording.AverageShift\x1a\x10.recording.Empty"\x00\x12R\n\x15GetConditioningMatrix\x12\x18.recording.EndpointIndex\x1a\x1d.recording.ConditioningMatrix"\x00\x12J\n\x15SetConditioningMatrix\x12\x1d.recording.ConditioningMatrix\x1a\x10.recording.Empty"\x00\x12R\n\x15GetConditioningOffset\x12\x18.recording.EndpointIndex\x1a\x1d.recording.ConditioningOffset"\x00\x12J\n\x15SetConditioningOffset\x12\x1d.recording.ConditioningOffset\x1a\x10.recording.Empty"\x00\x12H\n\x14GetInternalFrequency\x12\x18.recording.EndpointIndex\x1a\x14.recording.Frequency"\x00\x12@\n\x14SetInternalFrequency\x12\x14.recording.Frequency\x1a\x10.recording.Empty"\x00\x12L\n\x16GetInternalPhaseOffset\x12\x18.recording.EndpointIndex\x1a\x16.recording.PhaseOffset"\x00\x12\x44\n\x16SetInternalPhaseOffset\x12\x16.recording.PhaseOffset\x1a\x10.recording.Empty"\x00\x12I\n\x15GetReferenceFrequency\x12\x18.recording.EndpointIndex\x1a\x14.recording.Frequency"\x00\x12\x41\n\x15SetReferenceFrequency\x12\x14.recording.Frequency\x1a\x10.recording.Empty"\x00\x12J\n\x11GetReferenceDelay\x12\x18.recording.EndpointIndex\x1a\x19.recording.ReferenceDelay"\x00\x12\x42\n\x11SetReferenceDelay\x12\x19.recording.ReferenceDelay\x1a\x10.recording.Empty"\x00\x12\x44\n\x0eGetStateConfig\x12\x18.recording.EndpointIndex\x1a\x16.recording.StateConfig"\x00\x12<\n\x0eSetStateConfig\x12\x16.recording.StateConfig\x1a\x10.recording.Empty"\x00\x12\x44\n\x11GetAveragedResult\x12\x18.recording.EndpointIndex\x1a\x13.recording.IQResult"\x00\x12\x42\n\x0fGetSingleResult\x12\x18.recording.EndpointIndex\x1a\x13.recording.IQResult"\x00\x12L\n\x15GetResultMemoryStatus\x12\x18.recording.EndpointIndex\x1a\x17.recording.MemoryStatus"\x00\x12H\n\x13GetResultMemorySize\x12\x18.recording.EndpointIndex\x1a\x15.recording.MemorySize"\x00\x12\x43\n\x0fGetResultMemory\x12\x15.recording.MemorySize\x1a\x17.recording.ResultMemory"\x00\x12=\n\x0cGetRawMemory\x12\x15.recording.MemorySize\x1a\x14.recording.RawMemory"\x00\x62\x06proto3'
+    b'\n\x0frecording.proto\x12\trecording\x1a\x0f\x64\x61tatypes.proto"/\n\x0cStatusReport\x12\x0e\n\x06report\x18\x01 \x01(\t\x12\x0f\n\x07\x66\x61ilure\x18\x02 \x01(\x08"\\\n\x12InterferometerMode\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x19\n\x11is_interferometer\x18\x02 \x01(\x08"T\n\x0e\x43ontinuousMode\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x15\n\ris_continuous\x18\x02 \x01(\x08"\xdd\x01\n\x07Trigger\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12.\n\x05value\x18\x02 \x01(\x0e\x32\x1f.recording.Trigger.TriggerValue"u\n\x0cTriggerValue\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06SINGLE\x10\x01\x12\x0b\n\x07ONESHOT\x10\x02\x12\x14\n\x10START_CONTINUOUS\x10\x06\x12\x13\n\x0fSTOP_CONTINUOUS\x10\x07\x12\t\n\x05RESET\x10\x0e\x12\x0c\n\x08NCO_SYNC\x10\x0f"K\n\rTriggerOffset\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"O\n\x11RecordingDuration\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"H\n\nValueShift\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"N\n\x10ValueShiftOffset\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x05"J\n\x0c\x41verageShift\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"G\n\tFrequency\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"I\n\x0bPhaseOffset\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"L\n\x0eReferenceDelay\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"o\n\x0bStateConfig\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x10\n\x08value_ai\x18\x02 \x01(\x05\x12\x10\n\x08value_aq\x18\x03 \x01(\x05\x12\x0f\n\x07value_b\x18\x04 \x01(\x05",\n\x08IQResult\x12\x0f\n\x07i_value\x18\x01 \x01(\x05\x12\x0f\n\x07q_value\x18\x02 \x01(\x05"G\n\nMemorySize\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x0c\n\x04size\x18\x02 \x01(\r"x\n\x0cMemoryStatus\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x0c\n\x04size\x18\x02 \x01(\r\x12\r\n\x05\x65mpty\x18\x03 \x01(\x08\x12\x0c\n\x04\x66ull\x18\x04 \x01(\x08\x12\x10\n\x08overflow\x18\x05 \x01(\x08"2\n\x0cResultMemory\x12\x10\n\x08result_i\x18\x01 \x03(\x05\x12\x10\n\x08result_q\x18\x02 \x03(\x05")\n\tRawMemory\x12\r\n\x05raw_i\x18\x01 \x03(\x05\x12\r\n\x05raw_q\x18\x02 \x03(\x05"q\n\x12\x43onditioningMatrix\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\n\n\x02ii\x18\x02 \x01(\x01\x12\n\n\x02iq\x18\x03 \x01(\x01\x12\n\n\x02qi\x18\x04 \x01(\x01\x12\n\n\x02qq\x18\x05 \x01(\x01"W\n\x12\x43onditioningOffset\x12+\n\x05index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\t\n\x01i\x18\x02 \x01(\x05\x12\t\n\x01q\x18\x03 \x01(\x05\x32\x8a\x18\n\tRecording\x12=\n\x05Reset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12G\n\x0cReportStatus\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x17.recording.StatusReport"\x00\x12\x43\n\x0bResetStatus\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12>\n\x0eResetStatusAll\x12\x14.sdr.datatypes.Empty\x1a\x14.sdr.datatypes.Empty"\x00\x12U\n\x14IsInterferometerMode\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1d.recording.InterferometerMode"\x00\x12N\n\x15SetInterferometerMode\x12\x1d.recording.InterferometerMode\x1a\x14.sdr.datatypes.Empty"\x00\x12M\n\x10IsContinuousMode\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x19.recording.ContinuousMode"\x00\x12\x46\n\x11SetContinuousMode\x12\x19.recording.ContinuousMode\x1a\x14.sdr.datatypes.Empty"\x00\x12\x44\n\x0eGetLastTrigger\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x12.recording.Trigger"\x00\x12=\n\x0fTriggerManually\x12\x12.recording.Trigger\x1a\x14.sdr.datatypes.Empty"\x00\x12L\n\x10GetTriggerOffset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x18.recording.TriggerOffset"\x00\x12\x44\n\x10SetTriggerOffset\x12\x18.recording.TriggerOffset\x1a\x14.sdr.datatypes.Empty"\x00\x12T\n\x14GetRecordingDuration\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1c.recording.RecordingDuration"\x00\x12L\n\x14SetRecordingDuration\x12\x1c.recording.RecordingDuration\x1a\x14.sdr.datatypes.Empty"\x00\x12\x46\n\rGetValueShift\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x15.recording.ValueShift"\x00\x12>\n\rSetValueShift\x12\x15.recording.ValueShift\x1a\x14.sdr.datatypes.Empty"\x00\x12M\n\x14GetValueShiftInitial\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x15.recording.ValueShift"\x00\x12R\n\x13GetValueShiftOffset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1b.recording.ValueShiftOffset"\x00\x12J\n\x13SetValueShiftOffset\x12\x1b.recording.ValueShiftOffset\x1a\x14.sdr.datatypes.Empty"\x00\x12J\n\x0fGetAverageShift\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x17.recording.AverageShift"\x00\x12\x42\n\x0fSetAverageShift\x12\x17.recording.AverageShift\x1a\x14.sdr.datatypes.Empty"\x00\x12V\n\x15GetConditioningMatrix\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1d.recording.ConditioningMatrix"\x00\x12N\n\x15SetConditioningMatrix\x12\x1d.recording.ConditioningMatrix\x1a\x14.sdr.datatypes.Empty"\x00\x12V\n\x15GetConditioningOffset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1d.recording.ConditioningOffset"\x00\x12N\n\x15SetConditioningOffset\x12\x1d.recording.ConditioningOffset\x1a\x14.sdr.datatypes.Empty"\x00\x12L\n\x14GetInternalFrequency\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.recording.Frequency"\x00\x12\x44\n\x14SetInternalFrequency\x12\x14.recording.Frequency\x1a\x14.sdr.datatypes.Empty"\x00\x12P\n\x16GetInternalPhaseOffset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x16.recording.PhaseOffset"\x00\x12H\n\x16SetInternalPhaseOffset\x12\x16.recording.PhaseOffset\x1a\x14.sdr.datatypes.Empty"\x00\x12M\n\x15GetReferenceFrequency\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.recording.Frequency"\x00\x12\x45\n\x15SetReferenceFrequency\x12\x14.recording.Frequency\x1a\x14.sdr.datatypes.Empty"\x00\x12N\n\x11GetReferenceDelay\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x19.recording.ReferenceDelay"\x00\x12\x46\n\x11SetReferenceDelay\x12\x19.recording.ReferenceDelay\x1a\x14.sdr.datatypes.Empty"\x00\x12H\n\x0eGetStateConfig\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x16.recording.StateConfig"\x00\x12@\n\x0eSetStateConfig\x12\x16.recording.StateConfig\x1a\x14.sdr.datatypes.Empty"\x00\x12H\n\x11GetAveragedResult\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x13.recording.IQResult"\x00\x12\x46\n\x0fGetSingleResult\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x13.recording.IQResult"\x00\x12P\n\x15GetResultMemoryStatus\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x17.recording.MemoryStatus"\x00\x12L\n\x13GetResultMemorySize\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x15.recording.MemorySize"\x00\x12\x43\n\x0fGetResultMemory\x12\x15.recording.MemorySize\x1a\x17.recording.ResultMemory"\x00\x12=\n\x0cGetRawMemory\x12\x15.recording.MemorySize\x1a\x14.recording.RawMemory"\x00\x62\x06proto3'
 )
 
 
-_ENDPOINTINDEX = DESCRIPTOR.message_types_by_name["EndpointIndex"]
 _STATUSREPORT = DESCRIPTOR.message_types_by_name["StatusReport"]
 _INTERFEROMETERMODE = DESCRIPTOR.message_types_by_name["InterferometerMode"]
 _CONTINUOUSMODE = DESCRIPTOR.message_types_by_name["ContinuousMode"]
 _TRIGGER = DESCRIPTOR.message_types_by_name["Trigger"]
 _TRIGGEROFFSET = DESCRIPTOR.message_types_by_name["TriggerOffset"]
 _RECORDINGDURATION = DESCRIPTOR.message_types_by_name["RecordingDuration"]
 _VALUESHIFT = DESCRIPTOR.message_types_by_name["ValueShift"]
@@ -50,27 +37,15 @@
 _IQRESULT = DESCRIPTOR.message_types_by_name["IQResult"]
 _MEMORYSIZE = DESCRIPTOR.message_types_by_name["MemorySize"]
 _MEMORYSTATUS = DESCRIPTOR.message_types_by_name["MemoryStatus"]
 _RESULTMEMORY = DESCRIPTOR.message_types_by_name["ResultMemory"]
 _RAWMEMORY = DESCRIPTOR.message_types_by_name["RawMemory"]
 _CONDITIONINGMATRIX = DESCRIPTOR.message_types_by_name["ConditioningMatrix"]
 _CONDITIONINGOFFSET = DESCRIPTOR.message_types_by_name["ConditioningOffset"]
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
 _TRIGGER_TRIGGERVALUE = _TRIGGER.enum_types_by_name["TriggerValue"]
-EndpointIndex = _reflection.GeneratedProtocolMessageType(
-    "EndpointIndex",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _ENDPOINTINDEX,
-        "__module__": "recording_pb2"
-        # @@protoc_insertion_point(class_scope:recording.EndpointIndex)
-    },
-)
-_sym_db.RegisterMessage(EndpointIndex)
-
 StatusReport = _reflection.GeneratedProtocolMessageType(
     "StatusReport",
     (_message.Message,),
     {
         "DESCRIPTOR": _STATUSREPORT,
         "__module__": "recording_pb2"
         # @@protoc_insertion_point(class_scope:recording.StatusReport)
@@ -283,71 +258,56 @@
         "DESCRIPTOR": _CONDITIONINGOFFSET,
         "__module__": "recording_pb2"
         # @@protoc_insertion_point(class_scope:recording.ConditioningOffset)
     },
 )
 _sym_db.RegisterMessage(ConditioningOffset)
 
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "recording_pb2"
-        # @@protoc_insertion_point(class_scope:recording.Empty)
-    },
-)
-_sym_db.RegisterMessage(Empty)
-
 _RECORDING = DESCRIPTOR.services_by_name["Recording"]
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _ENDPOINTINDEX._serialized_start = 30
-    _ENDPOINTINDEX._serialized_end = 60
-    _STATUSREPORT._serialized_start = 62
-    _STATUSREPORT._serialized_end = 109
-    _INTERFEROMETERMODE._serialized_start = 111
-    _INTERFEROMETERMODE._serialized_end = 199
-    _CONTINUOUSMODE._serialized_start = 201
-    _CONTINUOUSMODE._serialized_end = 281
-    _TRIGGER._serialized_start = 284
-    _TRIGGER._serialized_end = 501
-    _TRIGGER_TRIGGERVALUE._serialized_start = 384
-    _TRIGGER_TRIGGERVALUE._serialized_end = 501
-    _TRIGGEROFFSET._serialized_start = 503
-    _TRIGGEROFFSET._serialized_end = 574
-    _RECORDINGDURATION._serialized_start = 576
-    _RECORDINGDURATION._serialized_end = 651
-    _VALUESHIFT._serialized_start = 653
-    _VALUESHIFT._serialized_end = 721
-    _VALUESHIFTOFFSET._serialized_start = 723
-    _VALUESHIFTOFFSET._serialized_end = 797
-    _AVERAGESHIFT._serialized_start = 799
-    _AVERAGESHIFT._serialized_end = 869
-    _FREQUENCY._serialized_start = 871
-    _FREQUENCY._serialized_end = 938
-    _PHASEOFFSET._serialized_start = 940
-    _PHASEOFFSET._serialized_end = 1009
-    _REFERENCEDELAY._serialized_start = 1011
-    _REFERENCEDELAY._serialized_end = 1083
-    _STATECONFIG._serialized_start = 1085
-    _STATECONFIG._serialized_end = 1192
-    _IQRESULT._serialized_start = 1194
-    _IQRESULT._serialized_end = 1238
-    _MEMORYSIZE._serialized_start = 1240
-    _MEMORYSIZE._serialized_end = 1307
-    _MEMORYSTATUS._serialized_start = 1309
-    _MEMORYSTATUS._serialized_end = 1425
-    _RESULTMEMORY._serialized_start = 1427
-    _RESULTMEMORY._serialized_end = 1477
-    _RAWMEMORY._serialized_start = 1479
-    _RAWMEMORY._serialized_end = 1520
-    _CONDITIONINGMATRIX._serialized_start = 1522
-    _CONDITIONINGMATRIX._serialized_end = 1631
-    _CONDITIONINGOFFSET._serialized_start = 1633
-    _CONDITIONINGOFFSET._serialized_end = 1716
-    _EMPTY._serialized_start = 1718
-    _EMPTY._serialized_end = 1725
-    _RECORDING._serialized_start = 1728
-    _RECORDING._serialized_end = 4642
+    _STATUSREPORT._serialized_start = 47
+    _STATUSREPORT._serialized_end = 94
+    _INTERFEROMETERMODE._serialized_start = 96
+    _INTERFEROMETERMODE._serialized_end = 188
+    _CONTINUOUSMODE._serialized_start = 190
+    _CONTINUOUSMODE._serialized_end = 274
+    _TRIGGER._serialized_start = 277
+    _TRIGGER._serialized_end = 498
+    _TRIGGER_TRIGGERVALUE._serialized_start = 381
+    _TRIGGER_TRIGGERVALUE._serialized_end = 498
+    _TRIGGEROFFSET._serialized_start = 500
+    _TRIGGEROFFSET._serialized_end = 575
+    _RECORDINGDURATION._serialized_start = 577
+    _RECORDINGDURATION._serialized_end = 656
+    _VALUESHIFT._serialized_start = 658
+    _VALUESHIFT._serialized_end = 730
+    _VALUESHIFTOFFSET._serialized_start = 732
+    _VALUESHIFTOFFSET._serialized_end = 810
+    _AVERAGESHIFT._serialized_start = 812
+    _AVERAGESHIFT._serialized_end = 886
+    _FREQUENCY._serialized_start = 888
+    _FREQUENCY._serialized_end = 959
+    _PHASEOFFSET._serialized_start = 961
+    _PHASEOFFSET._serialized_end = 1034
+    _REFERENCEDELAY._serialized_start = 1036
+    _REFERENCEDELAY._serialized_end = 1112
+    _STATECONFIG._serialized_start = 1114
+    _STATECONFIG._serialized_end = 1225
+    _IQRESULT._serialized_start = 1227
+    _IQRESULT._serialized_end = 1271
+    _MEMORYSIZE._serialized_start = 1273
+    _MEMORYSIZE._serialized_end = 1344
+    _MEMORYSTATUS._serialized_start = 1346
+    _MEMORYSTATUS._serialized_end = 1466
+    _RESULTMEMORY._serialized_start = 1468
+    _RESULTMEMORY._serialized_end = 1518
+    _RAWMEMORY._serialized_start = 1520
+    _RAWMEMORY._serialized_end = 1561
+    _CONDITIONINGMATRIX._serialized_start = 1563
+    _CONDITIONINGMATRIX._serialized_end = 1676
+    _CONDITIONINGOFFSET._serialized_start = 1678
+    _CONDITIONINGOFFSET._serialized_end = 1765
+    _RECORDING._serialized_start = 1768
+    _RECORDING._serialized_end = 4850
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/recording_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/recording_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,231 +1,217 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import recording_pb2 as recording__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.recording_pb2 as recording__pb2
 
 
 class RecordingStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Reset = channel.unary_unary(
             "/recording.Recording/Reset",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.ReportStatus = channel.unary_unary(
             "/recording.Recording/ReportStatus",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.StatusReport.FromString,
         )
         self.ResetStatus = channel.unary_unary(
             "/recording.Recording/ResetStatus",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.ResetStatusAll = channel.unary_unary(
             "/recording.Recording/ResetStatusAll",
-            request_serializer=recording__pb2.Empty.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.IsInterferometerMode = channel.unary_unary(
             "/recording.Recording/IsInterferometerMode",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.InterferometerMode.FromString,
         )
         self.SetInterferometerMode = channel.unary_unary(
             "/recording.Recording/SetInterferometerMode",
             request_serializer=recording__pb2.InterferometerMode.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.IsContinuousMode = channel.unary_unary(
             "/recording.Recording/IsContinuousMode",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.ContinuousMode.FromString,
         )
         self.SetContinuousMode = channel.unary_unary(
             "/recording.Recording/SetContinuousMode",
             request_serializer=recording__pb2.ContinuousMode.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetLastTrigger = channel.unary_unary(
             "/recording.Recording/GetLastTrigger",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.Trigger.FromString,
         )
         self.TriggerManually = channel.unary_unary(
             "/recording.Recording/TriggerManually",
             request_serializer=recording__pb2.Trigger.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetTriggerOffset = channel.unary_unary(
             "/recording.Recording/GetTriggerOffset",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.TriggerOffset.FromString,
         )
         self.SetTriggerOffset = channel.unary_unary(
             "/recording.Recording/SetTriggerOffset",
             request_serializer=recording__pb2.TriggerOffset.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetRecordingDuration = channel.unary_unary(
             "/recording.Recording/GetRecordingDuration",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.RecordingDuration.FromString,
         )
         self.SetRecordingDuration = channel.unary_unary(
             "/recording.Recording/SetRecordingDuration",
             request_serializer=recording__pb2.RecordingDuration.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetValueShift = channel.unary_unary(
             "/recording.Recording/GetValueShift",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.ValueShift.FromString,
         )
         self.SetValueShift = channel.unary_unary(
             "/recording.Recording/SetValueShift",
             request_serializer=recording__pb2.ValueShift.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetValueShiftInitial = channel.unary_unary(
             "/recording.Recording/GetValueShiftInitial",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.ValueShift.FromString,
         )
         self.GetValueShiftOffset = channel.unary_unary(
             "/recording.Recording/GetValueShiftOffset",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.ValueShiftOffset.FromString,
         )
         self.SetValueShiftOffset = channel.unary_unary(
             "/recording.Recording/SetValueShiftOffset",
             request_serializer=recording__pb2.ValueShiftOffset.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetAverageShift = channel.unary_unary(
             "/recording.Recording/GetAverageShift",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.AverageShift.FromString,
         )
         self.SetAverageShift = channel.unary_unary(
             "/recording.Recording/SetAverageShift",
             request_serializer=recording__pb2.AverageShift.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetConditioningMatrix = channel.unary_unary(
             "/recording.Recording/GetConditioningMatrix",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.ConditioningMatrix.FromString,
         )
         self.SetConditioningMatrix = channel.unary_unary(
             "/recording.Recording/SetConditioningMatrix",
             request_serializer=recording__pb2.ConditioningMatrix.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetConditioningOffset = channel.unary_unary(
             "/recording.Recording/GetConditioningOffset",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.ConditioningOffset.FromString,
         )
         self.SetConditioningOffset = channel.unary_unary(
             "/recording.Recording/SetConditioningOffset",
             request_serializer=recording__pb2.ConditioningOffset.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetInternalFrequency = channel.unary_unary(
             "/recording.Recording/GetInternalFrequency",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.Frequency.FromString,
         )
         self.SetInternalFrequency = channel.unary_unary(
             "/recording.Recording/SetInternalFrequency",
             request_serializer=recording__pb2.Frequency.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetInternalPhaseOffset = channel.unary_unary(
             "/recording.Recording/GetInternalPhaseOffset",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.PhaseOffset.FromString,
         )
         self.SetInternalPhaseOffset = channel.unary_unary(
             "/recording.Recording/SetInternalPhaseOffset",
             request_serializer=recording__pb2.PhaseOffset.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetReferenceFrequency = channel.unary_unary(
             "/recording.Recording/GetReferenceFrequency",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.Frequency.FromString,
         )
         self.SetReferenceFrequency = channel.unary_unary(
             "/recording.Recording/SetReferenceFrequency",
             request_serializer=recording__pb2.Frequency.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetReferenceDelay = channel.unary_unary(
             "/recording.Recording/GetReferenceDelay",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.ReferenceDelay.FromString,
         )
         self.SetReferenceDelay = channel.unary_unary(
             "/recording.Recording/SetReferenceDelay",
             request_serializer=recording__pb2.ReferenceDelay.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetStateConfig = channel.unary_unary(
             "/recording.Recording/GetStateConfig",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.StateConfig.FromString,
         )
         self.SetStateConfig = channel.unary_unary(
             "/recording.Recording/SetStateConfig",
             request_serializer=recording__pb2.StateConfig.SerializeToString,
-            response_deserializer=recording__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetAveragedResult = channel.unary_unary(
             "/recording.Recording/GetAveragedResult",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.IQResult.FromString,
         )
         self.GetSingleResult = channel.unary_unary(
             "/recording.Recording/GetSingleResult",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.IQResult.FromString,
         )
         self.GetResultMemoryStatus = channel.unary_unary(
             "/recording.Recording/GetResultMemoryStatus",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.MemoryStatus.FromString,
         )
         self.GetResultMemorySize = channel.unary_unary(
             "/recording.Recording/GetResultMemorySize",
-            request_serializer=recording__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=recording__pb2.MemorySize.FromString,
         )
         self.GetResultMemory = channel.unary_unary(
             "/recording.Recording/GetResultMemory",
             request_serializer=recording__pb2.MemorySize.SerializeToString,
             response_deserializer=recording__pb2.ResultMemory.FromString,
         )
@@ -486,205 +472,205 @@
         raise NotImplementedError("Method not implemented!")
 
 
 def add_RecordingServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "Reset": grpc.unary_unary_rpc_method_handler(
             servicer.Reset,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "ReportStatus": grpc.unary_unary_rpc_method_handler(
             servicer.ReportStatus,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.StatusReport.SerializeToString,
         ),
         "ResetStatus": grpc.unary_unary_rpc_method_handler(
             servicer.ResetStatus,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "ResetStatusAll": grpc.unary_unary_rpc_method_handler(
             servicer.ResetStatusAll,
-            request_deserializer=recording__pb2.Empty.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "IsInterferometerMode": grpc.unary_unary_rpc_method_handler(
             servicer.IsInterferometerMode,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.InterferometerMode.SerializeToString,
         ),
         "SetInterferometerMode": grpc.unary_unary_rpc_method_handler(
             servicer.SetInterferometerMode,
             request_deserializer=recording__pb2.InterferometerMode.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "IsContinuousMode": grpc.unary_unary_rpc_method_handler(
             servicer.IsContinuousMode,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.ContinuousMode.SerializeToString,
         ),
         "SetContinuousMode": grpc.unary_unary_rpc_method_handler(
             servicer.SetContinuousMode,
             request_deserializer=recording__pb2.ContinuousMode.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetLastTrigger": grpc.unary_unary_rpc_method_handler(
             servicer.GetLastTrigger,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.Trigger.SerializeToString,
         ),
         "TriggerManually": grpc.unary_unary_rpc_method_handler(
             servicer.TriggerManually,
             request_deserializer=recording__pb2.Trigger.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetTriggerOffset": grpc.unary_unary_rpc_method_handler(
             servicer.GetTriggerOffset,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.TriggerOffset.SerializeToString,
         ),
         "SetTriggerOffset": grpc.unary_unary_rpc_method_handler(
             servicer.SetTriggerOffset,
             request_deserializer=recording__pb2.TriggerOffset.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetRecordingDuration": grpc.unary_unary_rpc_method_handler(
             servicer.GetRecordingDuration,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.RecordingDuration.SerializeToString,
         ),
         "SetRecordingDuration": grpc.unary_unary_rpc_method_handler(
             servicer.SetRecordingDuration,
             request_deserializer=recording__pb2.RecordingDuration.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetValueShift": grpc.unary_unary_rpc_method_handler(
             servicer.GetValueShift,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.ValueShift.SerializeToString,
         ),
         "SetValueShift": grpc.unary_unary_rpc_method_handler(
             servicer.SetValueShift,
             request_deserializer=recording__pb2.ValueShift.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetValueShiftInitial": grpc.unary_unary_rpc_method_handler(
             servicer.GetValueShiftInitial,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.ValueShift.SerializeToString,
         ),
         "GetValueShiftOffset": grpc.unary_unary_rpc_method_handler(
             servicer.GetValueShiftOffset,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.ValueShiftOffset.SerializeToString,
         ),
         "SetValueShiftOffset": grpc.unary_unary_rpc_method_handler(
             servicer.SetValueShiftOffset,
             request_deserializer=recording__pb2.ValueShiftOffset.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetAverageShift": grpc.unary_unary_rpc_method_handler(
             servicer.GetAverageShift,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.AverageShift.SerializeToString,
         ),
         "SetAverageShift": grpc.unary_unary_rpc_method_handler(
             servicer.SetAverageShift,
             request_deserializer=recording__pb2.AverageShift.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetConditioningMatrix": grpc.unary_unary_rpc_method_handler(
             servicer.GetConditioningMatrix,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.ConditioningMatrix.SerializeToString,
         ),
         "SetConditioningMatrix": grpc.unary_unary_rpc_method_handler(
             servicer.SetConditioningMatrix,
             request_deserializer=recording__pb2.ConditioningMatrix.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetConditioningOffset": grpc.unary_unary_rpc_method_handler(
             servicer.GetConditioningOffset,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.ConditioningOffset.SerializeToString,
         ),
         "SetConditioningOffset": grpc.unary_unary_rpc_method_handler(
             servicer.SetConditioningOffset,
             request_deserializer=recording__pb2.ConditioningOffset.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetInternalFrequency": grpc.unary_unary_rpc_method_handler(
             servicer.GetInternalFrequency,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.Frequency.SerializeToString,
         ),
         "SetInternalFrequency": grpc.unary_unary_rpc_method_handler(
             servicer.SetInternalFrequency,
             request_deserializer=recording__pb2.Frequency.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetInternalPhaseOffset": grpc.unary_unary_rpc_method_handler(
             servicer.GetInternalPhaseOffset,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.PhaseOffset.SerializeToString,
         ),
         "SetInternalPhaseOffset": grpc.unary_unary_rpc_method_handler(
             servicer.SetInternalPhaseOffset,
             request_deserializer=recording__pb2.PhaseOffset.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetReferenceFrequency": grpc.unary_unary_rpc_method_handler(
             servicer.GetReferenceFrequency,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.Frequency.SerializeToString,
         ),
         "SetReferenceFrequency": grpc.unary_unary_rpc_method_handler(
             servicer.SetReferenceFrequency,
             request_deserializer=recording__pb2.Frequency.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetReferenceDelay": grpc.unary_unary_rpc_method_handler(
             servicer.GetReferenceDelay,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.ReferenceDelay.SerializeToString,
         ),
         "SetReferenceDelay": grpc.unary_unary_rpc_method_handler(
             servicer.SetReferenceDelay,
             request_deserializer=recording__pb2.ReferenceDelay.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetStateConfig": grpc.unary_unary_rpc_method_handler(
             servicer.GetStateConfig,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.StateConfig.SerializeToString,
         ),
         "SetStateConfig": grpc.unary_unary_rpc_method_handler(
             servicer.SetStateConfig,
             request_deserializer=recording__pb2.StateConfig.FromString,
-            response_serializer=recording__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetAveragedResult": grpc.unary_unary_rpc_method_handler(
             servicer.GetAveragedResult,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.IQResult.SerializeToString,
         ),
         "GetSingleResult": grpc.unary_unary_rpc_method_handler(
             servicer.GetSingleResult,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.IQResult.SerializeToString,
         ),
         "GetResultMemoryStatus": grpc.unary_unary_rpc_method_handler(
             servicer.GetResultMemoryStatus,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.MemoryStatus.SerializeToString,
         ),
         "GetResultMemorySize": grpc.unary_unary_rpc_method_handler(
             servicer.GetResultMemorySize,
-            request_deserializer=recording__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=recording__pb2.MemorySize.SerializeToString,
         ),
         "GetResultMemory": grpc.unary_unary_rpc_method_handler(
             servicer.GetResultMemory,
             request_deserializer=recording__pb2.MemorySize.FromString,
             response_serializer=recording__pb2.ResultMemory.SerializeToString,
         ),
@@ -717,16 +703,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/Reset",
-            recording__pb2.EndpointIndex.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -746,15 +732,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/ReportStatus",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.StatusReport.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -775,16 +761,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/ResetStatus",
-            recording__pb2.EndpointIndex.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -804,16 +790,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/ResetStatusAll",
-            recording__pb2.Empty.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -833,15 +819,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/IsInterferometerMode",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.InterferometerMode.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -863,15 +849,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetInterferometerMode",
             recording__pb2.InterferometerMode.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -891,15 +877,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/IsContinuousMode",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.ContinuousMode.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -921,15 +907,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetContinuousMode",
             recording__pb2.ContinuousMode.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -949,15 +935,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetLastTrigger",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.Trigger.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -979,15 +965,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/TriggerManually",
             recording__pb2.Trigger.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1007,15 +993,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetTriggerOffset",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.TriggerOffset.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1037,15 +1023,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetTriggerOffset",
             recording__pb2.TriggerOffset.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1065,15 +1051,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetRecordingDuration",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.RecordingDuration.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1095,15 +1081,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetRecordingDuration",
             recording__pb2.RecordingDuration.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1123,15 +1109,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetValueShift",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.ValueShift.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1153,15 +1139,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetValueShift",
             recording__pb2.ValueShift.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1181,15 +1167,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetValueShiftInitial",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.ValueShift.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1210,15 +1196,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetValueShiftOffset",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.ValueShiftOffset.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1240,15 +1226,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetValueShiftOffset",
             recording__pb2.ValueShiftOffset.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1268,15 +1254,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetAverageShift",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.AverageShift.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1298,15 +1284,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetAverageShift",
             recording__pb2.AverageShift.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1326,15 +1312,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetConditioningMatrix",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.ConditioningMatrix.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1356,15 +1342,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetConditioningMatrix",
             recording__pb2.ConditioningMatrix.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1384,15 +1370,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetConditioningOffset",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.ConditioningOffset.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1414,15 +1400,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetConditioningOffset",
             recording__pb2.ConditioningOffset.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1442,15 +1428,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetInternalFrequency",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.Frequency.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1472,15 +1458,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetInternalFrequency",
             recording__pb2.Frequency.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1500,15 +1486,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetInternalPhaseOffset",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.PhaseOffset.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1530,15 +1516,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetInternalPhaseOffset",
             recording__pb2.PhaseOffset.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1558,15 +1544,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetReferenceFrequency",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.Frequency.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1588,15 +1574,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetReferenceFrequency",
             recording__pb2.Frequency.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1616,15 +1602,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetReferenceDelay",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.ReferenceDelay.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1646,15 +1632,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetReferenceDelay",
             recording__pb2.ReferenceDelay.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1674,15 +1660,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetStateConfig",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.StateConfig.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1704,15 +1690,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/SetStateConfig",
             recording__pb2.StateConfig.SerializeToString,
-            recording__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1732,15 +1718,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetAveragedResult",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.IQResult.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1761,15 +1747,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetSingleResult",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.IQResult.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1790,15 +1776,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetResultMemoryStatus",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.MemoryStatus.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1819,15 +1805,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/recording.Recording/GetResultMemorySize",
-            recording__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             recording__pb2.MemorySize.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/rfdc_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/rfdc_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,8 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: rfdc.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
@@ -25,16 +10,19 @@
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\nrfdc.proto\x12\x04rfdc"Z\n\x0e\x43onverterIndex\x12\x0c\n\x04tile\x18\x01 \x01(\r\x12\r\n\x05\x62lock\x18\x02 \x01(\r\x12+\n\x0e\x63onverter_type\x18\x03 \x01(\x0e\x32\x13.rfdc.ConverterType"F\n\tTileIndex\x12\x0c\n\x04tile\x18\x01 \x01(\r\x12+\n\x0e\x63onverter_type\x18\x02 \x01(\x0e\x32\x13.rfdc.ConverterType"\x97\x01\n\x0b\x42lockStatus\x12\x11\n\tfrequency\x18\x01 \x01(\r\x12\x14\n\x0c\x61nalogstatus\x18\x02 \x01(\r\x12\x15\n\rdigitalstatus\x18\x03 \x01(\r\x12\x13\n\x0b\x63lockstatus\x18\x04 \x01(\r\x12\x18\n\x10\x66ifoflagsenabled\x18\x05 \x01(\r\x12\x19\n\x11\x66ifoflagsasserted\x18\x06 \x01(\r"?\n\tFrequency\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\r\n\x05value\x18\x02 \x01(\x01"A\n\x0bNyquistZone\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\r\n\x05value\x18\x02 \x01(\r"W\n\nInvSincFIR\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12$\n\x05value\x18\x02 \x01(\x0e\x32\x15.rfdc.InvSincFIR_Enum"K\n\x11ThresholdToUpdate\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x11\n\tthreshold\x18\x02 \x01(\r"J\n\x11InterruptSettings\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x10\n\x08intrmask\x18\x02 \x01(\r";\n\x05Phase\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\r\n\x05value\x18\x02 \x01(\x01"f\n\rMixerSettings\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x1d\n\x04mode\x18\x02 \x01(\x0e\x32\x0f.rfdc.MixerMode\x12\x11\n\tfrequency\x18\x03 \x01(\x01"%\n\x04Mode\x12\x1d\n\x04mode\x18\x01 \x01(\x0e\x32\x0f.rfdc.MixerMode".\n\x08\x44\x61taType\x12"\n\x05value\x18\x01 \x01(\x0e\x32\x13.rfdc.DataType_Enum"D\n\rInterpolation\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x0e\n\x06\x66\x61\x63tor\x18\x02 \x01(\r"A\n\nDecimation\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x0e\n\x06\x66\x61\x63tor\x18\x02 \x01(\r"\x8b\x01\n\x0cStatusReport\x12\x0f\n\x07\x66\x61ilure\x18\x01 \x01(\x08\x12\x0e\n\x06report\x18\x02 \x01(\t\x12+\n\radc_overrange\x18\x03 \x03(\x0b\x32\x14.rfdc.ConverterIndex\x12-\n\x0f\x61\x64\x63_overvoltage\x18\x04 \x03(\x0b\x32\x14.rfdc.ConverterIndex"\x07\n\x05\x45mpty*!\n\rConverterType\x12\x07\n\x03\x41\x44\x43\x10\x00\x12\x07\n\x03\x44\x41\x43\x10\x01*F\n\x0fInvSincFIR_Enum\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x11\n\rFIRST_NYQUIST\x10\x01\x12\x12\n\x0eSECOND_NYQUIST\x10\x02*V\n\tMixerMode\x12\x07\n\x03OFF\x10\x00\x12\x16\n\x12\x43OMPLEX_TO_COMPLEX\x10\x01\x12\x13\n\x0f\x43OMPLEX_TO_REAL\x10\x02\x12\x13\n\x0fREAL_TO_COMPLEX\x10\x03*!\n\rDataType_Enum\x12\x08\n\x04REAL\x10\x00\x12\x06\n\x02IQ\x10\x01\x32\x9c\n\n\x0bRFdcService\x12;\n\x0eGetBlockStatus\x12\x14.rfdc.ConverterIndex\x1a\x11.rfdc.BlockStatus"\x00\x12<\n\x11GetMixerFrequency\x12\x14.rfdc.ConverterIndex\x1a\x0f.rfdc.Frequency"\x00\x12\x33\n\x11SetMixerFrequency\x12\x0f.rfdc.Frequency\x1a\x0b.rfdc.Empty"\x00\x12/\n\x08GetPhase\x12\x14.rfdc.ConverterIndex\x1a\x0b.rfdc.Phase"\x00\x12&\n\x08SetPhase\x12\x0b.rfdc.Phase\x1a\x0b.rfdc.Empty"\x00\x12\x32\n\x0cGetMixerMode\x12\x14.rfdc.ConverterIndex\x1a\n.rfdc.Mode"\x00\x12\x36\n\x10SetMixerSettings\x12\x13.rfdc.MixerSettings\x1a\x0b.rfdc.Empty"\x00\x12\x35\n\x0bGetDataType\x12\x14.rfdc.ConverterIndex\x1a\x0e.rfdc.DataType"\x00\x12?\n\x10GetInterpolation\x12\x14.rfdc.ConverterIndex\x1a\x13.rfdc.Interpolation"\x00\x12\x36\n\x10SetInterpolation\x12\x13.rfdc.Interpolation\x1a\x0b.rfdc.Empty"\x00\x12\x39\n\rGetDecimation\x12\x14.rfdc.ConverterIndex\x1a\x10.rfdc.Decimation"\x00\x12\x30\n\rSetDecimation\x12\x10.rfdc.Decimation\x1a\x0b.rfdc.Empty"\x00\x12\x39\n\rGetInvSincFIR\x12\x14.rfdc.ConverterIndex\x1a\x10.rfdc.InvSincFIR"\x00\x12\x30\n\rSetInvSincFIR\x12\x10.rfdc.InvSincFIR\x1a\x0b.rfdc.Empty"\x00\x12\x41\n\x17SetThresholdStickyClear\x12\x17.rfdc.ThresholdToUpdate\x1a\x0b.rfdc.Empty"\x00\x12)\n\x07StartUp\x12\x0f.rfdc.TileIndex\x1a\x0b.rfdc.Empty"\x00\x12*\n\x08Shutdown\x12\x0f.rfdc.TileIndex\x1a\x0b.rfdc.Empty"\x00\x12\'\n\x05Reset\x12\x0f.rfdc.TileIndex\x1a\x0b.rfdc.Empty"\x00\x12\x35\n\x0eInterruptClear\x12\x14.rfdc.ConverterIndex\x1a\x0b.rfdc.Empty"\x00\x12\x45\n\x12GetInterruptStatus\x12\x14.rfdc.ConverterIndex\x1a\x17.rfdc.InterruptSettings"\x00\x12;\n\x0eGetNyquistZone\x12\x14.rfdc.ConverterIndex\x1a\x11.rfdc.NyquistZone"\x00\x12\x32\n\x0eSetNyquistZone\x12\x11.rfdc.NyquistZone\x1a\x0b.rfdc.Empty"\x00\x12\x31\n\x0cReportStatus\x12\x0b.rfdc.Empty\x1a\x12.rfdc.StatusReport"\x00\x12)\n\x0bResetStatus\x12\x0b.rfdc.Empty\x1a\x0b.rfdc.Empty"\x00\x62\x06proto3'
+    b'\n\nrfdc.proto\x12\x04rfdc\x1a\x0f\x64\x61tatypes.proto"Z\n\x0e\x43onverterIndex\x12\x0c\n\x04tile\x18\x01 \x01(\r\x12\r\n\x05\x62lock\x18\x02 \x01(\r\x12+\n\x0e\x63onverter_type\x18\x03 \x01(\x0e\x32\x13.rfdc.ConverterType"F\n\tTileIndex\x12\x0c\n\x04tile\x18\x01 \x01(\r\x12+\n\x0e\x63onverter_type\x18\x02 \x01(\x0e\x32\x13.rfdc.ConverterType"\x97\x01\n\x0b\x42lockStatus\x12\x11\n\tfrequency\x18\x01 \x01(\x01\x12\x14\n\x0c\x61nalogstatus\x18\x02 \x01(\r\x12\x15\n\rdigitalstatus\x18\x03 \x01(\r\x12\x13\n\x0b\x63lockstatus\x18\x04 \x01(\r\x12\x18\n\x10\x66ifoflagsenabled\x18\x05 \x01(\r\x12\x19\n\x11\x66ifoflagsasserted\x18\x06 \x01(\r"?\n\tFrequency\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\r\n\x05value\x18\x02 \x01(\x01"A\n\x0bNyquistZone\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\r\n\x05value\x18\x02 \x01(\r"W\n\nInvSincFIR\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12$\n\x05value\x18\x02 \x01(\x0e\x32\x15.rfdc.InvSincFIR_Enum"K\n\x11ThresholdToUpdate\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x11\n\tthreshold\x18\x02 \x01(\r"J\n\x11InterruptSettings\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x10\n\x08intrmask\x18\x02 \x01(\r";\n\x05Phase\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\r\n\x05value\x18\x02 \x01(\x01"f\n\rMixerSettings\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x1d\n\x04mode\x18\x02 \x01(\x0e\x32\x0f.rfdc.MixerMode\x12\x11\n\tfrequency\x18\x03 \x01(\x01"%\n\x04Mode\x12\x1d\n\x04mode\x18\x01 \x01(\x0e\x32\x0f.rfdc.MixerMode".\n\x08\x44\x61taType\x12"\n\x05value\x18\x01 \x01(\x0e\x32\x13.rfdc.DataType_Enum"D\n\rInterpolation\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x0e\n\x06\x66\x61\x63tor\x18\x02 \x01(\r"A\n\nDecimation\x12#\n\x05index\x18\x01 \x01(\x0b\x32\x14.rfdc.ConverterIndex\x12\x0e\n\x06\x66\x61\x63tor\x18\x02 \x01(\r"\x8b\x01\n\x0cStatusReport\x12\x0f\n\x07\x66\x61ilure\x18\x01 \x01(\x08\x12\x0e\n\x06report\x18\x02 \x01(\t\x12+\n\radc_overrange\x18\x03 \x03(\x0b\x32\x14.rfdc.ConverterIndex\x12-\n\x0f\x61\x64\x63_overvoltage\x18\x04 \x03(\x0b\x32\x14.rfdc.ConverterIndex*!\n\rConverterType\x12\x07\n\x03\x41\x44\x43\x10\x00\x12\x07\n\x03\x44\x41\x43\x10\x01*F\n\x0fInvSincFIR_Enum\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x11\n\rFIRST_NYQUIST\x10\x01\x12\x12\n\x0eSECOND_NYQUIST\x10\x02*V\n\tMixerMode\x12\x07\n\x03OFF\x10\x00\x12\x16\n\x12\x43OMPLEX_TO_COMPLEX\x10\x01\x12\x13\n\x0f\x43OMPLEX_TO_REAL\x10\x02\x12\x13\n\x0fREAL_TO_COMPLEX\x10\x03*!\n\rDataType_Enum\x12\x08\n\x04REAL\x10\x00\x12\x06\n\x02IQ\x10\x01\x32\xa3\x0b\n\x0bRFdcService\x12;\n\x0eGetBlockStatus\x12\x14.rfdc.ConverterIndex\x1a\x11.rfdc.BlockStatus"\x00\x12<\n\x11GetMixerFrequency\x12\x14.rfdc.ConverterIndex\x1a\x0f.rfdc.Frequency"\x00\x12<\n\x11SetMixerFrequency\x12\x0f.rfdc.Frequency\x1a\x14.sdr.datatypes.Empty"\x00\x12/\n\x08GetPhase\x12\x14.rfdc.ConverterIndex\x1a\x0b.rfdc.Phase"\x00\x12/\n\x08SetPhase\x12\x0b.rfdc.Phase\x1a\x14.sdr.datatypes.Empty"\x00\x12\x32\n\x0cGetMixerMode\x12\x14.rfdc.ConverterIndex\x1a\n.rfdc.Mode"\x00\x12?\n\x10SetMixerSettings\x12\x13.rfdc.MixerSettings\x1a\x14.sdr.datatypes.Empty"\x00\x12\x35\n\x0bGetDataType\x12\x14.rfdc.ConverterIndex\x1a\x0e.rfdc.DataType"\x00\x12?\n\x10GetInterpolation\x12\x14.rfdc.ConverterIndex\x1a\x13.rfdc.Interpolation"\x00\x12?\n\x10SetInterpolation\x12\x13.rfdc.Interpolation\x1a\x14.sdr.datatypes.Empty"\x00\x12\x39\n\rGetDecimation\x12\x14.rfdc.ConverterIndex\x1a\x10.rfdc.Decimation"\x00\x12\x39\n\rSetDecimation\x12\x10.rfdc.Decimation\x1a\x14.sdr.datatypes.Empty"\x00\x12\x39\n\rGetInvSincFIR\x12\x14.rfdc.ConverterIndex\x1a\x10.rfdc.InvSincFIR"\x00\x12\x39\n\rSetInvSincFIR\x12\x10.rfdc.InvSincFIR\x1a\x14.sdr.datatypes.Empty"\x00\x12J\n\x17SetThresholdStickyClear\x12\x17.rfdc.ThresholdToUpdate\x1a\x14.sdr.datatypes.Empty"\x00\x12\x32\n\x07StartUp\x12\x0f.rfdc.TileIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12\x33\n\x08Shutdown\x12\x0f.rfdc.TileIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12\x30\n\x05Reset\x12\x0f.rfdc.TileIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12>\n\x0eInterruptClear\x12\x14.rfdc.ConverterIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12\x45\n\x12GetInterruptStatus\x12\x14.rfdc.ConverterIndex\x1a\x17.rfdc.InterruptSettings"\x00\x12;\n\x0eGetNyquistZone\x12\x14.rfdc.ConverterIndex\x1a\x11.rfdc.NyquistZone"\x00\x12;\n\x0eSetNyquistZone\x12\x11.rfdc.NyquistZone\x1a\x14.sdr.datatypes.Empty"\x00\x12:\n\x0cReportStatus\x12\x14.sdr.datatypes.Empty\x1a\x12.rfdc.StatusReport"\x00\x12;\n\x0bResetStatus\x12\x14.sdr.datatypes.Empty\x1a\x14.sdr.datatypes.Empty"\x00\x62\x06proto3'
 )
 
 _CONVERTERTYPE = DESCRIPTOR.enum_types_by_name["ConverterType"]
 ConverterType = enum_type_wrapper.EnumTypeWrapper(_CONVERTERTYPE)
 _INVSINCFIR_ENUM = DESCRIPTOR.enum_types_by_name["InvSincFIR_Enum"]
 InvSincFIR_Enum = enum_type_wrapper.EnumTypeWrapper(_INVSINCFIR_ENUM)
 _MIXERMODE = DESCRIPTOR.enum_types_by_name["MixerMode"]
@@ -65,15 +53,14 @@
 _PHASE = DESCRIPTOR.message_types_by_name["Phase"]
 _MIXERSETTINGS = DESCRIPTOR.message_types_by_name["MixerSettings"]
 _MODE = DESCRIPTOR.message_types_by_name["Mode"]
 _DATATYPE = DESCRIPTOR.message_types_by_name["DataType"]
 _INTERPOLATION = DESCRIPTOR.message_types_by_name["Interpolation"]
 _DECIMATION = DESCRIPTOR.message_types_by_name["Decimation"]
 _STATUSREPORT = DESCRIPTOR.message_types_by_name["StatusReport"]
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
 ConverterIndex = _reflection.GeneratedProtocolMessageType(
     "ConverterIndex",
     (_message.Message,),
     {
         "DESCRIPTOR": _CONVERTERINDEX,
         "__module__": "rfdc_pb2"
         # @@protoc_insertion_point(class_scope:rfdc.ConverterIndex)
@@ -231,65 +218,52 @@
         "DESCRIPTOR": _STATUSREPORT,
         "__module__": "rfdc_pb2"
         # @@protoc_insertion_point(class_scope:rfdc.StatusReport)
     },
 )
 _sym_db.RegisterMessage(StatusReport)
 
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "rfdc_pb2"
-        # @@protoc_insertion_point(class_scope:rfdc.Empty)
-    },
-)
-_sym_db.RegisterMessage(Empty)
-
 _RFDCSERVICE = DESCRIPTOR.services_by_name["RFdcService"]
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _CONVERTERTYPE._serialized_start = 1252
-    _CONVERTERTYPE._serialized_end = 1285
-    _INVSINCFIR_ENUM._serialized_start = 1287
-    _INVSINCFIR_ENUM._serialized_end = 1357
-    _MIXERMODE._serialized_start = 1359
-    _MIXERMODE._serialized_end = 1445
-    _DATATYPE_ENUM._serialized_start = 1447
-    _DATATYPE_ENUM._serialized_end = 1480
-    _CONVERTERINDEX._serialized_start = 20
-    _CONVERTERINDEX._serialized_end = 110
-    _TILEINDEX._serialized_start = 112
-    _TILEINDEX._serialized_end = 182
-    _BLOCKSTATUS._serialized_start = 185
-    _BLOCKSTATUS._serialized_end = 336
-    _FREQUENCY._serialized_start = 338
-    _FREQUENCY._serialized_end = 401
-    _NYQUISTZONE._serialized_start = 403
-    _NYQUISTZONE._serialized_end = 468
-    _INVSINCFIR._serialized_start = 470
-    _INVSINCFIR._serialized_end = 557
-    _THRESHOLDTOUPDATE._serialized_start = 559
-    _THRESHOLDTOUPDATE._serialized_end = 634
-    _INTERRUPTSETTINGS._serialized_start = 636
-    _INTERRUPTSETTINGS._serialized_end = 710
-    _PHASE._serialized_start = 712
-    _PHASE._serialized_end = 771
-    _MIXERSETTINGS._serialized_start = 773
-    _MIXERSETTINGS._serialized_end = 875
-    _MODE._serialized_start = 877
-    _MODE._serialized_end = 914
-    _DATATYPE._serialized_start = 916
-    _DATATYPE._serialized_end = 962
-    _INTERPOLATION._serialized_start = 964
-    _INTERPOLATION._serialized_end = 1032
-    _DECIMATION._serialized_start = 1034
-    _DECIMATION._serialized_end = 1099
-    _STATUSREPORT._serialized_start = 1102
-    _STATUSREPORT._serialized_end = 1241
-    _EMPTY._serialized_start = 1243
-    _EMPTY._serialized_end = 1250
-    _RFDCSERVICE._serialized_start = 1483
-    _RFDCSERVICE._serialized_end = 2791
+    _CONVERTERTYPE._serialized_start = 1260
+    _CONVERTERTYPE._serialized_end = 1293
+    _INVSINCFIR_ENUM._serialized_start = 1295
+    _INVSINCFIR_ENUM._serialized_end = 1365
+    _MIXERMODE._serialized_start = 1367
+    _MIXERMODE._serialized_end = 1453
+    _DATATYPE_ENUM._serialized_start = 1455
+    _DATATYPE_ENUM._serialized_end = 1488
+    _CONVERTERINDEX._serialized_start = 37
+    _CONVERTERINDEX._serialized_end = 127
+    _TILEINDEX._serialized_start = 129
+    _TILEINDEX._serialized_end = 199
+    _BLOCKSTATUS._serialized_start = 202
+    _BLOCKSTATUS._serialized_end = 353
+    _FREQUENCY._serialized_start = 355
+    _FREQUENCY._serialized_end = 418
+    _NYQUISTZONE._serialized_start = 420
+    _NYQUISTZONE._serialized_end = 485
+    _INVSINCFIR._serialized_start = 487
+    _INVSINCFIR._serialized_end = 574
+    _THRESHOLDTOUPDATE._serialized_start = 576
+    _THRESHOLDTOUPDATE._serialized_end = 651
+    _INTERRUPTSETTINGS._serialized_start = 653
+    _INTERRUPTSETTINGS._serialized_end = 727
+    _PHASE._serialized_start = 729
+    _PHASE._serialized_end = 788
+    _MIXERSETTINGS._serialized_start = 790
+    _MIXERSETTINGS._serialized_end = 892
+    _MODE._serialized_start = 894
+    _MODE._serialized_end = 931
+    _DATATYPE._serialized_start = 933
+    _DATATYPE._serialized_end = 979
+    _INTERPOLATION._serialized_start = 981
+    _INTERPOLATION._serialized_end = 1049
+    _DECIMATION._serialized_start = 1051
+    _DECIMATION._serialized_end = 1116
+    _STATUSREPORT._serialized_start = 1119
+    _STATUSREPORT._serialized_end = 1258
+    _RFDCSERVICE._serialized_start = 1491
+    _RFDCSERVICE._serialized_end = 2934
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/rfdc_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/rfdc_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import rfdc_pb2 as rfdc__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.rfdc_pb2 as rfdc__pb2
 
 
 class RFdcServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
@@ -38,120 +24,120 @@
             "/rfdc.RFdcService/GetMixerFrequency",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.Frequency.FromString,
         )
         self.SetMixerFrequency = channel.unary_unary(
             "/rfdc.RFdcService/SetMixerFrequency",
             request_serializer=rfdc__pb2.Frequency.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetPhase = channel.unary_unary(
             "/rfdc.RFdcService/GetPhase",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.Phase.FromString,
         )
         self.SetPhase = channel.unary_unary(
             "/rfdc.RFdcService/SetPhase",
             request_serializer=rfdc__pb2.Phase.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetMixerMode = channel.unary_unary(
             "/rfdc.RFdcService/GetMixerMode",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.Mode.FromString,
         )
         self.SetMixerSettings = channel.unary_unary(
             "/rfdc.RFdcService/SetMixerSettings",
             request_serializer=rfdc__pb2.MixerSettings.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetDataType = channel.unary_unary(
             "/rfdc.RFdcService/GetDataType",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.DataType.FromString,
         )
         self.GetInterpolation = channel.unary_unary(
             "/rfdc.RFdcService/GetInterpolation",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.Interpolation.FromString,
         )
         self.SetInterpolation = channel.unary_unary(
             "/rfdc.RFdcService/SetInterpolation",
             request_serializer=rfdc__pb2.Interpolation.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetDecimation = channel.unary_unary(
             "/rfdc.RFdcService/GetDecimation",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.Decimation.FromString,
         )
         self.SetDecimation = channel.unary_unary(
             "/rfdc.RFdcService/SetDecimation",
             request_serializer=rfdc__pb2.Decimation.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetInvSincFIR = channel.unary_unary(
             "/rfdc.RFdcService/GetInvSincFIR",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.InvSincFIR.FromString,
         )
         self.SetInvSincFIR = channel.unary_unary(
             "/rfdc.RFdcService/SetInvSincFIR",
             request_serializer=rfdc__pb2.InvSincFIR.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.SetThresholdStickyClear = channel.unary_unary(
             "/rfdc.RFdcService/SetThresholdStickyClear",
             request_serializer=rfdc__pb2.ThresholdToUpdate.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.StartUp = channel.unary_unary(
             "/rfdc.RFdcService/StartUp",
             request_serializer=rfdc__pb2.TileIndex.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.Shutdown = channel.unary_unary(
             "/rfdc.RFdcService/Shutdown",
             request_serializer=rfdc__pb2.TileIndex.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.Reset = channel.unary_unary(
             "/rfdc.RFdcService/Reset",
             request_serializer=rfdc__pb2.TileIndex.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.InterruptClear = channel.unary_unary(
             "/rfdc.RFdcService/InterruptClear",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetInterruptStatus = channel.unary_unary(
             "/rfdc.RFdcService/GetInterruptStatus",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.InterruptSettings.FromString,
         )
         self.GetNyquistZone = channel.unary_unary(
             "/rfdc.RFdcService/GetNyquistZone",
             request_serializer=rfdc__pb2.ConverterIndex.SerializeToString,
             response_deserializer=rfdc__pb2.NyquistZone.FromString,
         )
         self.SetNyquistZone = channel.unary_unary(
             "/rfdc.RFdcService/SetNyquistZone",
             request_serializer=rfdc__pb2.NyquistZone.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.ReportStatus = channel.unary_unary(
             "/rfdc.RFdcService/ReportStatus",
-            request_serializer=rfdc__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=rfdc__pb2.StatusReport.FromString,
         )
         self.ResetStatus = channel.unary_unary(
             "/rfdc.RFdcService/ResetStatus",
-            request_serializer=rfdc__pb2.Empty.SerializeToString,
-            response_deserializer=rfdc__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
 
 
 class RFdcServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetBlockStatus(self, request, context):
@@ -321,120 +307,120 @@
             servicer.GetMixerFrequency,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.Frequency.SerializeToString,
         ),
         "SetMixerFrequency": grpc.unary_unary_rpc_method_handler(
             servicer.SetMixerFrequency,
             request_deserializer=rfdc__pb2.Frequency.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetPhase": grpc.unary_unary_rpc_method_handler(
             servicer.GetPhase,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.Phase.SerializeToString,
         ),
         "SetPhase": grpc.unary_unary_rpc_method_handler(
             servicer.SetPhase,
             request_deserializer=rfdc__pb2.Phase.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetMixerMode": grpc.unary_unary_rpc_method_handler(
             servicer.GetMixerMode,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.Mode.SerializeToString,
         ),
         "SetMixerSettings": grpc.unary_unary_rpc_method_handler(
             servicer.SetMixerSettings,
             request_deserializer=rfdc__pb2.MixerSettings.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetDataType": grpc.unary_unary_rpc_method_handler(
             servicer.GetDataType,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.DataType.SerializeToString,
         ),
         "GetInterpolation": grpc.unary_unary_rpc_method_handler(
             servicer.GetInterpolation,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.Interpolation.SerializeToString,
         ),
         "SetInterpolation": grpc.unary_unary_rpc_method_handler(
             servicer.SetInterpolation,
             request_deserializer=rfdc__pb2.Interpolation.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetDecimation": grpc.unary_unary_rpc_method_handler(
             servicer.GetDecimation,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.Decimation.SerializeToString,
         ),
         "SetDecimation": grpc.unary_unary_rpc_method_handler(
             servicer.SetDecimation,
             request_deserializer=rfdc__pb2.Decimation.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetInvSincFIR": grpc.unary_unary_rpc_method_handler(
             servicer.GetInvSincFIR,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.InvSincFIR.SerializeToString,
         ),
         "SetInvSincFIR": grpc.unary_unary_rpc_method_handler(
             servicer.SetInvSincFIR,
             request_deserializer=rfdc__pb2.InvSincFIR.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "SetThresholdStickyClear": grpc.unary_unary_rpc_method_handler(
             servicer.SetThresholdStickyClear,
             request_deserializer=rfdc__pb2.ThresholdToUpdate.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "StartUp": grpc.unary_unary_rpc_method_handler(
             servicer.StartUp,
             request_deserializer=rfdc__pb2.TileIndex.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "Shutdown": grpc.unary_unary_rpc_method_handler(
             servicer.Shutdown,
             request_deserializer=rfdc__pb2.TileIndex.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "Reset": grpc.unary_unary_rpc_method_handler(
             servicer.Reset,
             request_deserializer=rfdc__pb2.TileIndex.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "InterruptClear": grpc.unary_unary_rpc_method_handler(
             servicer.InterruptClear,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetInterruptStatus": grpc.unary_unary_rpc_method_handler(
             servicer.GetInterruptStatus,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.InterruptSettings.SerializeToString,
         ),
         "GetNyquistZone": grpc.unary_unary_rpc_method_handler(
             servicer.GetNyquistZone,
             request_deserializer=rfdc__pb2.ConverterIndex.FromString,
             response_serializer=rfdc__pb2.NyquistZone.SerializeToString,
         ),
         "SetNyquistZone": grpc.unary_unary_rpc_method_handler(
             servicer.SetNyquistZone,
             request_deserializer=rfdc__pb2.NyquistZone.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "ReportStatus": grpc.unary_unary_rpc_method_handler(
             servicer.ReportStatus,
-            request_deserializer=rfdc__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=rfdc__pb2.StatusReport.SerializeToString,
         ),
         "ResetStatus": grpc.unary_unary_rpc_method_handler(
             servicer.ResetStatus,
-            request_deserializer=rfdc__pb2.Empty.FromString,
-            response_serializer=rfdc__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "rfdc.RFdcService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
@@ -515,15 +501,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetMixerFrequency",
             rfdc__pb2.Frequency.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -573,15 +559,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetPhase",
             rfdc__pb2.Phase.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -631,15 +617,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetMixerSettings",
             rfdc__pb2.MixerSettings.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -718,15 +704,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetInterpolation",
             rfdc__pb2.Interpolation.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -776,15 +762,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetDecimation",
             rfdc__pb2.Decimation.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -834,15 +820,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetInvSincFIR",
             rfdc__pb2.InvSincFIR.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -863,15 +849,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetThresholdStickyClear",
             rfdc__pb2.ThresholdToUpdate.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -892,15 +878,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/StartUp",
             rfdc__pb2.TileIndex.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -921,15 +907,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/Shutdown",
             rfdc__pb2.TileIndex.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -950,15 +936,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/Reset",
             rfdc__pb2.TileIndex.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -979,15 +965,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/InterruptClear",
             rfdc__pb2.ConverterIndex.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1066,15 +1052,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/SetNyquistZone",
             rfdc__pb2.NyquistZone.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -1094,15 +1080,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/ReportStatus",
-            rfdc__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             rfdc__pb2.StatusReport.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -1123,16 +1109,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/rfdc.RFdcService/ResetStatus",
-            rfdc__pb2.Empty.SerializeToString,
-            rfdc__pb2.Empty.FromString,
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/sequencer_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/pulsegen_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,156 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sequencer.proto
+# source: pulsegen.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0fsequencer.proto\x12\tsequencer"\x1e\n\rEndpointIndex\x12\r\n\x05value\x18\x01 \x01(\r"\x15\n\x04\x42ool\x12\r\n\x05value\x18\x01 \x01(\x08"A\n\x07\x41verage\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.sequencer.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"0\n\rRegisterIndex\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\r\x12\r\n\x05index\x18\x02 \x01(\r"B\n\x08Register\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.sequencer.RegisterIndex\x12\r\n\x05value\x18\x02 \x01(\r"\x1c\n\x0cRegisterList\x12\x0c\n\x04list\x18\x01 \x03(\r"H\n\x0eProgramCounter\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.sequencer.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\r"[\n\x05\x44\x65lay\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.sequencer.EndpointIndex\x12\x0b\n\x03reg\x18\x02 \x01(\r\x12\x0c\n\x04time\x18\x03 \x01(\x01\x12\x0e\n\x06\x63ycles\x18\x04 \x01(\r"]\n\x07Program\x12\'\n\x05index\x18\x01 \x01(\x0b\x32\x18.sequencer.EndpointIndex\x12\x14\n\x0cprogram_data\x18\x02 \x03(\r\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t"d\n\x0cStatusReport\x12\x0c\n\x04\x62usy\x18\x01 \x01(\x08\x12\x0f\n\x07relaxed\x18\x02 \x01(\x08\x12\x14\n\x0cwait_on_sync\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\t\x12\x10\n\x08warnings\x18\x05 \x03(\t"\x07\n\x05\x45mpty2\xa0\x08\n\x10SequencerService\x12\x36\n\x07GetBusy\x12\x18.sequencer.EndpointIndex\x1a\x0f.sequencer.Bool"\x00\x12\x39\n\nGetRelaxed\x12\x18.sequencer.EndpointIndex\x1a\x0f.sequencer.Bool"\x00\x12=\n\x0bGetAverages\x12\x18.sequencer.EndpointIndex\x1a\x12.sequencer.Average"\x00\x12\x35\n\x0bSetAverages\x12\x12.sequencer.Average\x1a\x10.sequencer.Empty"\x00\x12J\n\x11GetProgramCounter\x12\x18.sequencer.EndpointIndex\x1a\x19.sequencer.ProgramCounter"\x00\x12>\n\x0bGetRegister\x12\x18.sequencer.RegisterIndex\x1a\x13.sequencer.Register"\x00\x12\x36\n\x0bSetRegister\x12\x13.sequencer.Register\x1a\x10.sequencer.Empty"\x00\x12\x46\n\x0fGetAllRegisters\x12\x18.sequencer.EndpointIndex\x1a\x17.sequencer.RegisterList"\x00\x12\x30\n\x08SetDelay\x12\x10.sequencer.Delay\x1a\x10.sequencer.Empty"\x00\x12\x35\n\x0bLoadProgram\x12\x12.sequencer.Program\x1a\x10.sequencer.Empty"\x00\x12\x38\n\x07StartAt\x12\x19.sequencer.ProgramCounter\x1a\x10.sequencer.Empty"\x00\x12H\n\x0fGetStartAddress\x12\x18.sequencer.EndpointIndex\x1a\x19.sequencer.ProgramCounter"\x00\x12@\n\x0fSetStartAddress\x12\x19.sequencer.ProgramCounter\x1a\x10.sequencer.Empty"\x00\x12\x36\n\x06Resume\x12\x18.sequencer.EndpointIndex\x1a\x10.sequencer.Empty"\x00\x12\x35\n\x05Reset\x12\x18.sequencer.EndpointIndex\x1a\x10.sequencer.Empty"\x00\x12\x34\n\x04Stop\x12\x18.sequencer.EndpointIndex\x1a\x10.sequencer.Empty"\x00\x12\x43\n\x0cReportStatus\x12\x18.sequencer.EndpointIndex\x1a\x17.sequencer.StatusReport"\x00\x62\x06proto3'
-)
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
 
 
-_ENDPOINTINDEX = DESCRIPTOR.message_types_by_name["EndpointIndex"]
-_BOOL = DESCRIPTOR.message_types_by_name["Bool"]
-_AVERAGE = DESCRIPTOR.message_types_by_name["Average"]
-_REGISTERINDEX = DESCRIPTOR.message_types_by_name["RegisterIndex"]
-_REGISTER = DESCRIPTOR.message_types_by_name["Register"]
-_REGISTERLIST = DESCRIPTOR.message_types_by_name["RegisterList"]
-_PROGRAMCOUNTER = DESCRIPTOR.message_types_by_name["ProgramCounter"]
-_DELAY = DESCRIPTOR.message_types_by_name["Delay"]
-_PROGRAM = DESCRIPTOR.message_types_by_name["Program"]
-_STATUSREPORT = DESCRIPTOR.message_types_by_name["StatusReport"]
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
-EndpointIndex = _reflection.GeneratedProtocolMessageType(
-    "EndpointIndex",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _ENDPOINTINDEX,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.EndpointIndex)
-    },
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x0epulsegen.proto\x12\x08pulsegen\x1a\x0f\x64\x61tatypes.proto" \n\x0fTriggerSetIndex\x12\r\n\x05value\x18\x01 \x01(\r"c\n\x08IndexSet\x12,\n\x06\x63index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12)\n\x06tindex\x18\x02 \x01(\x0b\x32\x19.pulsegen.TriggerSetIndex"H\n\tFrequency\x12,\n\x06\x63index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\r\n\x05value\x18\x02 \x01(\x01"h\n\x14\x41mplitudeCalibration\x12,\n\x06\x63index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x10\n\x08i_factor\x18\x02 \x01(\x01\x12\x10\n\x08q_factor\x18\x03 \x01(\x01"?\n\x0bPhaseOffset\x12!\n\x05index\x18\x01 \x01(\x0b\x32\x12.pulsegen.IndexSet\x12\r\n\x05value\x18\x02 \x01(\x01"<\n\x08\x44uration\x12!\n\x05index\x18\x01 \x01(\x0b\x32\x12.pulsegen.IndexSet\x12\r\n\x05value\x18\x02 \x01(\x01";\n\x07\x41\x64\x64ress\x12!\n\x05index\x18\x01 \x01(\x0b\x32\x12.pulsegen.IndexSet\x12\r\n\x05value\x18\x02 \x01(\r"\x82\x01\n\x05Pulse\x12!\n\x05index\x18\x01 \x01(\x0b\x32\x12.pulsegen.IndexSet\x12\t\n\x01i\x18\x02 \x03(\x01\x12\t\n\x01q\x18\x03 \x03(\x01\x12\r\n\x05phase\x18\x04 \x01(\x01\x12\x0e\n\x06offset\x18\x05 \x01(\x01\x12\x0c\n\x04hold\x18\x06 \x01(\x08\x12\x13\n\x0bshift_phase\x18\x07 \x01(\x08"O\n\x0bStatusFlags\x12,\n\x06\x63index\x18\x01 \x01(\x0b\x32\x1c.sdr.datatypes.EndpointIndex\x12\x12\n\nsaturation\x18\x02 \x01(\x08\x32\x90\n\n\x0fPulseGenService\x12\x46\n\x0fGetNCOFrequency\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x13.pulsegen.Frequency"\x00\x12>\n\x0fSetNCOFrequency\x12\x13.pulsegen.Frequency\x1a\x14.sdr.datatypes.Empty"\x00\x12=\n\x05Reset\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12K\n\x13ResetEnvelopeMemory\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x12Y\n\x17GetAmplitudeCalibration\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x1e.pulsegen.AmplitudeCalibration"\x00\x12Q\n\x17SetAmplitudeCalibration\x12\x1e.pulsegen.AmplitudeCalibration\x1a\x14.sdr.datatypes.Empty"\x00\x12=\n\x0eGetPhaseOffset\x12\x12.pulsegen.IndexSet\x1a\x15.pulsegen.PhaseOffset"\x00\x12?\n\x0eSetPhaseOffset\x12\x15.pulsegen.PhaseOffset\x1a\x14.sdr.datatypes.Empty"\x00\x12G\n\x0eGetGlobalPhase\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x15.pulsegen.PhaseOffset"\x00\x12\x37\n\x0bGetDuration\x12\x12.pulsegen.IndexSet\x1a\x12.pulsegen.Duration"\x00\x12\x39\n\x0bSetDuration\x12\x12.pulsegen.Duration\x1a\x14.sdr.datatypes.Empty"\x00\x12;\n\x10GetStartAddressI\x12\x12.pulsegen.IndexSet\x1a\x11.pulsegen.Address"\x00\x12=\n\x10SetStartAddressI\x12\x11.pulsegen.Address\x1a\x14.sdr.datatypes.Empty"\x00\x12;\n\x10GetStartAddressQ\x12\x12.pulsegen.IndexSet\x1a\x11.pulsegen.Address"\x00\x12=\n\x10SetStartAddressQ\x12\x11.pulsegen.Address\x1a\x14.sdr.datatypes.Empty"\x00\x12=\n\x0fTriggerManually\x12\x12.pulsegen.IndexSet\x1a\x14.sdr.datatypes.Empty"\x00\x12\x34\n\tLoadPulse\x12\x0f.pulsegen.Pulse\x1a\x14.sdr.datatypes.Empty"\x00\x12G\n\x0eGetStatusFlags\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x15.pulsegen.StatusFlags"\x00\x12H\n\x10ResetStatusFlags\x12\x1c.sdr.datatypes.EndpointIndex\x1a\x14.sdr.datatypes.Empty"\x00\x62\x06proto3'
 )
-_sym_db.RegisterMessage(EndpointIndex)
 
-Bool = _reflection.GeneratedProtocolMessageType(
-    "Bool",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _BOOL,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.Bool)
-    },
-)
-_sym_db.RegisterMessage(Bool)
 
-Average = _reflection.GeneratedProtocolMessageType(
-    "Average",
+_TRIGGERSETINDEX = DESCRIPTOR.message_types_by_name["TriggerSetIndex"]
+_INDEXSET = DESCRIPTOR.message_types_by_name["IndexSet"]
+_FREQUENCY = DESCRIPTOR.message_types_by_name["Frequency"]
+_AMPLITUDECALIBRATION = DESCRIPTOR.message_types_by_name["AmplitudeCalibration"]
+_PHASEOFFSET = DESCRIPTOR.message_types_by_name["PhaseOffset"]
+_DURATION = DESCRIPTOR.message_types_by_name["Duration"]
+_ADDRESS = DESCRIPTOR.message_types_by_name["Address"]
+_PULSE = DESCRIPTOR.message_types_by_name["Pulse"]
+_STATUSFLAGS = DESCRIPTOR.message_types_by_name["StatusFlags"]
+TriggerSetIndex = _reflection.GeneratedProtocolMessageType(
+    "TriggerSetIndex",
     (_message.Message,),
     {
-        "DESCRIPTOR": _AVERAGE,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.Average)
+        "DESCRIPTOR": _TRIGGERSETINDEX,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.TriggerSetIndex)
     },
 )
-_sym_db.RegisterMessage(Average)
+_sym_db.RegisterMessage(TriggerSetIndex)
 
-RegisterIndex = _reflection.GeneratedProtocolMessageType(
-    "RegisterIndex",
+IndexSet = _reflection.GeneratedProtocolMessageType(
+    "IndexSet",
     (_message.Message,),
     {
-        "DESCRIPTOR": _REGISTERINDEX,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.RegisterIndex)
+        "DESCRIPTOR": _INDEXSET,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.IndexSet)
     },
 )
-_sym_db.RegisterMessage(RegisterIndex)
+_sym_db.RegisterMessage(IndexSet)
 
-Register = _reflection.GeneratedProtocolMessageType(
-    "Register",
+Frequency = _reflection.GeneratedProtocolMessageType(
+    "Frequency",
     (_message.Message,),
     {
-        "DESCRIPTOR": _REGISTER,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.Register)
+        "DESCRIPTOR": _FREQUENCY,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.Frequency)
     },
 )
-_sym_db.RegisterMessage(Register)
+_sym_db.RegisterMessage(Frequency)
 
-RegisterList = _reflection.GeneratedProtocolMessageType(
-    "RegisterList",
+AmplitudeCalibration = _reflection.GeneratedProtocolMessageType(
+    "AmplitudeCalibration",
     (_message.Message,),
     {
-        "DESCRIPTOR": _REGISTERLIST,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.RegisterList)
+        "DESCRIPTOR": _AMPLITUDECALIBRATION,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.AmplitudeCalibration)
     },
 )
-_sym_db.RegisterMessage(RegisterList)
+_sym_db.RegisterMessage(AmplitudeCalibration)
 
-ProgramCounter = _reflection.GeneratedProtocolMessageType(
-    "ProgramCounter",
+PhaseOffset = _reflection.GeneratedProtocolMessageType(
+    "PhaseOffset",
     (_message.Message,),
     {
-        "DESCRIPTOR": _PROGRAMCOUNTER,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.ProgramCounter)
+        "DESCRIPTOR": _PHASEOFFSET,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.PhaseOffset)
     },
 )
-_sym_db.RegisterMessage(ProgramCounter)
+_sym_db.RegisterMessage(PhaseOffset)
 
-Delay = _reflection.GeneratedProtocolMessageType(
-    "Delay",
+Duration = _reflection.GeneratedProtocolMessageType(
+    "Duration",
     (_message.Message,),
     {
-        "DESCRIPTOR": _DELAY,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.Delay)
+        "DESCRIPTOR": _DURATION,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.Duration)
     },
 )
-_sym_db.RegisterMessage(Delay)
+_sym_db.RegisterMessage(Duration)
 
-Program = _reflection.GeneratedProtocolMessageType(
-    "Program",
+Address = _reflection.GeneratedProtocolMessageType(
+    "Address",
     (_message.Message,),
     {
-        "DESCRIPTOR": _PROGRAM,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.Program)
+        "DESCRIPTOR": _ADDRESS,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.Address)
     },
 )
-_sym_db.RegisterMessage(Program)
+_sym_db.RegisterMessage(Address)
 
-StatusReport = _reflection.GeneratedProtocolMessageType(
-    "StatusReport",
+Pulse = _reflection.GeneratedProtocolMessageType(
+    "Pulse",
     (_message.Message,),
     {
-        "DESCRIPTOR": _STATUSREPORT,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.StatusReport)
+        "DESCRIPTOR": _PULSE,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.Pulse)
     },
 )
-_sym_db.RegisterMessage(StatusReport)
+_sym_db.RegisterMessage(Pulse)
 
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
+StatusFlags = _reflection.GeneratedProtocolMessageType(
+    "StatusFlags",
     (_message.Message,),
     {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "sequencer_pb2"
-        # @@protoc_insertion_point(class_scope:sequencer.Empty)
+        "DESCRIPTOR": _STATUSFLAGS,
+        "__module__": "pulsegen_pb2"
+        # @@protoc_insertion_point(class_scope:pulsegen.StatusFlags)
     },
 )
-_sym_db.RegisterMessage(Empty)
+_sym_db.RegisterMessage(StatusFlags)
 
-_SEQUENCERSERVICE = DESCRIPTOR.services_by_name["SequencerService"]
+_PULSEGENSERVICE = DESCRIPTOR.services_by_name["PulseGenService"]
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _ENDPOINTINDEX._serialized_start = 30
-    _ENDPOINTINDEX._serialized_end = 60
-    _BOOL._serialized_start = 62
-    _BOOL._serialized_end = 83
-    _AVERAGE._serialized_start = 85
-    _AVERAGE._serialized_end = 150
-    _REGISTERINDEX._serialized_start = 152
-    _REGISTERINDEX._serialized_end = 200
-    _REGISTER._serialized_start = 202
-    _REGISTER._serialized_end = 268
-    _REGISTERLIST._serialized_start = 270
-    _REGISTERLIST._serialized_end = 298
-    _PROGRAMCOUNTER._serialized_start = 300
-    _PROGRAMCOUNTER._serialized_end = 372
-    _DELAY._serialized_start = 374
-    _DELAY._serialized_end = 465
-    _PROGRAM._serialized_start = 467
-    _PROGRAM._serialized_end = 560
-    _STATUSREPORT._serialized_start = 562
-    _STATUSREPORT._serialized_end = 662
-    _EMPTY._serialized_start = 664
-    _EMPTY._serialized_end = 671
-    _SEQUENCERSERVICE._serialized_start = 674
-    _SEQUENCERSERVICE._serialized_end = 1730
+    _TRIGGERSETINDEX._serialized_start = 45
+    _TRIGGERSETINDEX._serialized_end = 77
+    _INDEXSET._serialized_start = 79
+    _INDEXSET._serialized_end = 178
+    _FREQUENCY._serialized_start = 180
+    _FREQUENCY._serialized_end = 252
+    _AMPLITUDECALIBRATION._serialized_start = 254
+    _AMPLITUDECALIBRATION._serialized_end = 358
+    _PHASEOFFSET._serialized_start = 360
+    _PHASEOFFSET._serialized_end = 423
+    _DURATION._serialized_start = 425
+    _DURATION._serialized_end = 485
+    _ADDRESS._serialized_start = 487
+    _ADDRESS._serialized_end = 546
+    _PULSE._serialized_start = 549
+    _PULSE._serialized_end = 679
+    _STATUSFLAGS._serialized_start = 681
+    _STATUSFLAGS._serialized_end = 760
+    _PULSEGENSERVICE._serialized_start = 763
+    _PULSEGENSERVICE._serialized_end = 2059
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/sequencer_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/sequencer_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,107 @@
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import sequencer_pb2 as sequencer__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.sequencer_pb2 as sequencer__pb2
 
 
 class SequencerServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetBusy = channel.unary_unary(
             "/sequencer.SequencerService/GetBusy",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=sequencer__pb2.Bool.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Bool.FromString,
         )
         self.GetRelaxed = channel.unary_unary(
             "/sequencer.SequencerService/GetRelaxed",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=sequencer__pb2.Bool.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Bool.FromString,
         )
         self.GetAverages = channel.unary_unary(
             "/sequencer.SequencerService/GetAverages",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=sequencer__pb2.Average.FromString,
         )
         self.SetAverages = channel.unary_unary(
             "/sequencer.SequencerService/SetAverages",
             request_serializer=sequencer__pb2.Average.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetProgramCounter = channel.unary_unary(
             "/sequencer.SequencerService/GetProgramCounter",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=sequencer__pb2.ProgramCounter.FromString,
         )
         self.GetRegister = channel.unary_unary(
             "/sequencer.SequencerService/GetRegister",
             request_serializer=sequencer__pb2.RegisterIndex.SerializeToString,
             response_deserializer=sequencer__pb2.Register.FromString,
         )
         self.SetRegister = channel.unary_unary(
             "/sequencer.SequencerService/SetRegister",
             request_serializer=sequencer__pb2.Register.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetAllRegisters = channel.unary_unary(
             "/sequencer.SequencerService/GetAllRegisters",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=sequencer__pb2.RegisterList.FromString,
         )
         self.SetDelay = channel.unary_unary(
             "/sequencer.SequencerService/SetDelay",
             request_serializer=sequencer__pb2.Delay.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.LoadProgram = channel.unary_unary(
             "/sequencer.SequencerService/LoadProgram",
             request_serializer=sequencer__pb2.Program.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.StartAt = channel.unary_unary(
             "/sequencer.SequencerService/StartAt",
             request_serializer=sequencer__pb2.ProgramCounter.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetStartAddress = channel.unary_unary(
             "/sequencer.SequencerService/GetStartAddress",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=sequencer__pb2.ProgramCounter.FromString,
         )
         self.SetStartAddress = channel.unary_unary(
             "/sequencer.SequencerService/SetStartAddress",
             request_serializer=sequencer__pb2.ProgramCounter.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.Resume = channel.unary_unary(
             "/sequencer.SequencerService/Resume",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.Reset = channel.unary_unary(
             "/sequencer.SequencerService/Reset",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.Stop = channel.unary_unary(
             "/sequencer.SequencerService/Stop",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
-            response_deserializer=sequencer__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.ReportStatus = channel.unary_unary(
             "/sequencer.SequencerService/ReportStatus",
-            request_serializer=sequencer__pb2.EndpointIndex.SerializeToString,
+            request_serializer=datatypes__pb2.EndpointIndex.SerializeToString,
             response_deserializer=sequencer__pb2.StatusReport.FromString,
         )
 
 
 class SequencerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -222,95 +208,95 @@
         raise NotImplementedError("Method not implemented!")
 
 
 def add_SequencerServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "GetBusy": grpc.unary_unary_rpc_method_handler(
             servicer.GetBusy,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
-            response_serializer=sequencer__pb2.Bool.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Bool.SerializeToString,
         ),
         "GetRelaxed": grpc.unary_unary_rpc_method_handler(
             servicer.GetRelaxed,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
-            response_serializer=sequencer__pb2.Bool.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Bool.SerializeToString,
         ),
         "GetAverages": grpc.unary_unary_rpc_method_handler(
             servicer.GetAverages,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=sequencer__pb2.Average.SerializeToString,
         ),
         "SetAverages": grpc.unary_unary_rpc_method_handler(
             servicer.SetAverages,
             request_deserializer=sequencer__pb2.Average.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetProgramCounter": grpc.unary_unary_rpc_method_handler(
             servicer.GetProgramCounter,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=sequencer__pb2.ProgramCounter.SerializeToString,
         ),
         "GetRegister": grpc.unary_unary_rpc_method_handler(
             servicer.GetRegister,
             request_deserializer=sequencer__pb2.RegisterIndex.FromString,
             response_serializer=sequencer__pb2.Register.SerializeToString,
         ),
         "SetRegister": grpc.unary_unary_rpc_method_handler(
             servicer.SetRegister,
             request_deserializer=sequencer__pb2.Register.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetAllRegisters": grpc.unary_unary_rpc_method_handler(
             servicer.GetAllRegisters,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=sequencer__pb2.RegisterList.SerializeToString,
         ),
         "SetDelay": grpc.unary_unary_rpc_method_handler(
             servicer.SetDelay,
             request_deserializer=sequencer__pb2.Delay.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "LoadProgram": grpc.unary_unary_rpc_method_handler(
             servicer.LoadProgram,
             request_deserializer=sequencer__pb2.Program.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "StartAt": grpc.unary_unary_rpc_method_handler(
             servicer.StartAt,
             request_deserializer=sequencer__pb2.ProgramCounter.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetStartAddress": grpc.unary_unary_rpc_method_handler(
             servicer.GetStartAddress,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=sequencer__pb2.ProgramCounter.SerializeToString,
         ),
         "SetStartAddress": grpc.unary_unary_rpc_method_handler(
             servicer.SetStartAddress,
             request_deserializer=sequencer__pb2.ProgramCounter.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "Resume": grpc.unary_unary_rpc_method_handler(
             servicer.Resume,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "Reset": grpc.unary_unary_rpc_method_handler(
             servicer.Reset,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "Stop": grpc.unary_unary_rpc_method_handler(
             servicer.Stop,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
-            response_serializer=sequencer__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "ReportStatus": grpc.unary_unary_rpc_method_handler(
             servicer.ReportStatus,
-            request_deserializer=sequencer__pb2.EndpointIndex.FromString,
+            request_deserializer=datatypes__pb2.EndpointIndex.FromString,
             response_serializer=sequencer__pb2.StatusReport.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "sequencer.SequencerService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
@@ -333,16 +319,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/GetBusy",
-            sequencer__pb2.EndpointIndex.SerializeToString,
-            sequencer__pb2.Bool.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Bool.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -362,16 +348,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/GetRelaxed",
-            sequencer__pb2.EndpointIndex.SerializeToString,
-            sequencer__pb2.Bool.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Bool.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -391,15 +377,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/GetAverages",
-            sequencer__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             sequencer__pb2.Average.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -421,15 +407,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/SetAverages",
             sequencer__pb2.Average.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -449,15 +435,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/GetProgramCounter",
-            sequencer__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             sequencer__pb2.ProgramCounter.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -508,15 +494,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/SetRegister",
             sequencer__pb2.Register.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -536,15 +522,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/GetAllRegisters",
-            sequencer__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             sequencer__pb2.RegisterList.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -566,15 +552,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/SetDelay",
             sequencer__pb2.Delay.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -595,15 +581,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/LoadProgram",
             sequencer__pb2.Program.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -624,15 +610,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/StartAt",
             sequencer__pb2.ProgramCounter.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -652,15 +638,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/GetStartAddress",
-            sequencer__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             sequencer__pb2.ProgramCounter.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -682,15 +668,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/SetStartAddress",
             sequencer__pb2.ProgramCounter.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -710,16 +696,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/Resume",
-            sequencer__pb2.EndpointIndex.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -739,16 +725,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/Reset",
-            sequencer__pb2.EndpointIndex.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -768,16 +754,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/Stop",
-            sequencer__pb2.EndpointIndex.SerializeToString,
-            sequencer__pb2.Empty.FromString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -797,15 +783,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/sequencer.SequencerService/ReportStatus",
-            sequencer__pb2.EndpointIndex.SerializeToString,
+            datatypes__pb2.EndpointIndex.SerializeToString,
             sequencer__pb2.StatusReport.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/servicehubcontrol_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/servicehubcontrol_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,41 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: servicehubcontrol.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17servicehubcontrol.proto\x12\x11servicehubcontrol"\x07\n\x05\x45mpty"2\n\x03Log\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t"\x18\n\tBuildPath\x12\x0b\n\x03str\x18\x01 \x01(\t"/\n\x08MultiLog\x12#\n\x03log\x18\x01 \x03(\x0b\x32\x16.servicehubcontrol.Log"8\n\nPluginInfo\x12\x13\n\x0bplugin_name\x18\x01 \x01(\t\x12\x15\n\rplugin_config\x18\x02 \x01(\t"4\n\x07Plugins\x12)\n\x02pi\x18\x01 \x03(\x0b\x32\x1d.servicehubcontrol.PluginInfo"B\n\x14\x45ndpointIndexRequest\x12\x13\n\x0bplugin_name\x18\x01 \x01(\t\x12\x15\n\rendpoint_name\x18\x02 \x01(\t"\x15\n\x06String\x12\x0b\n\x03str\x18\x01 \x01(\t"\x1b\n\x0cStringVector\x12\x0b\n\x03str\x18\x01 \x03(\t"\x16\n\x07Integer\x12\x0b\n\x03val\x18\x01 \x01(\x05"W\n\x0ePluginVersions\x12\x16\n\x0e\x64river_version\x18\x01 \x01(\t\x12\x15\n\rproto_version\x18\x02 \x01(\t\x12\x16\n\x0e\x63ommon_version\x18\x03 \x01(\t"_\n\x12ServiceHubVersions\x12\x1a\n\x12servicehub_version\x18\x01 \x01(\t\x12\x15\n\rproto_version\x18\x02 \x01(\t\x12\x16\n\x0e\x63ommon_version\x18\x03 \x01(\t2\xb2\x07\n\x18ServicehubControlService\x12>\n\x06Reload\x12\x18.servicehubcontrol.Empty\x1a\x18.servicehubcontrol.Empty"\x00\x12>\n\x06Reboot\x12\x18.servicehubcontrol.Empty\x1a\x18.servicehubcontrol.Empty"\x00\x12\x42\n\x07GetLogs\x12\x18.servicehubcontrol.Empty\x1a\x1b.servicehubcontrol.MultiLog"\x00\x12G\n\tCleanLogs\x12\x1b.servicehubcontrol.MultiLog\x1a\x1b.servicehubcontrol.MultiLog"\x00\x12\x44\n\nGetPlugins\x12\x18.servicehubcontrol.Empty\x1a\x1a.servicehubcontrol.Plugins"\x00\x12L\n\rGetPluginList\x12\x18.servicehubcontrol.Empty\x1a\x1f.servicehubcontrol.StringVector"\x00\x12T\n\x14GetEndpointsOfPlugin\x12\x19.servicehubcontrol.String\x1a\x1f.servicehubcontrol.StringVector"\x00\x12\x61\n\x18GetEndpointIndexOfPlugin\x12\'.servicehubcontrol.EndpointIndexRequest\x1a\x1a.servicehubcontrol.Integer"\x00\x12R\n\x10GetPluginVersion\x12\x19.servicehubcontrol.String\x1a!.servicehubcontrol.PluginVersions"\x00\x12Y\n\x14GetServiceHubVersion\x12\x18.servicehubcontrol.Empty\x1a%.servicehubcontrol.ServiceHubVersions"\x00\x12L\n\x10\x44umpCoverageData\x12\x18.servicehubcontrol.Empty\x1a\x1c.servicehubcontrol.BuildPath"\x00\x12?\n\x07IsAlive\x12\x18.servicehubcontrol.Empty\x1a\x18.servicehubcontrol.Empty"\x00\x62\x06proto3'
+    b'\n\x17servicehubcontrol.proto\x12\x11servicehubcontrol\x1a\x0f\x64\x61tatypes.proto"2\n\x03Log\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t"\x18\n\tBuildPath\x12\x0b\n\x03str\x18\x01 \x01(\t"/\n\x08MultiLog\x12#\n\x03log\x18\x01 \x03(\x0b\x32\x16.servicehubcontrol.Log"8\n\nPluginInfo\x12\x13\n\x0bplugin_name\x18\x01 \x01(\t\x12\x15\n\rplugin_config\x18\x02 \x01(\t"4\n\x07Plugins\x12)\n\x02pi\x18\x01 \x03(\x0b\x32\x1d.servicehubcontrol.PluginInfo"B\n\x14\x45ndpointIndexRequest\x12\x13\n\x0bplugin_name\x18\x01 \x01(\t\x12\x15\n\rendpoint_name\x18\x02 \x01(\t"\x15\n\x06String\x12\x0b\n\x03str\x18\x01 \x01(\t"\x1b\n\x0cStringVector\x12\x0b\n\x03str\x18\x01 \x03(\t"\x16\n\x07Integer\x12\x0b\n\x03val\x18\x01 \x01(\x05"W\n\x0ePluginVersions\x12\x16\n\x0e\x64river_version\x18\x01 \x01(\t\x12\x15\n\rproto_version\x18\x02 \x01(\t\x12\x16\n\x0e\x63ommon_version\x18\x03 \x01(\t"_\n\x12ServiceHubVersions\x12\x1a\n\x12servicehub_version\x18\x01 \x01(\t\x12\x15\n\rproto_version\x18\x02 \x01(\t\x12\x16\n\x0e\x63ommon_version\x18\x03 \x01(\t2\x86\x07\n\x18ServicehubControlService\x12\x36\n\x06Reload\x12\x14.sdr.datatypes.Empty\x1a\x14.sdr.datatypes.Empty"\x00\x12\x36\n\x06Reboot\x12\x14.sdr.datatypes.Empty\x1a\x14.sdr.datatypes.Empty"\x00\x12>\n\x07GetLogs\x12\x14.sdr.datatypes.Empty\x1a\x1b.servicehubcontrol.MultiLog"\x00\x12G\n\tCleanLogs\x12\x1b.servicehubcontrol.MultiLog\x1a\x1b.servicehubcontrol.MultiLog"\x00\x12@\n\nGetPlugins\x12\x14.sdr.datatypes.Empty\x1a\x1a.servicehubcontrol.Plugins"\x00\x12H\n\rGetPluginList\x12\x14.sdr.datatypes.Empty\x1a\x1f.servicehubcontrol.StringVector"\x00\x12T\n\x14GetEndpointsOfPlugin\x12\x19.servicehubcontrol.String\x1a\x1f.servicehubcontrol.StringVector"\x00\x12\x61\n\x18GetEndpointIndexOfPlugin\x12\'.servicehubcontrol.EndpointIndexRequest\x1a\x1a.servicehubcontrol.Integer"\x00\x12R\n\x10GetPluginVersion\x12\x19.servicehubcontrol.String\x1a!.servicehubcontrol.PluginVersions"\x00\x12U\n\x14GetServiceHubVersion\x12\x14.sdr.datatypes.Empty\x1a%.servicehubcontrol.ServiceHubVersions"\x00\x12H\n\x10\x44umpCoverageData\x12\x14.sdr.datatypes.Empty\x1a\x1c.servicehubcontrol.BuildPath"\x00\x12\x37\n\x07IsAlive\x12\x14.sdr.datatypes.Empty\x1a\x14.sdr.datatypes.Empty"\x00\x62\x06proto3'
 )
 
 
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
 _LOG = DESCRIPTOR.message_types_by_name["Log"]
 _BUILDPATH = DESCRIPTOR.message_types_by_name["BuildPath"]
 _MULTILOG = DESCRIPTOR.message_types_by_name["MultiLog"]
 _PLUGININFO = DESCRIPTOR.message_types_by_name["PluginInfo"]
 _PLUGINS = DESCRIPTOR.message_types_by_name["Plugins"]
 _ENDPOINTINDEXREQUEST = DESCRIPTOR.message_types_by_name["EndpointIndexRequest"]
 _STRING = DESCRIPTOR.message_types_by_name["String"]
 _STRINGVECTOR = DESCRIPTOR.message_types_by_name["StringVector"]
 _INTEGER = DESCRIPTOR.message_types_by_name["Integer"]
 _PLUGINVERSIONS = DESCRIPTOR.message_types_by_name["PluginVersions"]
 _SERVICEHUBVERSIONS = DESCRIPTOR.message_types_by_name["ServiceHubVersions"]
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "servicehubcontrol_pb2"
-        # @@protoc_insertion_point(class_scope:servicehubcontrol.Empty)
-    },
-)
-_sym_db.RegisterMessage(Empty)
-
 Log = _reflection.GeneratedProtocolMessageType(
     "Log",
     (_message.Message,),
     {
         "DESCRIPTOR": _LOG,
         "__module__": "servicehubcontrol_pb2"
         # @@protoc_insertion_point(class_scope:servicehubcontrol.Log)
@@ -177,34 +153,32 @@
 )
 _sym_db.RegisterMessage(ServiceHubVersions)
 
 _SERVICEHUBCONTROLSERVICE = DESCRIPTOR.services_by_name["ServicehubControlService"]
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _EMPTY._serialized_start = 46
-    _EMPTY._serialized_end = 53
-    _LOG._serialized_start = 55
-    _LOG._serialized_end = 105
-    _BUILDPATH._serialized_start = 107
-    _BUILDPATH._serialized_end = 131
-    _MULTILOG._serialized_start = 133
-    _MULTILOG._serialized_end = 180
-    _PLUGININFO._serialized_start = 182
-    _PLUGININFO._serialized_end = 238
-    _PLUGINS._serialized_start = 240
-    _PLUGINS._serialized_end = 292
-    _ENDPOINTINDEXREQUEST._serialized_start = 294
-    _ENDPOINTINDEXREQUEST._serialized_end = 360
-    _STRING._serialized_start = 362
-    _STRING._serialized_end = 383
-    _STRINGVECTOR._serialized_start = 385
-    _STRINGVECTOR._serialized_end = 412
-    _INTEGER._serialized_start = 414
-    _INTEGER._serialized_end = 436
-    _PLUGINVERSIONS._serialized_start = 438
-    _PLUGINVERSIONS._serialized_end = 525
-    _SERVICEHUBVERSIONS._serialized_start = 527
-    _SERVICEHUBVERSIONS._serialized_end = 622
-    _SERVICEHUBCONTROLSERVICE._serialized_start = 625
-    _SERVICEHUBCONTROLSERVICE._serialized_end = 1571
+    _LOG._serialized_start = 63
+    _LOG._serialized_end = 113
+    _BUILDPATH._serialized_start = 115
+    _BUILDPATH._serialized_end = 139
+    _MULTILOG._serialized_start = 141
+    _MULTILOG._serialized_end = 188
+    _PLUGININFO._serialized_start = 190
+    _PLUGININFO._serialized_end = 246
+    _PLUGINS._serialized_start = 248
+    _PLUGINS._serialized_end = 300
+    _ENDPOINTINDEXREQUEST._serialized_start = 302
+    _ENDPOINTINDEXREQUEST._serialized_end = 368
+    _STRING._serialized_start = 370
+    _STRING._serialized_end = 391
+    _STRINGVECTOR._serialized_start = 393
+    _STRINGVECTOR._serialized_end = 420
+    _INTEGER._serialized_start = 422
+    _INTEGER._serialized_end = 444
+    _PLUGINVERSIONS._serialized_start = 446
+    _PLUGINVERSIONS._serialized_end = 533
+    _SERVICEHUBVERSIONS._serialized_start = 535
+    _SERVICEHUBVERSIONS._serialized_end = 630
+    _SERVICEHUBCONTROLSERVICE._serialized_start = 633
+    _SERVICEHUBCONTROLSERVICE._serialized_end = 1535
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/servicehubcontrol_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/servicehubcontrol_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,52 @@
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import servicehubcontrol_pb2 as servicehubcontrol__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.servicehubcontrol_pb2 as servicehubcontrol__pb2
 
 
 class ServicehubControlServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Reload = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/Reload",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
-            response_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.Reboot = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/Reboot",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
-            response_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetLogs = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/GetLogs",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.MultiLog.FromString,
         )
         self.CleanLogs = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/CleanLogs",
             request_serializer=servicehubcontrol__pb2.MultiLog.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.MultiLog.FromString,
         )
         self.GetPlugins = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/GetPlugins",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.Plugins.FromString,
         )
         self.GetPluginList = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/GetPluginList",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.StringVector.FromString,
         )
         self.GetEndpointsOfPlugin = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/GetEndpointsOfPlugin",
             request_serializer=servicehubcontrol__pb2.String.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.StringVector.FromString,
         )
@@ -72,26 +58,26 @@
         self.GetPluginVersion = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/GetPluginVersion",
             request_serializer=servicehubcontrol__pb2.String.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.PluginVersions.FromString,
         )
         self.GetServiceHubVersion = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/GetServiceHubVersion",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.ServiceHubVersions.FromString,
         )
         self.DumpCoverageData = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/DumpCoverageData",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=servicehubcontrol__pb2.BuildPath.FromString,
         )
         self.IsAlive = channel.unary_unary(
             "/servicehubcontrol.ServicehubControlService/IsAlive",
-            request_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
-            response_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
 
 
 class ServicehubControlServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Reload(self, request, context):
@@ -199,63 +185,63 @@
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def DumpCoverageData(self, request, context):
         """*
         @brief Returns the build path and dumps coverage info. Fails if not a coverage build.
 
-        @param Empty
+        @param sdr.datatypes.Empty
         @return Build path
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def IsAlive(self, request, context):
         """*
         @brief Just an RPC that can be called to check if the gRPC server is reachable and responsive.
 
-        @param Empty
-        @return Empty
+        @param sdr.datatypes.Empty
+        @return sdr.datatypes.Empty
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
 def add_ServicehubControlServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "Reload": grpc.unary_unary_rpc_method_handler(
             servicer.Reload,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
-            response_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "Reboot": grpc.unary_unary_rpc_method_handler(
             servicer.Reboot,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
-            response_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetLogs": grpc.unary_unary_rpc_method_handler(
             servicer.GetLogs,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=servicehubcontrol__pb2.MultiLog.SerializeToString,
         ),
         "CleanLogs": grpc.unary_unary_rpc_method_handler(
             servicer.CleanLogs,
             request_deserializer=servicehubcontrol__pb2.MultiLog.FromString,
             response_serializer=servicehubcontrol__pb2.MultiLog.SerializeToString,
         ),
         "GetPlugins": grpc.unary_unary_rpc_method_handler(
             servicer.GetPlugins,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=servicehubcontrol__pb2.Plugins.SerializeToString,
         ),
         "GetPluginList": grpc.unary_unary_rpc_method_handler(
             servicer.GetPluginList,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=servicehubcontrol__pb2.StringVector.SerializeToString,
         ),
         "GetEndpointsOfPlugin": grpc.unary_unary_rpc_method_handler(
             servicer.GetEndpointsOfPlugin,
             request_deserializer=servicehubcontrol__pb2.String.FromString,
             response_serializer=servicehubcontrol__pb2.StringVector.SerializeToString,
         ),
@@ -267,26 +253,26 @@
         "GetPluginVersion": grpc.unary_unary_rpc_method_handler(
             servicer.GetPluginVersion,
             request_deserializer=servicehubcontrol__pb2.String.FromString,
             response_serializer=servicehubcontrol__pb2.PluginVersions.SerializeToString,
         ),
         "GetServiceHubVersion": grpc.unary_unary_rpc_method_handler(
             servicer.GetServiceHubVersion,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=servicehubcontrol__pb2.ServiceHubVersions.SerializeToString,
         ),
         "DumpCoverageData": grpc.unary_unary_rpc_method_handler(
             servicer.DumpCoverageData,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=servicehubcontrol__pb2.BuildPath.SerializeToString,
         ),
         "IsAlive": grpc.unary_unary_rpc_method_handler(
             servicer.IsAlive,
-            request_deserializer=servicehubcontrol__pb2.Empty.FromString,
-            response_serializer=servicehubcontrol__pb2.Empty.SerializeToString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "servicehubcontrol.ServicehubControlService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
@@ -308,16 +294,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/Reload",
-            servicehubcontrol__pb2.Empty.SerializeToString,
-            servicehubcontrol__pb2.Empty.FromString,
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -337,16 +323,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/Reboot",
-            servicehubcontrol__pb2.Empty.SerializeToString,
-            servicehubcontrol__pb2.Empty.FromString,
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -366,15 +352,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/GetLogs",
-            servicehubcontrol__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             servicehubcontrol__pb2.MultiLog.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -424,15 +410,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/GetPlugins",
-            servicehubcontrol__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             servicehubcontrol__pb2.Plugins.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -453,15 +439,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/GetPluginList",
-            servicehubcontrol__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             servicehubcontrol__pb2.StringVector.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -569,15 +555,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/GetServiceHubVersion",
-            servicehubcontrol__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             servicehubcontrol__pb2.ServiceHubVersions.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -598,15 +584,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/DumpCoverageData",
-            servicehubcontrol__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             servicehubcontrol__pb2.BuildPath.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -627,16 +613,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/servicehubcontrol.ServicehubControlService/IsAlive",
-            servicehubcontrol__pb2.Empty.SerializeToString,
-            servicehubcontrol__pb2.Empty.FromString,
+            datatypes__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/taskrunner_pb2.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/taskrunner_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,43 @@
 # -*- coding: utf-8 -*-
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: taskrunner.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x10taskrunner.proto\x12\ntaskrunner"\x07\n\x05\x45mpty"\xba\x01\n\x0bStatusReply\x12\x0f\n\x07\x63hip_id\x18\x01 \x01(\r\x12\x15\n\rfirmware_hash\x18\x02 \x01(\t\x12\x12\n\nbuild_date\x18\x03 \x01(\t\x12\x14\n\x0c\x62uild_commit\x18\x04 \x01(\t\x12\x11\n\ttask_name\x18\x05 \x01(\t\x12\x12\n\ntask_state\x18\x06 \x01(\r\x12\x15\n\rtask_progress\x18\x07 \x01(\r\x12\x1b\n\x13\x64\x61taboxes_available\x18\x08 \x01(\r"\x88\x01\n\x0eTaskStateReply\x12\x0c\n\x04\x62usy\x18\x01 \x01(\x08\x12\x0c\n\x04\x64one\x18\x02 \x01(\x08\x12\x0e\n\x06loaded\x18\x03 \x01(\x08\x12\x0f\n\x07looping\x18\x04 \x01(\x08\x12\x1b\n\x13\x65rror_msg_available\x18\x05 \x01(\x08\x12\x1c\n\x14\x65rror_msg_queue_full\x18\x06 \x01(\x08"0\n\x11\x44\x61taboxReplyINT32\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x05"1\n\x12\x44\x61taboxReplyUINT32\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\r"0\n\x11\x44\x61taboxReplyINT64\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x03"1\n\x12\x44\x61taboxReplyUINT64\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x04",\n\x19GetTaskErrorMessagesReply\x12\x0f\n\x07message\x18\x01 \x03(\t"&\n\x10ParameterRequest\x12\x12\n\nparameters\x18\x01 \x03(\x05"9\n\x10StartTaskRequest\x12\x0f\n\x07looping\x18\x01 \x01(\x08\x12\x14\n\x0cstop_running\x18\x02 \x01(\x08" \n\x0fStopTaskRequest\x12\r\n\x05reset\x18\x01 \x01(\x08"0\n\x12ProgramTaskRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04task\x18\x02 \x01(\x0c\x32\xd0\t\n\x11TaskRunnerService\x12\x39\n\tGetStatus\x12\x11.taskrunner.Empty\x1a\x17.taskrunner.StatusReply"\x00\x12?\n\x0cGetTaskState\x12\x11.taskrunner.Empty\x1a\x1a.taskrunner.TaskStateReply"\x00\x12\x41\n\x0cSetParameter\x12\x1c.taskrunner.ParameterRequest\x1a\x11.taskrunner.Empty"\x00\x12\x42\n\x0bProgramTask\x12\x1e.taskrunner.ProgramTaskRequest\x1a\x11.taskrunner.Empty"\x00\x12\x42\n\x0b\x43ompileTask\x12\x1e.taskrunner.ProgramTaskRequest\x1a\x11.taskrunner.Empty"\x00\x12>\n\tStartTask\x12\x1c.taskrunner.StartTaskRequest\x1a\x11.taskrunner.Empty"\x00\x12<\n\x08StopTask\x12\x1b.taskrunner.StopTaskRequest\x1a\x11.taskrunner.Empty"\x00\x12\x44\n\x0cGetDataboxes\x12\x11.taskrunner.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12H\n\x10GetDataboxesINT8\x12\x11.taskrunner.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12J\n\x11GetDataboxesUINT8\x12\x11.taskrunner.Empty\x1a\x1e.taskrunner.DataboxReplyUINT32"\x00\x30\x01\x12I\n\x11GetDataboxesINT16\x12\x11.taskrunner.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12K\n\x12GetDataboxesUINT16\x12\x11.taskrunner.Empty\x1a\x1e.taskrunner.DataboxReplyUINT32"\x00\x30\x01\x12I\n\x11GetDataboxesINT32\x12\x11.taskrunner.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12K\n\x12GetDataboxesUINT32\x12\x11.taskrunner.Empty\x1a\x1e.taskrunner.DataboxReplyUINT32"\x00\x30\x01\x12I\n\x11GetDataboxesINT64\x12\x11.taskrunner.Empty\x1a\x1d.taskrunner.DataboxReplyINT64"\x00\x30\x01\x12K\n\x12GetDataboxesUINT64\x12\x11.taskrunner.Empty\x1a\x1e.taskrunner.DataboxReplyUINT64"\x00\x30\x01\x12R\n\x14GetTaskErrorMessages\x12\x11.taskrunner.Empty\x1a%.taskrunner.GetTaskErrorMessagesReply"\x00\x62\x06proto3'
+    b'\n\x10taskrunner.proto\x12\ntaskrunner\x1a\x0f\x64\x61tatypes.proto"\xba\x01\n\x0bStatusReply\x12\x0f\n\x07\x63hip_id\x18\x01 \x01(\r\x12\x15\n\rfirmware_hash\x18\x02 \x01(\t\x12\x12\n\nbuild_date\x18\x03 \x01(\t\x12\x14\n\x0c\x62uild_commit\x18\x04 \x01(\t\x12\x11\n\ttask_name\x18\x05 \x01(\t\x12\x12\n\ntask_state\x18\x06 \x01(\r\x12\x15\n\rtask_progress\x18\x07 \x01(\r\x12\x1b\n\x13\x64\x61taboxes_available\x18\x08 \x01(\r"\x88\x01\n\x0eTaskStateReply\x12\x0c\n\x04\x62usy\x18\x01 \x01(\x08\x12\x0c\n\x04\x64one\x18\x02 \x01(\x08\x12\x0e\n\x06loaded\x18\x03 \x01(\x08\x12\x0f\n\x07looping\x18\x04 \x01(\x08\x12\x1b\n\x13\x65rror_msg_available\x18\x05 \x01(\x08\x12\x1c\n\x14\x65rror_msg_queue_full\x18\x06 \x01(\x08"0\n\x11\x44\x61taboxReplyINT32\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x05"1\n\x12\x44\x61taboxReplyUINT32\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\r"0\n\x11\x44\x61taboxReplyINT64\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x03"1\n\x12\x44\x61taboxReplyUINT64\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x04",\n\x19GetTaskErrorMessagesReply\x12\x0f\n\x07message\x18\x01 \x03(\t"&\n\x10ParameterRequest\x12\x12\n\nparameters\x18\x01 \x03(\x05"9\n\x10StartTaskRequest\x12\x0f\n\x07looping\x18\x01 \x01(\x08\x12\x14\n\x0cstop_running\x18\x02 \x01(\x08" \n\x0fStopTaskRequest\x12\r\n\x05reset\x18\x01 \x01(\x08"0\n\x12ProgramTaskRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04task\x18\x02 \x01(\x0c\x32\x83\n\n\x11TaskRunnerService\x12<\n\tGetStatus\x12\x14.sdr.datatypes.Empty\x1a\x17.taskrunner.StatusReply"\x00\x12\x42\n\x0cGetTaskState\x12\x14.sdr.datatypes.Empty\x1a\x1a.taskrunner.TaskStateReply"\x00\x12\x44\n\x0cSetParameter\x12\x1c.taskrunner.ParameterRequest\x1a\x14.sdr.datatypes.Empty"\x00\x12\x45\n\x0bProgramTask\x12\x1e.taskrunner.ProgramTaskRequest\x1a\x14.sdr.datatypes.Empty"\x00\x12\x45\n\x0b\x43ompileTask\x12\x1e.taskrunner.ProgramTaskRequest\x1a\x14.sdr.datatypes.Empty"\x00\x12\x41\n\tStartTask\x12\x1c.taskrunner.StartTaskRequest\x1a\x14.sdr.datatypes.Empty"\x00\x12?\n\x08StopTask\x12\x1b.taskrunner.StopTaskRequest\x1a\x14.sdr.datatypes.Empty"\x00\x12G\n\x0cGetDataboxes\x12\x14.sdr.datatypes.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12K\n\x10GetDataboxesINT8\x12\x14.sdr.datatypes.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12M\n\x11GetDataboxesUINT8\x12\x14.sdr.datatypes.Empty\x1a\x1e.taskrunner.DataboxReplyUINT32"\x00\x30\x01\x12L\n\x11GetDataboxesINT16\x12\x14.sdr.datatypes.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12N\n\x12GetDataboxesUINT16\x12\x14.sdr.datatypes.Empty\x1a\x1e.taskrunner.DataboxReplyUINT32"\x00\x30\x01\x12L\n\x11GetDataboxesINT32\x12\x14.sdr.datatypes.Empty\x1a\x1d.taskrunner.DataboxReplyINT32"\x00\x30\x01\x12N\n\x12GetDataboxesUINT32\x12\x14.sdr.datatypes.Empty\x1a\x1e.taskrunner.DataboxReplyUINT32"\x00\x30\x01\x12L\n\x11GetDataboxesINT64\x12\x14.sdr.datatypes.Empty\x1a\x1d.taskrunner.DataboxReplyINT64"\x00\x30\x01\x12N\n\x12GetDataboxesUINT64\x12\x14.sdr.datatypes.Empty\x1a\x1e.taskrunner.DataboxReplyUINT64"\x00\x30\x01\x12U\n\x14GetTaskErrorMessages\x12\x14.sdr.datatypes.Empty\x1a%.taskrunner.GetTaskErrorMessagesReply"\x00\x62\x06proto3'
 )
 
 
-_EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
 _STATUSREPLY = DESCRIPTOR.message_types_by_name["StatusReply"]
 _TASKSTATEREPLY = DESCRIPTOR.message_types_by_name["TaskStateReply"]
 _DATABOXREPLYINT32 = DESCRIPTOR.message_types_by_name["DataboxReplyINT32"]
 _DATABOXREPLYUINT32 = DESCRIPTOR.message_types_by_name["DataboxReplyUINT32"]
 _DATABOXREPLYINT64 = DESCRIPTOR.message_types_by_name["DataboxReplyINT64"]
 _DATABOXREPLYUINT64 = DESCRIPTOR.message_types_by_name["DataboxReplyUINT64"]
 _GETTASKERRORMESSAGESREPLY = DESCRIPTOR.message_types_by_name[
     "GetTaskErrorMessagesReply"
 ]
 _PARAMETERREQUEST = DESCRIPTOR.message_types_by_name["ParameterRequest"]
 _STARTTASKREQUEST = DESCRIPTOR.message_types_by_name["StartTaskRequest"]
 _STOPTASKREQUEST = DESCRIPTOR.message_types_by_name["StopTaskRequest"]
 _PROGRAMTASKREQUEST = DESCRIPTOR.message_types_by_name["ProgramTaskRequest"]
-Empty = _reflection.GeneratedProtocolMessageType(
-    "Empty",
-    (_message.Message,),
-    {
-        "DESCRIPTOR": _EMPTY,
-        "__module__": "taskrunner_pb2"
-        # @@protoc_insertion_point(class_scope:taskrunner.Empty)
-    },
-)
-_sym_db.RegisterMessage(Empty)
-
 StatusReply = _reflection.GeneratedProtocolMessageType(
     "StatusReply",
     (_message.Message,),
     {
         "DESCRIPTOR": _STATUSREPLY,
         "__module__": "taskrunner_pb2"
         # @@protoc_insertion_point(class_scope:taskrunner.StatusReply)
@@ -179,34 +155,32 @@
 )
 _sym_db.RegisterMessage(ProgramTaskRequest)
 
 _TASKRUNNERSERVICE = DESCRIPTOR.services_by_name["TaskRunnerService"]
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _EMPTY._serialized_start = 32
-    _EMPTY._serialized_end = 39
-    _STATUSREPLY._serialized_start = 42
-    _STATUSREPLY._serialized_end = 228
-    _TASKSTATEREPLY._serialized_start = 231
-    _TASKSTATEREPLY._serialized_end = 367
-    _DATABOXREPLYINT32._serialized_start = 369
-    _DATABOXREPLYINT32._serialized_end = 417
-    _DATABOXREPLYUINT32._serialized_start = 419
-    _DATABOXREPLYUINT32._serialized_end = 468
-    _DATABOXREPLYINT64._serialized_start = 470
-    _DATABOXREPLYINT64._serialized_end = 518
-    _DATABOXREPLYUINT64._serialized_start = 520
-    _DATABOXREPLYUINT64._serialized_end = 569
-    _GETTASKERRORMESSAGESREPLY._serialized_start = 571
-    _GETTASKERRORMESSAGESREPLY._serialized_end = 615
-    _PARAMETERREQUEST._serialized_start = 617
-    _PARAMETERREQUEST._serialized_end = 655
-    _STARTTASKREQUEST._serialized_start = 657
-    _STARTTASKREQUEST._serialized_end = 714
-    _STOPTASKREQUEST._serialized_start = 716
-    _STOPTASKREQUEST._serialized_end = 748
-    _PROGRAMTASKREQUEST._serialized_start = 750
-    _PROGRAMTASKREQUEST._serialized_end = 798
-    _TASKRUNNERSERVICE._serialized_start = 801
-    _TASKRUNNERSERVICE._serialized_end = 2033
+    _STATUSREPLY._serialized_start = 50
+    _STATUSREPLY._serialized_end = 236
+    _TASKSTATEREPLY._serialized_start = 239
+    _TASKSTATEREPLY._serialized_end = 375
+    _DATABOXREPLYINT32._serialized_start = 377
+    _DATABOXREPLYINT32._serialized_end = 425
+    _DATABOXREPLYUINT32._serialized_start = 427
+    _DATABOXREPLYUINT32._serialized_end = 476
+    _DATABOXREPLYINT64._serialized_start = 478
+    _DATABOXREPLYINT64._serialized_end = 526
+    _DATABOXREPLYUINT64._serialized_start = 528
+    _DATABOXREPLYUINT64._serialized_end = 577
+    _GETTASKERRORMESSAGESREPLY._serialized_start = 579
+    _GETTASKERRORMESSAGESREPLY._serialized_end = 623
+    _PARAMETERREQUEST._serialized_start = 625
+    _PARAMETERREQUEST._serialized_end = 663
+    _STARTTASKREQUEST._serialized_start = 665
+    _STARTTASKREQUEST._serialized_end = 722
+    _STOPTASKREQUEST._serialized_start = 724
+    _STOPTASKREQUEST._serialized_end = 756
+    _PROGRAMTASKREQUEST._serialized_start = 758
+    _PROGRAMTASKREQUEST._serialized_end = 806
+    _TASKRUNNERSERVICE._serialized_start = 809
+    _TASKRUNNERSERVICE._serialized_end = 2092
 # @@protoc_insertion_point(module_scope)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/grpc/taskrunner_pb2_grpc.py` & `qiclib-1.1.0/src/qiclib/packages/grpc/taskrunner_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,107 @@
-# Copyright© 2017-2023 Quantum Interface (quantuminterface@ipe.kit.edu)
-# Richard Gebauer, IPE, Karlsruhe Institute of Technology
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import taskrunner_pb2 as taskrunner__pb2
+import qiclib.packages.grpc.datatypes_pb2 as datatypes__pb2
+import qiclib.packages.grpc.taskrunner_pb2 as taskrunner__pb2
 
 
 class TaskRunnerServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetStatus = channel.unary_unary(
             "/taskrunner.TaskRunnerService/GetStatus",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.StatusReply.FromString,
         )
         self.GetTaskState = channel.unary_unary(
             "/taskrunner.TaskRunnerService/GetTaskState",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.TaskStateReply.FromString,
         )
         self.SetParameter = channel.unary_unary(
             "/taskrunner.TaskRunnerService/SetParameter",
             request_serializer=taskrunner__pb2.ParameterRequest.SerializeToString,
-            response_deserializer=taskrunner__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.ProgramTask = channel.unary_unary(
             "/taskrunner.TaskRunnerService/ProgramTask",
             request_serializer=taskrunner__pb2.ProgramTaskRequest.SerializeToString,
-            response_deserializer=taskrunner__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.CompileTask = channel.unary_unary(
             "/taskrunner.TaskRunnerService/CompileTask",
             request_serializer=taskrunner__pb2.ProgramTaskRequest.SerializeToString,
-            response_deserializer=taskrunner__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.StartTask = channel.unary_unary(
             "/taskrunner.TaskRunnerService/StartTask",
             request_serializer=taskrunner__pb2.StartTaskRequest.SerializeToString,
-            response_deserializer=taskrunner__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.StopTask = channel.unary_unary(
             "/taskrunner.TaskRunnerService/StopTask",
             request_serializer=taskrunner__pb2.StopTaskRequest.SerializeToString,
-            response_deserializer=taskrunner__pb2.Empty.FromString,
+            response_deserializer=datatypes__pb2.Empty.FromString,
         )
         self.GetDataboxes = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxes",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyINT32.FromString,
         )
         self.GetDataboxesINT8 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesINT8",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyINT32.FromString,
         )
         self.GetDataboxesUINT8 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesUINT8",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyUINT32.FromString,
         )
         self.GetDataboxesINT16 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesINT16",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyINT32.FromString,
         )
         self.GetDataboxesUINT16 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesUINT16",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyUINT32.FromString,
         )
         self.GetDataboxesINT32 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesINT32",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyINT32.FromString,
         )
         self.GetDataboxesUINT32 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesUINT32",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyUINT32.FromString,
         )
         self.GetDataboxesINT64 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesINT64",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyINT64.FromString,
         )
         self.GetDataboxesUINT64 = channel.unary_stream(
             "/taskrunner.TaskRunnerService/GetDataboxesUINT64",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.DataboxReplyUINT64.FromString,
         )
         self.GetTaskErrorMessages = channel.unary_unary(
             "/taskrunner.TaskRunnerService/GetTaskErrorMessages",
-            request_serializer=taskrunner__pb2.Empty.SerializeToString,
+            request_serializer=datatypes__pb2.Empty.SerializeToString,
             response_deserializer=taskrunner__pb2.GetTaskErrorMessagesReply.FromString,
         )
 
 
 class TaskRunnerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -222,95 +208,95 @@
         raise NotImplementedError("Method not implemented!")
 
 
 def add_TaskRunnerServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "GetStatus": grpc.unary_unary_rpc_method_handler(
             servicer.GetStatus,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.StatusReply.SerializeToString,
         ),
         "GetTaskState": grpc.unary_unary_rpc_method_handler(
             servicer.GetTaskState,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.TaskStateReply.SerializeToString,
         ),
         "SetParameter": grpc.unary_unary_rpc_method_handler(
             servicer.SetParameter,
             request_deserializer=taskrunner__pb2.ParameterRequest.FromString,
-            response_serializer=taskrunner__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "ProgramTask": grpc.unary_unary_rpc_method_handler(
             servicer.ProgramTask,
             request_deserializer=taskrunner__pb2.ProgramTaskRequest.FromString,
-            response_serializer=taskrunner__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "CompileTask": grpc.unary_unary_rpc_method_handler(
             servicer.CompileTask,
             request_deserializer=taskrunner__pb2.ProgramTaskRequest.FromString,
-            response_serializer=taskrunner__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "StartTask": grpc.unary_unary_rpc_method_handler(
             servicer.StartTask,
             request_deserializer=taskrunner__pb2.StartTaskRequest.FromString,
-            response_serializer=taskrunner__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "StopTask": grpc.unary_unary_rpc_method_handler(
             servicer.StopTask,
             request_deserializer=taskrunner__pb2.StopTaskRequest.FromString,
-            response_serializer=taskrunner__pb2.Empty.SerializeToString,
+            response_serializer=datatypes__pb2.Empty.SerializeToString,
         ),
         "GetDataboxes": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxes,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyINT32.SerializeToString,
         ),
         "GetDataboxesINT8": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesINT8,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyINT32.SerializeToString,
         ),
         "GetDataboxesUINT8": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesUINT8,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyUINT32.SerializeToString,
         ),
         "GetDataboxesINT16": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesINT16,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyINT32.SerializeToString,
         ),
         "GetDataboxesUINT16": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesUINT16,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyUINT32.SerializeToString,
         ),
         "GetDataboxesINT32": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesINT32,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyINT32.SerializeToString,
         ),
         "GetDataboxesUINT32": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesUINT32,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyUINT32.SerializeToString,
         ),
         "GetDataboxesINT64": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesINT64,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyINT64.SerializeToString,
         ),
         "GetDataboxesUINT64": grpc.unary_stream_rpc_method_handler(
             servicer.GetDataboxesUINT64,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.DataboxReplyUINT64.SerializeToString,
         ),
         "GetTaskErrorMessages": grpc.unary_unary_rpc_method_handler(
             servicer.GetTaskErrorMessages,
-            request_deserializer=taskrunner__pb2.Empty.FromString,
+            request_deserializer=datatypes__pb2.Empty.FromString,
             response_serializer=taskrunner__pb2.GetTaskErrorMessagesReply.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "taskrunner.TaskRunnerService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
@@ -333,15 +319,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetStatus",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.StatusReply.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -362,15 +348,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetTaskState",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.TaskStateReply.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -392,15 +378,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/SetParameter",
             taskrunner__pb2.ParameterRequest.SerializeToString,
-            taskrunner__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -421,15 +407,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/ProgramTask",
             taskrunner__pb2.ProgramTaskRequest.SerializeToString,
-            taskrunner__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -450,15 +436,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/CompileTask",
             taskrunner__pb2.ProgramTaskRequest.SerializeToString,
-            taskrunner__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -479,15 +465,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/StartTask",
             taskrunner__pb2.StartTaskRequest.SerializeToString,
-            taskrunner__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -508,15 +494,15 @@
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/StopTask",
             taskrunner__pb2.StopTaskRequest.SerializeToString,
-            taskrunner__pb2.Empty.FromString,
+            datatypes__pb2.Empty.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -536,15 +522,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxes",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyINT32.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -565,15 +551,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesINT8",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyINT32.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -594,15 +580,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesUINT8",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyUINT32.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -623,15 +609,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesINT16",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyINT32.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -652,15 +638,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesUINT16",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyUINT32.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -681,15 +667,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesINT32",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyINT32.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -710,15 +696,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesUINT32",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyUINT32.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -739,15 +725,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesINT64",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyINT64.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -768,15 +754,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_stream(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetDataboxesUINT64",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.DataboxReplyUINT64.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
@@ -797,15 +783,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/taskrunner.TaskRunnerService/GetTaskErrorMessages",
-            taskrunner__pb2.Empty.SerializeToString,
+            datatypes__pb2.Empty.SerializeToString,
             taskrunner__pb2.GetTaskErrorMessagesReply.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qiclib-1.0.0/src/qiclib/packages/qiskit/QiController_backend.py` & `qiclib-1.1.0/src/qiclib/packages/qiskit/QiController_backend.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/qiskit/QiController_job.py` & `qiclib-1.1.0/src/qiclib/packages/qiskit/QiController_job.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/qiskit/QiController_provider.py` & `qiclib-1.1.0/src/qiclib/packages/qiskit/QiController_provider.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/qiskit/QiGates.py` & `qiclib-1.1.0/src/qiclib/packages/qiskit/QiGates.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/qiskit/__init__.py` & `qiclib-1.1.0/src/qiclib/packages/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/qkit_polyfill.py` & `qiclib-1.1.0/src/qiclib/packages/qkit_polyfill.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/servicehub.py` & `qiclib-1.1.0/src/qiclib/packages/servicehub.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib/packages/utility.py` & `qiclib-1.1.0/src/qiclib/packages/utility.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/src/qiclib.egg-info/PKG-INFO` & `qiclib-1.1.0/src/qiclib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiclib
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library to connect to Quantum Interface's QiController.
 Home-page: https://github.com/quantuminterface/qiclib
 Author: Quantum Interface
 Author-email: quantuminterface@ipe.kit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `qiclib-1.0.0/src/qiclib.egg-info/SOURCES.txt` & `qiclib-1.1.0/src/qiclib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,18 @@
 src/qiclib/experiment/rtos_tasks/test/test_databox.c
 src/qiclib/experiment/rtos_tasks/test/time_test_code.c
 src/qiclib/experiment/rtos_tasks/test/timing_test.c
 src/qiclib/experiment/rtos_tasks/test/timing_test_axi.c
 src/qiclib/experiment/rtos_tasks/test/timing_test_single.c
 src/qiclib/hardware/__init__.py
 src/qiclib/hardware/controller.py
+src/qiclib/hardware/digital_trigger.py
 src/qiclib/hardware/pimc.py
 src/qiclib/hardware/platform_component.py
+src/qiclib/hardware/pulse_player.py
 src/qiclib/hardware/pulsegen.py
 src/qiclib/hardware/recording.py
 src/qiclib/hardware/rfdc.py
 src/qiclib/hardware/sequencer.py
 src/qiclib/hardware/servicehub.py
 src/qiclib/hardware/storage.py
 src/qiclib/hardware/taskrunner.py
@@ -134,16 +136,22 @@
 src/qiclib/measurement/measure_iq.py
 src/qiclib/packages/__init__.py
 src/qiclib/packages/constants.py
 src/qiclib/packages/qkit_polyfill.py
 src/qiclib/packages/servicehub.py
 src/qiclib/packages/utility.py
 src/qiclib/packages/grpc/__init__.py
+src/qiclib/packages/grpc/datatypes_pb2.py
+src/qiclib/packages/grpc/datatypes_pb2_grpc.py
+src/qiclib/packages/grpc/digital_trigger_pb2.py
+src/qiclib/packages/grpc/digital_trigger_pb2_grpc.py
 src/qiclib/packages/grpc/pimc_pb2.py
 src/qiclib/packages/grpc/pimc_pb2_grpc.py
+src/qiclib/packages/grpc/pulse_player_pb2.py
+src/qiclib/packages/grpc/pulse_player_pb2_grpc.py
 src/qiclib/packages/grpc/pulsegen_pb2.py
 src/qiclib/packages/grpc/pulsegen_pb2_grpc.py
 src/qiclib/packages/grpc/qic_storage_pb2.py
 src/qiclib/packages/grpc/qic_storage_pb2_grpc.py
 src/qiclib/packages/grpc/qic_unitcell_pb2.py
 src/qiclib/packages/grpc/qic_unitcell_pb2_grpc.py
 src/qiclib/packages/grpc/recording_pb2.py
```

### Comparing `qiclib-1.0.0/tests/test_experiments.py` & `qiclib-1.1.0/tests/test_experiments.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,28 @@
     rfdc,
     unit_cell,
     sequencer,
     servicehub_control,
     recording,
     pulse_gen,
     taskrunner,
+    digital_trigger,
 )
 
 
 @mocks.patch(
     pimc,
     rfdc,
     unit_cell,
     sequencer,
     servicehub_control,
     recording,
     pulse_gen,
     taskrunner,
+    digital_trigger,
 )
 class TestExperiments(unittest.TestCase):
     def test_ExperimentReadout(self):
         controller = QiController("IP")
         with QiJob() as job:
             q = QiCells(1)
             Wait(q[0], delay=0)
```

### Comparing `qiclib-1.0.0/tests/test_iq_fit.py` & `qiclib-1.1.0/tests/test_iq_fit.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_insert_mem_parameters.py` & `qiclib-1.1.0/tests/test_qi_insert_mem_parameters.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_jobs.py` & `qiclib-1.1.0/tests/test_qi_jobs.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_prog_builder.py` & `qiclib-1.1.0/tests/test_qi_prog_builder.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_pulse.py` & `qiclib-1.1.0/tests/test_qi_pulse.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_seq_instructions.py` & `qiclib-1.1.0/tests/test_qi_seq_instructions.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,18 +79,16 @@
             0b00001111000011110000_00000_0000100  # uses lower 20 Bits of immediate
         )
 
         if inst.get_riscv_instruction() != expected:
             self.fail(bin(inst.get_riscv_instruction()) + " != " + bin(expected))
 
     def test_trigger_instruction(self):
-        inst = SeqTrigger(5, 3, 4, 2, 1)
-        expected = (
-            0b01_0010_0100_11_0101_0000_00000_0000010  # uses lower 20 Bits of immediate
-        )
+        inst = SeqTrigger(5, 0, 4, 2, 1, 3)
+        expected = 0b11_01_10_0100_00_0101_00_0000000_0000010
 
         if inst.get_riscv_instruction() != expected:
             self.fail(bin(inst.get_riscv_instruction()) + " != " + bin(expected))
 
     def test_synch_start_immediate(self):
         inst = SeqEnd()
         expected = 0b0000000_00000_00000_000_00000_0001000
```

### Comparing `qiclib-1.0.0/tests/test_qi_sequencer.py` & `qiclib-1.1.0/tests/test_qi_sequencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     QiVariable,
     QiIntVariable,
     QiTimeVariable,
     QiCell,
     ForRange,
     QiCells,
     Wait,
+    cQiDigitalTrigger,
 )
 from qiclib.code.qi_jobs import (
     cQiPlay,
     cQiPlayReadout,
     cQiWait,
     cQiRecording,
     QiJob,
@@ -265,14 +266,21 @@
         play_cmd = cQiPlay(self.cell, QiPulse(length=CONTROLLER_CYCLE_TIME * 2))
 
         self.sequencer.add_trigger_cmd(play_cmd)
 
         self.assertIsInstance(self.sequencer.instruction_list[0], SeqTrigger)
         self.assertIsInstance(self.sequencer.instruction_list[1], SeqWaitImm)
 
+    def test_digital_trigger(self):
+        digital_trigger_cmd = cQiDigitalTrigger(self.cell, outputs=[3], length=12e-9)
+
+        self.sequencer.add_trigger_cmd(digital=digital_trigger_cmd)
+
+        self.assertIsInstance(self.sequencer.instruction_list[0], SeqTrigger)
+
     def test_play_commands_longest_wait(self):
         play_cmd = cQiPlay(self.cell, QiPulse(length=CONTROLLER_CYCLE_TIME * 2))
         readout_cmd = cQiPlayReadout(
             self.cell, QiPulse(length=CONTROLLER_CYCLE_TIME * 3)
         )
 
         self.sequencer.add_trigger_cmd(play_cmd, readout_cmd)
```

### Comparing `qiclib-1.0.0/tests/test_qi_types.py` & `qiclib-1.1.0/tests/test_qi_types.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_util.py` & `qiclib-1.1.0/tests/test_qi_util.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_var_definitions.py` & `qiclib-1.1.0/tests/test_qi_var_definitions.py`

 * *Files identical despite different names*

### Comparing `qiclib-1.0.0/tests/test_qi_visitor.py` & `qiclib-1.1.0/tests/test_qi_visitor.py`

 * *Files identical despite different names*

