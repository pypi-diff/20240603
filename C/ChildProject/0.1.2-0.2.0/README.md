# Comparing `tmp/ChildProject-0.1.2.tar.gz` & `tmp/ChildProject-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ChildProject/ChildProject/dist/.tmp-aev1xzcb/ChildProject-0.1.2.tar", last modified: Thu Mar 14 17:52:32 2024, max compression
+gzip compressed data, was "/home/runner/work/ChildProject/ChildProject/dist/.tmp-g112iuyw/ChildProject-0.2.0.tar", last modified: Mon Jun  3 09:52:47 2024, max compression
```

## Comparing `ChildProject-0.1.2.tar` & `ChildProject-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:52:32.000000 ChildProject-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87397 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/annotations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22870 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)    27018 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/derivations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/eafbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/fake_panoptes.py
--rw-r--r--   0 runner    (1001) docker     (127)    42859 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    28975 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/metricsFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    18865 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)    40200 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    41019 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/pipelines/zooniverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    37022 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/templates/basic.etf
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/templates/basic.pfsx
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/templates/native.etf
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/templates/native.pfsx
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/templates/non-native.etf
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/templates/non-native.pfsx
--rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-03-14 17:52:28.000000 ChildProject-0.1.2/ChildProject/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-14 17:52:32.000000 ChildProject-0.1.2/ChildProject.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-14 17:52:28.000000 ChildProject-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-14 17:52:32.000000 ChildProject-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-14 17:52:28.000000 ChildProject-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 17:52:32.000000 ChildProject-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-14 17:52:28.000000 ChildProject-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:52:32.000000 ChildProject-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29325 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_derivations.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_reliability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-03-14 17:52:28.000000 ChildProject-0.1.2/tests/test_zooniverse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:47.000000 ChildProject-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87398 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/annotations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23101 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27070 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/derivations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/eafbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/fake_panoptes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42699 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/metricsFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40062 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41876 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/pipelines/zooniverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37022 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/templates/basic.etf
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/templates/basic.pfsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/templates/native.etf
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/templates/native.pfsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/templates/non-native.etf
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/templates/non-native.pfsx
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-06-03 09:52:43.000000 ChildProject-0.2.0/ChildProject/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 09:52:47.000000 ChildProject-0.2.0/ChildProject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 09:52:43.000000 ChildProject-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-06-03 09:52:47.000000 ChildProject-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-06-03 09:52:43.000000 ChildProject-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-06-03 09:52:43.000000 ChildProject-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:52:47.000000 ChildProject-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:52:47.000000 ChildProject-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29341 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_derivations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_reliability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-06-03 09:52:43.000000 ChildProject-0.2.0/tests/test_zooniverse.py
```

### Comparing `ChildProject-0.1.2/ChildProject/annotations.py` & `ChildProject-0.2.0/ChildProject/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         IndexColumn(
             name="filter",
             description="source file to target. this field is dedicated to rttm and ALICE annotations that may combine annotations from several recordings into one same text file.",
             required=False,
         ),
         IndexColumn(
             name="annotation_filename",
-            description="output formatted annotation location, relative to `annotations/<set>/converted (automatic column, don't specify)",
+            description="output formatted annotation location, relative to `annotations/<set>/converted` (automatic column, don't specify)",
             filename=True,
             required=False,
             generated=True,
         ),
         IndexColumn(
             name="imported_at",
             description="importation date (automatic column, don't specify)",
```

### Comparing `ChildProject-0.1.2/ChildProject/cmdline.py` & `ChildProject-0.2.0/ChildProject/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
-from ChildProject.projects import ChildProject
-from ChildProject.annotations import AnnotationManager
+from .projects import ChildProject
+from .annotations import AnnotationManager
 from .pipelines.samplers import SamplerPipeline
 from .pipelines.eafbuilder import EafBuilderPipeline
 from .pipelines.zooniverse import ZooniversePipeline
 from .pipelines.metrics import MetricsPipeline
 from .pipelines.metrics import MetricsSpecificationPipeline
 from .pipelines.processors import AudioProcessingPipeline
 from .pipelines.anonymize import AnonymizationPipeline
 from .utils import read_wav, calculate_shift, get_audio_duration
-from ChildProject import __version__
+from . import __version__
+
 from ChildProject import __name__
 
 from .pipelines.derivations import DERIVATIONS
 
 import argparse
 import os
 import pandas as pd
@@ -351,14 +352,19 @@
         am.read()
         annotations = am.annotations
 
     intersection = AnnotationManager.intersection(annotations, args.sets)
     intersection.to_csv(args.destination, index=False)
 
 
+@subcommand([])
+def interpreter(args):
+    print(sys.executable)
+
+
 @subcommand(
     [
         arg("source", help="project path"),
         arg("--set", help="set to remove", required=True),
         arg("--recursive", help="enable recursive mode", action="store_true"),
     ]
 )
@@ -406,15 +412,18 @@
     project = ChildProject(args.source)
 
     perform_validation(project, require_success=True, ignore_recordings=True)
 
     am = AnnotationManager(project)
     project.read()
 
-    logger.info("\n\033[1mrecordings\033[0m:")
+    output = "\n\033[1mrecordings ({:.2f} hours)\033[0m:\n".format(
+        project.recordings.dropna(subset=["recording_filename"])["duration"].sum() / (3600 * 1000)
+    )
+
     _recordings = (
         project.recordings.dropna(subset=["recording_filename"])
         .sort_values(["recording_device_type", "date_iso"])
         .groupby("recording_device_type")
     )
 
     for recording_device_type, recordings in _recordings:
@@ -433,17 +442,19 @@
                     os.path.join(project.path, "recordings", "raw", recording_filename)
                 )
                 else 0
             )
             .sum()
         )
 
-        logger.info("\033[94m%s\033[0m: %d, %s/%d files locally available", recording_device_type, duration, available, len(recordings))
+        output += "\033[94m%s\033[0m: %s, %d/%d files locally available\n" % (
+                    recording_device_type, duration, available, len(recordings))
+
 
-    logger.info("\n\033[1mannotations\033[0m:")
+    output += "\n\033[1mannotations\033[0m:\n"
     _annotations = (
         am.annotations.dropna(subset=["annotation_filename"])
         .sort_values(["set", "imported_at"])
         .drop_duplicates(["set", "annotation_filename"], keep="last")
         .groupby("set")
     )
 
@@ -465,15 +476,18 @@
                     )
                 )
                 else 0
             )
             .sum()
         )
 
-        logger.info("\033[94m%s\033[0m: %.2f hours, %s/%s files locally available", annotation_set, duration_covered / (3600 * 1000), available, len(annotations))
+        output += "\033[94m%s\033[0m: %.2f hours, %s/%s files locally available\n" % (
+                    annotation_set, duration_covered / (3600 * 1000), available, len(annotations))
+
+    logger.info(output)
 
 
 @subcommand(
     [arg("source", help="source data path"), arg("variable", help="name of the variable")]
 )
 def explain(args):
     """prints information about a certain metadata variable"""
