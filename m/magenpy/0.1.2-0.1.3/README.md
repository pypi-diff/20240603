# Comparing `tmp/magenpy-0.1.2.tar.gz` & `tmp/magenpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magenpy-0.1.2.tar", last modified: Thu Apr 25 18:52:52 2024, max compression
+gzip compressed data, was "magenpy-0.1.3.tar", last modified: Mon Jun  3 01:06:38 2024, max compression
```

## Comparing `magenpy-0.1.2.tar` & `magenpy-0.1.3.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-25 18:52:40.000000 magenpy-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 18:52:40.000000 magenpy-0.1.2/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-25 18:52:40.000000 magenpy-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 18:52:40.000000 magenpy-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-25 18:52:52.805313 magenpy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-25 18:52:40.000000 magenpy-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.793313 magenpy-0.1.2/bin/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-25 18:52:40.000000 magenpy-0.1.2/bin/magenpy_ld
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-25 18:52:40.000000 magenpy-0.1.2/bin/magenpy_simulate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.793313 magenpy-0.1.2/magenpy/
--rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/AnnotationMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    44598 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/GWADataLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/GenotypeMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    55339 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/LDMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/SampleTable.py
--rw-r--r--   0 runner    (1001) docker     (127)    25688 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/SumstatsTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.793313 magenpy-0.1.2/magenpy/config/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/config/paths.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.797313 magenpy-0.1.2/magenpy/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1514113 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bed
--rw-r--r--   0 runner    (1001) docker     (127)   569420 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bim
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/1000G_eur_chr22.fam
--rw-r--r--   0 runner    (1001) docker     (127)   435206 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/ukb_height_chr22.fastGWA.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/annotation_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/misc_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/plink_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/sumstats_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/plot/gwa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/plot/ld.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/AnnotatedPhenotypeSimulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/MultiCohortPhenotypeSimulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15558 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/PhenotypeSimulator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/gwa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/gwa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/gwa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/h2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/h2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/h2/ldsc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/ld/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/c_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18884 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/stats/score/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/score.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/score_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/stats/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/transforms/genotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/transforms/phenotype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/stats/variant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/variant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/variant/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/compute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17719 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/system_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 18:52:40.000000 magenpy-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:52:52.805313 magenpy-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-25 18:52:40.000000 magenpy-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-25 18:52:40.000000 magenpy-0.1.2/tests/test_gdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 18:52:40.000000 magenpy-0.1.2/tests/test_ld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-25 18:52:40.000000 magenpy-0.1.2/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.272629 magenpy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-06-03 01:06:25.000000 magenpy-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-03 01:06:25.000000 magenpy-0.1.3/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-06-03 01:06:25.000000 magenpy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-03 01:06:25.000000 magenpy-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-06-03 01:06:38.272629 magenpy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-03 01:06:25.000000 magenpy-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.256629 magenpy-0.1.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)    11717 2024-06-03 01:06:25.000000 magenpy-0.1.3/bin/magenpy_ld
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-06-03 01:06:25.000000 magenpy-0.1.3/bin/magenpy_simulate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.260629 magenpy-0.1.3/magenpy/
+-rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/AnnotationMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/GWADataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/GenotypeMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58672 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/LDMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/SampleTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27954 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/SumstatsTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.260629 magenpy-0.1.3/magenpy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/config/paths.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.264629 magenpy-0.1.3/magenpy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1514113 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/data/1000G_eur_chr22.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   569420 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/data/1000G_eur_chr22.bim
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/data/1000G_eur_chr22.fam
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/data/lrld_hg19_GRCh37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   435206 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/data/ukb_height_chr22.fastGWA.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.264629 magenpy-0.1.3/magenpy/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/parsers/annotation_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/parsers/misc_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/parsers/plink_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/parsers/sumstats_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.264629 magenpy-0.1.3/magenpy/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/plot/gwa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/plot/ld.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/simulation/AnnotatedPhenotypeSimulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/simulation/MultiCohortPhenotypeSimulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15558 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/simulation/PhenotypeSimulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/stats/gwa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/gwa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/gwa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/stats/h2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/h2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/h2/ldsc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/stats/ld/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/ld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/ld/c_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/ld/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18877 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/ld/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/stats/score/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/score/score.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/score/score_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/score/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/stats/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/transforms/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/transforms/phenotype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.268629 magenpy-0.1.3/magenpy/stats/variant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/variant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/stats/variant/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.272629 magenpy-0.1.3/magenpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/utils/compute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/utils/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-06-03 01:06:25.000000 magenpy-0.1.3/magenpy/utils/system_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.272629 magenpy-0.1.3/magenpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-06-03 01:06:38.000000 magenpy-0.1.3/magenpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-06-03 01:06:38.000000 magenpy-0.1.3/magenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 01:06:38.000000 magenpy-0.1.3/magenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 01:06:37.000000 magenpy-0.1.3/magenpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-06-03 01:06:38.000000 magenpy-0.1.3/magenpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 01:06:38.000000 magenpy-0.1.3/magenpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-03 01:06:25.000000 magenpy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-03 01:06:25.000000 magenpy-0.1.3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-03 01:06:25.000000 magenpy-0.1.3/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 01:06:25.000000 magenpy-0.1.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-03 01:06:25.000000 magenpy-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 01:06:38.272629 magenpy-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-06-03 01:06:25.000000 magenpy-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 01:06:38.272629 magenpy-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-06-03 01:06:25.000000 magenpy-0.1.3/tests/test_gdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-06-03 01:06:25.000000 magenpy-0.1.3/tests/test_ld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-06-03 01:06:25.000000 magenpy-0.1.3/tests/test_simulation.py
```

### Comparing `magenpy-0.1.2/CHANGELOG.md` & `magenpy-0.1.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,42 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+
+## [0.1.3] - 2024-05-21
+
+### Changed
+
+- Updated the logic for `detect_outliers` in phenotype transforms to actually reflect the function
+name (before it was returning true for inliers...).
+- Updated `quantize` and `dequantize` to minimize data copying as much as possible.
+- Updated `LDMatrix.load_rows()` method to minimize data copying.
+- Fixed bug in `LDMatrix.n_neighbors` implementation.
+- Updated `dask` version in `requirements.txt` to avoid installing `dask-expr`.
+
+
+### Added
+
+- Added `get_peak_memory_usage` to `system_utils` to inspect peak memory usage of a process.
+- Placeholder method to perform QC on `SumstatsTable` objects (needs to be implemented still).
+- New attached dataset for long-range LD regions.
+- New method in SumstatsTable to impute rsID (if missing).
+- Preliminary support for matching with CHR+POS in SumstatsTable (still needs more work).
+- LDMatrix updates:
+  - New method to filter long-range LD regions.
+  - New method to prune LD matrix.
+- New algorithm for symmetrizing upper triangular and block diagonal LD matrices.
+  - Much faster and more memory efficient than using `scipy`.
+  - New `LDMatrix` class has efficient data loading in `.load_data` method.
+  - We still retain `load_rows` because it is useful for loading a subset of rows.
+
 ## [0.1.2] - 2024-04-24
 
 ### Changed
 
 - Fixed `manhattan` plot implementation to support various new features.
 - Added a warning when accessing `csr_matrix` property of `LDMatrix` when it hasn't been loaded
 previously.
```

### Comparing `magenpy-0.1.2/CITATION.md` & `magenpy-0.1.3/CITATION.md`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/LICENSE` & `magenpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/PKG-INFO` & `magenpy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magenpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modeling and Analysis of Statistical Genetics data in python
 Home-page: https://github.com/shz9/magenpy
 Author: Shadi Zabad
 Author-email: shadi.zabad@mail.mcgill.ca
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dask
+Requires-Dist: dask<=2024.1.0
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pandas-plink
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: zarr
```

### Comparing `magenpy-0.1.2/README.md` & `magenpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/bin/magenpy_ld` & `magenpy-0.1.3/bin/magenpy_ld`

 * *Files 3% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 import magenpy as mgp
 import time
 from datetime import timedelta
 from magenpy.utils.system_utils import valid_url
 from magenpy.GenotypeMatrix import xarrayGenotypeMatrix, plinkBEDGenotypeMatrix
 
 print(fr"""
-**********************************************                            
- _ __ ___   __ _  __ _  ___ _ __  _ __  _   _ 
-| '_ ` _ \ / _` |/ _` |/ _ \ '_ \| '_ \| | | |
-| | | | | | (_| | (_| |  __/ | | | |_) | |_| |
-|_| |_| |_|\__,_|\__, |\___|_| |_| .__/ \__, |
-                 |___/           |_|    |___/
-Modeling and Analysis of Genetics data in python
-Version: {mgp.__version__} | Release date: {mgp.__release_date__}
-Author: Shadi Zabad, McGill University
-**********************************************
-< Compute LD matrix and output in Zarr format >
+        **********************************************                            
+         _ __ ___   __ _  __ _  ___ _ __  _ __  _   _ 
+        | '_ ` _ \ / _` |/ _` |/ _ \ '_ \| '_ \| | | |
+        | | | | | | (_| | (_| |  __/ | | | |_) | |_| |
+        |_| |_| |_|\__,_|\__, |\___|_| |_| .__/ \__, |
+                         |___/           |_|    |___/
+        Modeling and Analysis of Genetics data in python
+        Version: {mgp.__version__} | Release date: {mgp.__release_date__}
+        Author: Shadi Zabad, McGill University
+        **********************************************
+        < Compute LD matrix and output in Zarr format >
 """)
 
 parser = argparse.ArgumentParser(description="""
     Commandline arguments for LD matrix computation
 """)
 
 # General options:
