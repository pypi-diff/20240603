# Comparing `tmp/nkululeko-0.86.3.tar.gz` & `tmp/nkululeko-0.86.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.86.3.tar", last modified: Thu May 30 11:06:33 2024, max compression
+gzip compressed data, was "nkululeko-0.86.4.tar", last modified: Mon Jun  3 09:34:05 2024, max compression
```

## Comparing `nkululeko-0.86.3.tar` & `nkululeko-0.86.4.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18447 2024-05-30 10:53:12.000000 nkululeko-0.86.3/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.86.3/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37305 2024-05-30 11:06:33.220938 nkululeko-0.86.3/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17587 2024-05-29 09:24:25.000000 nkululeko-0.86.3/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.208938 nkululeko-0.86.3/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.86.3/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.86.3/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.86.3/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.86.3/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.86.3/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.86.3/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.86.3/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.86.3/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.86.3/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.86.3/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.86.3/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.86.3/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.86.3/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.86.3/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.86.3/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.86.3/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.86.3/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.86.3/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.86.3/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.86.3/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.86.3/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.86.3/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.86.3/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.86.3/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.86.3/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.86.3/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.86.3/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.86.3/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.86.3/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.86.3/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.86.3/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.86.3/meta/demos/demo_best_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.86.3/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.86.3/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.86.3/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.216937 nkululeko-0.86.3/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.86.3/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.86.3/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.86.3/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.216937 nkululeko-0.86.3/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.86.3/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.86.3/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.86.3/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.86.3/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.86.3/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.216937 nkululeko-0.86.3/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.86.3/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.86.3/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.86.3/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-30 11:06:09.000000 nkululeko-0.86.3/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.216937 nkululeko-0.86.3/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.86.3/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.86.3/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3933 2024-05-21 10:44:53.000000 nkululeko-0.86.3/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.86.3/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.86.3/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.86.3/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30986 2024-05-29 14:39:21.000000 nkululeko-0.86.3/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.86.3/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.86.3/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.86.3/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1674 2024-05-30 10:55:30.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4028 2024-05-29 07:55:31.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-05-15 15:09:05.000000 nkululeko-0.86.3/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1541 2024-05-29 07:58:33.000000 nkululeko-0.86.3/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.86.3/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.86.3/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.86.3/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.86.3/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.86.3/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.86.3/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.86.3/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.86.3/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10452 2024-05-17 12:04:16.000000 nkululeko-0.86.3/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.86.3/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11639 2024-05-15 15:09:05.000000 nkululeko-0.86.3/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.86.3/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.86.3/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.86.3/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.86.3/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.86.3/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.86.3/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9856 2024-05-29 14:36:50.000000 nkululeko-0.86.3/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.86.3/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.86.3/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.86.3/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.86.3/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.86.3/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21146 2024-05-30 10:52:02.000000 nkululeko-0.86.3/nkululeko/models/model_tuned.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.86.3/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.86.3/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.86.3/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.86.3/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.86.3/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23070 2024-05-30 08:12:44.000000 nkululeko-0.86.3/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.86.3/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.86.3/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.86.3/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.86.3/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.86.3/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.86.3/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13445 2024-05-30 09:47:17.000000 nkululeko-0.86.3/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.86.3/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4267 2024-05-29 12:54:47.000000 nkululeko-0.86.3/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.86.3/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.86.3/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.86.3/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.86.3/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.86.3/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.86.3/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.86.3/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.86.3/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.86.3/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8465 2024-05-15 15:09:05.000000 nkululeko-0.86.3/nkululeko/test_pretrain.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.86.3/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.86.3/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.3/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13930 2024-05-30 10:56:40.000000 nkululeko-0.86.3/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37305 2024-05-30 11:06:33.000000 nkululeko-0.86.3/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5132 2024-05-30 11:06:33.000000 nkululeko-0.86.3/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-30 11:06:33.000000 nkululeko-0.86.3/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-30 11:06:33.000000 nkululeko-0.86.3/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-30 11:06:33.000000 nkululeko-0.86.3/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.86.3/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-30 11:06:33.220938 nkululeko-0.86.3/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.86.3/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.212937 nkululeko-0.86.3/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 11:06:33.220938 nkululeko-0.86.3/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.86.3/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.452042 nkululeko-0.86.4/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18514 2024-06-03 09:33:49.000000 nkululeko-0.86.4/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.86.4/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37480 2024-06-03 09:34:05.452042 nkululeko-0.86.4/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17695 2024-05-30 11:28:52.000000 nkululeko-0.86.4/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.86.4/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.86.4/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.86.4/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.86.4/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.86.4/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.86.4/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.86.4/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.86.4/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.86.4/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.86.4/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.86.4/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.86.4/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.86.4/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.86.4/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.86.4/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.86.4/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.86.4/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.86.4/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.86.4/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.86.4/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.86.4/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.86.4/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.86.4/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.86.4/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.86.4/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.86.4/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.86.4/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.86.4/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.86.4/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.86.4/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.86.4/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.444042 nkululeko-0.86.4/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.86.4/meta/demos/demo_best_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.86.4/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.86.4/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.86.4/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.448042 nkululeko-0.86.4/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.86.4/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.86.4/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.86.4/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.448042 nkululeko-0.86.4/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.86.4/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.86.4/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.86.4/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.86.4/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.86.4/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.448042 nkululeko-0.86.4/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.86.4/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.86.4/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.86.4/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-06-03 09:32:49.000000 nkululeko-0.86.4/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.448042 nkululeko-0.86.4/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.86.4/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.86.4/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3933 2024-05-21 10:44:53.000000 nkululeko-0.86.4/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5142 2024-06-03 09:32:25.000000 nkululeko-0.86.4/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.86.4/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.86.4/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    31041 2024-06-03 09:32:25.000000 nkululeko-0.86.4/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.86.4/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.86.4/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.448042 nkululeko-0.86.4/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.86.4/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1674 2024-05-30 10:55:30.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4028 2024-05-29 07:55:31.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-05-15 15:09:05.000000 nkululeko-0.86.4/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1541 2024-05-29 07:58:33.000000 nkululeko-0.86.4/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.86.4/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.86.4/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.86.4/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.86.4/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.86.4/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.448042 nkululeko-0.86.4/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.86.4/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.86.4/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.86.4/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10452 2024-05-17 12:04:16.000000 nkululeko-0.86.4/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.452042 nkululeko-0.86.4/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.86.4/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11639 2024-05-15 15:09:05.000000 nkululeko-0.86.4/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.86.4/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.86.4/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.86.4/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.86.4/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.86.4/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.86.4/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9856 2024-05-29 14:36:50.000000 nkululeko-0.86.4/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.86.4/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.86.4/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.86.4/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.86.4/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.86.4/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21340 2024-06-03 09:32:25.000000 nkululeko-0.86.4/nkululeko/models/model_tuned.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.86.4/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.86.4/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.86.4/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.86.4/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.86.4/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23070 2024-05-30 08:12:44.000000 nkululeko-0.86.4/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.86.4/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.452042 nkululeko-0.86.4/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.86.4/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.86.4/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.86.4/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.86.4/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.86.4/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13447 2024-06-03 09:32:25.000000 nkululeko-0.86.4/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.86.4/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4267 2024-05-29 12:54:47.000000 nkululeko-0.86.4/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.86.4/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.86.4/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.86.4/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.452042 nkululeko-0.86.4/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.86.4/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.86.4/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.86.4/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.86.4/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.86.4/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.86.4/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8465 2024-05-15 15:09:05.000000 nkululeko-0.86.4/nkululeko/test_pretrain.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.452042 nkululeko-0.86.4/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.86.4/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.86.4/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.4/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    14123 2024-06-03 09:32:25.000000 nkululeko-0.86.4/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.452042 nkululeko-0.86.4/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37480 2024-06-03 09:34:05.000000 nkululeko-0.86.4/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5132 2024-06-03 09:34:05.000000 nkululeko-0.86.4/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-06-03 09:34:05.000000 nkululeko-0.86.4/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-06-03 09:34:05.000000 nkululeko-0.86.4/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-06-03 09:34:05.000000 nkululeko-0.86.4/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.86.4/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-06-03 09:34:05.452042 nkululeko-0.86.4/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.86.4/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.440042 nkululeko-0.86.4/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-06-03 09:34:05.452042 nkululeko-0.86.4/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.86.4/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.86.3/CHANGELOG.md` & `nkululeko-0.86.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.86.4
+--------------
+* add finetuning to the demo module
+
 Version 0.86.3
 --------------
 * bugfixed: nan in finetuned model and double saving
 * import features now get multiindex automatically
 
 Version 0.86.2
 --------------