```

### Comparing `ChildProject-0.1.2/ChildProject/converters.py` & `ChildProject-0.2.0/ChildProject/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import defaultdict
 import pandas as pd
 import re
 from enum import Enum
+from .pipelines.metricsFunctions import voc_speaker
 
 converters = {}
 
 class Formats(Enum):
     CSV = 'csv'
     VTC = 'vtc_rttm'
     VCM = 'vcm_rttm'
```

### Comparing `ChildProject-0.1.2/ChildProject/metrics.py` & `ChildProject-0.2.0/ChildProject/metrics.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/anonymize.py` & `ChildProject-0.2.0/ChildProject/pipelines/anonymize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import glob
 import os
 import pandas as pd
 import json
 import re
 import shutil
 
-from ChildProject.projects import ChildProject
-from ChildProject.annotations import AnnotationManager
-from ChildProject.pipelines.pipeline import Pipeline
+from ..projects import ChildProject
+from ..annotations import AnnotationManager
+from .pipeline import Pipeline
 
 
 class AnonymizationPipeline(Pipeline):
     """Anonymize a set of its annotations (`input_set`) and saves it as `output_set`."""
 
     DEFAULT_REPLACEMENTS = {
         "PrimaryChild": {"DOB": "1000-01-01"},
```

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/derivations.py` & `ChildProject-0.2.0/ChildProject/pipelines/derivations.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/eafbuilder.py` & `ChildProject-0.2.0/ChildProject/pipelines/eafbuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import argparse
 import pandas as pd
 import sys
 import os
 import shutil
+from pathlib import Path
 
-from ChildProject.projects import ChildProject
-from ChildProject.annotations import AnnotationManager
-from ChildProject.pipelines.pipeline import Pipeline
-from ChildProject.tables import assert_dataframe, assert_columns_presence
-from ChildProject.converters import Formats
+from ..projects import ChildProject
+from ..annotations import AnnotationManager
+from .pipeline import Pipeline
+from ..tables import assert_dataframe, assert_columns_presence
+from ..converters import Formats
 
 FORMAT_SPEECH = {Formats.VTC.value,Formats.VCM.value} #formats for which nan must be replaced with SPEECH
 CHILDPROJECT_TYPE = "childProject_generated"
 
 def create_eaf(
     etf_path: str,
     id: str,
     output_dir: str,
     recording_filename: str,
     timestamps_list: list,
     eaf_type: str,
     contxt_on: int,
     contxt_off: int,
-    template: str,
     speech_segments: pd.DataFrame = None,
     imported_set: str = None,
     imported_format: str = None,
 ):
     import pympi
 
     eaf = pympi.Elan.Eaf(etf_path)
@@ -65,15 +65,15 @@
         for segment in speech_segments.to_dict(orient="records"):
             speaker_id = None
 
             if "speaker_id" in segment and not pd.isnull(segment["speaker_id"]):
                 speaker_id = segment["speaker_id"]
             elif "speaker_type" in segment:
                 speaker_id = segment["speaker_type"]
-                if pd.isnull(speaker_id) and imported_format in FORMAT_SPEECH : speaker_id = "SPEECH" #replace  nan with SPEECH for some formats
+                if pd.isnull(speaker_id) and imported_format in FORMAT_SPEECH: speaker_id = "SPEECH" #replace  nan with SPEECH for some formats
 
             if speaker_id is None:
                 continue
             
             if imported_set: speaker_id = "{}-{}".format(imported_set.replace("/","_").upper(),speaker_id)
 
             if speaker_id not in eaf.tiers:
@@ -179,15 +179,16 @@
         if prefill:
             project = ChildProject(path)
             am = AnnotationManager(project)
             am.read()
             imported_set = import_speech_from
 
         for recording_filename, segs in segments.groupby("recording_filename"):
-            recording_prefix = os.path.splitext(recording_filename)[0]
+            full_recording = Path(recording_filename)
+            recording_prefix = full_recording.stem
             output_filename = (
                 recording_prefix + "_" + eaf_type + "_" + os.path.basename(template)
             )
 
             # TODO: This list of timestamps as tuples might not be ideal/should perhaps be optimized, but I am just replicating the original eaf creation code here.
             timestamps = [
                 (on, off)
@@ -213,26 +214,25 @@
                     matches = matches["format"].drop_duplicates()
                     if len(matches.index) == 1:
                         imported_format = matches.iloc[0]
                 except KeyError:
                     imported_format = None
                     
 
-            output_dir = os.path.join(destination, recording_prefix)
+            output_dir = os.path.join(destination, full_recording.parent)
 
             create_eaf(
                 etf_path,
                 output_filename,
                 output_dir,
                 recording_filename,
                 timestamps,
                 eaf_type,
                 context_onset,
                 context_offset,
-                template,
                 speech_segments,
                 imported_set,
                 imported_format,
             )
 
             shutil.copy(
                 pfsx_path, os.path.join(output_dir, "{}.pfsx".format(output_filename))
```

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/fake_panoptes.py` & `ChildProject-0.2.0/ChildProject/pipelines/fake_panoptes.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/metrics.py` & `ChildProject-0.2.0/ChildProject/pipelines/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 import numpy as np
 import pandas as pd
 from typing import Union, List
 import yaml
 from git import Repo
 from git.exc import InvalidGitRepositoryError
 
-import ChildProject
-from ChildProject.pipelines.pipeline import Pipeline
-
-from ChildProject.tables import assert_dataframe, assert_columns_presence, read_csv_with_dtype
-import ChildProject.pipelines.metricsFunctions as metfunc
+from ..projects import ChildProject
+from ..annotations import AnnotationManager
+from ..tables import assert_dataframe, assert_columns_presence, read_csv_with_dtype
 from ..utils import TimeInterval, time_intervals_intersect
+from .pipeline import Pipeline
+from . import metricsFunctions as metfunc
+
+from ChildProject import __version__
 
 pipelines = {}
 
 class Metrics(ABC):
     """
     Main class for generating metrics from a project object and a list of desired metrics
     
@@ -44,29 +46,29 @@
     :param segments: DataFrame or path to csv file of the segments to extract from, containing 'recording_filename', 'segment_onset' and 'segment_offset' columns. To use this option, the option must be set to 'segments'. Also, this option cannot be combined with options [recordings,period,from_time,to_time].
     :type segments: Union[str, pd.DataFrame], optional
     :param threads: amount of threads to run on, defaults to 1
     :type threads: int, optional
     """
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         metrics_list: pd.DataFrame,
         by: str = "recording_filename",
         recordings: Union[str, List[str], pd.DataFrame] = None,
         from_time: str = None,
         to_time: str = None,
         rec_cols: str = None,
         child_cols: str = None,
         period: str = None,
         segments: Union[str, pd.DataFrame] = None,
         threads: int = 1,
     ):
 
         self.project = project
-        self.am = ChildProject.annotations.AnnotationManager(self.project)
+        self.am = AnnotationManager(self.project)
         self.threads = int(threads)
         
         #check that the callable column is either a callable function or a string that can be found as being part of the list of metrics in ChildProject/pipelines/metricsFunctions.py
         def check_callable(row):
             if callable(row["callable"]): return row["callable"]
             if isinstance(row["callable"],str):
                 try:
