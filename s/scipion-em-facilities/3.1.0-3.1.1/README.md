# Comparing `tmp/scipion-em-facilities-3.1.0.tar.gz` & `tmp/scipion-em-facilities-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-facilities-3.1.0.tar", last modified: Fri May 31 09:36:58 2024, max compression
+gzip compressed data, was "scipion-em-facilities-3.1.1.tar", last modified: Mon Jun  3 10:25:58 2024, max compression
```

## Comparing `scipion-em-facilities-3.1.0.tar` & `scipion-em-facilities-3.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.645657 scipion-em-facilities-3.1.0/emfacilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/getnifs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_good_classes_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_2d_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_movie_gain.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    41018 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_trackUsedItems.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_volume_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    55485 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/pynvml.py
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/report_html.py
--rw-r--r--   0 runner    (1001) docker     (127)    23362 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/report_influx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/summary_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    39513 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/templates/execution.summary.template.html
--rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/templates/facility_SPA_streaming.json.template
--rw-r--r--   0 runner    (1001) docker     (127)    22634 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocol_good_classes_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocol_volume_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8374 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_high_throughput.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20446 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/emfacilities/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/viewers/viewer_good_classes_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/viewers/viewer_monitors.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/secrets_template.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.949268 scipion-em-facilities-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-06-03 10:25:58.949268 scipion-em-facilities-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.941268 scipion-em-facilities-3.1.1/emfacilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.945268 scipion-em-facilities-3.1.1/emfacilities/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/getnifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_good_classes_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_2d_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_movie_gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41018 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_trackUsedItems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7702 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_volume_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55485 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/pynvml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/report_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23362 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/report_influx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/summary_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.945268 scipion-em-facilities-3.1.1/emfacilities/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    39513 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/templates/execution.summary.template.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/templates/facility_SPA_streaming.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)    22634 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.945268 scipion-em-facilities-3.1.1/emfacilities/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.945268 scipion-em-facilities-3.1.1/emfacilities/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocol_good_classes_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocol_volume_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocols_ctf_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocols_ctf_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocols_system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.945268 scipion-em-facilities-3.1.1/emfacilities/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/workflows/test_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8374 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/workflows/test_workflow_high_throughput.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20446 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/tests/workflows/test_workflow_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.945268 scipion-em-facilities-3.1.1/emfacilities/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/viewers/viewer_good_classes_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/emfacilities/viewers/viewer_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:25:58.949268 scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-06-03 10:25:58.000000 scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-06-03 10:25:58.000000 scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:25:58.000000 scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-03 10:25:58.000000 scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 10:25:58.000000 scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 10:25:58.000000 scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/secrets_template.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 10:25:58.949268 scipion-em-facilities-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-06-03 10:25:15.000000 scipion-em-facilities-3.1.1/setup.py
```

### Comparing `scipion-em-facilities-3.1.0/CHANGES.txt` & `scipion-em-facilities-3.1.1/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/LICENSE` & `scipion-em-facilities-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/PKG-INFO` & `scipion-em-facilities-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-facilities
-Version: 3.1.0
+Version: 3.1.1
 Summary: Plugin for Cryo-EM facilities to be used within Scipion framework
 Home-page: https://scipion-em.github.io/docs/docs/facilities/facilities.html
 Author: J.M. De la Rosa Trevin, Roberto Marabini, David Maluenda
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Scipion for facilities
```

### Comparing `scipion-em-facilities-3.1.0/README.rst` & `scipion-em-facilities-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/__init__.py` & `scipion-em-facilities-3.1.1/emfacilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 import os
 import pwem
 
 from .constants import *
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 _logo = "facilityLogo.png"
 _references = ["delaRosaTrevin201693"]
 
 
 class Plugin(pwem.Plugin):
     _homeVar = EMFACILITIES_HOME_VARNAME 
     _pathVars = [EMFACILITIES_HOME_VARNAME]
```

### Comparing `scipion-em-facilities-3.1.0/emfacilities/bibtex.py` & `scipion-em-facilities-3.1.1/emfacilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/constants.py` & `scipion-em-facilities-3.1.1/emfacilities/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/__init__.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/getnifs.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/getnifs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_good_classes_extractor.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_good_classes_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,27 +31,30 @@
 
 from pyworkflow.utils import prettyTime
 import pyworkflow.protocol.params as params
 from pyworkflow.object import Set
 from pyworkflow.protocol import ProtStreamingBase, STEPS_PARALLEL
 from pwem.protocols import EMProtocol
 from pwem.objects import SetOfParticles, SetOfAverages, SetOfClasses2D
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 
 OUTPUT_PARTICLES = "outputParticles"
 OUTPUT_DISCARDED_PARTICLES = "outputParticlesDiscarded"
 LAST_DONE_FILE = "last_done.txt"
 
 
 class ProtGoodClassesExtractor(EMProtocol, ProtStreamingBase):
     """ Extracts items from a SetOfClasses based on a list of IDs or a set of given good averages/classes
     """
 
     _label = "good classes extractor"
     outputsToDefine = {}