```

### Comparing `nkululeko-0.86.3/LICENSE` & `nkululeko-0.86.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/PKG-INFO` & `nkululeko-0.86.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.86.3
+Version: 0.86.4
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -233,14 +233,15 @@
 * [Specifying database disk location](http://blog.syntheticspeech.de/2022/02/21/specifying-database-disk-location-with-nkululeko/) 
 * [Add dropout with MLP models](http://blog.syntheticspeech.de/2022/02/25/adding-dropout-to-mlp-models-with-nkululeko/)
 * [Do cross-validation](http://blog.syntheticspeech.de/2022/03/23/how-to-do-cross-validation-with-nkululeko/)
 * [Combine predictions per speaker](http://blog.syntheticspeech.de/2022/03/24/how-to-combine-predictions-per-speaker-with-nkululeko/)
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
+* [Export acoustic features](http://blog.syntheticspeech.de/2024/05/30/nkululeko-export-acoustic-features/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
 * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
 * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 * [Check your dataset](http://blog.syntheticspeech.de/2023/07/11/nkululeko-check-your-dataset/) 
@@ -330,14 +331,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.86.4
+--------------
+* add finetuning to the demo module
+
 Version 0.86.3
 --------------
 * bugfixed: nan in finetuned model and double saving
 * import features now get multiindex automatically
 
 Version 0.86.2
 --------------
```

### Comparing `nkululeko-0.86.3/README.md` & `nkululeko-0.86.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 * [Specifying database disk location](http://blog.syntheticspeech.de/2022/02/21/specifying-database-disk-location-with-nkululeko/) 
 * [Add dropout with MLP models](http://blog.syntheticspeech.de/2022/02/25/adding-dropout-to-mlp-models-with-nkululeko/)
 * [Do cross-validation](http://blog.syntheticspeech.de/2022/03/23/how-to-do-cross-validation-with-nkululeko/)
 * [Combine predictions per speaker](http://blog.syntheticspeech.de/2022/03/24/how-to-combine-predictions-per-speaker-with-nkululeko/)
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
+* [Export acoustic features](http://blog.syntheticspeech.de/2024/05/30/nkululeko-export-acoustic-features/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
 * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
 * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 * [Check your dataset](http://blog.syntheticspeech.de/2023/07/11/nkululeko-check-your-dataset/)
```

### Comparing `nkululeko-0.86.3/data/aesdd/process_database.py` & `nkululeko-0.86.4/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/androids/process_database.py` & `nkululeko-0.86.4/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/androids_orig/process_database.py` & `nkululeko-0.86.4/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/androids_test/process_database.py` & `nkululeko-0.86.4/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/ased/process_database.py` & `nkululeko-0.86.4/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/asvp-esd/process_database.py` & `nkululeko-0.86.4/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/baved/process_database.py` & `nkululeko-0.86.4/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/cafe/process_database.py` & `nkululeko-0.86.4/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/clac/process_database.py` & `nkululeko-0.86.4/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/cmu-mosei/process_database.py` & `nkululeko-0.86.4/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/demos/process_database.py` & `nkululeko-0.86.4/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/ekorpus/process_database.py` & `nkululeko-0.86.4/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/emns/process_database.py` & `nkululeko-0.86.4/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/emofilm/convert_to_16k.py` & `nkululeko-0.86.4/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/emofilm/process_database.py` & `nkululeko-0.86.4/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/emorynlp/process_database.py` & `nkululeko-0.86.4/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/emov-db/process_database.py` & `nkululeko-0.86.4/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/emovo/process_database.py` & `nkululeko-0.86.4/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/emozionalmente/create.py` & `nkululeko-0.86.4/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/enterface/process_database.py` & `nkululeko-0.86.4/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/esd/process_database.py` & `nkululeko-0.86.4/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/gerparas/process_database.py` & `nkululeko-0.86.4/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/iemocap/process_database.py` & `nkululeko-0.86.4/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/jl/process_database.py` & `nkululeko-0.86.4/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/jtes/process_database.py` & `nkululeko-0.86.4/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/meld/process_database.py` & `nkululeko-0.86.4/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/mesd/process_database.py` & `nkululeko-0.86.4/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/mess/process_database.py` & `nkululeko-0.86.4/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/mlendsnd/process_database.py` & `nkululeko-0.86.4/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/msp-improv/process_database2.py` & `nkululeko-0.86.4/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/msp-podcast/process_database.py` & `nkululeko-0.86.4/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/oreau2/process_database.py` & `nkululeko-0.86.4/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/portuguese/process_database.py` & `nkululeko-0.86.4/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/ravdess/process_database.py` & `nkululeko-0.86.4/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/ravdess/process_database_speaker.py` & `nkululeko-0.86.4/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/savee/process_database.py` & `nkululeko-0.86.4/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/shemo/process_database.py` & `nkululeko-0.86.4/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/subesco/process_database.py` & `nkululeko-0.86.4/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/tess/process_database.py` & `nkululeko-0.86.4/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/thorsten-emotional/process_database.py` & `nkululeko-0.86.4/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/urdu/process_database.py` & `nkululeko-0.86.4/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/data/vivae/process_database.py` & `nkululeko-0.86.4/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/docs/source/conf.py` & `nkululeko-0.86.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/meta/demos/demo_best_model.py` & `nkululeko-0.86.4/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/meta/demos/my_experiment.py` & `nkululeko-0.86.4/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/meta/demos/my_experiment_local.py` & `nkululeko-0.86.4/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/meta/demos/plot_faster_anim.py` & `nkululeko-0.86.4/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/aug_train.py` & `nkululeko-0.86.4/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/augment.py` & `nkululeko-0.86.4/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/augmenting/augmenter.py` & `nkululeko-0.86.4/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.86.4/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.86.4/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/augmenting/resampler.py` & `nkululeko-0.86.4/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_age.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.86.4/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.86.4/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/cacheddataset.py` & `nkululeko-0.86.4/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/data/dataset.py` & `nkululeko-0.86.4/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/data/dataset_csv.py` & `nkululeko-0.86.4/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/demo.py` & `nkululeko-0.86.4/nkululeko/demo_feats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,34 @@
-# demo.py
-# Demonstration code to use the ML-experiment framework
-# Test the loading of a previously trained model and demo mode
-# needs the project config file to run before
-"""This script is used to test the loading of a previously trained model.
-
-And run it in demo mode.
-It requires the project config file to be run before.
-
-Usage:  
-python -m nkululeko.demo [--config CONFIG] [--file FILE] [--list LIST] [--folder FOLDER] [--outfile OUTFILE]  
-
-Options:   \n
---config CONFIG     The base configuration file (default: exp.ini) \n  
---file FILE         A file that should be processed (16kHz mono wav) \n  
---list LIST         A file with a list of files, one per line, that should be processed (16kHz mono wav) \n  
---folder FOLDER     A name of a folder where the files within the list are in   (default: ./) \n   
---outfile OUTFILE   A filename to store the results in CSV  (default: None)  
-"""
-import argparse
-import configparser
-import os
+# demo_feats.py
+# Test some features extracted
 
-from nkululeko.constants import VERSION
 from nkululeko.experiment import Experiment
-import nkululeko.glob_conf as glob_conf
+import configparser
 from nkululeko.utils.util import Util
+from nkululeko.constants import VERSION
+import argparse
+import os
 
 
 def main(src_dir):
-    parser = argparse.ArgumentParser(description="Call the nkululeko DEMO framework.")
+    parser = argparse.ArgumentParser(description="Call the nkululeko framework.")
     parser.add_argument("--config", default="exp.ini", help="The base configuration")
     parser.add_argument(
         "--file", help="A file that should be processed (16kHz mono wav)"
     )
     parser.add_argument(
         "--list",
         help=(
             "A file with a list of files, one per line, that should be"
             " processed (16kHz mono wav)"
         ),
         nargs="?",
         default=None,
     )
     parser.add_argument(
-        "--folder",
-        help=("A name of a folder where the files within the list are in."),
-        nargs="?",
-        default="./",
-    )
-    parser.add_argument(
         "--outfile",
         help=("A filename to store the results in CSV"),
         nargs="?",
         default=None,
     )
     args = parser.parse_args()
     if args.config is not None:
@@ -67,33 +43,29 @@
 
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
 
     # create a new experiment
     expr = Experiment(config)
-    module = "demo"
+    module = "demo_feats"
     expr.set_module(module)
     util = Util(module)
     util.debug(
         f"running {expr.name} from config {config_file}, nkululeko version"
         f" {VERSION}"
     )
 
-    # load the experiment
-    expr.load(f"{util.get_save_name()}")
-    if args.folder is not None:
-        glob_conf.config["DATA"]["test_folder"] = args.folder
     if args.file is None and args.list is None:
-        expr.demo(None, False, args.outfile)
+        expr.demo_feats(None, False, args.outfile)
     else:
         if args.list is None:
-            expr.demo(args.file, False, args.outfile)
+            expr.demo_feats(args.file, False, args.outfile)
         else:
-            expr.demo(args.list, True, args.outfile)
+            expr.demo_feats(args.list, True, args.outfile)
 
     print("DONE")
 
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
     main(cwd)  # use this if you want to state the config file path on command line
```

### Comparing `nkululeko-0.86.3/nkululeko/demo_feats.py` & `nkululeko-0.86.4/nkululeko/nkululeko.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,73 @@
-# demo_feats.py
-# Test some features extracted
-
-from nkululeko.experiment import Experiment
-import configparser
-from nkululeko.utils.util import Util
-from nkululeko.constants import VERSION
+# nkululeko.py
+# Entry script to do a Nkululeko experiment
 import argparse
-import os
+import configparser
+import os.path
 
+import numpy as np
 
-def main(src_dir):
-    parser = argparse.ArgumentParser(description="Call the nkululeko framework.")
-    parser.add_argument("--config", default="exp.ini", help="The base configuration")
-    parser.add_argument(
-        "--file", help="A file that should be processed (16kHz mono wav)"
-    )
-    parser.add_argument(
-        "--list",
-        help=(
-            "A file with a list of files, one per line, that should be"
-            " processed (16kHz mono wav)"
-        ),
-        nargs="?",
-        default=None,
-    )
-    parser.add_argument(
-        "--outfile",
-        help=("A filename to store the results in CSV"),
-        nargs="?",
-        default=None,
-    )
-    args = parser.parse_args()
-    if args.config is not None:
-        config_file = args.config
-    else:
-        config_file = f"{src_dir}/exp.ini"
+from nkululeko.constants import VERSION
+import nkululeko.experiment as exp
+from nkululeko.utils.util import Util
 
+
+def doit(config_file):
     # test if the configuration file exists
     if not os.path.isfile(config_file):
         print(f"ERROR: no such file: {config_file}")
         exit()
 
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
 
     # create a new experiment
-    expr = Experiment(config)
-    module = "demo_feats"
+    expr = exp.Experiment(config)
+    module = "nkululeko"
     expr.set_module(module)
     util = Util(module)
     util.debug(
         f"running {expr.name} from config {config_file}, nkululeko version"
         f" {VERSION}"
     )
 
-    if args.file is None and args.list is None:
-        expr.demo_feats(None, False, args.outfile)
-    else:
-        if args.list is None:
-            expr.demo_feats(args.file, False, args.outfile)
-        else:
-            expr.demo_feats(args.list, True, args.outfile)
+    if util.config_val("EXP", "no_warnings", False):
+        import warnings
+
+        warnings.filterwarnings("ignore")
+
+    # load the data
+    expr.load_datasets()
+
+    # split into train and test
+    expr.fill_train_and_tests()
+    util.debug(f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}")
 
+    # extract features
+    expr.extract_feats()
+
+    # initialize a run manager
+    expr.init_runmanager()
+
+    # run the experiment
+    reports, last_epochs = expr.run()
+    result = expr.get_best_report(reports).result.test
+    expr.store_report()
     print("DONE")
+    return result, int(np.asarray(last_epochs).min())
+
+
+def main(src_dir):
+    parser = argparse.ArgumentParser(description="Call the nkululeko framework.")
+    parser.add_argument("--config", default="exp.ini", help="The base configuration")
+    args = parser.parse_args()
+    if args.config is not None:
+        config_file = args.config
+    else:
+        config_file = f"{src_dir}/exp.ini"
+    doit(config_file)
 
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
     main(cwd)  # use this if you want to state the config file path on command line
```

### Comparing `nkululeko-0.86.3/nkululeko/demo_predictor.py` & `nkululeko-0.86.4/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/experiment.py` & `nkululeko-0.86.4/nkululeko/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,16 @@
         labels = self.util.config_val("DATA", "labels", False)
         auto_labels = list(next(iter(self.datasets.values())).df[self.target].unique())
         if labels:
             self.labels = ast.literal_eval(labels)
             self.util.debug(f"Target labels (from config): {labels}")
         else:
             self.labels = auto_labels
-            self.util.debug(f"Target labels (from database): {auto_labels}")
+        # print autolabel no matter it is specified or not
+        self.util.debug(f"Target labels (from database): {auto_labels}")
         glob_conf.set_labels(self.labels)
         self.util.debug(f"loaded databases {dbs}")
 
     def _import_csv(self, storage):
         # df = pd.read_csv(storage, header=0, index_col=[0,1,2])
         # df.index.set_levels(pd.to_timedelta(df.index.levels[1]), level=1)
         # df.index.set_levels(pd.to_timedelta(df.index.levels[2]), level=2)
```

### Comparing `nkululeko-0.86.3/nkululeko/explore.py` & `nkululeko-0.86.4/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/export.py` & `nkululeko-0.86.4/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feats_whisper.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/featureset.py` & `nkululeko-0.86.4/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.86.4/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/feature_extractor.py` & `nkululeko-0.86.4/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/file_checker.py` & `nkululeko-0.86.4/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/filter_data.py` & `nkululeko-0.86.4/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/glob_conf.py` & `nkululeko-0.86.4/nkululeko/glob_conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/losses/loss_ccc.py` & `nkululeko-0.86.4/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.86.4/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/modelrunner.py` & `nkululeko-0.86.4/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model.py` & `nkululeko-0.86.4/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_cnn.py` & `nkululeko-0.86.4/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_gmm.py` & `nkululeko-0.86.4/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_knn.py` & `nkululeko-0.86.4/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_knn_reg.py` & `nkululeko-0.86.4/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_mlp.py` & `nkululeko-0.86.4/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.86.4/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_svm.py` & `nkululeko-0.86.4/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_svr.py` & `nkululeko-0.86.4/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/models/model_tuned.py` & `nkululeko-0.86.4/nkululeko/models/model_tuned.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,17 +50,19 @@
             self.measure = self.util.config_val("MODEL", "measure", "ccc")
         self.util.debug(f"evaluation metrics: {self.measure}")
         self.batch_size = int(self.util.config_val("MODEL", "batch_size", "8"))
         self.util.debug(f"batch size: {self.batch_size}")
         self.learning_rate = float(
             self.util.config_val("MODEL", "learning_rate", "0.0001")
         )
-        self.max_duration = float(self.util.config_val("MODEL", "max_duration", "8.0"))
+        self.max_duration = float(
+            self.util.config_val("MODEL", "max_duration", "8.0"))
         self.df_train, self.df_test = df_train, df_test
         self.epoch_num = int(self.util.config_val("EXP", "epochs", 1))
+        self.util.debug(f"num of epochs: {self.epoch_num}")
         drop = self.util.config_val("MODEL", "drop", False)
         self.drop = 0.1
         if drop:
             self.drop = float(drop)
         self.util.debug(f"init: training with dropout: {self.drop}")
         self.push = eval(self.util.config_val("MODEL", "push_to_hub", "False"))
         self._init_model()
@@ -133,15 +135,14 @@
         tokenizer = transformers.Wav2Vec2CTCTokenizer("./vocab.json")
         tokenizer.save_pretrained(".")
 
         # uoload tokenizer to hub if true
         if self.push:
             tokenizer.push_to_hub(self.util.get_name())
 
-
         feature_extractor = transformers.Wav2Vec2FeatureExtractor(
             feature_size=1,
             sampling_rate=16000,
             padding_value=0.0,
             do_normalize=True,
             return_attention_mask=True,
         )
@@ -263,25 +264,27 @@
                     self.util.debug(f"train weights: {train_weights}")
                     criterion = torch.nn.CrossEntropyLoss(
                         weight=torch.Tensor(train_weights).to("cuda"),
                     )
                 else:
                     criterion = torch.nn.CrossEntropyLoss()
             else:
-                self.util.error(f"criterion {criterion} not supported for classifier")
+                self.util.error(
+                    f"criterion {criterion} not supported for classifier")
         else:
             self.criterion = self.util.config_val("MODEL", "loss", "ccc")
             if criterion == "1-ccc":
                 criterion = ConcordanceCorCoeff()
             elif criterion == "mse":
                 criterion = torch.nn.MSELoss()
             elif criterion == "mae":
                 criterion = torch.nn.L1Loss()
             else:
-                self.util.error(f"criterion {criterion} not supported for regressor")
+                self.util.error(
+                    f"criterion {criterion} not supported for regressor")
 
         # set push_to_hub value, default false
         # push = eval(self.util.config_val("MODEL", "push_to_hub", "False"))
 
         class Trainer(transformers.Trainer):
             def compute_loss(
                 self,
@@ -312,53 +315,56 @@
         elif metrics_for_best_model == "CCC":
             greater_is_better = True
         elif metrics_for_best_model == "MSE":
             greater_is_better = False
         elif metrics_for_best_model == "MAE":
             greater_is_better = False
         else:
-            self.util.error(f"unknown metric/measure: {metrics_for_best_model}")
+            self.util.error(
+                f"unknown metric/measure: {metrics_for_best_model}")
 
         training_args = transformers.TrainingArguments(
-            output_dir=self.torch_root,
+            output_dir=model_root,
             logging_dir=self.log_root,
             per_device_train_batch_size=self.batch_size,
             per_device_eval_batch_size=self.batch_size,
             gradient_accumulation_steps=self.accumulation_steps,
             evaluation_strategy="steps",
             num_train_epochs=self.epoch_num,
-            fp16=self.device == "cuda",
+            fp16=self.device != "cpu",
+            use_cpu=self.device == "cpu",
             save_steps=num_steps,
             eval_steps=num_steps,
             logging_steps=num_steps,
             logging_strategy="epoch",
             learning_rate=self.learning_rate,
             save_total_limit=2,
             metric_for_best_model=metrics_for_best_model,
             greater_is_better=greater_is_better,
             load_best_model_at_end=True,
             remove_unused_columns=False,
             report_to="none",
             push_to_hub=self.push,
             hub_model_id=f"{self.util.get_name()}",
+            overwrite_output_dir=True,
         )
 
         trainer = Trainer(
             model=self.model,
             data_collator=self.data_collator,
             args=training_args,
             compute_metrics=self.compute_metrics,
             train_dataset=self.dataset["train"],
             eval_dataset=self.dataset["dev"],
             tokenizer=self.processor.feature_extractor,
             callbacks=[transformers.integrations.TensorBoardCallback()],
         )
 
         trainer.train()
-        # trainer.save_model(self.torch_root)
+        trainer.save_model(self.torch_root)
         log_file = os.path.join(
             self.log_root,
             "log.txt",
         )
         with open(log_file, "w") as text_file:
             print(trainer.state.log_history, file=text_file)
         self.util.debug(f"saved best model to {self.torch_root}")
@@ -443,23 +449,23 @@
 
     def load_path(self, path, run, epoch):
         self.set_id(run, epoch)
         with open(path, "rb") as handle:
             self.clf = pickle.load(handle)
 
 
-@dataclasses.dataclass
+@ dataclasses.dataclass
 class ModelOutput(transformers.file_utils.ModelOutput):
 
     logits: torch.FloatTensor = None
     hidden_states: typing.Tuple[torch.FloatTensor] = None
     cnn_features: torch.FloatTensor = None
 
 
-@dataclasses.dataclass
+@ dataclasses.dataclass
 class ModelOutputReg(transformers.file_utils.ModelOutput):
 
     logits: torch.FloatTensor
     hidden_states: typing.Tuple[torch.FloatTensor] = None
     attentions: typing.Tuple[torch.FloatTensor] = None
     logits_framewise: torch.FloatTensor = None
     hidden_states_framewise: torch.FloatTensor = None
@@ -520,17 +526,17 @@
             )
             hidden_states = hidden_states * torch.reshape(
                 attention_mask,
                 (-1, attention_mask.shape[-1], 1),
             )
             outputs = torch.sum(hidden_states, dim=1)
             attention_sum = torch.sum(attention_mask, dim=1)
-            
-            epsilon = 1e-6 # to avoid division by zero and numerical instability
-            outputs = outputs / (torch.reshape(attention_sum, (-1, 1)) + 
+
+            epsilon = 1e-6  # to avoid division by zero and numerical instability
+            outputs = outputs / (torch.reshape(attention_sum, (-1, 1)) +
                                  epsilon)
 
         return outputs
 
     def forward(
         self,
         input_values,
```

### Comparing `nkululeko-0.86.3/nkululeko/multidb.py` & `nkululeko-0.86.4/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/nkuluflag.py` & `nkululeko-0.86.4/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/nkululeko.py` & `nkululeko-0.86.4/nkululeko/predict.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,78 @@
-# nkululeko.py
-# Entry script to do a Nkululeko experiment
+# predict.py
+# use some model and add automatically predicted labels to train and test splits
+# then save as a new dataset
+
+"""This script is used to call the nkululeko PREDICT framework. 
+
+It loads a configuration file, creates a new experiment,
+and performs automatic prediction on the train and test datasets. The predicted labels are added to the datasets and
+saved as a new dataset.
+
+Usage: \n
+    python3 -m nkululeko.predict [--config CONFIG_FILE] \n
+
+Arguments: \n
+    --config (str): The path to the base configuration file (default: exp.ini)
+"""
+
 import argparse
 import configparser
-import os.path
-
-import numpy as np
+import os
 
 from nkululeko.constants import VERSION
-import nkululeko.experiment as exp
+from nkululeko.experiment import Experiment
 from nkululeko.utils.util import Util
 
 
-def doit(config_file):
+def main(src_dir):
+    parser = argparse.ArgumentParser(
+        description="Call the nkululeko PREDICT framework.")
+    parser.add_argument("--config", default="exp.ini",
+                        help="The base configuration")
+    args = parser.parse_args()
+    if args.config is not None:
+        config_file = args.config
+    else:
+        config_file = f"{src_dir}/exp.ini"
+
     # test if the configuration file exists
     if not os.path.isfile(config_file):
         print(f"ERROR: no such file: {config_file}")
         exit()
 
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
-
     # create a new experiment
-    expr = exp.Experiment(config)
-    module = "nkululeko"
+    expr = Experiment(config)
+    module = "predict"
     expr.set_module(module)
     util = Util(module)
     util.debug(
         f"running {expr.name} from config {config_file}, nkululeko version"
         f" {VERSION}"
     )
 
-    if util.config_val("EXP", "no_warnings", False):
-        import warnings
-
-        warnings.filterwarnings("ignore")
-
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
-    util.debug(f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}")
-
-    # extract features
-    expr.extract_feats()
-
-    # initialize a run manager
-    expr.init_runmanager()
+    util.debug(
+        f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}")
 
-    # run the experiment
-    reports, last_epochs = expr.run()
-    result = expr.get_best_report(reports).result.test
-    expr.store_report()
+    # process the data
+    df = expr.autopredict()
+    target = util.config_val("DATA", "target", "emotion")
+    if "class_label" in df.columns:
+        df = df.drop(columns=[target])
+        df = df.rename(columns={"class_label": target})
+    name = util.get_data_name() + "_predicted"
+    df.to_csv(f"{expr.data_dir}/{name}.csv")
+    util.debug(f"saved {name}.csv to {expr.data_dir}")
     print("DONE")
-    return result, int(np.asarray(last_epochs).min())
-
-
-def main(src_dir):
-    parser = argparse.ArgumentParser(description="Call the nkululeko framework.")
-    parser.add_argument("--config", default="exp.ini", help="The base configuration")
-    args = parser.parse_args()
-    if args.config is not None:
-        config_file = args.config
-    else:
-        config_file = f"{src_dir}/exp.ini"
-    doit(config_file)
 
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
     main(cwd)  # use this if you want to state the config file path on command line
```

### Comparing `nkululeko-0.86.3/nkululeko/plots.py` & `nkululeko-0.86.4/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/reporting/defines.py` & `nkululeko-0.86.4/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/reporting/latex_writer.py` & `nkululeko-0.86.4/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/reporting/report.py` & `nkululeko-0.86.4/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/reporting/report_item.py` & `nkululeko-0.86.4/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/reporting/reporter.py` & `nkululeko-0.86.4/nkululeko/reporting/reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         fig = ax.figure
         plt.xlabel("epochs")
         plt.ylabel(f"{self.MEASURE}")
         plot_path = f"{fig_dir}{plot_name}.{self.format}"
         plt.savefig(plot_path)
         self.util.debug(f"plotted epoch progression to {plot_path}")
         plt.close(fig)
-        fig.clear()
+        # fig.clear()
 
     def plot_epoch_progression(self, reports, out_name):
         fig_dir = self.util.get_path("fig_dir")
         results, losses, train_results, losses_eval = [], [], [], []
         for r in reports:
             results.append(r.get_result().test)
             losses.append(r.get_result().loss)
```

### Comparing `nkululeko-0.86.3/nkululeko/reporting/result.py` & `nkululeko-0.86.4/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/resample.py` & `nkululeko-0.86.4/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/runmanager.py` & `nkululeko-0.86.4/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/scaler.py` & `nkululeko-0.86.4/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/segment.py` & `nkululeko-0.86.4/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.86.4/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.86.4/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/syllable_nuclei.py` & `nkululeko-0.86.4/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/test.py` & `nkululeko-0.86.4/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/test_predictor.py` & `nkululeko-0.86.4/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/test_pretrain.py` & `nkululeko-0.86.4/nkululeko/test_pretrain.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/utils/files.py` & `nkululeko-0.86.4/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/utils/stats.py` & `nkululeko-0.86.4/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/nkululeko/utils/util.py` & `nkululeko-0.86.4/nkululeko/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         else:
             self.caller = ""
         if has_config:
             try:
                 import nkululeko.glob_conf as glob_conf
 
                 self.config = glob_conf.config
-                self.got_data_roots = self.config_val("DATA", "root_folders", False)
+                self.got_data_roots = self.config_val(
+                    "DATA", "root_folders", False)
                 if self.got_data_roots:
                     # if there is a global data rootfolder file, read from there
                     if not os.path.isfile(self.got_data_roots):
                         self.error(f"no such file: {self.got_data_roots}")
                     self.data_roots = configparser.ConfigParser()
                     self.data_roots.read(self.got_data_roots)
             except (ModuleNotFoundError, AttributeError):
@@ -112,15 +113,16 @@
                 except KeyError:
                     if not default in self.stopvals:
                         self.debug(
                             f"value for {key} not found, using default:" f" {default}"
                         )
                     return default
             if not default in self.stopvals:
-                self.debug(f"value for {key} not found, using default: {default}")
+                self.debug(
+                    f"value for {key} not found, using default: {default}")
             return default
 
     def set_config(self, config):
         self.config = config
 
     def get_save_name(self):
         """Return a relative path to a name to save the experiment"""
@@ -155,16 +157,18 @@
         audeer.mkdir(dir_name)
         return dir_name
 
     def make_segmented_index(self, df):
         if len(df) == 0:
             return df
         if not isinstance(df.index, pd.MultiIndex):
-            self.debug("converting to segmented index, this might take a while...")
-            df.index = audformat.utils.to_segmented_index(df.index, allow_nat=False)
+            self.debug(
+                "converting to segmented index, this might take a while...")
+            df.index = audformat.utils.to_segmented_index(
+                df.index, allow_nat=False)
         return df
 
     def _get_value_descript(self, section, name):
         if self.config_val(section, name, False):
             val = self.config_val(section, name, False)
             val = str(val).strip(".")
             return f"_{name}-{str(val)}"
@@ -191,14 +195,17 @@
             ds = "_".join(ast.literal_eval(self.config["DATA"]["databases"]))
         return_string = f"{ds}"
         if not only_data:
             mt = self.get_model_description()
             return_string = return_string + "_" + mt
         return return_string.replace("__", "_")
 
+    def get_model_type(self):
+        return self.config["MODEL"]["type"]
+
     def get_model_description(self):
         mt = ""
         mt = f'{self.config["MODEL"]["type"]}'
         ft = "_".join(ast.literal_eval(self.config["FEATS"]["type"]))
         ft += "_"
         layer_string = ""
         layer_s = self.config_val("MODEL", "layers", False)
@@ -267,23 +274,25 @@
     def config_val(self, section, key, default):
         if self.config is None:
             return default
         try:
             return self.config[section][key]
         except KeyError:
             if default not in self.stopvals:
-                self.debug(f"value for {key} not found, using default: {default}")
+                self.debug(
+                    f"value for {key} not found, using default: {default}")
             return default
 
     def config_val_list(self, section, key, default):
         try:
             return ast.literal_eval(self.config[section][key])
         except KeyError:
             if not default in self.stopvals:
-                self.debug(f"value for {key} not found, using default: {default}")
+                self.debug(
+                    f"value for {key} not found, using default: {default}")
             return default
 
     def continuous_to_categorical(self, series):
         """
         discretize a categorical variable.
         uses the labels and bins from the ini if present
```

### Comparing `nkululeko-0.86.3/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.86.4/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.86.3
+Version: 0.86.4
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -233,14 +233,15 @@
 * [Specifying database disk location](http://blog.syntheticspeech.de/2022/02/21/specifying-database-disk-location-with-nkululeko/) 
 * [Add dropout with MLP models](http://blog.syntheticspeech.de/2022/02/25/adding-dropout-to-mlp-models-with-nkululeko/)
 * [Do cross-validation](http://blog.syntheticspeech.de/2022/03/23/how-to-do-cross-validation-with-nkululeko/)
 * [Combine predictions per speaker](http://blog.syntheticspeech.de/2022/03/24/how-to-combine-predictions-per-speaker-with-nkululeko/)
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
+* [Export acoustic features](http://blog.syntheticspeech.de/2024/05/30/nkululeko-export-acoustic-features/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
 * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
 * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 * [Check your dataset](http://blog.syntheticspeech.de/2023/07/11/nkululeko-check-your-dataset/) 
@@ -330,14 +331,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.86.4
+--------------
+* add finetuning to the demo module
+
 Version 0.86.3
 --------------
 * bugfixed: nan in finetuned model and double saving
 * import features now get multiindex automatically
 
 Version 0.86.2
 --------------
```

### Comparing `nkululeko-0.86.3/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.86.4/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/setup.cfg` & `nkululeko-0.86.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.3/venv/bin/activate_this.py` & `nkululeko-0.86.4/venv/bin/activate_this.py`

 * *Files identical despite different names*