@@ -415,15 +417,15 @@
     :type threads: int, optional
     """
     
     SUBCOMMAND = "custom"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         metrics: str,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         from_time: str = None,
         to_time: str = None,       
         rec_cols: str = None,
         child_cols: str = None,
         by: str = "recording_filename",
@@ -473,15 +475,15 @@
     :type threads: int, optional
     """
 
     SUBCOMMAND = "lena"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         set: str,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         from_time: str = None,
         to_time: str = None,       
         rec_cols: str = None,
         child_cols: str = None,
         by: str = "recording_filename",
@@ -566,15 +568,15 @@
     :type threads: int, optional
     """
 
     SUBCOMMAND = "aclew"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         vtc: str = "vtc",
         alice: str = "alice",
         vcm: str = "vcm",
         recordings: Union[str, List[str], pd.DataFrame] = None,
         from_time: str = None,
         to_time: str = None,
         rec_cols: str = None,
@@ -585,15 +587,15 @@
         threads: int = 1,
     ):
         
         self.vtc = vtc
         self.alice = alice
         self.vcm = vcm
         
-        am = ChildProject.annotations.AnnotationManager(project) #temporary instance to check for existing sets. This is suboptimal because an annotation manager will be created by Metrics. However, the metrics class raises a ValueError for every set passed that does not exist, here we want to check in advance which of the alice and vcm sets exist without raising an error
+        am = AnnotationManager(project) #temporary instance to check for existing sets. This is suboptimal because an annotation manager will be created by Metrics. However, the metrics class raises a ValueError for every set passed that does not exist, here we want to check in advance which of the alice and vcm sets exist without raising an error
               
         METRICS = np.array(
             [["voc_speaker_ph",self.vtc,'FEM'],
              ["voc_speaker_ph",self.vtc,'MAL'],
              ["voc_speaker_ph",self.vtc,'OCH'],
              ["voc_speaker_ph",self.vtc,'CHI'],
              ["voc_dur_speaker_ph",self.vtc,'FEM'],
@@ -668,15 +670,15 @@
             key: parameters[key]
             for key in parameters
             if key not in ["self", "kwargs", "func"] #not sure what func parameter is for, seems unecessary to keep
         }
         for key in kwargs: #add all kwargs to dictionary
             parameters[key] = kwargs[key]
         
-        self.project = ChildProject.projects.ChildProject(path)
+        self.project = ChildProject(path)
         self.project.read()
         
         try:
             datarepo = Repo(path)
             parameters['dataset_hash'] = datarepo.head.object.hexsha
         except InvalidGitRepositoryError:
             print("Your dataset is not currently a git repository")
@@ -697,15 +699,15 @@
         parameters['metrics_list'] = [ {k:v for k,v in m.items() if pd.notnull(v)} for m in metrics_df.to_dict(orient='records')]
         date = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
         # create a yaml file with all the parameters used
         self.parameters_path = os.path.splitext(self.destination)[0] + "_parameters_{}.yml".format(date)
         print("exported metrics to {}".format(self.destination))
         yaml.dump(
             {
-                "package_version": ChildProject.__version__,
+                "package_version": __version__,
                 "date": date,
                 "parameters": parameters,
             },
             open(self.parameters_path, "w+"),sort_keys=False,
         )
         print("exported sampler parameters to {}".format(self.parameters_path))
 
@@ -807,15 +809,15 @@
         
         try:
             datarepo = Repo(parameters["path"])
             parameters['dataset_hash'] = datarepo.head.object.hexsha
         except InvalidGitRepositoryError:
             print("Your dataset is not currently a git repository")
         
-        self.project = ChildProject.projects.ChildProject(parameters["path"])
+        self.project = ChildProject(parameters["path"])
         self.project.read()
         
         self.destination = parameters['destination']
         
         unwanted_keys = {'metrics', 'pipeline'}
         for i in unwanted_keys:
             if i in parameters : del parameters[i]
@@ -840,15 +842,15 @@
         parameters['metrics_list'] = [ {k:v for k,v in m.items() if pd.notnull(v)} for m in metrics_df.to_dict(orient='records')]
         date = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
         # create a yaml file with all the parameters used
         self.parameters_path = os.path.splitext(self.destination)[0] + "_parameters_{}.yml".format(date)
         print("exported metrics to {}".format(self.destination))
         yaml.dump(
             {
-                "package_version": ChildProject.__version__,
+                "package_version": __version__,
                 "date": date,
                 "parameters": parameters,
             },
             open(self.parameters_path, "w+"),sort_keys=False,
         )
         print("exported metrics parameters to {}".format(self.parameters_path))
```

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/metricsFunctions.py` & `ChildProject-0.2.0/ChildProject/pipelines/metricsFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             # if we have results, return the max, else return NaN
             if len(result_array):
                 return np.nanmax(result_array)
             else:
                 return np.nan
 
         # wraps will give the same name and doc, so we need to slightly edit them for the peak function
-        new_func.__doc__ = "Computing the peak for 1h for the following metric:\n" + function.__doc__
+        new_func.__doc__ = "Computing the peak for 1h for the following metric:\n\n" + function.__doc__
         new_func.__name__ = "peak_" + function.__name__
         new_func.__qualname__ = "peak_" + function.__qualname__
         return new_func
     return decorator
 
 
 def per_hour_metric():
@@ -156,15 +156,15 @@
             """
         @functools.wraps(function)
         def new_func(annotations: pd.DataFrame, duration: int, **kwargs):
             # time to consider for periods, here 1h by default, else put it in kwargs
             return function(annotations, duration, **kwargs) * (3600000 / duration)
 
         # wraps will give the same name and doc, so we need to slightly edit them for the peak function
-        new_func.__doc__ = function.__doc__ + "This value is a 'per hour' value."
+        new_func.__doc__ = function.__doc__ + "\nThis value is a 'per hour' value."
         new_func.__name__ = function.__name__ + '_ph'
         new_func.__qualname__ = function.__qualname__ + '_ph'
         return new_func
     return decorator
 
 
 def voc_speaker(annotations: pd.DataFrame, duration: int, **kwargs):