+    _devStatus = NEW
+
     _possibleOutputs = {OUTPUT_PARTICLES: SetOfParticles,
                         OUTPUT_DISCARDED_PARTICLES: SetOfParticles}
     # Mode
     LIST_CLASSES = 0
     LIST_IDS = 1
 
     def __init__(self, **args):
```

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_2d_streamer.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_2d_streamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,25 @@
 import time
 
 import pyworkflow.object as pwobj
 import pyworkflow.protocol.params as params
 from pyworkflow.project import Manager
 
 from .protocol_monitor import ProtMonitor
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 
 class ProtMonitor2dStreamer(ProtMonitor):
     """ This protocol will monitor an input set of particles
     (usually in streaming) and will run/schedule many copies
      of a given 2D classification protocol but using subsets
      of the input particles as the 2D classification input.
     """
     _label = '2d classification launcher'
+    _devStatus = UPDATED
 
     NONE_OPTION = 0
     CLASSIFICATION_JOBS = 1
     NUMBER_PARTICLES = 2
 
     def __init__(self, **kwargs):
         ProtMonitor.__init__(self, **kwargs)
```

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_ctf.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_movie_gain.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_movie_gain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_summary.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,27 @@
 
 from .report_influx import ReportInflux
 from .report_html import ReportHtml
 from .protocol_monitor import ProtMonitor, Monitor
 from .protocol_monitor_ctf import MonitorCTF
 from .protocol_monitor_movie_gain import MonitorMovieGain
 from .protocol_monitor_system import MonitorSystem
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 
 class ProtMonitorSummary(ProtMonitor):
     """ Provide some summary of the basic steps of the Scipion-Box:
     - Import movies
     - Align movies (global and/or local)
     - CTF estimation
     - Movie gain estimation.
     """
     _label = 'monitor summary'
     _lastUpdateVersion = VERSION_1_1
+    _devStatus = UPDATED
 
     def __init__(self, **kwargs):
         ProtMonitor.__init__(self, **kwargs)
         self.reportDir = ''
         self.reportPath = ''
 
     def _defineParams(self, form):
```

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_system.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_monitor_system.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_trackUsedItems.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_trackUsedItems.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_volume_extractor.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/protocol_volume_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pyworkflow.protocol.params as params
 import pwem.objects as emobj
 from pwem.protocols import EMProtocol
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 
 OUTPUT_PARTICLES = "outputParticles"
 OUTPUT_VOLUME = "bestVolume"
 
 
 class ProtVolumeExtractor(EMProtocol):
     """
     Extracts items (particles, volume or both) from a SetOf3DClasses based on number of items assigned to the class
     or by a reference ID
     """
 
     _label = "volume extractor"
+    _devStatus = NEW
 
     _possibleOutputs = {OUTPUT_PARTICLES: emobj.SetOfParticles,
                         OUTPUT_VOLUME: emobj.Volume}
     outputsToDefine = {}
 
     PARTICLES = 0
     VOLUME = 1
```

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/pynvml.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/pynvml.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/report_html.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/report_html.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/report_influx.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/report_influx.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/summary_provider.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/summary_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols/transport.py` & `scipion-em-facilities-3.1.1/emfacilities/protocols/transport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/protocols.conf` & `scipion-em-facilities-3.1.1/emfacilities/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/templates/execution.summary.template.html` & `scipion-em-facilities-3.1.1/emfacilities/templates/execution.summary.template.html`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/templates/facility_SPA_streaming.json.template` & `scipion-em-facilities-3.1.1/emfacilities/templates/facility_SPA_streaming.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template` & `scipion-em-facilities-3.1.1/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/__init__.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocol_good_classes_extractor.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocol_good_classes_extractor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocol_volume_extractor.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocol_volume_extractor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_monitor.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocols_ctf_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_streaming.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocols_ctf_streaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_system_monitor.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/protocols/test_protocols_system_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_high_throughput.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/workflows/test_workflow_high_throughput.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_streaming.py` & `scipion-em-facilities-3.1.1/emfacilities/tests/workflows/test_workflow_streaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/viewers/__init__.py` & `scipion-em-facilities-3.1.1/emfacilities/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/viewers/viewer_good_classes_extractor.py` & `scipion-em-facilities-3.1.1/emfacilities/viewers/viewer_good_classes_extractor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/emfacilities/viewers/viewer_monitors.py` & `scipion-em-facilities-3.1.1/emfacilities/viewers/viewer_monitors.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/PKG-INFO` & `scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-facilities
-Version: 3.1.0
+Version: 3.1.1
 Summary: Plugin for Cryo-EM facilities to be used within Scipion framework
 Home-page: https://scipion-em.github.io/docs/docs/facilities/facilities.html
 Author: J.M. De la Rosa Trevin, Roberto Marabini, David Maluenda
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Scipion for facilities
```

### Comparing `scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/SOURCES.txt` & `scipion-em-facilities-3.1.1/scipion_em_facilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/secrets_template.cfg` & `scipion-em-facilities-3.1.1/secrets_template.cfg`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.1.0/setup.py` & `scipion-em-facilities-3.1.1/setup.py`

 * *Files identical despite different names*