@@ -78,24 +78,24 @@
                          'information about the genotype data from which the LD matrix was computed, such as '
                          'the biobank/samples, cohort characteristics (e.g. ancestry), etc. Keys and values '
                          'should be separated by =, such that inputs are in the form of:'
                          '--metadata Biobank=UKB,Ancestry=EUR,Date=April2024')
 
 # Argument for the float precision:
 parser.add_argument('--storage-dtype', dest='storage_dtype', type=str,
-                    default='int16', help='The data type for the entries of the LD matrix.',
+                    default='int8', help='The data type for the entries of the LD matrix.',
                     choices={'float32', 'float64', 'int16', 'int8'})
 
 # Add arguments for the compressor:
 parser.add_argument('--compressor', dest='compressor', type=str,
-                    default='lz4', help='The compressor name or compression algorithm to use for the LD matrix.',
+                    default='zstd', help='The compressor name or compression algorithm to use for the LD matrix.',
                     choices={'lz4', 'zstd', 'gzip', 'zlib'})
 
 parser.add_argument('--compression-level', dest='compression_level', type=int,
-                    default=5, help='The compression level to use for the entries of the LD matrix (1-9).')
+                    default=7, help='The compression level to use for the entries of the LD matrix (1-9).')
 
 # Options for the various LD estimators:
 
 # For the windowed estimator:
 parser.add_argument('--ld-window', dest='ld_window', type=int,
                     help='Maximum number of neighboring SNPs to consider when computing LD.')
 parser.add_argument('--ld-window-kb', dest='ld_window_kb', type=float,
@@ -225,24 +225,32 @@
                       args.output_dir,
                       dtype=args.storage_dtype,
                       compressor_name=args.compressor,
                       compression_level=args.compression_level,
                       **ld_kwargs)
 
 # Store metadata (if provided):
+
 if args.metadata is not None:
     parsed_metadata = {
         k: v for entry in args.metadata.split(',') for k, v in [entry.strip().split('=')]
         if len(entry.strip()) > 0
     }
 
     if len(parsed_metadata) > 0:
         for k, v in parsed_metadata.items():
             ld_mat.set_store_attr(k, v)
 
+    if 'Date' not in parsed_metadata:
+        # Store the date when the computation was done:
+        ld_mat.set_store_attr('Date', time.strftime("%Y-%m-%d"))
+
+else:
+    # Store the date when the computation was done:
+    ld_mat.set_store_attr('Date', time.strftime("%Y-%m-%d"))
 
 # Clean up all intermediate files and directories:
 g.cleanup()
 
 print("Done!")
 print("> Output directory:\n\t", args.output_dir)
 # Record the end time:
```

### Comparing `magenpy-0.1.2/bin/magenpy_simulate` & `magenpy-0.1.3/bin/magenpy_simulate`

 * *Files 1% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 import warnings
 from magenpy.simulation.PhenotypeSimulator import PhenotypeSimulator
 from magenpy.utils.system_utils import makedir, get_filenames
 import argparse
 
 
 print(fr"""
-**********************************************                            
- _ __ ___   __ _  __ _  ___ _ __  _ __  _   _ 
-| '_ ` _ \ / _` |/ _` |/ _ \ '_ \| '_ \| | | |
-| | | | | | (_| | (_| |  __/ | | | |_) | |_| |
-|_| |_| |_|\__,_|\__, |\___|_| |_| .__/ \__, |
-                 |___/           |_|    |___/
-Modeling and Analysis of Genetics data in python
-Version: {mgp.__version__} | Release date: {mgp.__release_date__}
-Author: Shadi Zabad, McGill University
-**********************************************
-< Simulate complex quantitative or case-control traits >
+        ********************************************************                            
+             _ __ ___   __ _  __ _  ___ _ __  _ __  _   _ 
+            | '_ ` _ \ / _` |/ _` |/ _ \ '_ \| '_ \| | | |
+            | | | | | | (_| | (_| |  __/ | | | |_) | |_| |
+            |_| |_| |_|\__,_|\__, |\___|_| |_| .__/ \__, |
+                             |___/           |_|    |___/
+            Modeling and Analysis of Genetics data in python
+            Version: {mgp.__version__} | Release date: {mgp.__release_date__}
+            Author: Shadi Zabad, McGill University
+        ********************************************************
+        < Simulate complex quantitative or case-control traits >
 """)
 
 # --------- Options ---------
 
 parser = argparse.ArgumentParser(description="""
     Commandline arguments for the complex trait simulator
 """)
```

### Comparing `magenpy-0.1.2/magenpy/AnnotationMatrix.py` & `magenpy-0.1.3/magenpy/AnnotationMatrix.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/GWADataLoader.py` & `magenpy-0.1.3/magenpy/GWADataLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -411,21 +411,21 @@
         # Depending on the backend, select the `GenotypeMatrix` class:
         if self.backend == 'xarray':
             gmat_class = xarrayGenotypeMatrix
         else:
             gmat_class = plinkBEDGenotypeMatrix
 
         if self.verbose and len(bed_files) < 2:
-            print("> Reading BED file...")
+            print("> Reading genotype metadata...")
 
         self.genotype = {}
 
         for bfile in tqdm(bed_files,
                           total=len(bed_files),
-                          desc="Reading BED files",
+                          desc="Reading genotype metadata",
                           disable=not self.verbose or len(bed_files) < 2):
             # Read BED file and update the genotypes dictionary:
             self.genotype.update(gmat_class.from_file(bfile,
                                                       temp_dir=self.temp_dir,
                                                       threads=self.threads).split_by_chromosome())
 
         # After reading the genotype matrices, apply some standard filters:
@@ -535,24 +535,27 @@
             sumstats_files = sumstats_path
 
         if len(sumstats_files) < 1:
             warnings.warn(f"No summary statistics files were found at: {sumstats_path}")
             return
 
         if self.verbose and len(sumstats_files) < 2:
-            print("> Reading summary statistics file...")
+            print("> Reading summary statistics...")
 
         self.sumstats_table = {}
 
         for f in tqdm(sumstats_files,
                       total=len(sumstats_files),
-                      desc="Reading summary statistics files",
+                      desc="Reading summary statistics",
                       disable=not self.verbose or len(sumstats_files) < 2):
 
-            ss_tab = SumstatsTable.from_file(f, sumstats_format=sumstats_format, parser=parser, **parse_kwargs)
+            ss_tab = SumstatsTable.from_file(f,
+                                             sumstats_format=sumstats_format,
+                                             parser=parser,
+                                             **parse_kwargs)
 
             if drop_duplicated:
                 ss_tab.drop_duplicates()
 
             if 'CHR' in ss_tab.table.columns:
                 self.sumstats_table.update(ss_tab.split_by_chromosome())
             else:
@@ -561,14 +564,27 @@
                 elif self.ld is not None:
                     ref_table = {c: ld.snps for c, ld in self.ld.items()}
                 else:
                     raise ValueError("Cannot index summary statistics tables without chromosome information!")
 
                 self.sumstats_table.update(ss_tab.split_by_chromosome(snps_per_chrom=ref_table))
 
+        # If SNP information is not present in the sumstats tables, try to impute it
+        # using other reference tables:
+
+        missing_snp = any('SNP' not in ss.table.columns for ss in self.sumstats_table.values())
+
+        if missing_snp and (self.genotype is not None or self.ld is not None):
+
+            ref_table = self.to_snp_table(col_subset=['CHR', 'POS', 'SNP'], per_chromosome=True)
+
+            for c, ss in self.sumstats_table.items():
+                if 'SNP' not in ss.table.columns and c in ref_table:
+                    ss.infer_snp_id(ref_table[c], allow_na=True)
+
     def read_ld(self, ld_store_paths):
         """
         Read the LD matrix files stored on-disk in Zarr array format.
         :param ld_store_paths: The path to the LD matrices. This may be a wildcard to accommodate reading data
         for multiple chromosomes.
         """
 
@@ -581,21 +597,21 @@
             ld_store_files = ld_store_paths
 
         if len(ld_store_files) < 1:
             warnings.warn(f"No LD matrix files were found at: {ld_store_paths}")
             return
 
         if self.verbose and len(ld_store_files) < 2:
-            print("> Reading LD matrix...")
+            print("> Reading LD metadata...")
 
         self.ld = {}
 
         for f in tqdm(ld_store_files,
                       total=len(ld_store_files),
-                      desc="Reading LD matrices",
+                      desc="Reading LD metadata",
                       disable=not self.verbose or len(ld_store_files) < 2):
             z = LDMatrix.from_path(f)
             self.ld[z.chromosome] = z
 
     def load_ld(self):
         """
         A utility method to load the LD matrices to memory from on-disk storage.
@@ -611,17 +627,17 @@
         if self.ld is not None:
             for ld in self.ld.values():
                 ld.release()
 
     def compute_ld(self,
                    estimator,
                    output_dir,
-                   dtype='int16',
-                   compressor_name='lz4',
-                   compression_level=5,
+                   dtype='int8',
+                   compressor_name='zstd',
+                   compression_level=7,
                    **ld_kwargs):
         """
         Compute the Linkage-Disequilibrium (LD) matrix or SNP-by-SNP Pearson
         correlation matrix between genetic variants. This function only considers correlations
         between SNPs on the same chromosome. This is a utility function that calls the
         `.compute_ld()` method of the `GenotypeMatrix` objects associated with
         GWADataLoader.
@@ -668,14 +684,18 @@
         each variant.
 
         !!! note
             This method is called automatically during the initialization of the `GWADataLoader` object.
             However, if you read or manipulate the data sources after initialization,
             you may need to call this method again to ensure that the data sources remain aligned.
 
+        !!! warning
+            Harmonization for now depends on having SNP rsID be present in all the resources. Hopefully
+            this requirement will be relaxed in the future.
+
         """
 
         data_sources = (self.genotype, self.sumstats_table, self.ld, self.annotation)
         initialized_data_sources = [ds for ds in data_sources if ds is not None]
 
         # If less than two data sources are present, skip harmonization...
         if len(initialized_data_sources) < 2:
@@ -701,30 +721,37 @@
                 # Is this the best way to handle the missingness? Should we just post a warning?
                 for ds in initialized_data_sources:
                     if c in ds:
                         del ds[c]
 
             else:
 
-                # Find the set of SNPs that are shared across all data sources:
-                common_snps = np.array(list(set.intersection(*[set(ds[c].snps)
+                # Find the set of SNPs that are shared across all data sources (exclude missing values):
+                common_snps = np.array(list(set.intersection(*[set(ds[c].snps[~pd.isnull(ds[c].snps)])
                                                                for ds in initialized_data_sources])))
 
                 # If necessary, filter the data sources to only have the common SNPs:
                 for ds in initialized_data_sources:
                     if ds[c].n_snps != len(common_snps):
                         ds[c].filter_snps(extract_snps=common_snps)
 
                 # Harmonize the summary statistics data with either genotype or LD reference.
                 # This procedure checks for flips in the effect allele between data sources.
                 if self.sumstats_table is not None:
+
+                    id_cols = self.sumstats_table[c].identifier_cols
+
                     if self.genotype is not None:
-                        self.sumstats_table[c].match(self.genotype[c].get_snp_table(col_subset=['SNP', 'A1', 'A2']))
+                        self.sumstats_table[c].match(self.genotype[c].get_snp_table(
+                            col_subset=id_cols + ['A1', 'A2']
+                        ))
                     elif self.ld is not None:
-                        self.sumstats_table[c].match(self.ld[c].to_snp_table(col_subset=['SNP', 'A1', 'A2']))
+                        self.sumstats_table[c].match(self.ld[c].to_snp_table(
+                            col_subset=id_cols + ['A1', 'A2']
+                        ))
 
                     # If during the allele matching process we discover incompatibilities,
                     # we filter those SNPs:
                     for ds in initialized_data_sources:
                         if ds[c].n_snps != self.sumstats_table[c].n_snps:
                             ds[c].filter_snps(extract_snps=self.sumstats_table[c].snps)
 
@@ -759,23 +786,25 @@
         :param standardize_genotype: If True, standardize the genotype matrix before scoring.
         """
 
         if beta is None:
             try:
                 beta = {c: s.marginal_beta or s.get_snp_pseudo_corr() for c, s in self.sumstats_table.items()}
             except Exception:
-                raise ValueError("To perform linear scoring, you must provide effect size estimates (BETA)!")
+                raise ValueError("To perform linear scoring, you must "
+                                 "provide effect size estimates (BETA)!")
 
         # Here, we have a very ugly way of accounting for
         # the fact that the chromosomes may be coded differently between the genotype
         # and the beta dictionary. Maybe we can find a better solution in the future.
         common_chr_g, common_chr_b = match_chromosomes(self.genotype.keys(), beta.keys(), return_both=True)
 
         if len(common_chr_g) < 1:
-            raise ValueError("No common chromosomes found between the genotype and the effect size estimates!")
+            raise ValueError("No common chromosomes found between "
+                             "the genotype and the effect size estimates!")
 
         if self.verbose and len(common_chr_g) < 2:
             print("> Generating polygenic scores...")
 
         pgs = None
 
         for c_g, c_b in tqdm(zip(common_chr_g, common_chr_b),
@@ -827,38 +856,57 @@
         """
         :return: A plink-style dataframe with each individual's Family ID (FID),
         Individual ID (IID), and phenotype value.
         """
 
         return self.sample_table.get_phenotype_table()
 
-    def to_snp_table(self, col_subset=None, per_chromosome=False):
+    def to_snp_table(self, col_subset=None, per_chromosome=False, resource='auto'):
         """
         Get a dataframe of SNP data for all variants
         across different chromosomes.
 
         :param col_subset: The subset of columns to obtain.
         :param per_chromosome: If True, returns a dictionary where the key
         is the chromosome number and the value is the SNP table per
         chromosome.
+        :param resource: The data source to extract the SNP table from. By default, the method
+        will try to extract the SNP table from the genotype matrix. If the genotype matrix is not
+        available, then it will try to extract the SNP information from the LD matrix or the summary
+        statistics table. Possible values: `auto`, `genotype`, `ld`, `sumstats`.
 
         :return: A dataframe (or dictionary of dataframes) of SNP data.
         """
 
+        # Sanity checks:
+        assert resource in ('auto', 'genotype', 'ld', 'sumstats')
+        if resource != 'auto':
+            if resource == 'genotype' and self.genotype is None:
+                raise ValueError("Genotype matrix is not available!")
+            if resource == 'ld' and self.ld is None:
+                raise ValueError("LD matrix is not available!")
+            if resource == 'sumstats' and self.sumstats_table is None:
+                raise ValueError("Summary statistics table is not available!")
+        else:
+            if all(ds is None for ds in (self.genotype, self.ld, self.sumstats_table)):
+                raise ValueError("No data sources available to extract SNP data from!")
+
+        # Extract the SNP data:
+
         snp_tables = {}
 
-        for c in self.chromosomes:
-            if self.sumstats_table is not None:
-                snp_tables[c] = self.sumstats_table[c].to_table(col_subset=col_subset)
-            elif self.genotype is not None:
+        if resource in ('auto', 'genotype') and self.genotype is not None:
+            for c in self.chromosomes:
                 snp_tables[c] = self.genotype[c].get_snp_table(col_subset=col_subset)
-            elif self.ld is not None:
+        elif resource in ('auto', 'ld') and self.ld is not None:
+            for c in self.chromosomes:
                 snp_tables[c] = self.ld[c].to_snp_table(col_subset=col_subset)
-            else:
-                raise ValueError("GWADataLoader instance is not properly initialized!")
+        else:
+            return self.to_summary_statistics_table(col_subset=col_subset,
+                                                    per_chromosome=per_chromosome)
 
         if per_chromosome:
             return snp_tables
         else:
             return pd.concat(list(snp_tables.values()))
 
     def to_summary_statistics_table(self, col_subset=None, per_chromosome=False):
```

### Comparing `magenpy-0.1.2/magenpy/GenotypeMatrix.py` & `magenpy-0.1.3/magenpy/GenotypeMatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,17 +337,17 @@
         """
         if self.snp_table is not None and attr in self.snp_table.columns:
             return self.snp_table[attr].values
 
     def compute_ld(self,
                    estimator,
                    output_dir,
-                   dtype='int16',
-                   compressor_name='lz4',
-                   compression_level=5,
+                   dtype='int8',
+                   compressor_name='zstd',
+                   compression_level=7,
                    **ld_kwargs):
         """
 
         Compute the Linkage-Disequilibrium (LD) or SNP-by-SNP correlation matrix
         for the variants defined in the genotype matrix.
 
         :param estimator: The estimator for the LD matrix. We currently support
```

### Comparing `magenpy-0.1.2/magenpy/LDMatrix.py` & `magenpy-0.1.3/magenpy/LDMatrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,20 +112,22 @@
         return cls.from_path(ld_store_path)
 
     @classmethod
     def from_csr(cls,
                  csr_mat,
                  store_path,
                  overwrite=False,
-                 dtype='int16',
-                 compressor_name='lz4',
-                 compression_level=5):
+                 dtype='int8',
+                 compressor_name='zstd',
+                 compression_level=7):
         """
         Initialize an LDMatrix object from a sparse CSR matrix.
 
+        TODO: Determine the chunksize based on the avg neighborhood size?
+
         :param csr_mat: The sparse CSR matrix.
         :param store_path: The path to the Zarr LD store where the data will be stored.
         :param overwrite: If True, it overwrites the LD store at `store_path`.
         :param dtype: The data type for the entries of the LD matrix (supported data types are float32, float64
         and integer quantized data types int8 and int16).
         :param compressor_name: The name of the compressor or compression algorithm to use with Zarr.
         :param compression_level: The compression level to use with the compressor (1-9).
@@ -165,20 +167,21 @@
     @classmethod
     def from_plink_table(cls,
                          plink_ld_file,
                          snps,
                          store_path,
                          pandas_chunksize=None,
                          overwrite=False,
-                         dtype='int16',
-                         compressor_name='lz4',
-                         compression_level=5):
+                         dtype='int8',
+                         compressor_name='zstd',
+                         compression_level=7):
         """
-        Construct a Zarr LD matrix using output tables from plink1.9.
-        This class method takes the following inputs:
+        Construct a Zarr LD matrix using LD tables generated by plink1.9.
+
+        TODO: Determine the chunksize based on the avg neighborhood size?
 
         :param plink_ld_file: The path to the plink LD table file.
         :param snps: An iterable containing the list of SNPs in the LD matrix.
         :param store_path: The path to the Zarr LD store.
         :param pandas_chunksize: If the LD table is large, provide chunk size
         (i.e. number of rows to process at each step) to keep memory footprint manageable.
         :param overwrite: If True, it overwrites the LD store at `store_path`.
@@ -253,22 +256,24 @@
     @classmethod
     def from_dense_zarr_matrix(cls,
                                dense_zarr,
                                ld_boundaries,
                                store_path,
                                overwrite=False,
                                delete_original=False,
-                               dtype='int16',
-                               compressor_name='lz4',
-                               compression_level=5):
+                               dtype='int8',
+                               compressor_name='zstd',
+                               compression_level=7):
         """
          Initialize a new LD matrix object using a Zarr array object. This method is
          useful for converting a dense LD matrix computed using Dask (or other distributed computing
          software) to a sparse or banded one.
 
+         TODO: Determine the chunksize based on the avg neighborhood size?
+
          :param dense_zarr: The path to the dense Zarr array object.
          :param ld_boundaries: The LD boundaries for each SNP in the LD matrix (delineates the indices of
             the leftmost and rightmost neighbors of each SNP).
          :param store_path: The path where to store the new LD matrix.
          :param overwrite: If True, it overwrites the LD store at `store_path`.
          :param delete_original: If True, it deletes the original dense LD matrix.
          :param dtype: The data type for the entries of the LD matrix (supported data types are float32, float64
@@ -350,24 +355,26 @@
 
     @classmethod
     def from_ragged_zarr_matrix(cls,
                                 ragged_zarr,
                                 store_path,
                                 overwrite=False,
                                 delete_original=False,
-                                dtype='int16',
-                                compressor_name='lz4',
-                                compression_level=5):
+                                dtype='int8',
+                                compressor_name='zstd',
+                                compression_level=7):
         """
         Initialize a new LD matrix object using a Zarr array object
         conforming to the old LD Matrix format from magenpy v<=0.0.12.
 
         This utility function will also copy some of the stored attributes
         associated with the matrix in the old format.
 
+        TODO: Determine the chunksize based on the avg neighborhood size?
+
         :param ragged_zarr: The path to the ragged Zarr array object.
         :param store_path: The path where to store the new LD matrix.
         :param overwrite: If True, it overwrites the LD store at `store_path`.
         :param delete_original: If True, it deletes the original ragged LD matrix.
         :param dtype: The data type for the entries of the LD matrix (supported data types are float32, float64
         and integer quantized data types int8 and int16).
         :param compressor_name: The name of the compressor or compression algorithm to use with Zarr.
@@ -718,15 +725,15 @@
 
         !!! note
             This includes the variant itself if the matrix is in memory and is symmetric.
 
         :return: The number of variants in the LD window for each SNP.
 
         """
-        return self.window_size()
+        return self.window_size
 
     @property
     def csr_matrix(self):
         """
         ..note ::
             If the LD matrix is not in-memory, then it'll be loaded using default settings.
             This means that the matrix will be loaded as upper-triangular matrix with
@@ -785,14 +792,48 @@
         sparse CSR representation of the lD matrix.
         """
         if self.in_memory:
             return self.csr_matrix.indptr
         else:
             return self._zg['matrix/indptr']
 
+    def filter_long_range_ld_regions(self):
+        """
+        A utility method to exclude variants that are in long-range LD regions. The
+        boundaries of those regions are derived from here:
+
+        https://genome.sph.umich.edu/wiki/Regions_of_high_linkage_disequilibrium_(LD)
+
+        Which is based on the work of
+
+        > Anderson, Carl A., et al. "Data quality control in genetic case-control association studies." Nature protocols 5.9 (2010): 1564-1573.
+
+        .. note ::
+            This method is experimental and may not work as expected for all LD matrices.
+        """
+
+        from .parsers.annotation_parsers import parse_annotation_bed_file
+        from .utils.data_utils import lrld_path
+
+        bed_df = parse_annotation_bed_file(lrld_path())
+
+        # Filter to only regions specific to the chromosome of this matrix:
+        bed_df = bed_df.loc[bed_df['CHR'] == self.chromosome]
+
+        bp_pos = self.bp_position
+        snp_mask = np.ones(len(bp_pos), dtype=bool)
+
+        # Loop over the LRLD region on this chromosome and exclude the SNPs in these regions:
+        for _, row in bed_df.iterrows():
+            start, end = row['Start'], row['End']
+            snp_mask &= ~((bp_pos >= start) & (bp_pos <= end))
+
+        # Filter the SNP to only those not in the LRLD regions:
+        self.filter_snps(self.snps[snp_mask])
+
     def filter_snps(self, extract_snps=None, extract_file=None):
         """
         Filter the LDMatrix to keep a subset of variants. This mainly sets
         the mask for the LD matrix, which is used to hide/remove some SNPs from the LD matrix,
         without altering the stored objects on-disk.
 
         :param extract_snps: A list or array of SNP rsIDs to keep.
@@ -835,29 +876,51 @@
         else:
             self._mask = mask
 
         # If the data is already in memory, reload:
         if self.in_memory:
             self.load(force_reload=True,
                       return_symmetric=self.is_symmetric,
-                      fill_diag=self.is_symmetric,
                       dtype=self.dtype)
 
     def reset_mask(self):
         """
         Reset the mask to its default value (None).
         """
         self._mask = None
 
         if self.in_memory:
             self.load(force_reload=True,
                       return_symmetric=self.is_symmetric,
-                      fill_diag=self.is_symmetric,
                       dtype=self.dtype)
 
+    def prune(self, threshold):
+        """
+        Perform LD pruning to remove variants that are in high LD with other variants.
+        If two variants are in high LD, this function keeps the variant that occurs
+        earlier in the matrix. This behavior will be updated in the future to allow
+        for arbitrary ordering of variants.
+
+        !!! note
+            Experimental for now. Needs further testing & improvement.
+
+        :param threshold: The absolute value of the Pearson correlation coefficient above which to prune variants.
+        :return: A boolean array indicating whether a variant is kept after pruning. A positive floating point number
+        between 0. and 1.
+        """
+
+        from .stats.ld.c_utils import prune_ld_ut
+
+        assert 0. < threshold <= 1.
+
+        if np.issubdtype(self.stored_dtype, np.integer):
+            threshold = quantize(np.array([threshold]), int_dtype=self.stored_dtype)[0]
+
+        return prune_ld_ut(self.indptr[:], self.data[:], threshold)
+
     def to_snp_table(self, col_subset=None):
         """
         :param col_subset: The subset of columns to add to the table. If None, it returns
         all available columns.
 
         :return: A `pandas` dataframe of the SNP attributes and metadata for variants
         included in the LD matrix.
@@ -1092,99 +1155,135 @@
 
         # TODO: Check that this covers most cases and would not result in unexpected behavior
         if np.issubdtype(self.stored_dtype, np.integer) and np.issubdtype(new_csr.dtype, np.floating):
             self._zg['matrix/data'][data_start:data_end] = quantize(new_csr.data, int_dtype=self.stored_dtype)
         else:
             self._zg['matrix/data'][data_start:data_end] = new_csr.data.astype(self.stored_dtype)
 
-    def low_memory_load(self, dtype=None):
+    def load_data(self,
+                  return_symmetric=False,
+                  dtype=None,
+                  return_as_csr=False):
         """
-        A utility method to load the LD matrix in low-memory mode.
-        The method will load the entries of the upper triangular portion of the matrix,
-        perform filtering based on the mask (if set), and return the filtered data
-        and index pointer (`indptr`) arrays.
-
-        This is useful for some application, such as the `low_memory` version of
-        the `viprs` method, because it avoids reconstructing the `indices` array for the CSR matrix,
-        which can potentially be a very long array of large integers.
+        A utility function to load and process the LD matrix data.
+        This function is particularly useful for filtering, symmetrizing, and dequantizing the LD matrix
+        after it's loaded into memory.
 
-        !!! note
-            The method, by construction, does not support loading the full symmetric matrix. If
-            that's the goal, use the `.load()` or `.load_rows()` methods.
-
-        !!! seealso "See Also"
-            * [load_rows][magenpy.LDMatrix.LDMatrix.load_rows]
-            * [load][magenpy.LDMatrix.LDMatrix.load]
+        TODO: Support loading subset of rows of the matrix, similar to `load_rows` (i.e. replace `load_rows`
+        with newer implementation).
 
+        :param return_symmetric: If True, return a full symmetric representation of the LD matrix.
         :param dtype: The data type for the entries of the LD matrix.
+        :param return_as_csr: If True, return the data in the CSR format.
 
-        :return: A tuple of the data and index pointer arrays for the LD matrix.
-
+        :return: A tuple of the index pointer array, the data array, and the leftmost index array. If
+        `return_as_csr` is set to True, we return the data as a CSR matrix.
         """
 
-        # Determine the final data type for the LD matrix entries
-        # and whether we need to perform dequantization or not depending on
-        # the stored data type and the requested data type.
-
+        # -------------- Step 1: Preparing input data type --------------
         if dtype is None:
             dtype = self.stored_dtype
             dequantize_data = False
         else:
             dtype = np.dtype(dtype)
             if np.issubdtype(self.stored_dtype, np.integer) and np.issubdtype(dtype, np.floating):
                 dequantize_data = True
             else:
                 dequantize_data = False
 
+        # -------------- Step 2: Fetch the indptr array --------------
+
         # Get the index pointer array:
         indptr = self._zg['matrix/indptr'][:]
 
+        # -------------- Step 3: Checking data masking --------------
+
         # Filter the index pointer array based on the mask:
         if self._mask is not None:
 
             if np.issubdtype(self._mask.dtype, np.integer):
                 mask = np.zeros(self.stored_n_snps, dtype=np.int8)
                 mask[self._mask] = 1
             else:
                 mask = self._mask
 
-            from .stats.ld.c_utils import filter_ut_csr_matrix_low_memory
+            from .stats.ld.c_utils import filter_ut_csr_matrix
 
-            data_mask, indptr = filter_ut_csr_matrix_low_memory(indptr, mask)
-            # Unfortunately, .vindex is very slow in Zarr right now (~order of magnitude)
-            # So for now, we load the entire data array before performing the mask selection:
+            data_mask, indptr = filter_ut_csr_matrix(indptr, mask)
+            # .oindex and .vindex are slow and convert to integer indices in the background,
+            # which unnecessarily increases memory usage. Unfortunately, here we have to load the entire
+            # data and index it using the boolean array afterward.
+            # Something to be improved in the future. :)
             data = self._zg['matrix/data'][:][data_mask]
+            del data_mask
         else:
             data = self._zg['matrix/data'][:]
 
+        # -------------- Step 4: Symmetrizing input matrix --------------
+
+        if return_symmetric:
+
+            from .stats.ld.c_utils import symmetrize_ut_csr_matrix
+
+            if np.issubdtype(self.stored_dtype, np.integer):
+                fill_val = np.iinfo(self.stored_dtype).max
+            else:
+                fill_val = 1.
+
+            data, indptr, leftmost_idx = symmetrize_ut_csr_matrix(indptr, data, fill_val)
+        else:
+            leftmost_idx = np.arange(1, indptr.shape[0], dtype=np.int32)
+
+        # -------------- Step 5: Dequantizing/type cast requested data --------------
+
         if dequantize_data:
-            return dequantize(data, float_dtype=dtype), indptr
+            data = dequantize(data, float_dtype=dtype)
+        else:
+            data = data.astype(dtype, copy=False)
+
+        # ---------------------------------------------------------------------------
+        # Return the requested data:
+
+        if return_as_csr:
+
+            from .stats.ld.c_utils import expand_ranges
+
+            indices = expand_ranges(leftmost_idx,
+                                    (np.diff(indptr) + leftmost_idx).astype(np.int32),
+                                    data.shape[0])
+
+            return csr_matrix(
+                (
+                    data,
+                    indices,
+                    indptr
+                ),
+                dtype=dtype
+            )
         else:
-            return data.astype(dtype), indptr
+            return data, indptr, leftmost_idx
 
     def load_rows(self,
                   start_row=None,
                   end_row=None,
                   return_symmetric=False,
                   fill_diag=False,
                   keep_shape=True,
                   dtype=None):
         """
         A utility function to allow for loading a subset of the LD matrix.
         By specifying `start_row` and `end_row`, the user can process or inspect small
         blocks of the LD matrix without loading the whole thing into memory.
 
-        TODO: Consider using `low_memory_load` internally to avoid reconstructing the `indices` array.
-
         !!! note
             This method does not perform any filtering on the stored data.
-            To access the LD matrix with filtering, use `.load()` or `low_memory_load`.
+            To access the LD matrix with filtering, use `.load()` or `load_data`.
 
         !!! seealso "See Also"
-            * [low_memory_load][magenpy.LDMatrix.LDMatrix.low_memory_load]
+            * [load_data][magenpy.LDMatrix.LDMatrix.load_data]
             * [load][magenpy.LDMatrix.LDMatrix.load]
 
         :param start_row: The start row to load to memory
         :param end_row: The end row (not inclusive) to load to memory
         :param return_symmetric: If True, return a full symmetric representation of the LD matrix.
         :param fill_diag: If True, fill the diagonal of the LD matrix with ones.
         :param keep_shape: If True, return the LD matrix with the same shape as the original. Here,
@@ -1278,15 +1377,15 @@
         if return_symmetric:
 
             # First, replace explicit zeros with invalid value (this is a hack to prevent scipy
             # from eliminating those zeros when making the matrix symmetric):
             mat.data[mat.data == 0] = invalid_value
 
             # Add the matrix transpose to make it symmetric:
-            mat = (mat + mat.T).astype(dtype)
+            mat += mat.T
 
             # If the user requested filling the diagonals, do it here:
             if fill_diag:
                 diag_vals = np.concatenate([np.zeros(start_row, dtype=dtype),
                                             identity_val*np.ones(end_row - start_row, dtype=dtype),
                                             np.zeros(n_snps - end_row, dtype=dtype)])
                 mat += diags(diag_vals, dtype=dtype, shape=mat.shape)
@@ -1310,28 +1409,26 @@
             return mat
         else:
             return mat[start_row:end_row, :]
 
     def load(self,
              force_reload=False,
              return_symmetric=True,
-             fill_diag=True,
              dtype=None):
 
         """
         Load the LD matrix from on-disk storage in the form of Zarr arrays to memory,
         in the form of sparse CSR matrices.
 
         !!! seealso "See Also"
-            * [low_memory_load][magenpy.LDMatrix.LDMatrix.low_memory_load]
+            * [load_data][magenpy.LDMatrix.LDMatrix.load_data]
             * [load_rows][magenpy.LDMatrix.LDMatrix.load_rows]
 
         :param force_reload: If True, it will reload the data even if it is already in memory.
         :param return_symmetric: If True, return a full symmetric representation of the LD matrix.
-        :param fill_diag: If True, fill the diagonal elements of the LD matrix with ones.
         :param dtype: The data type for the entries of the LD matrix.
 
         :return: The LD matrix as a sparse CSR matrix.
         """
 
         if dtype is not None:
             dtype = np.dtype(dtype)
@@ -1351,21 +1448,17 @@
                     return
                 elif self._mat.data.dtype == dtype:
                     return
 
         # If we are re-loading the matrix, make sure to release the current one:
         self.release()
 
-        self._mat = self.load_rows(return_symmetric=return_symmetric,
-                                   fill_diag=fill_diag,
-                                   dtype=dtype)
-
-        # If a mask is set, apply it:
-        if self._mask is not None:
-            self._mat = self._mat[self._mask, :][:, self._mask]
+        self._mat = self.load_data(return_symmetric=return_symmetric,
+                                   dtype=dtype,
+                                   return_as_csr=True)
 
         # Update the flags:
         self.in_memory = True
         self.is_symmetric = return_symmetric
 
     def release(self):
         """
@@ -1441,15 +1534,15 @@
         self.index = 0
         self._mask = None
 
         if mask is not None:
             self.set_mask(mask)
 
         if in_mem:
-            self.load(return_symmetric=is_symmetric, fill_diag=is_symmetric, dtype=dtype)
+            self.load(return_symmetric=is_symmetric, dtype=dtype)
 
     def __len__(self):
         return self.n_snps
 
     def __getitem__(self, index):
         return self.get_row(index)
```

### Comparing `magenpy-0.1.2/magenpy/SampleTable.py` & `magenpy-0.1.3/magenpy/SampleTable.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/SumstatsTable.py` & `magenpy-0.1.3/magenpy/SumstatsTable.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,30 +30,37 @@
         :param ss_table: A pandas DataFrame containing the summary statistics.
 
         !!! seealso "See Also"
             * [from_file][magenpy.SumstatsTable.SumstatsTable.from_file]
         """
         self.table: pd.DataFrame = ss_table
 
-        assert all([col in self.table.columns for col in ('SNP', 'A1')])
+        # Check that the table contains some of the required columns (non exhaustive):
+
+        # Either has SNP or CHR+POS:
+        assert 'SNP' in self.table.columns or all([col in self.table.columns for col in ('CHR', 'POS')])
+        # Assert that the table has at least one of the alleles:
+        assert any([col in self.table.columns for col in ('A1', 'A2')])
+        # TODO: Add other assertions?
 
     @property
     def shape(self):
         """
-        :return: he shape of the summary statistics table.
+        :return: The shape of the summary statistics table.
         """
         return self.table.shape
 
     def __len__(self):
         return len(self.table)
 
     @property
     def chromosome(self):
         """
-        A convenience method to return the chromosome number if there is only one chromosome in the summary statistics.
+        A convenience method to return the chromosome number if there is only
+        one chromosome in the summary statistics.
         If multiple chromosomes are present, it returns None.
 
         :return: The chromosome number if there is only one chromosome in the summary statistics.
         """
         chrom = self.chromosomes
         if chrom is not None and len(chrom) == 1:
             return chrom[0]
@@ -73,14 +80,21 @@
             * [n_snps][magenpy.SumstatsTable.SumstatsTable.n_snps]
 
         :return: The number of variants in the summary statistics table.
         """
         return self.n_snps
 
     @property
+    def identifier_cols(self):
+        if 'SNP' in self.table.columns:
+            return ['SNP']
+        else:
+            return ['CHR', 'POS']
+
+    @property
     def n_snps(self):
         """
         !!! seealso "See Also"
             * [m][magenpy.SumstatsTable.SumstatsTable.m]
 
         :return: The number of variants in the summary statistics table.
         """
@@ -337,65 +351,103 @@
                     return np.sign(ss_value)
 
         raise KeyError("No signed statistic to extract the sign from!")
 
     def infer_a2(self, reference_table, allow_na=False):
         """
         Infer the reference allele A2 (if not present in the SumstatsTable)
-        from a reference table. Make sure that the reference table contains the SNP ID,
-        the reference allele A2 and the alternative (i.e. effect) allele A1. It is the
-        user's responsibility to make sure that the reference table matches the summary
-        statistics in terms of the specification of reference vs. alternative. They are
-        allowed to be flipped, but they have to be consistent across the two tables.
+        from a reference table. Make sure that the reference table contains the identifier information
+        for each SNP, in addition to the reference allele A2 and the alternative (i.e. effect) allele A1.
+        It is the user's responsibility to make sure that the reference table matches the summary
+        statistics in terms of the specification of reference vs. alternative. They have to be consistent
+        across the two tables.
 
         :param reference_table: A pandas table containing the following columns at least:
-        `SNP`, `A1`, `A2`.
+        SNP identifiers (`SNP` or `CHR` & `POS`) and allele information (`A1` & `A2`).
         :param allow_na: If True, allow the reference allele to be missing from the final result.
         """
 
-        # Merge the summary statistics table with the reference table on `SNP` ID:
-        merged_table = self.table[['SNP', 'A1']].merge(reference_table[['SNP', 'A1', 'A2']],
-                                                       how='left',
-                                                       on='SNP')
+        # Get the identifier columns for this table:
+        id_cols = self.identifier_cols
+
+        # Sanity checks:
+        assert all([col in reference_table.columns for col in id_cols + ['A1', 'A2']])
+
+        # Merge the summary statistics table with the reference table on unique ID:
+        merged_table = self.table[id_cols + ['A1']].merge(
+            reference_table[id_cols + ['A1', 'A2']],
+            how='left',
+            on=id_cols
+        )
         # If `A1_x` agrees with `A1_y`, then `A2` is indeed the reference allele.
         # Otherwise, they are flipped and `A1_y` should be the reference allele:
         merged_table['A2'] = np.where(merged_table['A1_x'] == merged_table['A1_y'],
                                       merged_table['A2'],
                                       merged_table['A1_y'])
 
         # Check that the reference allele could be inferred for all SNPs:
         if not allow_na and merged_table['A2'].isna().any():
             raise ValueError("The reference allele could not be inferred for some SNPs!")
         else:
             self.table['A2'] = merged_table['A2']
 
+    def infer_snp_id(self, reference_table, allow_na=False):
+        """
+        Infer the SNP ID (if not present in the SumstatsTable) from a reference table.
+        Make sure that the reference table contains the SNP ID, chromosome ID, and position.
+
+        :param reference_table: A pandas table containing the following columns at least:
+        `SNP`, `CHR`, `POS`.
+        :param allow_na: If True, allow the SNP ID to be missing from the final result.
+        """
+
+        # Merge the summary statistics table with the reference table:
+        merged_table = self.table[['CHR', 'POS']].merge(reference_table[['SNP', 'CHR', 'POS']], how='left')
+
+        # Check that the SNP ID could be inferred for all SNPs:
+        if not allow_na and merged_table['SNP'].isna().any():
+            raise ValueError("The SNP ID could not be inferred for some SNPs!")
+        else:
+            self.table['SNP'] = merged_table['SNP'].values
+
     def set_sample_size(self, n):
         """
         Set the sample size for each variant in the summary table.
         This can be useful when the overall sample size from the GWAS analysis is available,
         but not on a per-SNP basis.
 
         :param n: A scalar or array of sample sizes for each variant.
         """
         self.table['N'] = n
 
+    def run_quality_control(self, reference_table=None):
+        """
+        Run quality control checks on the summary statistics table.
+        TODO: Implement quality control checks following recommendations given by Prive et al.:
+        https://doi.org/10.1016/j.xhgg.2022.100136
+        Given user fine-control over which checks to run and which to skip.
+        Maybe move parts of this implementation to a module in `stats` (TBD)
+        """
+        pass
+
     def match(self, reference_table, correct_flips=True):
         """
         Match the summary statistics table with a reference table,
         correcting for potential flips in the effect alleles.
 
         :param reference_table: The SNP table to use as a reference. Must be a pandas
-        table with at least three columns: SNP, A1, A2.
+        table with the following columns: SNP identifier (either `SNP` or `CHR` & `POS`) and allele information
+        (`A1` & `A2`).
         :param correct_flips: If True, correct the direction of effect size
          estimates if the effect allele is reversed.
         """
 
         from .utils.model_utils import merge_snp_tables
 
-        self.table = merge_snp_tables(ref_table=reference_table[['SNP', 'A1', 'A2']],
+        self.table = merge_snp_tables(ref_table=reference_table[self.identifier_cols + ['A1', 'A2']],
                                       alt_table=self.table,
                                       how='inner',
                                       correct_flips=correct_flips)
 
     def filter_by_allele_frequency(self, min_maf=None, min_mac=None):
         """
         Filter variants in the summary statistics table by minimum minor allele frequency or allele count
@@ -443,22 +495,23 @@
         if extract_snps is not None:
             extract_index = intersect_arrays(self.snps, extract_snps, return_index=True)
 
         if extract_index is not None:
             self.table = self.table.iloc[extract_index, ].reset_index(drop=True)
         else:
             raise Exception("To filter a summary statistics table, you must provide "
-                            "the list of SNPs, a file containing the list of SNPs, or a list of indices to retain.")
+                            "the list of SNPs, a file containing the list of SNPs, "
+                            "or a list of indices to retain.")
 
     def drop_duplicates(self):
         """
         Drop variants with duplicated rsIDs from the summary statistics table.
         """
 
-        self.table = self.table.drop_duplicates(subset='SNP', keep=False)
+        self.table = self.table.drop_duplicates(subset=self.identifier_cols, keep=False)
 
     def get_col(self, col_name):
         """
         :param col_name: The name of the column to extract.
 
         :return: The column associated with `col_name` from summary statistics table.
         """
@@ -569,15 +622,15 @@
 
         :return: A dictionary where the keys are the chromosome number and the value is a `SumstatsTable` object.
         """
 
         if 'CHR' in self.table.columns:
             chrom_tables = self.table.groupby('CHR')
             return {
-                c: SumstatsTable(chrom_tables.get_group(c))
+                c: SumstatsTable(chrom_tables.get_group(c).copy())
                 for c in chrom_tables.groups
             }
         elif snps_per_chrom is not None:
             chrom_dict = {
                 c: SumstatsTable(pd.DataFrame({'SNP': snps}).merge(self.table))
                 for c, snps in snps_per_chrom.items()
             }
```

### Comparing `magenpy-0.1.2/magenpy/__init__.py` & `magenpy-0.1.3/magenpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 from .simulation.PhenotypeSimulator import PhenotypeSimulator
 
 # Data utilities:
 
 from .utils.data_utils import *
 
-__version__ = '0.1.2'
-__release_date__ = 'April 2024'
+__version__ = '0.1.3'
+__release_date__ = 'May 2024'
 
 
 config = configparser.ConfigParser()
 config.read(glob.glob(osp.join(osp.dirname(__file__), 'config/*.ini')))
 
 
 def print_options():
```

### Comparing `magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bed` & `magenpy-0.1.3/magenpy/data/1000G_eur_chr22.bed`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bim` & `magenpy-0.1.3/magenpy/data/1000G_eur_chr22.bim`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/data/1000G_eur_chr22.fam` & `magenpy-0.1.3/magenpy/data/1000G_eur_chr22.fam`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/data/ukb_height_chr22.fastGWA.gz` & `magenpy-0.1.3/magenpy/data/ukb_height_chr22.fastGWA.gz`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/parsers/annotation_parsers.py` & `magenpy-0.1.3/magenpy/parsers/annotation_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/parsers/misc_parsers.py` & `magenpy-0.1.3/magenpy/parsers/misc_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/parsers/plink_parsers.py` & `magenpy-0.1.3/magenpy/parsers/plink_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/parsers/sumstats_parsers.py` & `magenpy-0.1.3/magenpy/parsers/sumstats_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/plot/gwa.py` & `magenpy-0.1.3/magenpy/plot/gwa.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/plot/ld.py` & `magenpy-0.1.3/magenpy/plot/ld.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     :param include_colorbar: If True, include a colorbar in the plot.
     """
 
     if row_subset is None:
         row_subset = np.arange(ldm.shape[0])
 
     # TODO: Figure out a way to do this without loading the entire matrix:
-    ldm.load(return_symmetric=True, fill_diag=True, dtype='float32')
+    ldm.load(return_symmetric=True, dtype='float32')
 
     mat = ldm.csr_matrix[row_subset, :][:, row_subset].toarray()
 
     if display == 'upper':
         mat = np.triu(mat, k=1)
     elif display == 'lower':
         mat = np.tril(mat, k=1)
```

### Comparing `magenpy-0.1.2/magenpy/simulation/AnnotatedPhenotypeSimulator.py` & `magenpy-0.1.3/magenpy/simulation/AnnotatedPhenotypeSimulator.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/simulation/MultiCohortPhenotypeSimulator.py` & `magenpy-0.1.3/magenpy/simulation/MultiCohortPhenotypeSimulator.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/simulation/PhenotypeSimulator.py` & `magenpy-0.1.3/magenpy/simulation/PhenotypeSimulator.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/stats/gwa/utils.py` & `magenpy-0.1.3/magenpy/stats/gwa/utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/stats/h2/ldsc.py` & `magenpy-0.1.3/magenpy/stats/h2/ldsc.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/stats/ld/estimator.py` & `magenpy-0.1.3/magenpy/stats/ld/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,17 @@
         return np.array((np.zeros(m), np.ones(m)*m)).astype(np.int64)
 
     def compute(self,
                 output_dir,
                 temp_dir='temp',
                 overwrite=True,
                 delete_original=True,
-                dtype='int16',
-                compressor_name='lz4',
-                compression_level=5):
+                dtype='int8',
+                compressor_name='zstd',
+                compression_level=7):
         """
         A utility method to compute the LD matrix and store in Zarr array format.
         The computes the LD matrix and stores it in Zarr array format, set its attributes,
         and performs simple validation at the end.
 
         :param output_dir: The path where to store the resulting LD matrix.
         :param temp_dir: A temporary directory to store intermediate files and results.
@@ -234,17 +234,17 @@
             ])
 
     def compute(self,
                 output_dir,
                 temp_dir='temp',
                 overwrite=True,
                 delete_original=True,
-                dtype='int16',
-                compressor_name='lz4',
-                compression_level=5):
+                dtype='int8',
+                compressor_name='zstd',
+                compression_level=7):
         """
 
         Compute the windowed LD matrix and store in Zarr array format.
 
         :param output_dir: The path where to store the resulting LD matrix.
         :param temp_dir: A temporary directory to store intermediate files and results.
         :param overwrite: If True, overwrite any existing LD matrices in `temp_dir` and `output_dir`.
@@ -342,17 +342,17 @@
                                             self.threshold)
 
     def compute(self,
                 output_dir,
                 temp_dir='temp',
                 overwrite=True,
                 delete_original=True,
-                dtype='int16',
-                compressor_name='lz4',
-                compression_level=5,
+                dtype='int8',
+                compressor_name='zstd',
+                compression_level=7,
                 chunk_size=1000):
         """
 
         TODO: Add a mechanism to either automatically adjust the shrinkage threshold depending on the
         float precision (dtype) or purge trailing zero entries that got quantized to zero. For example,
         if we select a shrinkage threshold of 1e-3 with (int8), then we will have a lot of
         trailing zeros stored in the resulting LD matrix. It's better if we got rid of those zeros to
@@ -461,17 +461,17 @@
         return find_ld_block_boundaries(self.genotype_matrix.bp_pos, self.ld_blocks)
 
     def compute(self,
                 output_dir,
                 temp_dir='temp',
                 overwrite=True,
                 delete_original=True,
-                dtype='int16',
-                compressor_name='lz4',
-                compression_level=5):
+                dtype='int8',
+                compressor_name='zstd',
+                compression_level=7):
         """
 
         Compute the block-based LD matrix and store in Zarr array format.
 
         :param output_dir: The path where to store the resulting LD matrix.
         :param temp_dir: A temporary directory to store intermediate files and results.
         :param overwrite: If True, overwrite any existing LD matrices in `temp_dir` and `output_dir`.
```

### Comparing `magenpy-0.1.2/magenpy/stats/ld/utils.py` & `magenpy-0.1.3/magenpy/stats/ld/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
         # Update the LD matrix object inplace:
         ld_mat_obj.update_rows_inplace(csr_mat, start_row=start_row, end_row=end_row)
 
     return ld_mat_obj
 
 
-def estimate_rows_per_chunk(rows, cols, dtype='int16', mem_size=128):
+def estimate_rows_per_chunk(rows, cols, dtype='int8', mem_size=128):
     """
     Estimate the number of rows per chunk for matrices conditional on the desired size of the chunk in MB.
     The estimator takes as input the number of rows, columns, data type, and projected size of the chunk in memory.
 
     :param rows: Total number of rows in the matrix.
     :param cols: Total number of columns. If sparse matrix with uneven columns, provide average column size.
     :param dtype: The data type for the matrix entries.
@@ -251,17 +251,17 @@
 
 
 def compute_ld_plink1p9(genotype_matrix,
                         ld_boundaries,
                         output_dir,
                         temp_dir='temp',
                         overwrite=True,
-                        dtype='int16',
-                        compressor_name='lz4',
-                        compression_level=5):
+                        dtype='int8',
+                        compressor_name='zstd',
+                        compression_level=7):
 
     """
     Compute LD matrices using plink 1.9.
 
     :param genotype_matrix: A plinkBEDGenotypeMatrix object
     :param ld_boundaries: An array of LD boundaries for every SNP
     :param output_dir: The output directory for the final LD matrix file (after processing).
@@ -350,15 +350,15 @@
     plink1.verbose = True
 
     # ---------------------------------------------------------
 
     plink1.execute(cmd)
 
     # Convert from PLINK LD files to Zarr:
-    fin_ld_store = osp.join(output_dir, 'ld', 'chr_' + str(genotype_matrix.chromosome))
+    fin_ld_store = osp.join(output_dir, 'chr_' + str(genotype_matrix.chromosome))
 
     # Compute the pandas chunk_size
     # The goal of this is to process chunks of the LD table without overwhelming memory resources:
     avg_ncols = int((ld_boundaries[1, :] - ld_boundaries[0, :]).mean())
     rows_per_chunk = estimate_rows_per_chunk(ld_boundaries.shape[1], avg_ncols, dtype=dtype)
 
     if rows_per_chunk > 0.1*ld_boundaries.shape[1]:
@@ -378,17 +378,17 @@
 
 def compute_ld_xarray(genotype_matrix,
                       ld_boundaries,
                       output_dir,
                       temp_dir='temp',
                       overwrite=True,
                       delete_original=True,
-                      dtype='int16',
-                      compressor_name='lz4',
-                      compression_level=5):
+                      dtype='int8',
+                      compressor_name='zstd',
+                      compression_level=7):
 
     """
     Compute the Linkage Disequilibrium matrix or snp-by-snp
     correlation matrix assuming that the genotypes are represented
     by `xarray` or `dask`-like matrix objects. This function computes the
     entire X'X/N and stores the result on-disk in Zarr arrays. Then, we call the utilities
     from the `LDMatrix` class to sparsify the dense matrix according to the parameters
```

### Comparing `magenpy-0.1.2/magenpy/stats/score/score.hpp` & `magenpy-0.1.3/magenpy/stats/score/score.hpp`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/stats/score/score_cpp.pyx` & `magenpy-0.1.3/magenpy/stats/score/score_cpp.pyx`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/stats/score/utils.py` & `magenpy-0.1.3/magenpy/stats/score/utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/stats/transforms/genotype.py` & `magenpy-0.1.3/magenpy/stats/transforms/genotype.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/stats/transforms/phenotype.py` & `magenpy-0.1.3/magenpy/stats/transforms/phenotype.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,29 +31,32 @@
 
     from scipy.stats import rankdata, norm
 
     ranked_pheno = rankdata(phenotype, method="average")
     return norm.ppf((ranked_pheno - offset) / (len(ranked_pheno) - 2 * offset + 1))
 
 
-def detect_outliers(phenotype, sigma_threshold=5):
+def detect_outliers(phenotype, sigma_threshold=5, nan_policy='omit'):
     """
     Detect samples with outlier phenotype values.
     This function takes a vector of quantitative phenotypes,
     computes the z-score for every individual, and returns a
     boolean vector indicating whether individual i has phenotype value
     within the specified standard deviations `sigma_threshold`.
     :param phenotype: A numpy vector of continuous or quantitative phenotypes.
     :param sigma_threshold: The multiple of standard deviations or sigmas after
     which we consider the phenotypic value an outlier.
+    :param nan_policy: The policy to use when encountering NaN values in the phenotype vector.
+    By default, we compute the z-scores ignoring NaN values.
 
-    :return: A boolean array indicating whether the phenotype value is an outlier.
+    :return: A boolean array indicating whether the phenotype value is an outlier (i.e.
+    True indicates outlier).
     """
     from scipy.stats import zscore
-    return np.abs(zscore(phenotype)) < sigma_threshold
+    return np.abs(zscore(phenotype, nan_policy=nan_policy)) > sigma_threshold
 
 
 def standardize(phenotype):
     """
     Standardize the phenotype vector to have mean zero and unit variance
     :param phenotype: A numpy vector of continuous or quantitative phenotypes.
 
@@ -105,12 +108,12 @@
                 if rint_phenotype:
                     phenotype = rint(phenotype)
 
             elif transform == 'outlier_removal':
                 # Remove outlier samples whose phenotypes are more than `threshold` standard deviations from the mean:
                 if outlier_sigma_threshold is not None:
                     # Find outliers:
-                    mask = detect_outliers(phenotype, outlier_sigma_threshold)
-                    # Filter phenotype vector:
+                    mask = ~detect_outliers(phenotype, outlier_sigma_threshold)
+                    # Filter phenotype vector to exclude outliers:
                     phenotype = phenotype[mask]
 
     return phenotype, mask
```

### Comparing `magenpy-0.1.2/magenpy/stats/variant/utils.py` & `magenpy-0.1.3/magenpy/stats/variant/utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/utils/compute_utils.py` & `magenpy-0.1.3/magenpy/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/utils/executors.py` & `magenpy-0.1.3/magenpy/utils/executors.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/magenpy/utils/model_utils.py` & `magenpy-0.1.3/magenpy/utils/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,35 +370,43 @@
     info = np.iinfo(int_dtype)
 
     # Compute the scale and zero point
     # NOTE: We add 1 to the info.min here to force the zero point to be exactly at 0.
     # See discussions on Scale Quantization Mapping.
     scale = 2. / (info.max - (info.min + 1))
 
-    # Quantize the floats to int
-    return np.clip((floats / scale).round(), info.min, info.max).astype(int_dtype)
+    # Use as much in-place operations as possible
+    # (Currently, we copy the data twice)
+    scaled_floats = floats / scale
+    np.round(scaled_floats, out=scaled_floats)
+    np.clip(scaled_floats, info.min, info.max, out=scaled_floats)
+
+    return scaled_floats.astype(int_dtype)
 
 
 def dequantize(ints, float_dtype=np.float32):
     """
     Dequantize integers to the specified floating point type.
     NOTE: Assumes original floats are in the range [-1, 1].
     :param ints: A numpy array of integers
-    :param float_dtype: The floating point type to dequantize to.
+    :param float_dtype: The floating point data type to dequantize the integers to.
     """
 
     # Infer the boundaries from the integer type
     info = np.iinfo(ints.dtype)
 
     # Compute the scale and zero point
     # NOTE: We add 1 to the info.min here to force the zero point to be exactly at 0.
     # See discussions on Scale Quantization Mapping.
     scale = 2. / (info.max - (info.min + 1))
 
-    return ints.astype(float_dtype) * scale
+    dq = ints.astype(float_dtype)
+    dq *= scale  # in-place multiplication
+
+    return dq
 
 
 def multinomial_rvs(n, p):
     """
     Copied from Warren Weckesser:
     https://stackoverflow.com/a/55830796
```

### Comparing `magenpy-0.1.2/magenpy/utils/system_utils.py` & `magenpy-0.1.3/magenpy/utils/system_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,55 @@
 import errno
 import os
 import os.path as osp
 import subprocess
 import glob
 import psutil
+import sys
 
 
 def available_cpu():
     """
     Get the number of available CPUs on the system.
     """
     return psutil.cpu_count() - 1
 
 
+def get_peak_memory_usage(include_children=False):
+    """
+    Get the peak memory usage of the running process in Mega Bytes (MB).
+
+    !!! warning
+        This function is only available on Unix-based systems for now.
+
+    :param include_children: A boolean flag to include the memory usage of the child processes.
+    :return: The peak memory usage of the running process in Mega Bytes (MB).
+    """
+
+    try:
+        import resource
+    except ImportError:
+        return
+
+    mem_usage_self = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
+
+    if include_children:
+        mem_usage_self = max(mem_usage_self, resource.getrusage(resource.RUSAGE_CHILDREN).ru_maxrss)
+
+    if sys.platform != 'darwin':
+        mem_usage_self /= 1024
+    else:
+        mem_usage_self /= 1024**2
+
+    return mem_usage_self
+
+
 def get_memory_usage():
     """
-    Get the memory usage of the current process in Mega Bytes (MB)
+    Get the current memory usage of the running process in Mega Bytes (MB)
     """
     process = psutil.Process(os.getpid())
     mem_info = process.memory_info()
     return mem_info.rss / (1024 ** 2)
 
 
 def valid_url(path):
@@ -141,9 +171,9 @@
     """
     Delete temporary files with the given `prefix`.
     :param prefix: A string with the prefix of the temporary files to delete.
     """
     for f in glob.glob(f"{prefix}*"):
         try:
             os.remove(f)
-        except Exception as e:
+        except Exception:
             continue
```

### Comparing `magenpy-0.1.2/magenpy.egg-info/PKG-INFO` & `magenpy-0.1.3/magenpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magenpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modeling and Analysis of Statistical Genetics data in python
 Home-page: https://github.com/shz9/magenpy
 Author: Shadi Zabad
 Author-email: shadi.zabad@mail.mcgill.ca
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dask
+Requires-Dist: dask<=2024.1.0
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pandas-plink
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: zarr
```

### Comparing `magenpy-0.1.2/magenpy.egg-info/SOURCES.txt` & `magenpy-0.1.3/magenpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 magenpy.egg-info/not-zip-safe
 magenpy.egg-info/requires.txt
 magenpy.egg-info/top_level.txt
 magenpy/config/paths.ini
 magenpy/data/1000G_eur_chr22.bed
 magenpy/data/1000G_eur_chr22.bim
 magenpy/data/1000G_eur_chr22.fam
+magenpy/data/lrld_hg19_GRCh37.txt
 magenpy/data/ukb_height_chr22.fastGWA.gz
 magenpy/parsers/__init__.py
 magenpy/parsers/annotation_parsers.py
 magenpy/parsers/misc_parsers.py
 magenpy/parsers/plink_parsers.py
 magenpy/parsers/sumstats_parsers.py
 magenpy/plot/__init__.py
```

### Comparing `magenpy-0.1.2/setup.py` & `magenpy-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 with open("requirements-docs.txt") as fp:
     docs_requires = fp.read().strip().split("\n")
 
 # ------------------------------------------------------
 
 setup(
     name="magenpy",
-    version="0.1.2",
+    version="0.1.3",
     author="Shadi Zabad",
     author_email="shadi.zabad@mail.mcgill.ca",
     description="Modeling and Analysis of Statistical Genetics data in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shz9/magenpy",
     classifiers=[
```

### Comparing `magenpy-0.1.2/tests/test_gdl.py` & `magenpy-0.1.3/tests/test_gdl.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/tests/test_ld.py` & `magenpy-0.1.3/tests/test_ld.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.2/tests/test_simulation.py` & `magenpy-0.1.3/tests/test_simulation.py`

 * *Files identical despite different names*