```

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/pipeline.py` & `ChildProject-0.2.0/ChildProject/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/processors.py` & `ChildProject-0.2.0/ChildProject/pipelines/processors.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 import pandas as pd
 import shutil
 import subprocess
 from typing import Union, List
 from yaml import dump
 import logging
 
-import ChildProject
-from ChildProject.pipelines.pipeline import Pipeline
+from ..projects import ChildProject, CONVERTED_RECORDINGS
+from .pipeline import Pipeline
+
+from ChildProject import __version__
 
 # Create a logger for the module (file)
 logger_annotations = logging.getLogger(__name__)
 # messages are propagated to the higher level logger (ChildProject), used in cmdline.py
 logger_annotations.propagate = True
 
 pipelines = {}
 
 
 class AudioProcessor(ABC):
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         name: str,
         input_profile: str = None,
         threads: int = 1,
         recordings: Union[str, List[str], pd.DataFrame] = None,
     ):
 
         self.project = project
@@ -39,15 +41,15 @@
         self.recordings = Pipeline.recordings_from_list(recordings)
 
         self.input_profile = input_profile
 
         if self.input_profile:
             input_path = os.path.join(
                 self.project.path,
-                ChildProject.projects.CONVERTED_RECORDINGS,
+                CONVERTED_RECORDINGS,
                 self.input_profile,
             )
 
             assert os.path.exists(
                 input_path
             ), f"provided input profile {input_profile} does not exist"
 
@@ -56,15 +58,15 @@
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         pipelines[cls.SUBCOMMAND] = cls
 
     def output_directory(self):
         return os.path.join(
             self.project.path,
-            ChildProject.projects.CONVERTED_RECORDINGS,
+            CONVERTED_RECORDINGS,
             self.name,
         )
 
     def read_metadata(self):
         path = os.path.join(self.output_directory(), "recordings.csv")
 
         if os.path.exists(path):
@@ -128,15 +130,15 @@
 
 
 class BasicProcessor(AudioProcessor):
     SUBCOMMAND = "basic"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         name: str,
         format: str,
         codec: str,
         sampling: int,
         threads: int = 1,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         skip_existing: bool = False,
@@ -261,15 +263,15 @@
 
 
 class VettingProcessor(AudioProcessor):
     SUBCOMMAND = "vetting"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         name: str,
         segments_path: str,
         threads: int = 1,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         input_profile: str = None,
     ):
 
@@ -353,15 +355,15 @@
 
 
 class ChannelMapper(AudioProcessor):
     SUBCOMMAND = "channel-mapping"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         name: str,
         channels: list,
         threads: int = 1,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         input_profile: str = None,
     ):
 
@@ -440,15 +442,15 @@
         )
 
 class AudioStandard(AudioProcessor):
     SUBCOMMAND = "standard"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         threads: int = 1,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         skip_existing: bool = False,
         input_profile: str = None,
     ):
 
         super().__init__(
@@ -575,15 +577,15 @@
             {key: parameters[key]}
             for key in parameters
             if key not in ["self", "kwargs"]
         ]
         parameters.extend([{key: kwargs[key]} for key in kwargs])
 
         date = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-        self.project = ChildProject.projects.ChildProject(path)
+        self.project = ChildProject(path)
         self.project.read()
 
         if processor not in pipelines:
             raise NotImplementedError(f"invalid pipeline '{processor}'")
 
         proc = pipelines[processor](self.project, threads=threads, **kwargs)
         proc.process(f"parameters_{date}.yml")
@@ -597,15 +599,15 @@
 
         parameters_path = os.path.join(
             proc.output_directory(), f"parameters_{date}.yml"
         )
         dump(
             {
                 "parameters": parameters,
-                "package_version": ChildProject.__version__,
+                "package_version": __version__,
                 "date": date,
             },
             open(parameters_path, "w+"),
         )
         
         logger_annotations.info(
             "exported processor parameters to ",
```

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/samplers.py` & `ChildProject-0.2.0/ChildProject/pipelines/samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 from pydub import AudioSegment
 import sys
 import traceback
 from typing import Union, List
 from yaml import dump
 import logging
 
-import ChildProject
-from ChildProject.pipelines.pipeline import Pipeline
+from ..projects import ChildProject
+from ..annotations import AnnotationManager
+from .pipeline import Pipeline
+
+from ChildProject import __version__
 
 # Create a logger for the module (file)
 logger_annotations = logging.getLogger(__name__)
 # messages are propagated to the higher level logger (ChildProject), used in cmdline.py
 logger_annotations.propagate = True
 
 pipelines = {}
 
 
 class Sampler(ABC):
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         exclude: Union[str, pd.DataFrame] = None,
     ):
 
         self.project = project
 
         self.segments = pd.DataFrame()
@@ -71,15 +74,15 @@
 
     def sample(self):
         self._sample()
         self.remove_excluded()
         return self.segments
 
     def retrieve_segments(self, recording_filename=None):
-        am = ChildProject.annotations.AnnotationManager(self.project)
+        am = AnnotationManager(self.project)
         annotations = am.annotations
         annotations = annotations[annotations["set"] == self.annotation_set]
 
         if recording_filename:
             annotations = annotations[
                 annotations["recording_filename"] == recording_filename
             ]
@@ -174,15 +177,15 @@
 
 
 class CustomSampler(Sampler):
     SUBCOMMAND = "custom"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         segments_path: str,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         exclude: Union[str, pd.DataFrame] = None,
     ):
 
         super().__init__(project, recordings, exclude)
         self.segments_path = segments_path
@@ -212,15 +215,15 @@
     :type recordings: Union[str, List[str], pd.DataFrame], optional
     """
 
     SUBCOMMAND = "periodic"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         length: int,
         period: int,
         offset: int = 0,
         profile: str = None,
         recordings: Union[str, List[str], pd.DataFrame] = None,
         exclude: Union[str, pd.DataFrame] = None,
     ):
@@ -315,15 +318,15 @@
     :type threads: int, optional
     """
 
     SUBCOMMAND = "random-vocalizations"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         annotation_set: str,
         target_speaker_type: list,
         sample_size: int,
         threads: int = 1,
         by: str = "recording_filename",
         recordings: Union[str, List[str], pd.DataFrame] = None,
         exclude: Union[str, pd.DataFrame] = None,
@@ -431,15 +434,15 @@
     :type threads: int, optional
     """
 
     SUBCOMMAND = "energy-detection"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         windows_length: int,
         windows_spacing: int,
         windows_count: int,
         windows_offset: int = 0,
         threshold: float = 0.8,
         low_freq: int = 0,
         high_freq: int = 100000,
@@ -666,15 +669,15 @@
     :type threads: int
     """
 
     SUBCOMMAND = "high-volubility"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         annotation_set: str,
         metric: str,
         windows_length: int,
         windows_count: int,
         speakers: List[str] = ["FEM", "MAL", "CHI"],
         threads: int = 1,
         by: str = "recording_filename",
@@ -880,15 +883,15 @@
     :type exclude: Union[str, pd.DataFrame], optional
     """
 
     SUBCOMMAND = "conversations"
 
     def __init__(
         self,
-        project: ChildProject.projects.ChildProject,
+        project: ChildProject,
         annotation_set: str,
         count: int,
         interval: int = 1000,
         speakers: List[str] = ["FEM", "MAL", "CHI"],
         threads: int = 1,
         by: str = "recording_filename",
         recordings: Union[str, List[str], pd.DataFrame] = None,
@@ -1020,15 +1023,15 @@
         parameters = [
             {key: parameters[key]}
             for key in parameters
             if key not in ["self", "kwargs"]
         ]
         parameters.extend([{key: kwargs[key]} for key in kwargs])
 
-        self.project = ChildProject.projects.ChildProject(path)
+        self.project = ChildProject(path)
         self.project.read()
 
         if sampler not in pipelines:
             raise NotImplementedError(f"invalid pipeline '{sampler}'")
 
         splr = pipelines[sampler](self.project, **kwargs)
 
@@ -1049,15 +1052,15 @@
         logger_annotations.info(
                 "exported sampled segments to %s", 
                 segments_path, 
                 )
         dump(
             {
                 "parameters": parameters,
-                "package_version": ChildProject.__version__,
+                "package_version": __version__,
                 "date": date,
             },
             open(parameters_path, "w+"),
         )
         logger_annotations.info(
                 "exported sampler parameters to %s", 
                 parameters_path,
```

### Comparing `ChildProject-0.1.2/ChildProject/pipelines/zooniverse.py` & `ChildProject-0.2.0/ChildProject/pipelines/zooniverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,43 @@
 
 from pydub import AudioSegment
 from pydub.utils import get_array_type
 
 from parselmouth import Sound
 from parselmouth import SpectralAnalysisWindowShape
 
-import ChildProject
-from ChildProject.pipelines.pipeline import Pipeline
-from ChildProject.tables import assert_dataframe, assert_columns_presence
-from ChildProject.utils import retry_func
+from ..projects import ChildProject
+from .pipeline import Pipeline
+from ..tables import assert_dataframe, assert_columns_presence
+from ..utils import retry_func
+
+from ChildProject import __version__
 
 from typing import Tuple
 
 import time
 
+CHUNKS_DTYPES = {
+    'recording_filename':  'string',
+    'onset': int,
+    'offset': int,
+    'segment_onset': int,
+    'segment_offset': int,
+    'wav': 'string',
+    'mp3': 'string',
+    'date_extracted': 'string',
+    'uploaded': 'boolean',
+    'project_id': 'Int64',
+    'subject_set': 'string',
+    'zooniverse_id': 'Int64',
+    'keyword': 'string',
+    'subject_set_id': 'Int64',
+    'dataset' : 'string',
+}
+
 # Create a logger for the module (file)
 logger_annotations = logging.getLogger(__name__)
 # messages are propagated to the higher level logger (ChildProject), used in cmdline.py
 logger_annotations.propagate = True
 
 def pad_interval(
     onset: int, offset: int, chunks_length: int, chunks_min_amount: int = 1
@@ -268,15 +288,15 @@
             {key: parameters[key]}
             for key in parameters
             if key not in ["self", "kwargs"]
         ]
         parameters.extend([{key: kwargs[key]} for key in kwargs])
 
         self.destination = destination
-        self.project = ChildProject.projects.ChildProject(path)
+        self.project = ChildProject(path)
         self.project.read()
 
         self.chunks_length = int(chunks_length)
         self.chunks_min_amount = int(chunks_min_amount)
         self.spectro = spectrogram
         self.profile = profile
 
@@ -318,18 +338,18 @@
                     "wav": c.getbasename("wav"),
                     "mp3": c.getbasename("mp3"),
                     "png": c.getbasename("png") if self.spectro else "NA",
                     "date_extracted": datetime.datetime.now().strftime(
                         "%Y-%m-%d %H:%M:%S"
                     ),
                     "uploaded": False,
-                    "project_id": "",
+                    "project_id": pd.NA,
                     "subject_set": "",
                     "subject_set_id": pd.NA,
-                    "zooniverse_id": 0,
+                    "zooniverse_id": pd.NA,
                     "keyword": keyword,
                     "dataset": self.project.experiment
                 }
                 for c in self.chunks
             ]
         )
 
@@ -343,15 +363,15 @@
         parameters_path = os.path.join(destination, "parameters_{}.yml".format(date))
 
         self.chunks.to_csv(chunks_path)
         logger_annotations.info("exported chunks metadata to %s", chunks_path)
         dump(
             {
                 "parameters": parameters,
-                "package_version": ChildProject.__version__,
+                "package_version": __version__,
                 "date": date,
             },
             open(parameters_path, "w+"),
         )
         logger_annotations.info("exported extract-chunks parameters to %s", parameters_path)
 
         return chunks_path, parameters_path
@@ -392,29 +412,29 @@
         """
 
         self.chunks_file = chunks
         self.get_credentials(zooniverse_login, zooniverse_pwd)
 
         metadata_location = os.path.join(self.chunks_file)
         try:
-            self.chunks = pd.read_csv(metadata_location, index_col="index")
+            self.chunks = pd.read_csv(metadata_location, index_col="index", dtype=CHUNKS_DTYPES)
         except:
             raise Exception(
                 "cannot read chunk metadata from {}.".format(metadata_location)
             )
 
         assert_dataframe("chunks", self.chunks)
         assert_columns_presence(
             "chunks",
             self.chunks,
             {"recording_filename", "onset", "offset", "uploaded", "mp3"},
         )
         
         if test_endpoint:
-            from ChildProject.pipelines.fake_panoptes import Panoptes, Project, Subject, SubjectSet, PanoptesAPIException, reset_tests, TEST_MAX_SUBJECT
+            from .fake_panoptes import Panoptes, Project, Subject, SubjectSet, PanoptesAPIException, reset_tests, TEST_MAX_SUBJECT
             reset_tests()
             if test_endpoint == 2: Subject.max_subjects = TEST_MAX_SUBJECT
         else:
             from panoptes_client import Panoptes, Project, Subject, SubjectSet
             from panoptes_client.panoptes import PanoptesAPIException
 
 
@@ -497,66 +517,74 @@
                 chunk_index,
                 subject_set.display_name,
                 str(e),
                 )
                 logger_annotations.error("%s", traceback.format_exc())
                 
                 chunk["index"] = chunk_index
-                chunk["zooniverse_id"] = str(subject.id)
-                chunk["project_id"] = str(project_id)
+                chunk["zooniverse_id"] = subject.id
+                chunk["project_id"] = project_id
                 chunk["subject_set"] = ""
                 chunk['subject_set_id'] = pd.NA
                 chunk["uploaded"] = True
                 self.orphan_chunks.append(chunk)
                 
                 if ignore_errors:
                     continue
                 else:
                     logger_annotations.error("subject upload halting here.")
                     break
 
             chunk["index"] = chunk_index
-            chunk["zooniverse_id"] = str(subject.id)
-            chunk["project_id"] = str(project_id)
+            chunk["zooniverse_id"] = subject.id
+            chunk["project_id"] = project_id
             chunk["subject_set"] = str(subject_set.display_name)
-            chunk["subject_set_id"] = str(subject_set.id)
+            chunk["subject_set_id"] = subject_set.id
             chunk["uploaded"] = True
             self.subjects_metadata.append(chunk)
 
         if len(self.subjects_metadata) + len(self.orphan_chunks) == 0:
             return
 
-        if len(self.subjects_metadata) : self.chunks.update(pd.DataFrame(self.subjects_metadata).set_index("index"))
-        
+        if len(self.subjects_metadata):
+            self.chunks.update(pd.DataFrame(self.subjects_metadata).set_index("index"))
+
         if record_orphan and len(self.orphan_chunks): 
             self.chunks.update(pd.DataFrame(self.orphan_chunks).set_index("index"))
 
             logger_annotations.warning(
                 "%d chunks were uploaded but not linked to the subject set '%s'. To attempt to relink them, try link_orphan_subjects",
                 len(self.orphan_chunks),
                 subject_set.display_name,
                 )
 
+        # known issue in pandas < 2.0, dtypes are changed with update, save the dtypes and restore them
+        self.chunks = self.chunks.astype(CHUNKS_DTYPES)
         self.chunks.to_csv(self.chunks_file)
         
         signal.signal(signal.SIGINT, original_sigint_handler)
         signal.signal(signal.SIGTERM, original_sigterm_handler)
         
     def exit_upload(self, *args, rec_orphan, sub_set):
         if len(self.subjects_metadata) + len(self.orphan_chunks) != 0:
-            if len(self.subjects_metadata) : self.chunks.update(pd.DataFrame(self.subjects_metadata).set_index("index"))
+
+            if len(self.subjects_metadata):
+                self.chunks.update(pd.DataFrame(self.subjects_metadata).set_index("index"))
             
             if rec_orphan and len(self.orphan_chunks): 
                 self.chunks.update(pd.DataFrame(self.orphan_chunks).set_index("index"))
+
                 logger_annotations.warning(
                 "%d chunks were uploaded but not linked to the subject set '%s'. To attempt to relink them, try link_orphan_subjects",
                 len(self.orphan_chunks),
                 sub_set,
                 )
-                
+
+            # known issue in pandas < 2.0, dtypes are changed with update, save the dtypes and restore them
+            self.chunks.astype(CHUNKS_DTYPES)
             self.chunks.to_csv(self.chunks_file)
         logger_annotations.warning('Signal interruption %s, exited gracefully', args[0])
         sys.exit(0)
         
         
     def link_orphan_subjects(
         self,
@@ -592,29 +620,29 @@
         """
         
         self.chunks_file = chunks
         self.get_credentials(zooniverse_login, zooniverse_pwd)
 
         metadata_location = os.path.join(self.chunks_file)
         try:
-            self.chunks = pd.read_csv(metadata_location, index_col="index")
+            self.chunks = pd.read_csv(metadata_location, index_col="index", dtype=CHUNKS_DTYPES)
         except:
             raise Exception(
                 "cannot read chunk metadata from {}.".format(metadata_location)
             )
 
         assert_dataframe("chunks", self.chunks)
         assert_columns_presence(
             "chunks",
             self.chunks,
             {"recording_filename", "onset", "offset", "uploaded", "mp3", "zooniverse_id", "project_id", "subject_set"},
         )
         
         if test_endpoint:
-            from ChildProject.pipelines.fake_panoptes import Panoptes, Project, Subject, SubjectSet, PanoptesAPIException, reset_tests
+            from .fake_panoptes import Panoptes, Project, Subject, SubjectSet, PanoptesAPIException, reset_tests
             reset_tests() 
         else:
             from panoptes_client import Panoptes, Project, Subject, SubjectSet
             from panoptes_client.panoptes import PanoptesAPIException
 
         Panoptes.connect(username=self.zooniverse_login, password=self.zooniverse_pwd)
         zooniverse_project = Project(project_id)
@@ -686,22 +714,24 @@
                     continue
                 else:
                     logger_annotations.error("subject linking halting here.")
                     break
 
             chunk["index"] = chunk_index
             chunk["subject_set"] = str(subject_set.display_name)
-            chunk["subject_set_id"] = str(subject_set.id)
+            chunk["subject_set_id"] = subject_set.id
             subjects_metadata.append(chunk)
 
         if len(subjects_metadata):
             tmp = pd.DataFrame(subjects_metadata)
             logger_annotations.info('%s \n%s', tmp.columns, tmp)
             self.chunks.update(pd.DataFrame(subjects_metadata).set_index("index"))
 
+            # known issue in pandas < 2.0, dtypes are changed with update, save the dtypes and restore them
+            self.chunks = self.chunks.astype(CHUNKS_DTYPES)
             self.chunks.to_csv(self.chunks_file)
         logger_annotations.info('linked %d/%d subjects', len(subjects_metadata), len(chunks_to_link))
         
     def reset_orphan_subjects(
         self,
         chunks: str,
         **kwargs
@@ -714,15 +744,15 @@
         :type chunks: [type]
         """
         
         self.chunks_file = chunks
 
         metadata_location = os.path.join(self.chunks_file)
         try:
-            self.chunks = pd.read_csv(metadata_location, index_col="index")
+            self.chunks = pd.read_csv(metadata_location, index_col="index", dtype=CHUNKS_DTYPES)
         except:
             raise Exception(
                 "cannot read chunk metadata from {}.".format(metadata_location)
             )
 
         assert_dataframe("chunks", self.chunks)
         assert_columns_presence(
@@ -733,15 +763,15 @@
 
         # select chunks that are uploaded, have an id and project but no set
         selection = ((self.chunks["uploaded"] == True) &
                       (~self.chunks['zooniverse_id'].isnull()) &
                       (~self.chunks['project_id'].isnull()) &
                       (self.chunks['subject_set'].isnull()))
 
-        self.chunks.loc[selection , ['uploaded','zooniverse_id','project_id']] = (False, "", "") 
+        self.chunks.loc[selection , ['uploaded','zooniverse_id','project_id']] = (False, pd.NA, pd.NA)
 
         nb_reset = selection[selection == True]
         if nb_reset.shape[0]:
             self.chunks.to_csv(self.chunks_file)
             
             logger_annotations.info('reset %d orphan subjects', nb_reset)
         else:
@@ -773,15 +803,15 @@
         :param chunks: the list of chunk metadata files to match the classifications to. If provided, only the classifications that have a match will be returned.
         :type chunks: List[str], optional
         """
         self.get_credentials(zooniverse_login, zooniverse_pwd)
 
         # if used in tests, use the fake functions
         if test_endpoint:
-            from ChildProject.pipelines.fake_panoptes import Panoptes, Project, Classification
+            from .fake_panoptes import Panoptes, Project, Classification
         else:
             from panoptes_client import Panoptes, Project, Classification
             
         Panoptes.connect(username=self.zooniverse_login, password=self.zooniverse_pwd)
         project = Project(project_id)
 
         answers_translation_table = []
```

### Comparing `ChildProject-0.1.2/ChildProject/projects.py` & `ChildProject-0.2.0/ChildProject/projects.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/tables.py` & `ChildProject-0.2.0/ChildProject/tables.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/templates/basic.etf` & `ChildProject-0.2.0/ChildProject/templates/basic.etf`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/templates/basic.pfsx` & `ChildProject-0.2.0/ChildProject/templates/basic.pfsx`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/templates/native.etf` & `ChildProject-0.2.0/ChildProject/templates/native.etf`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/templates/native.pfsx` & `ChildProject-0.2.0/ChildProject/templates/native.pfsx`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/templates/non-native.etf` & `ChildProject-0.2.0/ChildProject/templates/non-native.etf`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/templates/non-native.pfsx` & `ChildProject-0.2.0/ChildProject/templates/non-native.pfsx`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/ChildProject/utils.py` & `ChildProject-0.2.0/ChildProject/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 from datetime import datetime
-from scipy.fftpack import fft, ifft
 import numpy as np
 import pandas as pd
 
 def path_is_parent(parent_path: str, child_path: str):
     # Smooth out relative path names, note: if you are concerned about symbolic links, you should use os.path.realpath too
     parent_path = os.path.abspath(parent_path)
     child_path = os.path.abspath(child_path)
@@ -200,26 +199,25 @@
     # straight up difference of the audio signal averaged over the 2 segments analysed
     # times 1000 is arbitrary, just to have an easily readable and comparable score output
     res = np.abs(ref - test).sum() * 1000 /(len(ref))
 
     return res,len(ref)
 
 def find_lines_involved_in_overlap(df: pd.DataFrame, onset_label: str = 'range_onset', offset_label:str = 'range_offset', labels = []):
-    """
-    takes a dataframe as input. The dataframe is supposed to have a column for the onset
+    """takes a dataframe as input. The dataframe is supposed to have a column for the onset
     og a timeline and one for the offset. The function returns a boolean series where
     all indexes having 'True' are lines involved in overlaps and 'False' when not
     e.g. to select all lines involved in overlaps, use:
-        ```
-        ovl_segments = df[find_lines_involved_in_overlap(df, 'segment_onset', 'segment_offset')]
-        ```
-        and to select line that never overlap, use:
-        ```
-        ovl_segments = df[~find_lines_involved_in_overlap(df, 'segment_onset', 'segment_offset')]
-        ```
+    ```
+    ovl_segments = df[find_lines_involved_in_overlap(df, 'segment_onset', 'segment_offset')]
+    ```
+    and to select line that never overlap, use:
+    ```
+    ovl_segments = df[~find_lines_involved_in_overlap(df, 'segment_onset', 'segment_offset')]
+    ```
         
     :param df: pandas DataFrame where we want to find overlaps, having some time segments described by 2 columns (onset and offset)
     :type df: pd.DataFrame
     :param onset_label: column label for the onset of time segments
     :type onset_label: str
     :param offset_label: columns label for the offset of time segments
     :type offset_label: str
```

### Comparing `ChildProject-0.1.2/ChildProject.egg-info/PKG-INFO` & `ChildProject-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-Metadata-Version: 2.1
-Name: ChildProject
-Version: 0.1.2
-Summary: LAAC@LSCP
-Home-page: https://github.com/LAAC-LSCP/ChildProject
-Author: Lucas Gautheron
-Author-email: lucas.gautheron@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ChildProject
 ============
+[![PyPI](https://img.shields.io/pypi/v/childproject.svg)](https://pypi.org/project/childproject/)
+[![GitHub tests](https://github.com/LAAC-LSCP/ChildProject/actions/workflows/tests.yml/badge.svg)](https://github.com/LAAC-LSCP/ChildProject/actions/workflows/tests.yml)
+[![Travis CI Status](https://app.travis-ci.com/LAAC-LSCP/ChildProject.svg?token=1d35csHFpystSMdwuSY8&branch=master)](https://app.travis-ci.com/LAAC-LSCP/ChildProject)
+[![ReadTheDocs](https://readthedocs.org/projects/childproject/badge/?version=latest)](https://childproject.readthedocs.io/en/latest/)
+[![License](https://img.shields.io/pypi/l/childproject.svg)](https://github.com/LAAC-LSCP/ChildProject/blob/master/LICENSE)
+
 
 - [Introduction](#introduction)
 - [Available tools](#available-tools)
 - [Installation](#installation)
 
 Introduction
 ------------
```

### Comparing `ChildProject-0.1.2/ChildProject.egg-info/SOURCES.txt` & `ChildProject-0.2.0/ChildProject.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 ChildProject/__init__.py
 ChildProject/annotations.py
 ChildProject/cmdline.py
 ChildProject/converters.py
 ChildProject/metrics.py
 ChildProject/projects.py
 ChildProject/tables.py
 ChildProject/utils.py
 ChildProject.egg-info/PKG-INFO
 ChildProject.egg-info/SOURCES.txt
 ChildProject.egg-info/dependency_links.txt
 ChildProject.egg-info/entry_points.txt
-ChildProject.egg-info/not-zip-safe
 ChildProject.egg-info/requires.txt
 ChildProject.egg-info/top_level.txt
 ChildProject/pipelines/__init__.py
 ChildProject/pipelines/anonymize.py
 ChildProject/pipelines/derivations.py
 ChildProject/pipelines/eafbuilder.py
 ChildProject/pipelines/fake_panoptes.py
```

### Comparing `ChildProject-0.1.2/LICENSE` & `ChildProject-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_annotations.py` & `ChildProject-0.2.0/tests/test_annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,16 +815,16 @@
     truth["utterances"] = truth.apply(
         partial(gather_columns_to_dict, "startUtt", "endUtt"), axis=1
     ).astype(str)
     truth["vfxs"] = truth.apply(
         partial(gather_columns_to_dict, "startVfx", "endVfx"), axis=1
     ).astype(str)
 
-    truth["segment_onset"] = (truth["segment_onset"] * 1000).astype(int)
-    truth["segment_offset"] = (truth["segment_offset"] * 1000).astype(int)
+    truth["segment_onset"] = (truth["segment_onset"] * 1000).round().astype(int)
+    truth["segment_offset"] = (truth["segment_offset"] * 1000).round().astype(int)
 
     truth["lena_conv_floor_type"].fillna("NA", inplace=True)
     truth["lena_conv_turn_type"].fillna("NA", inplace=True)
     truth["lena_response_count"].fillna("NA", inplace=True)
 
     columns = [
         "segment_onset",
```

### Comparing `ChildProject-0.1.2/tests/test_cli.py` & `ChildProject-0.2.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 def cli(cmd):
     process = subprocess.Popen(cmd, stderr=subprocess.PIPE, stdout=subprocess.PIPE)
     stdout, stderr = process.communicate()
     exit_code = process.wait()
     return stdout, stderr, exit_code
 
+
 @pytest.fixture(scope="function")
 def project(request):
     if os.path.exists(PATH):
         # shutil.copytree(src="examples/valid_raw_data", dst=PATH)
         shutil.rmtree(PATH)
     shutil.copytree(src="examples/valid_raw_data", dst=PATH)
 
@@ -24,14 +25,16 @@
     yield project
 
 
 def test_validate(project):
     stdout, stderr, exit_code = cli(
         ["child-project", "validate", PATH]
     )
+    print(stdout)
+    print(stderr)
     assert exit_code == 0
 
 
 def test_overview(project):
     stdout, stderr, exit_code = cli(
         ["child-project", "overview", PATH]
     )
```

### Comparing `ChildProject-0.1.2/tests/test_convert.py` & `ChildProject-0.2.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_derivations.py` & `ChildProject-0.2.0/tests/test_derivations.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_documentation.py` & `ChildProject-0.2.0/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_metrics.py` & `ChildProject-0.2.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_pipelines.py` & `ChildProject-0.2.0/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_projects.py` & `ChildProject-0.2.0/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_reliability.py` & `ChildProject-0.2.0/tests/test_reliability.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_samplers.py` & `ChildProject-0.2.0/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_utils.py` & `ChildProject-0.2.0/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,26 +24,26 @@
                        datetime.datetime(1900,1,1,12,19,21,0),
                        pd.NaT,
                        ])
     
     #convert to datetime using the formats for start_time listed in the project RECORDINGS_COLUMNS.Index(name == 'start_time')
     converted_time = series_to_datetime(only_time, project.RECORDINGS_COLUMNS, 'start_time')
     
-    pd.testing.assert_series_equal(converted_time, truth)
+    pd.testing.assert_series_equal(converted_time, truth, check_index_type=False, check_dtype=False)
     
     truth = pd.Series([datetime.datetime(2022,1,23,3,12,0,0),
                        datetime.datetime(2022,1,23,4,14,0,0),
                        datetime.datetime(2022,1,23,12,19,21,0),
                        pd.NaT,
                        ])
     
     #convert to datetime using the formats for start_time and date_iso listed in the project RECORDINGS_COLUMNS.Index(name == 'start_time') and Index(name == 'date_iso')
     converted_time = series_to_datetime(only_time, project.RECORDINGS_COLUMNS, 'start_time', only_date, project.RECORDINGS_COLUMNS, 'date_iso')
     
-    pd.testing.assert_series_equal(converted_time, truth)
+    pd.testing.assert_series_equal(converted_time, truth, check_index_type=False, check_dtype=False)
     
 def test_time_intervals_intersect():
     truth = [TimeInterval(datetime.datetime(1900,1,1,10,36),datetime.datetime(1900,1,1,21,4))]
     res = time_intervals_intersect(TimeInterval(datetime.datetime(1900,1,1,8,57),datetime.datetime(1900,1,1,21,4)),TimeInterval(datetime.datetime(1900,1,1,10,36),datetime.datetime(1900,1,1,22,1)))
     
     for i in range(len(truth)):
         assert truth[i] == res[i] 
@@ -99,8 +99,8 @@
     
     
     
     
     
     
     
-    
+
```

### Comparing `ChildProject-0.1.2/tests/test_validation.py` & `ChildProject-0.2.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `ChildProject-0.1.2/tests/test_zooniverse.py` & `ChildProject-0.2.0/tests/test_zooniverse.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 import shutil
 
 from ChildProject.projects import ChildProject
 from ChildProject.pipelines.samplers import PeriodicSampler
 from ChildProject.pipelines.zooniverse import ZooniversePipeline, pad_interval
 from ChildProject.pipelines.fake_panoptes import LOCATION_FAIL
+from ChildProject.pipelines.zooniverse import CHUNKS_DTYPES
 
 
 def test_padding():
     assert pad_interval(300, 800, 500, 1) == (300, 800)
     assert pad_interval(200, 800, 500, 2) == (0, 1000)
 
     assert pad_interval(300, 900, 500, 1) == (100, 1100)
@@ -40,15 +41,15 @@
         keyword="test",
         segments="output/zooniverse/sampled_segments.csv",
         chunks_length=250,
         chunks_min_amount=2,
         spectrogram=True,
     )
 
-    chunks = pd.read_csv(chunks)
+    chunks = pd.read_csv(chunks, dtype=CHUNKS_DTYPES)
 
     assert len(chunks) == 2 * len(segments)
     assert all(
         chunks["wav"]
         .apply(lambda f: os.path.exists(os.path.join("output/zooniverse/chunks", f)))
         .tolist()
     )
@@ -81,32 +82,32 @@
     df = pd.read_csv(BASE_CHUNKS)
     
     zooniverse = ZooniversePipeline()
     
     if amount is None: amount = 1000
     
     if not location_fail: df = df[df['mp3'] != LOCATION_FAIL]
-    
+
     df.to_csv(new_path,index=False)
     
     zooniverse.upload_chunks(new_path,
                              404,
                              'test_subject_set',
                              'test_username',
                              'test_password',
                              amount,
                              ignore_errors,
                              record_orphan,
                              test_endpoint=True if result != 'max_subjects_continue.csv' else 2,
                              )
     
-    truth = pd.read_csv(os.path.join('tests','truth','zoochunks',result))
-    #shutil.copy(new_path, os.path.join('tests','truth','zoochunks',result))
+    truth = pd.read_csv(os.path.join('tests','truth','zoochunks',result), dtype=CHUNKS_DTYPES)
+    # shutil.copy(new_path, os.path.join('tests','truth','zoochunks',result))
     
-    pd.testing.assert_frame_equal(truth, pd.read_csv(new_path), check_like=True)
+    pd.testing.assert_frame_equal(truth, pd.read_csv(new_path, dtype=CHUNKS_DTYPES), check_like=True)
    
 #might benefit from a test using invalid csv or/and a test with a csv having no orphan chunk     
 BASE_ORPHAN_CHUNKS = os.path.join('tests', 'data', 'chunks_test_orphan.csv')   
 @pytest.mark.parametrize("ignore_errors,result", 
                          [(False,'link_orphan_stop.csv'),
                          (True,'link_orphan_continue.csv'),
                          ])
@@ -122,28 +123,30 @@
                                     404,
                                     'test_subject_set',
                                     'test_username',
                                     'test_password',
                                     ignore_errors,
                                     test_endpoint=True,
                                     )
-   # shutil.copy(new_path, os.path.join('tests','truth','zoochunks',result))
-    pd.testing.assert_frame_equal(pd.read_csv(os.path.join('tests','truth','zoochunks',result)), pd.read_csv(new_path))
+    # shutil.copy(new_path, os.path.join('tests','truth','zoochunks',result))
+    pd.testing.assert_frame_equal(pd.read_csv(os.path.join('tests','truth','zoochunks',result), dtype=CHUNKS_DTYPES),
+                                  pd.read_csv(new_path, dtype=CHUNKS_DTYPES))
     
 @pytest.mark.parametrize("result", 
                          [('reset_orphan.csv'),
                          ])
 def test_reset_orphan(result):
     new_path = os.path.join('output', 'zooniverse', 'chunks_test_reset_orphan.csv')
     os.makedirs("output/zooniverse", exist_ok=True)
     
     shutil.copy(BASE_ORPHAN_CHUNKS,new_path)
     
     zooniverse = ZooniversePipeline()
     
     zooniverse.reset_orphan_subjects(new_path)
     
-    #shutil.copy(new_path, os.path.join('tests','truth','zoochunks',result))
-    pd.testing.assert_frame_equal(pd.read_csv(os.path.join('tests','truth','zoochunks',result)), pd.read_csv(new_path))
+    # shutil.copy(new_path, os.path.join('tests','truth','zoochunks',result))
+    pd.testing.assert_frame_equal(pd.read_csv(os.path.join('tests','truth','zoochunks',result), dtype=CHUNKS_DTYPES),
+                                  pd.read_csv(new_path, dtype=CHUNKS_DTYPES))
     
 def test_classification():
     pass
```

